---
type: VERIFY Tracker
tags:
  - type/verify-tracker
  - status/active
  - engine/business-development
---

# VV Partner Map — VERIFY Tracker

**Type:** Consolidated VERIFY Tracker (Business-Development corpus)
**Status:** Active
**Created:** 2026-07-15
**Scope:** [[VV_Partner_Map_Master]] and [[VV_Integrated_Strategy_Master]] (both dated May 2026)
**Session date at time of this pass:** 2026-07-15 (~2.5 months after source documents were finalised)

---

## Why This Exists

This tracker applies the same discipline the Policy Dump corpus side already enforces (⚠VERIFY BEFORE PUBLISHING flags, consolidated in [[Corpus_Index_MOC]]) to the business-development roadmap documents, which had no equivalent discipline until now. It is deliberately a **companion file**, not an edit to [[VV_Partner_Map_Master]] itself — the source document stays byte-for-byte as authored, consistent with this vault's "never replicate/alter primary source" convention. Flags are numbered independently (`PM-V##`) to avoid colliding with the Policy Dump's own VERIFY numbering.

**This pass does not re-verify against live sources** (no web check was performed) — it identifies which claims in the source documents are *time-sensitive enough to need re-checking*, given how much calendar time has passed since May 2026. Treat every flag below as "needs a live check," not "confirmed wrong."

---

## Flags

| ID | Entity/Claim | Source | Why Flagged | Priority |
|---|---|---|---|---|
| PM-V1 | Karnataka Committee on Responsible AI "constituted March 2026 (90-day mandate)" | Part 6 — Karnataka | 90 days from March 2026 lands in early-to-mid June 2026 — the Committee's **mandate itself**, not just the interim-report window already flagged in [[Karnataka_Responsible_AI_Committee_Expert_Note_Template]] (F1), may have already expired, been extended, or converted to a final-report phase as of session date 2026-07-15. This is the sharper, upstream version of the F1 flag. | **High** |
| PM-V2 | Tamil Nadu "AI Governance Conference at iTNT Hub (May 2026)" | Part 6 — Tamil Nadu | Event date has passed as of session date. Already flagged at instance level in [[Tamil_Nadu_iTNT_Hub_Outreach_Template]] (F3); flagging here too since it's the same stale fact propagating from this source. | **High** (duplicate of F3, tracked once at source) |
| PM-V3 | India AI Impact Summit date inconsistency: Andhra Pradesh section cites **February 2026**; Brookings section cites **January 2026** for what reads as the same event | Part 3 (Brookings) vs. Part 6 (Andhra Pradesh) | Internal inconsistency in the source document itself, independent of elapsed time — worth resolving so future outreach doesn't cite the wrong month. | **Medium** — factual consistency, not staleness |
| PM-V4 | MeitY "constituting" TPEC, AIGG, and AI Safety Institute (AISI) | Part 1 — MeitY | Described as an in-progress constitution process as of the May 2026 document date. ~2.5 months have elapsed — these bodies may now be formally operating, which changes the correct engagement route (a constituted body has known membership/application channels; an in-progress one doesn't). | **Medium** |
| PM-V5 | SEBI "CSCRF and 2024-25 AI Advisory... are live" | Part 1 — SEBI | "2024-25" is a specific cycle reference; a 2025-26 or later cycle may have superseded it by now. | **Medium** |
| PM-V6 | IRDAI "has initiated an empanelment process for service providers" | Part 1 — IRDAI | No date given in source; empanelment windows typically close. Status unknown without a live check. | **Medium** |
| PM-V7 | ORF America Fellowship "Inaugural cohort included ONDC, EY India, RAND, and Beacon Global Strategies" | Part 3 — ORF America | Describes the *inaugural* cohort specifically — a second cohort's composition, timeline, and application window (if annual) may already differ. | **Medium** |
| PM-V8 | Kerala "Regional AI Impact Summit under IndiaAI Mission 2026" | Part 6 — Kerala | Only "2026" given, no month — cannot currently tell if this event is past or upcoming relative to session date. | **Medium** |
| PM-V9 | IAPP "September" annual application window | Part 3 — IAPP | Not yet stale (September 2026 is still ahead of session date), but the exact open date should be reconfirmed closer to the window. Cross-reference: already partially flagged in [[IAPP_Training_Advisory_Board_Application_Template]] (F4). | **Low** (forward-looking, not yet actionable) |
| PM-V10 | Telangana TAIH programme status (2 lakh AI engineers target, AI University, Future City concept; MoU with Blaize "signed at Davos, January 2026") | Part 6 — Telangana | The Davos MoU date itself is a safe historical anchor (low risk); the broader programme's current status/milestones should be reconfirmed given elapsed time, since outreach language references it as presently live. | **Low** |
| PM-V11 | All per-entity "Indicative Value" (₹ lakh/crore) figures across every Part | Throughout | These are May 2026 estimates with no stated re-pricing mechanism. Not stale in the sense of being wrong, but should be checked against actual market feedback the first time any real engagement closes, rather than treated as a permanent benchmark. | **Low** — structural note, not a factual claim to verify |
| PM-V12 | Esya Centre "Covered MeitY's AIGEG formation (April 2026)" | Part 2 — Esya Centre | Low-risk historical reference; confirm "AIGEG" naming hasn't been superseded before citing it in outreach. | **Low** |
| PM-V13 | IndiaAI Mission "₹10,371.92 crore outlay for five years" | Part 1 — IndiaAI | Large multi-year figure, low near-term staleness risk; confirm no budget revision before citing precisely in a formal proposal. | **Low** |

---

## Priority Summary

**High (2):** PM-V1, PM-V2 — both concern the Karnataka/Tamil Nadu urgency claims that directly drive Bucket F instance templates. Re-verify before any Bucket F/A7 outreach tied to these two entities.

**Medium (5):** PM-V3 through PM-V8 — mostly "has this process concluded/moved to its next phase" questions where the wrong answer would mean approaching the wrong contact or channel, not a reputational risk.

**Low (6):** PM-V9 through PM-V13 — either not yet actionable (forward-looking dates) or low-consequence historical anchors.

---

## How to Close a Flag

1. Re-check the claim against a live source (regulator website, official notification, news).
2. Record the check date and outcome here (add a "Resolved" column entry).
3. If the fact has changed, update the relevant template's frontmatter (`deadline`, `source_url`, `source_verified_on`) — do **not** edit [[VV_Partner_Map_Master]] itself; the correction lives in the derived template layer, consistent with this vault's primary-source-preservation convention.
4. Cross-reference [[Karnataka_Responsible_AI_Committee_Expert_Note_Template]] and [[Tamil_Nadu_iTNT_Hub_Outreach_Template]] specifically when closing PM-V1/PM-V2 — those two templates should have their `verify_before_use` flag cleared only after this tracker's corresponding entry is closed.

---

## Linked Vault Nodes

**Source:** [[VV_Partner_Map_Master]], [[VV_Integrated_Strategy_Master]]

**Downstream templates carrying related flags:** [[Karnataka_Responsible_AI_Committee_Expert_Note_Template]] (F1), [[Tamil_Nadu_iTNT_Hub_Outreach_Template]] (F3), [[IAPP_Training_Advisory_Board_Application_Template]] (F4)

**Index:** [[VV_Advisory_BD_Authority_Index]]

**Convention precedent:** [[Corpus_Index_MOC]] (the equivalent tracker for the Policy Dump corpus side)

---

_Back to [[VV_Advisory_BD_Authority_Index]]_
