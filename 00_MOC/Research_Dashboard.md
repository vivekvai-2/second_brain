---
type: MOC
status: active
last_updated: 2026-07-21
tags:
  - type/moc
  - status/active
  - engine/phd
---

# PRIS Daily Dashboard

**Redesigned:** 2026-07-21 (DJ-10) — see note below.
**Purpose:** Cross-project *signal* view — what's overdue, what's gone quiet, what's legitimately blocked, what's actually moving. This is not a task list; task execution (next actions, reminders, nudges) lives in Reminders/your phone, where interrupt-driven tools belong. This page answers one question in under two minutes: is anything I should know about slipping silently?

**How it stays current:** Papers (`02_Projects/`) carry two manual fields you update yourself — `last_session` (bump it whenever you log a session) and `next_deadline` (the nearest unmet hard date). Everything else on this page — Consulting inbound staleness, the Corpus/Wiki-Intake activity comparison — computes automatically from `file.mtime`, so it requires zero maintenance. If a section here looks wrong, the fix is almost always a stale `last_session`/`next_deadline` value in the relevant project note, not this file.

---

## 🔴 Overdue — Deadline Has Passed

*Anything with `next_deadline` in the past and status not deferred. This is the section that would have caught the 1 May 2026 P2 abstract and the 31 May 2026 fsQCA OQ-09 decision the day they slipped, not months later.*

```dataview
TABLE WITHOUT ID
  file.link AS "Project",
  regexreplace(join(filter(file.tags, (t) => startswith(t, "status/")), ""), "status/", "") AS "Status",
  next_deadline AS "Deadline"
FROM "02_Projects"
WHERE next_deadline AND date(today) > date(next_deadline)
  AND !contains(file.tags, "status/deferred")
SORT next_deadline ASC
```

---

## 🟡 Stale — No Session Logged in 21+ Days

*Silent-rot detector. Catches a project going quiet before it becomes a missed deadline. Excludes anything already listed as Blocked below — blocked-and-quiet is expected, unblocked-and-quiet is the actual warning.*

```dataview
TABLE WITHOUT ID
  file.link AS "Project",
  regexreplace(join(filter(file.tags, (t) => startswith(t, "status/")), ""), "status/", "") AS "Status",
  last_session AS "Last Session",
  (date(today) - date(last_session)) AS "Silent For"
FROM "02_Projects"
WHERE last_session
  AND (date(today) - date(last_session)) > dur(21 days)
  AND !contains(file.tags, "status/deferred")
  AND !blocked_by
SORT last_session ASC
```

---

## ⛓ Blocked (Not Stale) — Waiting On Something Else

*Legitimately dormant, not delinquent. Shown separately so a gated project doesn't look identical to an abandoned one.*

```dataview
TABLE WITHOUT ID
  file.link AS "Project",
  blocked_by AS "Waiting On",
  last_session AS "Last Session"
FROM "02_Projects"
WHERE blocked_by
SORT file.name ASC
```

---

## 🟢 On Track

*Session logged within the last 21 days. What's actually moving right now.*

```dataview
TABLE WITHOUT ID
  file.link AS "Project",
  regexreplace(join(filter(file.tags, (t) => startswith(t, "status/")), ""), "status/", "") AS "Status",
  last_session AS "Last Session"
FROM "02_Projects"
WHERE last_session
  AND (date(today) - date(last_session)) <= dur(21 days)
  AND !contains(file.tags, "status/deferred")
SORT last_session DESC
```

---

## 🟡 Stale — Consulting Inbound

*Active or assessed inbound opportunities not touched (any edit, via file.mtime) in 21+ days. Excludes hold/delivered/conflict-hold — those are intentionally paused, not stalled.*

```dataview
TABLE WITHOUT ID
  file.link AS "Opportunity",
  regexreplace(join(filter(file.tags, (t) => startswith(t, "status/")), ""), "status/", "") AS "Status",
  file.mtime AS "Last Touched"
FROM "10_Consulting"
WHERE contains(file.tags, "type/consulting")
  AND (contains(file.tags, "status/active") OR contains(file.tags, "status/assessed"))
  AND (date(today) - date(file.mtime)) > dur(21 days)
SORT file.mtime ASC
```

---

## ⚖️ Build vs. Output Balance — Last 21 Days

*Two lists, deliberately not summarised into a single verdict. If the left list is long and the right list is short or empty, that's the "vault as procrastination engine" pattern the ontology itself warns against — corpus/intake work continuing while paper output stalls. Read them side by side, not as a score.*

**Corpus / Wiki-Intake files touched:**

```dataview
TABLE WITHOUT ID
  file.link AS "File",
  file.mtime AS "Last Touched"
FROM "07_Institutions/Corpus" OR "04_Knowledge_Products/Wiki_Intake"
WHERE (date(today) - date(file.mtime)) <= dur(21 days)
SORT file.mtime DESC
```

**Papers with a session logged:**

```dataview
TABLE WITHOUT ID
  file.link AS "Project",
  last_session AS "Last Session"
FROM "02_Projects"
WHERE last_session AND (date(today) - date(last_session)) <= dur(21 days)
SORT last_session DESC
```

---

## 📱 LinkedIn Content Queue — Ready to Post

*All nodes with extractable carousel or wiki content and no gate blocking*

```dataview
TABLE WITHOUT ID
  file.link AS "Node",
  type AS "Type",
  file.folder AS "Folder"
FROM ""
WHERE contains(file.tags, "content/carousel-ready")
AND contains(file.tags, "gate/open")
SORT type ASC
```

---

## 🏢 Consulting — Actionable Now

*Engagements and assessed inbound opportunities with no gate*

```dataview
TABLE WITHOUT ID
  file.link AS "Node",
  type AS "Type",
  status AS "Status"
FROM ""
WHERE contains(file.tags, "engine/consulting")
AND contains(file.tags, "gate/open")
SORT status ASC
```

---

## 📦 Knowledge Products Pipeline

*What exists · what each gate unlocks*

```dataview
TABLE WITHOUT ID
  file.link AS "Product",
  type AS "Type",
  status AS "Status"
FROM "04_Knowledge_Products"
SORT status ASC
```

---

## ⚠️ Conflict Hold — Do Not Engage

```dataview
TABLE WITHOUT ID
  file.link AS "Node",
  type AS "Type",
  status AS "Status"
FROM ""
WHERE contains(file.tags, "gate/conflict-hold")
```

---

## 🔒 Post-Army / Post-Defence Queue

*Parked until May 2027 exit or PhD defence — visible but not actionable*

```dataview
TABLE WITHOUT ID
  file.link AS "Node",
  type AS "Type",
  status AS "Status"
FROM ""
WHERE contains(file.tags, "gate/army-exit")
  OR (contains(file.tags, "status/deferred") AND contains(file.tags, "type/project"))
SORT status ASC
```

---

## 📚 Reference Layer — Placeholders Needing Zotero Completion

```dataview
TABLE WITHOUT ID
  file.link AS "Reference File",
  type AS "Type"
FROM "02_Projects/References"
WHERE contains(file.tags, "ref/placeholder")
SORT file.name ASC
```

---

## 🔗 Shared Anchors — Cross-Paper Theoretical Foundations

```dataview
TABLE WITHOUT ID
  file.link AS "Anchor",
  type AS "Type"
FROM "02_Projects/Shared_Anchors"
SORT file.name ASC
```

---

## 📊 Projects — Full Pipeline View

```dataview
TABLE WITHOUT ID
  file.link AS "Paper / Deliverable",
  type AS "Type",
  status AS "Status"
FROM "02_Projects"
SORT status ASC
```

---

_Back to [[PRIS_Master_MOC]]_
