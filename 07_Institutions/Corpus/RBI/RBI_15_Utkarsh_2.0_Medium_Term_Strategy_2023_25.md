---
type: Corpus Node
node-id: RBI_15
institution: RBI
date: 2022-12-30
status: active
last_updated: 2026-08-09
wiki-section: S1
tier: A
ai-explicit: true
tags:
  - type/corpus-node
  - status/active
  - status/institutional-strategy
  - engine/phd
  - jurisdiction/india
  - institution/rbi
  - tier/A
  - batch/ad-hoc-20260809
  - concept/Governance_Debt
  - concept/Decision_Infrastructure
  - project/p3
  - project/p4
---

# RBI_15 — Utkarsh 2.0: Medium-Term Strategy Framework (2023-25)

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/RBI/RBI_15_Utkarsh_2.0_Medium_Term_Strategy_2023_25.md`
**Institution:** [[07_Institutions/RBI]]
**Issuing body:** Reserve Bank of India — Governor's Foreword by Shaktikanta Das
**Document date:** **30 December 2022** (Foreword date); covers the period **2023–25**
**Pages:** 14 pages; Preface + 3 chapters
**Domain:** [[03_Domains/BFSI_Governance]] (institutional strategy, not AI-specific)

---

## ⚠ Scoping note — read before citing

**This is an internal institutional strategy document, not a regulatory instrument.** It creates no obligations for regulated entities and has no deontic content in the sense the rest of this corpus tracks (no SHALL/SHOULD directed outward). It is admitted to the corpus for three reasons only: (1) it resolves part of ⚠#335's Utkarsh lineage question; (2) paragraph III.6 is a dated, primary-text AI-adoption commitment by RBI itself; (3) Vision 1's FinTech/CBDC/SupTech/RegTech items (15–18) are the strategic-intent layer that plausibly authorises later AI-adjacent instruments (RBI_9, RBI_14, RBI_FREE_AI_2025). **Do not cite this node for regulatory content** — it has none.

---

## Instrument Identity

**Full title:** Utkarsh 2.0 — Medium-Term Strategy Framework (2023-25)
**Type:** Internal strategic planning document — self-described as "a living document that sets out the course that the Bank adopts"
**Predecessor:** **Utkarsh 2022**, RBI's first medium-term strategy framework, approved by the Central Board of Directors and **launched July 2019**, steered by a high-level Strategy Sub-Committee. Utkarsh 2022 replaced the Bank's prior Annual Action Plans, which lacked a single point of reference and were "perceived to be too short a period for pursuing strategic objectives" (para I.2).
**Structure:** Three layers — Visions, Strategies, Milestones (Chart II.1) — a simplification from Utkarsh 2022's structure, redrafted "to make it sharper and to ensure that there are no overlapping terminologies" (para I.4)
**Scale:** **60 strategies** across **6 visions**: V1 Excellence in Functions (24), V2 Trust of Citizens (8), V3 National/Global Relevance (3), V4 Internal Governance (13), V5 Digital/Physical Infrastructure (4), V6 Human Resources (8)
**Context marker:** Utkarsh 2.0 "commences from 2023, when India assumes the G-20 Presidency" (Foreword) — the document explicitly times itself to the presidency window (para III.5)

### ✅ Partial resolution of ⚠#335 — the Utkarsh lineage

[[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] para 2 cites "paragraph I.10 of **Utkarsh 2029**" as the source of a deferred commitment that further AI-model requirements "may be issued later," and ⚠#335 flagged that Utkarsh 2029 does not exist in the vault.

**This document is not Utkarsh 2029.** It is a distinct, earlier edition — Utkarsh 2.0, covering 2023–25. The lineage is now three generations deep:

| Edition | Period | Status in vault |
|---|---|---|
| Utkarsh 2022 | Launched July 2019 | Not held; referenced only in this document's Preface |
| **Utkarsh 2.0 (this node)** | **2023–25** | **Held — RBI_15** |
| Utkarsh 2029 | Presumably ~2026–28/29, given RBI_14 (June 2026) cites it as current | **Not held — ⚠#335 remains open** |

**⚠#335 is narrowed, not closed.** It is now confirmed that RBI issues these frameworks on a roughly three-year cadence (2019 → 2023 → presumably 2026), which makes "Utkarsh 2029" plausible as the *next* edition after this one rather than a separate document — but this text contains nothing that names its own successor, so that inference is not sourced from primary text. **Source Utkarsh 2029 directly before relying on this inference.**

---

## Analytical Classification

**Wiki section:** S1 (National/Institutional AI-Adjacent Strategy) primary — grouped with MeitY_2, NITI_1, NITI_7 as strategy-not-instrument documents
**Jurisdiction:** India
**Confidence:** High — full primary text supplied by Vivek
**AI explicit:** **Yes, but minimally.** One paragraph (III.6) commits RBI itself to AI/ML adoption; four strategy items (Vision 1, #15–18) name FinTech/CBDC/SupTech/RegTech without operational detail
**Tier classification:** **Tier A** — primary text, but content-thin by design; tier reflects sourcing confidence, not AI-governance density
**AI Governance Wiki relevance:** **LOW-MEDIUM** — institutional-lineage and strategic-authorisation value, not doctrinal content

---

## Substantive Content

### S3.1 The one direct AI paragraph

Para III.6, Chapter III (Conclusion):

> "In this age of data, the Bank plays the dual role of data collection as well as information dissemination. With this comes the responsibility of reliability of data collected to create meaningful and accurate information. Therefore, **adoption of Artificial Intelligence (AI) and Machine Learning (ML) driven tools for data analysis and information creation will be an integral part of Utkarsh 2.0.**"

This is a commitment to AI/ML for RBI's **own internal** data-analysis and dissemination function — not a governance provision directed at regulated entities, and not tied to any specific strategy item in Vision 1–6's enumerated 60. It sits in the Conclusion chapter as a closing-statement commitment rather than an operationalised strategy line.

### S3.2 Vision 1, items 15–18 — the FinTech/CBDC/SupTech/RegTech cluster

Table II.2 (Vision 1: Excellence in the Performance of its Functions, 24 strategies total) contains four consecutive AI-adjacent items:

| # | Strategy (verbatim) |
|---|---|
| 15 | Developing an appropriate framework for managing FinTech ecosystem in the country |
| 16 | Phased introduction of Central Bank Digital Currency |
| 17 | Adoption of emerging SupTech solutions for effective supervision and efficient implementation of regulations |
| 18 | Facilitation in development of RegTech solutions for Regulated Entities |

**These are strategic-intent bullets, not instruments.** No milestone detail, timeline, or operational specification is given in the text supplied — Chart II.1's "Milestones" layer, which would carry that detail, is not reproduced in this document. Items 17–18 (SupTech/RegTech) are the most directly relevant to this vault's AI-governance tracking: they are RBI's own 2022-dated strategic acknowledgement that supervisory and compliance technology would need to evolve, roughly 18 months before RBI_FREE_AI_2025's Seven Sutras and RBI_9/RBI_14's 2026 AI-specific instruments.

### S3.3 Everything else — institutional housekeeping

The remaining 56 of 60 strategies (Visions 2–6, and 20 of Vision 1's 24) cover currency management, reserve management, FEMA review, internationalisation of the Rupee, public debt management, citizen trust and grievance redress, international financial diplomacy (G-20, BIS, IMF, FSB), internal audit and enterprise risk management, green/physical infrastructure, and human resources (re-skilling, counselling, Rajbhasha promotion). None of this carries AI-governance content and none is reproduced here in detail — see the full text supplied by Vivek if institutional-strategy detail beyond the AI-adjacent items is needed.

---

## Analytical Significance for PRIS Research

### S5.1 — Aspiration predates instrument, by a wide and now-measured margin

[[05_Concepts/05_Concepts_Signature/Governance_Debt]]'s Deontic-Placement Debt sub-pattern tracks cases where a regulator holds AI vocabulary in a hortatory instrument while its binding instrument on the same subject omits it. This document supplies an **earlier and starker version of the same mechanism**: RBI committed to AI/ML adoption and named SupTech/RegTech as strategic priorities in **December 2022**, roughly **three and a half years before** RBI_8 (the first binding technology-risk instrument in the corpus, 31 July 2026) and **RBI_8 contains zero AI provisions**. The aspiration-to-obligation lag recorded elsewhere in the corpus at the instrument level (RBI_9/RBI_14 vs RBI_8, six weeks) has a strategic-document-level counterpart measured in **years, not weeks**, once Utkarsh 2.0 is added as the starting point.

### S5.2 — A dated strategic-authorisation layer for SupTech/RegTech

[[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] and [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] both track the absence of instruments governing automated supervisory tooling. Vision 1 item 17 ("Adoption of emerging SupTech solutions for effective supervision") is the **earliest dated institutional signal in the corpus** that RBI intended to move toward automated supervision tooling — predating any operative SupTech instrument by several years. It supplies a strategic-intent anchor but no operational content; treat as background dating evidence, not as a governance instance.

---

## ⚠ VERIFY Flags

- **⚠ #344 (MEDIUM).** Whether "Utkarsh 2029" (cited in RBI_14 para 2) is (a) a distinct third-generation edition following this document, (b) an internal working title for an edition covering a different period than its name suggests, or (c) something else entirely, **cannot be determined from this text.** This document contains no forward reference to a successor edition. Source Utkarsh 2029 directly, or obtain RBI's own citation trail for it, before treating the three-generation lineage table above as confirmed rather than inferred.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]] | [[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] (names "Utkarsh 2029," the still-unsourced successor edition) | [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] | [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] | [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]]
**Related domains:** [[03_Domains/BFSI_Governance]]
**Related institutions:** [[07_Institutions/RBI]]
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] (low-medium — dating/lineage value only) | [[02_Projects/P4_Doctrinal_IJLIT]] (low — aspiration-to-obligation lag illustration)

---

## Coding Status

- **P3 NVivo:** Low priority. No enumerated regulatory units; institutional strategy document only.
- **IG 2.0 / ADICO:** Not applicable — no deontic content directed at regulated entities.
- **Wiki intake status:** Complete, low priority.

---

## Log

- 2026-08-09: Corpus node created from full text supplied by Vivek. **Not a duplicate** — no prior Utkarsh node existed in the vault. **Partially resolves ⚠#335**: confirms this document (Utkarsh 2.0, 2023-25) is distinct from "Utkarsh 2029" cited in RBI_14 — a three-generation lineage (Utkarsh 2022 → Utkarsh 2.0 → Utkarsh 2029) is now inferred but not fully sourced; new flag ⚠#344 raised for the unconfirmed relationship between this edition and the next. Two findings recorded: an earlier, multi-year-scale instance of the Deontic-Placement Debt mechanism (S5.1), and a dated strategic-authorisation anchor for SupTech/RegTech pre-dating any operative instrument (S5.2). Scoped deliberately thin — this is an institutional strategy document, not a regulatory instrument, and is flagged accordingly at the top of the node.
