---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/meity
---

# MeitY_3 — National Data Governance Framework Policy (Draft)

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/MeitY/MeitY_3.md`
**Institution:** [[07_Institutions/MEITY]]
**Issuing body:** Ministry of Electronics and Information Technology (MeitY)
**Document date:** Draft, May 2022
**Pages:** Not fully determinable
**Domain:** [[03_Domains/DPI_Governance]] | [[03_Domains/Privacy_DataProtection]]

---

## Instrument Identity

**Full title:** National Data Governance Framework Policy (Draft)
**Type:** Draft Policy (non-binding, consultation stage as of extraction)
**Target entities:** Government departments/agencies (data-generating entities); research/startup ecosystem (data users); proposed India Data Management Office
**Legal basis:** MeitY draft policy — status of finalisation not confirmed
**Companion documents:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (DPDP Rules 2025 — personal data counterpart to this non-personal/anonymised data framework)

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) and S5 (Data, Privacy & Security) — non-personal data governance dimension
**Jurisdiction:** India
**Confidence:** Low — text extraction was significantly garbled (OCR-like duplication artefacts, e.g., "Digitization of of government, governance governance"); core objectives discernible but exact wording unreliable
**AI explicit:** No (data governance infrastructure policy; AI relevance is indirect — as an enabler of AI training-data ecosystems)
**Tier classification:** Tier C — AI-adjacent (data infrastructure precursor to AI governance, not AI-specific)
**AI Governance Wiki relevance:** MEDIUM — establishes the **non-personal/anonymised data governance institutional architecture** (India Data Management Office, India Datasets program) that would underpin any future AI-training-data governance regime, complementing DPDP's personal-data framework.

---

## Substantive Content

⚠ VERIFY BEFORE PUBLISHING — the following is based on a garbled extraction (duplicated-word OCR artefacts); core concepts appear reliable but exact policy wording, scope thresholds, and institutional powers must be re-verified against a clean copy of the source PDF before citation.

### Core proposals (as discernible)
- **India Data Management Office (IDMO)**: proposed as the institutional body to frame, manage, and periodically review the data governance framework, standards, and guidelines for non-personal/anonymised datasets.
- **India Datasets program**: a proposed government initiative to create a platform/repository of anonymised, non-personal datasets from government and potentially private sources, intended to support AI/ML research, startups, and the research ecosystem.
- **Rules-based access**: anonymisation and access-control rules for datasets shared through the program, intended to balance data utility (for research/innovation) against privacy risk.
- **Scope**: appears to apply primarily to government ministries/departments and their data, with potential extension/encouragement to private-sector data sharing on a voluntary basis (exact scope unverified).

### Relationship to DPDP (MeitY_1)
Where DPDP Rules 2025 ([[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]]) govern **personal** data, this draft policy is intended to govern **non-personal and anonymised** data — together they would form the two halves of a comprehensive Indian data governance architecture. As of the May 2022 draft, it is unclear whether this policy was ever finalised or superseded.

---

## Analytical Significance for PRIS Research

### For P2 (DPI Governance, JSIS) and Institutional Coherence
MeitY_3 (if finalised) would be the **non-personal data counterpart** to MeitY_1 (DPDP, personal data) — together forming a two-track data governance architecture potentially analogous to (and feeding) AI training-data governance debates. The proposed India Data Management Office is structurally similar in concept to RBI_FREE_AI_2025's and India AI Governance Guidelines' (MeitY_2) proposed institutional bodies (AIGG, AISI, TPEC) — a recurring pattern of **"new coordinating body" as the default Indian institutional response** to emerging governance domains (data, AI). This pattern itself may be worth coding as a recurring institutional-design choice across the corpus for [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]].

### Coordination / Parallelism Pattern
Existing node: [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]]. Pattern: **Complementary scope split (intra-ministry)** — MeitY_1 (personal data, finalised 2025) and MeitY_3 (non-personal data, draft 2022) represent a deliberate scope division within the same ministry; the ~3-year gap between draft (2022) and DPDP finalisation (2025) raises the question (for future verification) of whether MeitY_3 was finalised in parallel, superseded, or remains in draft limbo — relevant to [[05_Concepts/05_Concepts_Signature/Governance_Debt]] (a 2022 draft with no confirmed finalisation by 2025-26 would itself be an instance of governance debt).

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]], [[07_Institutions/Corpus/MeitY/MeitY_2]], [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Governance_Debt]], [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]]
**Related frameworks:** —
**Related projects:** [[02_Projects/P2_DPI_JSIS]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** PrivacyWeave (non-personal data governance is adjacent to DPDP purpose-limitation enforcement scope)

---

## Coding Status

- **P3 NVivo:** Not applicable (not BFSI-specific)
- **Wiki intake status:** Pending — flagged for re-extraction (clean OCR pass needed)

---

## Log

- 2026-06-14: Corpus node created. Batch 3. Cowork session. Source: National-Data-Governance-Framework-Policy.pdf. Originally proposed for "International frameworks" batch — rerouted to MeitY/ on confirming this is a MeitY (Indian) draft policy. Extraction quality poor (OCR duplication artefacts) — flagged for re-extraction.
