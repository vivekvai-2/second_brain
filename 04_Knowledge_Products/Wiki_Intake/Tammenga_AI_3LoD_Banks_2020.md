---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - engine/phd
  - theme/3lod
  - theme/model-risk
  - theme/ai-governance
---

# Tammenga (2020) — The Application of AI in Banks in the Context of the Three Lines of Defence Model

**Source:** Alette Tammenga (2020), *Maandblad voor Accountancy en Bedrijfseconomie* (MAB) 94(5/6): 219–230, DOI 10.5117/mab.94.47158
**Year:** Received Oct 2019 / Published 30 June 2020
**Full title:** "The application of Artificial Intelligence in banks in the context of the three lines of defence model"
**File ID:** F021
**Zotero key:** ⚠ VERIFY — not yet assigned
**Wiki section(s):** S6 (Model Risk) / S4 (Agentic AI Governance, precursor framing) / S1 (Governance Fundamentals)
**Confidence:** High (peer-reviewed practitioner-academic journal; author is a risk-management consultant, Transcendent Group NL)
**Jurisdiction:** Netherlands / EU (general, FSB/BCBS-referenced — not India-specific)

---

## Classification

Academic/practitioner research article applying the IIA's Three Lines of Defence (3LoD) model to AI/ML deployment in banks. Pre-dates the IIA's 2020 "Three Lines Model" rebrand (cf. F003) but is the **earliest item in the corpus to explicitly map AI/ML use cases onto 3LoD structure** — establishes the doctrinal starting point for the lineage already captured via F006 (SR 11-7, 2011) → F008 (Davies & Zhivitskaya, 2018) → F009 (Bantleon et al., 2020) → F010 (Arndorfer & Minto, 2015) → F003 (IIA, 2024) → F007 (Schuett, 2023) → F013 (Kurshan, Shen & Chen, 2020). Tammenga (2020) sits chronologically between Davies & Zhivitskaya (2018) and the IIA's later "Three Lines Model" update, and is one of the first to operationalise 3LoD specifically for AI/ML (as opposed to general model risk).

---

## Reusable Findings

1. **3LoD mapping of AI/ML use cases by line (feeds S6):** Empirical taxonomy (Fig. 2) places AI/ML applications predominantly in the *first line* (chatbots, robo-advice, market-risk portfolio monitoring) and *first-and-second-line joint* applications (credit risk modelling/approval, transaction monitoring/AML, fraud detection, regulatory capital optimisation). Critically, **no AI/ML applications were observed in the third line (internal audit) as of 2020** — a baseline that can be compared against later corpus nodes (e.g., F007 Schuett 2023, F013 Kurshan et al. 2020) to track whether internal-audit AI adoption has since materialised.

2. **"Role-based" 3LoD operationalisation for AI/ML models (feeds S6/S4):** Drawing on Burt et al. (2018), the paper proposes assigning five functional roles — Data Owners, Data Scientists, Business Owners (1st line); Validators and Governance Personnel (2nd line); Internal Audit (3rd line) — as a more granular alternative to applying 3LoD wholesale to AI/ML projects. This role-based decomposition is a reusable framework for **agentic AI governance RACI design** (P3/P4) where traditional 3LoD boundaries blur because the same function (e.g., risk management) may both build and oversee a model.

3. **"Materiality-proportionate" 3LoD intensity principle (feeds S6):** The paper argues the *intensity and frequency* of 2nd/3rd line involvement should scale with model materiality/impact — an early articulation of the **risk-tiering logic** later formalised in EU AI Act risk categories and RBI FREE-AI's proportionality principle (cf. RBI_FREE_AI_2025). Useful as a **pre-2023 precedent** for proportionality-based AI oversight design, strengthening [[Regulatory_Parallelism]] claims about convergent evolution.

4. **Explainability–accuracy trade-off as a governance decision point (feeds S6/S1):** Citing Burt et al. (2018), the paper frames the explainability/accuracy trade-off not as a technical constant but as a **documented governance decision** subject to challenge by other 3LoD functions — i.e., the trade-off itself becomes an auditable artefact. This is a reusable diagnostic for [[Institutional_Coherence]]: regulatory frameworks that fail to require documentation of this trade-off (rather than just "explainability" in the abstract) may have a coherence gap.

5. **Systemic-risk channel: collective/herd adoption of AI/ML (feeds S6/S2):** Citing FSB (2017), the paper identifies a **macro-prudential channel** distinct from firm-level model risk — if multiple institutions converge on similar AI/ML-driven strategies using common data sources, a shock to those sources could propagate system-wide ("single node" effect). This pre-figures more recent "third-party concentration risk" framings (cf. FSB Third-Party Risk Management reports in corpus) and is a useful **systemic-risk citation anchor** for P1 SLR sections on AI-driven financial stability risk, predating by ~5 years the more developed treatments in BIS/FSB 2024–25 papers.

---

## Consulting / Teaching Reuse

- The **5-role 3LoD operationalisation table** (Data Owner / Data Scientist / Business Owner / Validator / Governance Personnel) is directly reusable as a slide/checklist for board-level AI governance training — maps cleanly onto practitioner audiences (CISOs, CROs) familiar with 3LoD vocabulary but unfamiliar with AI-specific role allocation.
- The **"no AI in third line yet" (2020) vs. now** framing is a strong before/after hook for a LinkedIn post on internal-audit AI maturity, especially paired with F013 (Kurshan et al., AI/ML model governance, 2020) and more recent agentic-AI-audit corpus items (e.g., "Industry News 2025 — The Growing Challenge of Auditing Agentic AI").
- The **materiality-proportionate oversight principle** is reusable in P3/P4 as an early (2020) conceptual antecedent to RBI FREE-AI's proportionality approach — useful for the regulatory-parallelism "convergent evolution" argument (concepts converge across jurisdictions and time independent of direct citation).

---

## Cross-Links

- [[04_Knowledge_Products/Wiki_Intake/Davies_Zhivitskaya_3LoD_2018]] — Tammenga cites Davies & Zhivitskaya's critique of 3LoD ("false sense of security" when three groups share responsibility); extends this critique specifically to AI/ML governance.
- [[04_Knowledge_Products/Wiki_Intake/Kurshan_Shen_Chen_AI_Model_Governance_2020]] (F013) — contemporaneous (2020) treatment of AI/ML model governance vs. traditional MRM; Tammenga's 3LoD-role framework complements Kurshan et al.'s MRM-lifecycle framing.
- [[04_Knowledge_Products/Wiki_Intake/IIA_Three_Lines_Model_2024]] (F003) — Tammenga (2020) pre-dates and is superseded in doctrinal terms by IIA's 2020/2024 "Three Lines Model" update; useful as the "applied to AI" companion piece the IIA model itself does not provide.
- [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] — proportionality/materiality principle parallels RBI FREE-AI's risk-tiered oversight approach (see [[Regulatory_Parallelism]]).
- [[Institutional_Coherence]] — explainability/accuracy trade-off documentation requirement as a coherence diagnostic.
- [[Agentic_AI_Governance]] — role-based decomposition (Data Owner/Scientist/Validator/Governance) as a precursor framework for agentic AI RACI matrices.

---

## ⚠ VERIFY BEFORE PUBLISHING

- Zotero key not yet assigned — add on next Zotero sync.
- Confirm whether Tammenga (2020) has been cited by any of the corpus's 2023–2025 3LoD/AI papers (e.g., F007 Schuett, F013 Kurshan et al.) — if so, this strengthens the doctrinal lineage claim; if not, treat the lineage as thematic/structural similarity only (per the caution already applied to flag #6, International_4 FEAT→sutras).

---

## Processing Status

- [x] PDF read in full (12 pages incl. references)
- [x] Classified — Format B, Wiki Intake Note
- [x] Reusable findings extracted (5)
- [x] Cross-links identified
- [ ] Indexing pass (Corpus_Index_MOC, Instances in Corpus) — pending, end of Batch 6

---

## Log

- 2026-06-14: Processed as F021, Batch 6. Identified via direct raw-corpus selection (3LoD/Model-Risk theme), confirmed not a duplicate of F003/F006/F007/F013.

---

_Back to [[Corpus_Index_MOC]] | [[PRIS_Master_MOC]]_
