---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - engine/phd
  - theme/ai-risk-taxonomy
  - theme/control-framework
  - theme/regulatory-mapping
---

# Eisenberg, Gamboa & Sherman (2025) — The Unified Control Framework: Establishing a Common Foundation for Enterprise AI Governance, Risk Management and Regulatory Compliance

**Source:** Ian W. Eisenberg, Lucía Gamboa & Eli Sherman (Credo AI)
**Year:** 2025 (arXiv preprint, 11 Mar 2025, arXiv:2503.05937v1 [cs.CY])
**Full title:** "The Unified Control Framework: Establishing a Common Foundation for Enterprise AI Governance, Risk Management and Regulatory Compliance"
**File ID:** F026
**Zotero key:** ⚠ VERIFY — not yet assigned
**Wiki section(s):** S1 (Governance Fundamentals — control frameworks) / S3 (AI Risk Taxonomies & Classification) / S4 (Agentic AI Governance — frontier-AI/alignment controls) / S6 (Model Risk)
**Confidence:** High (industry-research arXiv preprint, methodologically transparent; Credo AI is an established AI governance platform vendor with prior AAAI-published work — cf. Sherman & Eisenberg 2024)
**Jurisdiction:** Global / US-centric validation case (Colorado AI Act SB 24-205); cross-referenced against EU AI Act, ISO/IEC 42001, NIST AI RMF, South Korea AI Basic Act

---

## Classification

Conceptual/applied framework paper proposing the **Unified Control Framework (UCF)**: a tripartite architecture linking (1) a 15-category/50-scenario MECE risk taxonomy synthesized from the MIT AI Risk Repository, NIST AI RMF, and IBM AI Risk Atlas; (2) a "policy requirements library" translating regulatory text (validated against the Colorado AI Act, 12 requirements) into structured obligations; and (3) a parsimonious **42-control library** with detailed implementation guidance, each control mapped many-to-many to both risk scenarios (mean 4.1 risks/control) and policy requirements. Format B Wiki Intake Note — the most structurally complete **risk-to-control-to-regulation mapping artefact** in the corpus, directly complementing F025's agentic-specific control taxonomy.

---

## Reusable Findings

1. **15-category/50-scenario risk taxonomy as a coding frame for India BFSI regulatory gap analysis (feeds S3/P3):** The taxonomy's 15 risk types (AI Agency, Environmental Harm, Explainability & Transparency, Fairness & Bias, Harmful Content, Human-AI Interaction, Information Integrity, Legal, Malicious Use, Operational, Performance & Robustness, Privacy, Security, Societal Impact, Third Party) is explicitly MECE-constructed (via Claude-assisted clustering + 6-7 expert interviews) and synthesizes three major prior taxonomies plus 16 newly authored scenarios. The authors flag that "Operational" risk was **entirely absent from prior taxonomies** — a finding directly useful for assessing whether RBI/SEBI AI circulars similarly under-address operational integration/maintenance/scalability risk relative to the more commonly regulated categories (Fairness, Privacy, Security).

2. **42-control library as a "minimal sufficient set" benchmark for governance-cost arguments (feeds S1/Governance_Debt):** Through iterative consolidation, the authors reduced an initial >100-control set to 42 "parsimonious" controls while retaining coverage of all 50 risk scenarios and 13/14 Colorado AI Act requirements (one gap — algorithmic-discrimination disclosure, Section 6-1-1703.7 — required adding Control-042). This **"42 controls = comprehensive coverage" benchmark** is a reusable comparator for evaluating whether India's emerging sectoral AI guidance (RBI FREE-AI, SEBI circulars, DPDP Rules) collectively approaches or falls short of this control-completeness threshold — useful for a P3/P4 "regulatory completeness scorecard."

3. **Many-to-many control mapping as the structural innovation reducing compliance duplication (feeds S1/Regulatory_Parallelism):** The paper's central efficiency claim — that a single control (e.g., "Establish AI system documentation framework," Control-009) can simultaneously satisfy EU AI Act technical-documentation requirements, Colorado AI Act disclosure requirements, and ISO/IEC 42001 — is a citable formalization of the "convergent compliance" logic underlying [[Regulatory_Parallelism]]. This gives P3's regulatory-parallelism argument a concrete worked example (Section 2.3, training-data documentation) showing how one control discharges obligations across jurisdictions without bespoke jurisdiction-specific processes.

4. **Colorado AI Act gap (algorithmic-discrimination disclosure, Section 6-1-1703.7) as the framework's only validation failure (feeds S1/P4):** Of 14 Colorado AI Act policy requirements mapped, only ONE (CO-DEPLOYER.C7, mandatory disclosure of discovered algorithmic discrimination) had no corresponding existing control — necessitating a new "general purpose incident response mechanism" (Control-042). This is a precise, citable instance of a **risk-derived control library failing to anticipate a specific regulatory disclosure obligation**, useful as a worked example of the "risk-to-regulation translation gap" — i.e., risk taxonomies built from technical/societal harm catalogues do not automatically generate the *procedural/disclosure* obligations that regulators add. Directly relevant to assessing whether India's AI governance circulars (which emphasize disclosure/grievance-redress under DPDP) are adequately anticipated by risk-derived control catalogues like F025's agentic framework.

5. **LLM-assisted taxonomy/control development methodology as a second corroborating precedent for P1 automated coding (feeds S7/P1):** Independent of F024 (Rao et al.), this paper documents a parallel LLM-assisted methodology: Claude used for semantic clustering of risk descriptions, gap-driven risk synthesis, and quantitative scoring (clarity/specificity/enterprise relevance) of risk descriptions, plus Claude+GPT-4o run in parallel for control-guidance drafting, with human expert panels (6-7 reviewers, 1-3 reviewers/control) validating outputs. Two independent 2025 papers (F024, F026) both using "LLM-assisted taxonomy construction + human expert validation" as a methodology strengthens the case for citing this as an **emerging standard practice** in P1's methods section, with two citable precedents rather than one.

---

## Consulting / Teaching Reuse

- The **Figure 1 "bidirectional mapping" diagram** (risk taxonomy ↔ controls ↔ policy requirements, governance context as configurator) is a strong visual for explaining to BFSI boards why a single well-designed control can discharge multiple regulatory obligations — directly supports "governance efficiency" pitches to CROs/CISOs facing multi-regulator overlap (RBI/SEBI/IRDAI/DPDP).
- The **Colorado AI Act validation gap (13/14, missing algorithmic-discrimination disclosure)** is a reusable cautionary example for client workshops: even a well-constructed risk-derived control library can miss specific statutory disclosure triggers — underscoring the need for a parallel "regulatory requirements checklist" alongside any risk-based control framework.
- The **"Operational" risk category being entirely new/absent from prior taxonomies** is a useful talking point when advising clients that mainstream AI risk frameworks (NIST, MIT, IBM) under-cover integration, maintenance, and scalability risk — areas where Indian BFSI legacy-system integration challenges are particularly acute.

---

## Cross-Links

- [[04_Knowledge_Products/Wiki_Intake/AgenticRisks_Enterprise_Wide_Agentic_AI_Risk_Controls_2025]] (F025) — both are 2025 control-taxonomy frameworks; F026's 42 generic enterprise controls and F025's 242 agentic-specific controls are complementary layers (general AI governance vs. agentic-specific extension). A combined "general + agentic" control-coverage map is a strong P4 deliverable.
- [[04_Knowledge_Products/Wiki_Intake/Rao_Scepanovic_AI_Model_Risk_Catalog_2025]] (F024) — both papers independently use LLM-assisted (Claude) taxonomy/classification methodology with expert validation; corroborating methodological precedent for P1.
- [[Regulatory_Parallelism]] — many-to-many control-to-policy-requirement mapping as the formal mechanism underlying convergent multi-jurisdictional compliance.
- [[Governance_Debt]] — 42-control "parsimonious sufficient set" as a completeness benchmark against which under-resourced governance regimes can be measured.
- [[Institutional_Coherence]] — the single Colorado AI Act validation gap (disclosure of discovered discrimination) as a precise instance of risk-taxonomy/regulatory-requirement misalignment.
- [[P1_SLR_RG]] — second LLM-assisted-taxonomy methodological precedent (alongside F024).

---

## ⚠ VERIFY BEFORE PUBLISHING

- Zotero key not yet assigned.
- This is an **arXiv preprint from an AI governance vendor (Credo AI)** — not independently peer-reviewed at time of writing; when cited in P1 SLR, note vendor affiliation and frame as industry-research rather than fully independent academic literature (though methodology is transparent and the authors have a prior AAAI-published track record — cf. Sherman & Eisenberg 2024, cited within).
- Confirm whether a peer-reviewed/conference version has since been published (check for AAAI/FAccT 2025 proceedings versions before final citation).
- The "42 controls" / "50 risk scenarios" / "13/14 Colorado AI Act requirements mapped" figures are as self-reported by the authors; treat as framework-internal validation, not independently audited.

---

## Processing Status

- [x] PDF read in full (31 pages incl. full risk taxonomy and control library appendices)
- [x] Classified — Format B, Wiki Intake Note
- [x] Reusable findings extracted (5)
- [x] Cross-links identified
- [ ] Indexing pass (Corpus_Index_MOC, Instances in Corpus) — pending, end of Batch 6

---

## Log

- 2026-06-14: Processed as F026, Batch 6. Selected from raw corpus (Unified Control Framework / enterprise AI governance theme); confirmed not a duplicate — first comprehensive risk-taxonomy-to-control-to-regulation mapping framework in the corpus, complementary to F025's agentic-specific control catalogue.

---

_Back to [[Corpus_Index_MOC]] | [[PRIS_Master_MOC]]_
