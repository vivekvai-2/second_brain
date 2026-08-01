---
type: Consulting Template
tags:
  - type/consulting-template
  - status/active
  - engine/consulting
---

# Inbound Opportunity — Intake Template

**Type:** Consulting Deliverable Template
**Status:** Active
**Created:** 2026-07-15
**Formalizes:** the pattern already used consistently across [[CyberMesh_PS69_Inbound]], [[CyberMesh_PS74_Inbound]], [[AEGIS_OS_Inbound]], [[Offline_Intelligence_Inbound]], and [[PrivacyWeave_Inbound]] — this template did not exist as a written artefact; it is the shape those five notes already share.

---

## How to Use

Copy this file to `10_Consulting/{StartupName}_Inbound.md` for every new unsolicited advisory/founder outreach. Fill all seven sections before deciding on any response beyond acknowledgement. Add the new entry to [[Inbound_Pipeline_Index]] Pipeline Status and Leverage Map tables in the same session.

---

## Frontmatter block (copy into new note)

```yaml
---
type: Inbound Opportunity
tags:
  - type/consulting
  - status/assessed        # or: status/hold, status/delivered
  - phase/0-now             # or: gate/army-exit, gate/conflict-hold
  - gate/open                # or: gate/army-exit, gate/conflict-hold
  - engine/consulting
---
```

---

## 1. What They Do

- Company/product name, founder(s), stage.
- Core architecture or value proposition in 2–4 sentences — enough that a reader unfamiliar with the space understands the mechanism, not just the pitch language.
- Key technical or business differentiators.
- India relevance, if any (regulatory hooks — DPDP, RBI, SEBI, defence procurement).

## 2. What They Are Asking For

- State explicitly if asked; otherwise mark **"Not stated — inferred"** and give the inference with reasoning (prior pattern: most inbound asks are implicit).

## 3. Conflict / Gate Assessment

Use the three-tier flag convention already established:

- 🟢 **Clean** — no defence/government-procurement/SCOMET exposure; standard commercial advisory rules apply.
- 🟡 **Partial** — scope-dependent; separate the clean commercial angle from the defence/procurement-adjacent angle explicitly, and gate only the latter.
- 🔴 **Hard conflict** — active defence procurement or serving-officer conflict; no engagement of any kind beyond acknowledgement until the stated gate clears.

For every 🟡 or 🔴, name the specific service-conduct or procurement-integrity risk dimension(s), not just the flag colour.

**Gate:** state the exact condition that clears the gate (e.g. "Army exit May 2027", "scope clarification from founder").

**Recommended action:** one line — acknowledge only / respond to clean angle only / full engagement permitted.

## 4. Research Leverage — What This Inbound Teaches the Vault

Table format, one row per insight:

| Insight | Research Connection |
|---|---|
| | |

Close with a **"Strongest reuse opportunity"** paragraph naming the single highest-value connection — usually a specific concept file, knowledge product chapter, or fsQCA/doctrinal paper this inbound provides a concrete illustration for.

## 5. Future Engagement Options

| Option | Timing | Gate |
|---|---|---|
| | | |

Include at minimum: an immediate/no-gate option if one exists, and a post-superannuation option if defence-adjacent.

## 6. Linked Vault Nodes

List every wikilink used above, grouped by type (Domains / Knowledge Products / Concepts / Frameworks / Institutions / Methods / Projects / Content / Consulting) — mirrors the convention in all five existing inbound notes.

## 7. Decision Journal Entry

Per the Inbound Pipeline Index operating rule: **nothing progresses from this folder to an active engagement without a conflict clearance entry in `12_Decision Journal`.** Log the assessed conflict tier and recommended action there in the same session this note is created.

---

## After Filling Out

1. Add a row to [[Inbound_Pipeline_Index]] Pipeline Status table (Startup | Domain | Ask | Conflict Flag | Gate | Status).
2. Add rows to the Leverage Map — Vault Connections table for each concept/framework touched.
3. If defence-adjacent, add to the Post-Superannuation Opportunity Queue.
4. Log the conflict clearance decision in `12_Decision Journal`.

---

## Linked Vault Nodes

**Consulting:** [[Inbound_Pipeline_Index]], [[CyberMesh_PS69_Inbound]], [[CyberMesh_PS74_Inbound]], [[AEGIS_OS_Inbound]], [[Offline_Intelligence_Inbound]], [[PrivacyWeave_Inbound]], [[Consulting_Deliverable_Templates_Index]]

---

_Back to [[Consulting_Deliverable_Templates_Index]]_
