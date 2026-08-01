---
type: MOC
status: active
last_updated: 2026-08-01
tags:
  - type/convention
  - status/active
  - engine/infrastructure
---

# PRIS Git Version Control Protocol (GVCP)

**Authoritative Operational Guide for Vault Version History, Backup, and Recovery**
*Owner: Vivek Vaidyanathan & AI Co-working Agents | Status: ACTIVE | Established: 2026-08-01 | Version: 1.0*

---

## 1. Purpose

The vault (`/Users/vivek/Documents/Second Brain`) is under full Git version control, backed up to a private GitHub repository, with automatic commits so that no manual save discipline is required. This protocol exists so that, if a file is ever lost, corrupted, or needs to be checked back to an earlier state, the recovery procedure is documented rather than reconstructed from memory.

The vault changes through exactly two channels — Cowork sessions and the Gemini agent plugin inside Obsidian — and both are captured identically, because version control operates on the folder on disk rather than on either tool.

---

## 2. Architecture

| Component | Detail |
|---|---|
| **Local repository** | `/Users/vivek/Documents/Second Brain/.git` — full commit history lives here |
| **Remote (backup)** | Private GitHub repo: `https://github.com/vivekvai-2/second_brain.git` |
| **Tracked scope** | All content folders (`00_MOC` through `12_Decision Journal`, `99_Archive`, `gemini-scribe`, etc.) |
| **Excluded** (`.gitignore`) | `.obsidian/` (app config, plugin binaries, workspace state), `.DS_Store`, `.fuse_hidden*`, lock/tmp files |
| **Auto-commit script** | `~/Scripts/second_brain_autocommit.sh` |
| **Scheduler** | `~/Library/LaunchAgents/com.vivek.secondbrain.autocommit.plist` (macOS `launchd`, runs every 60s) |
| **Activity log** | `~/Library/Logs/second_brain_autocommit.log` |
| **Error log** | `~/Library/Logs/second_brain_autocommit.stderr.log` |

### How the automation works

Every 60 seconds, `launchd` runs the script, which:
1. Checks `git status` — if nothing changed, exits immediately.
2. If something changed, checks how long it's been since the most recently modified file — if less than 5 minutes, exits (session likely still active).
3. If quiet for 5+ minutes, stages everything (`git add -A`), commits with an auto-generated message (`[Auto] N file(s) updated — filename(s)`), and pushes to `origin/main`.

This means edits from a Cowork session or from the Gemini plugin in Obsidian are captured the same way — the watcher doesn't know or care which tool made the change, only that the folder on disk was quiet for 5 minutes.

A manual trigger remains available as a fallback: asking Claude in a Cowork session for an ad hoc commit, or running `git add -A && git commit -m "..."` directly.

---

## 3. Recovering / Checking Back a Version

All commands below are run from Terminal, in the vault directory:

```bash
cd "/Users/vivek/Documents/Second Brain"
```

### 3.1 View history

```bash
git log --oneline -20              # last 20 commits, one line each
git log --oneline -- "path/to/note.md"   # history of one specific file
```

### 3.2 See what changed in a specific commit

```bash
git show <commit-hash>
```

### 3.3 Restore a single file to an earlier version

```bash
git checkout <commit-hash> -- "path/to/note.md"
```
This overwrites the current version of that file with the version from the specified commit. The file appears as a staged change — commit it normally (or let the auto-commit watcher pick it up) if you want to keep the restored version.

### 3.4 View an old version without restoring it

```bash
git show <commit-hash>:"path/to/note.md"
```
Prints the file's contents at that commit to the terminal without touching the current file — useful for checking what something used to say before deciding whether to restore it.

### 3.5 Restore a file that was deleted

```bash
git log --oneline --diff-filter=D -- "path/to/note.md"   # find the commit just before deletion
git checkout <commit-hash>^ -- "path/to/note.md"           # restore it
```

### 3.6 Roll back the entire vault to an earlier point in time

Only for serious situations (e.g. a bad bulk edit or corruption across many files):

```bash
git reset --hard <commit-hash>
```
**Caution:** this discards all local changes made after that commit. Since everything is also pushed to GitHub, nothing is unrecoverable, but any commits after the target point will need `git push --force` to also roll back the remote — do not do this without confirming intent, since it rewrites shared history.

### 3.7 Compare two points in time

```bash
git diff <older-commit-hash> <newer-commit-hash> -- "path/to/note.md"
```

---

## 4. Verifying the Automation Is Running

```bash
launchctl list | grep secondbrain
```
Should return a line with a PID (or `-` if idle) and exit status `0`. If the job is missing, reload it:

```bash
launchctl unload ~/Library/LaunchAgents/com.vivek.secondbrain.autocommit.plist
launchctl load ~/Library/LaunchAgents/com.vivek.secondbrain.autocommit.plist
```

To watch it work in real time:
```bash
tail -f ~/Library/Logs/second_brain_autocommit.log
```

---

## 5. Known Dependency: macOS Full Disk Access

The script runs as `/bin/bash`, spawned silently by `launchd` with no user-facing prompt. Because the vault lives under `~/Documents` — a TCC-protected folder on macOS — bash must be explicitly granted **Full Disk Access** (System Settings → Privacy & Security → Full Disk Access → add `/bin/bash`, toggle on). Without this, every tick fails with `fatal: Unable to read current working directory: Operation not permitted` in the stderr log. This has already been granted and confirmed working as of 2026-08-01; noting it here in case the grant is ever reset (e.g. after a macOS update) and the symptom needs to be re-diagnosed.

---

## 6. GitHub Authentication

Push authentication uses a GitHub fine-grained Personal Access Token embedded in the remote URL, cached by macOS Keychain (`credential.helper osxkeychain`) after first use — no repeated prompts under normal operation. The token requires **Contents: Read and write** permission on the `second_brain` repository specifically (fine-grained tokens do not get repository access by default — this must be explicitly granted per-token, per-repo).

If push authentication ever fails (`403` or "repository not found"), check in this order:
1. Confirm the repo exists at `github.com/vivekvai-2/second_brain`.
2. Confirm the active token has `second_brain` in its repository access list.
3. Confirm the token's **Contents** permission is set to Read and write (not the default Read-only/No access).
4. If a token is ever exposed (e.g. pasted somewhere it shouldn't be), revoke it immediately at [github.com/settings/tokens](https://github.com/settings/tokens) and issue a fresh one, then update the remote: `git remote set-url origin https://NEW_TOKEN@github.com/vivekvai-2/second_brain.git`.

---

## 7. Change Control and Integration

This protocol is a living system integrated into:
- `00_MOC/PRIS_Master_MOC.md` (Strategic Layer)
- `00_MOC/Workflow_Discipline_Protocol.md` (session close-out disciplines — Git history is the underlying safety net for all Tiered Close-out levels)

Changes to this protocol (e.g. changing the quiet-window duration, switching auth method, adding a new watched directory) should be logged as a Decision Journal entry and updated here with a version increment.

**Version:** 1.0
**Established:** 2026-08-01
**Change Log:** Initial version — documents the GitHub backup + `launchd` auto-commit system set up 2026-08-01, first verified working via F138 intake note commit `a19a6b3`.

---

*Back to [[PRIS_Master_MOC]]*
