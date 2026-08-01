---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - topic/ai-governance-structures
  - topic/accountability
  - institution/agility-at-scale
---

# RACI Matrix for AI Accountability: Template, Guide, and Implementation — Intake Note

**Source:** agility at scale (consultancy)
**Year:** 2026 (10 March 2026)
**Full title:** RACI Matrix for AI Accountability: Template, Guide, and Implementation
**File ID:** F079
**Zotero key:** [blank]
**Wiki section(s):** S1 (Governance Fundamentals — organisational governance-structure design), S6 (Implementation & Governance Artifacts — practitioner template, direct fit for the stated "vendor templates" gap)
**Confidence:** Low — **TIER CAVEAT: single-author consultancy web article, not an institutional or peer-reviewed source.** Author (Morne Wiggins) and publisher ("agility at scale," a boutique SAFe/agile-transformation consultancy per its own site navigation) carry no independent authority comparable to NACD, ISACA, or a Big 4 methodology. Statistical claims in the article (e.g., "nearly one-third of project failures") are asserted with no citation trail. Treat as a practitioner opinion/template source, not an empirically grounded one.
**Jurisdiction:** Global (generic organisational framework, not jurisdiction-specific; references EU AI Act, NIST AI RMF, ISO/IEC 42001 in passing)

---

## Classification

**Document type:** Industry Guide / Consultancy Web Article
**Primary audience:** Practitioner (AI governance/PMO leads implementing accountability structures)
**AI explicit:** Yes

---

## 3–5 Reusable Findings

1. **Single-Accountable-Owner rule, with an explicit Responsible/Accountable conflation warning** (feeds S1): "The most dangerous confusion organizations encounter is between Responsible and Accountable... In AI governance, these must be separated" — a crisp, quotable governance principle: exactly one Accountable owner per activity, distinct from whoever executes the work.

2. **Six-step RACI construction methodology** (feeds S6): Define AI Governance Scope and Objectives → Enumerate AI Lifecycle Activities → Identify All Stakeholder Roles → Assign RACI Designations → Socialize and Validate with Stakeholders → Embed in Governance Workflows. A concrete, template-ready governance-artifact-construction process.

3. **Full AI-lifecycle-stage RACI table** (feeds S6): Maps seven lifecycle stages (Data Acquisition, Model Development, Validation, Deployment, Monitoring, Audit, Decommissioning) to named roles (CTO, ML Engineer, AI Ethics Officer, CRO, Compliance Officer, DPO, Board) across all four RACI designations. The single most directly reusable practitioner artifact in this node — a strong candidate for a LinkedIn practitioner-checklist carousel or client-deliverable template.

4. **Five RACI failure patterns and fixes** (feeds S1/S6): Multiple Accountable Owners; RACI Overload; treating RACI as a one-time exercise; Accountability Without Authority; missing Consulted stakeholders — a diagnostic checklist usable to audit an existing (or client) AI governance structure for common design failures.

5. **Autonomous-system accountability principle** (feeds S1, AEGIS_OS-relevant): "Someone must be Accountable for the outputs of an autonomous system, even when no human directly triggered the specific action" — directly aligned with AEGIS_OS's runtime-enforcement/authority-binding thesis; accountability must attach to a person even for agentic/autonomous decisioning.

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The full lifecycle-stage RACI table is directly usable as a client-deliverable template or as a LinkedIn carousel — matches the stated visual-branding preference for structured practitioner checklists exactly.
**Consulting connections:** AEGIS_OS (direct — "Accountability Without Authority" pitfall and the autonomous-system accountability principle both support the runtime-enforcement/authority-binding narrative); PrivacyWeave (the DPO's Consulted role in the lifecycle RACI table maps to purpose-limitation oversight).
**Teaching connection:** Strong template exercise for a governance workshop — have participants build a RACI matrix against the seven-stage lifecycle table.

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S1, S6
**Concepts:** [[05_Concepts/05_Concepts_Standard/Accountability]]
**Corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/IAPP_AIGP_Body_of_Knowledge_v21_2026]] (F055 — Domain I governance-structures competency area this node concretises); [[04_Knowledge_Products/Wiki_Intake/F035_Microsoft_Administering_Governing_Agents]] (three-tier End User/Maker/Developer accountability spectrum — comparator RACI-adjacent model)
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes
- [ ] Marked processed

---

## ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| #221 | **Source tier caveat** — single-author consultancy blog, no institutional peer review; statistical claims ("nearly one-third of project failures across industries," "more than five seconds") are asserted with zero citation trail in the source itself. Do not cite these figures externally without independent verification; cite the RACI methodology/template only as a practitioner framework, not as empirically grounded research | HIGH |
| #222 | "Under the EU AI Act, high-risk AI systems require documented human oversight and clear accountability chains" and similar EU AI Act paraphrases in the source are generic characterisations, not precise article citations — verify against the Act's actual text (Art. 14 human oversight, Art. 26 deployer obligations) before citing as a precise legal claim | MEDIUM |

---

## Log

- 2026-07-15: Wiki intake note created. NotebookLM extraction relay, PROMPT 0b. Ad hoc pre-Batch 19 session. Sourced via a Perplexity Deep Research prompt targeting the S1 governance-structure-design gap identified in this session's AIGP BoK (F055) gap analysis. Duplicate check run against "RACI Matrix," "agility at scale," "Morne Wiggins" — no prior match; confirmed new node. Tier caveat applied given single-author consultancy-blog provenance.
