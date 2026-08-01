---
node_id: F085
series: Format_B
title: "Model Validation Practice in Banking: A Structured Approach for Predictive Models"
short_ref: "Sudjianto & Zhang (H2O.ai/Wells Fargo/UNC Charlotte), 2024"
wiki_section: S6, S1
tier: High
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/model-risk-management
  - topic/explainability
  - topic/model-validation
  - topic/credit-scoring
  - institution/wells-fargo
  - institution/h2o-ai
date_ingested: 2026-07-15
verify_flags: 0
---

# F085 — Sudjianto, A. & Zhang, A. *Model Validation Practice in Banking: A Structured Approach for Predictive Models.* Revision 10/15/2024, 37 pp.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Authors** | Agus Sudjianto (H2O.ai; University of North Carolina at Charlotte); Aijun Zhang (Wells Fargo) |
| **Publishing context** | Independent academic/industry preprint or whitepaper — authors note views do not necessarily reflect Wells Fargo's |
| **Revision date** | 10/15/2024 |
| **Pages** | 37 |
| **Document type** | Academic/industry technical research paper |

---

## Classification

**Document type:** Academic/Industry Research Paper (technical methodology)
**Primary audience:** Model risk management practitioner / quantitative validator / ML engineer
**AI explicit:** Yes — traditional predictive-model validation with explicit extensibility claim to Generative AI
**Confidence tier:** **High** — technically rigorous, no ambiguous/contradictory items identified in the extraction itself, senior industry (Wells Fargo model-risk practitioner) + academic (H2O.ai/UNC Charlotte) co-authorship. Note: Sudjianto is affiliated with H2O.ai, a commercial interpretable-ML platform vendor, and the paper references the **PiML toolbox** (from the same research lineage) — a mild tool-affiliation context worth noting, though this does not appear to distort the paper's technical content, which is methodologically standard and well-grounded in established statistics (KS test, PSI, SHAP, LIME are all widely-used, non-proprietary methods).

---

## 3–5 Reusable Findings

1. **Three-component model validation framework, extending SR11-7** (feeds S1/S6): Conceptual Soundness Evaluation → Outcome Analysis → Ongoing Monitoring. This directly operationalises the high-level development/validation/governance triad from [[04_Knowledge_Products/Wiki_Intake/Fed_OCC_SR11-7_Model_Risk_Management_2011]] (2011) into granular, technically specific validation steps — the corpus's most detailed technical bridge between SR11-7's principles-level framework and actual ML validation practice, 13 years later.

2. **Explicit CFPB Circular 2022-03 regulatory hook** (feeds S2/S6): "CFPB Circular 2022-03 clarifies that creditors using complex algorithms for credit decisions must comply with the Equal Credit Opportunity Act (ECOA) by providing specific reasons for any adverse actions... Creditors must also ensure the accuracy of any post-hoc explanations." CFPB is already referenced elsewhere in the corpus ([[04_Knowledge_Products/Wiki_Intake/Turk_Overlapping_Legal_Rules_Financial_Regulation_2020]], [[04_Knowledge_Products/Wiki_Intake/IAPP_AIGP_Body_of_Knowledge_v21_2026]], International_8, International_9), but this is the corpus's most specific, actionable CFPB obligation citation — a named circular with a concrete adverse-action-explanation and post-hoc-explanation-accuracy requirement — directly comparable to India's absence of an equivalent ECOA-style mandate for AI-driven credit scoring (cf. [[04_Knowledge_Products/Wiki_Intake/Sejwal_Gupta_ADM_Indian_Credit_Scoring_2026]]).

3. **Comprehensive explainability/interpretability technical taxonomy** (feeds S6, teaching): Post-hoc tools (PDP, ALE, SHAP, LIME) vs. inherently interpretable architectures (Deep ReLU networks as piecewise-linear functions, Boosted Linear Trees/LightGBM with linear leaf models, functional ANOVA/fANOVA decomposition into main effects and low-order interactions). This is the most granular explainability-methods taxonomy in the corpus, complementing the documentation-*standard* pair already ingested ([[04_Knowledge_Products/Wiki_Intake/F080_Mitchell_et_al_Model_Cards_for_Model_Reporting_2019]], [[04_Knowledge_Products/Wiki_Intake/F081_Gebru_et_al_Datasheets_for_Datasets_2018]]) with the actual technical *methods* those documentation standards would need to report.

4. **Distribution-shift/drift-detection statistical method taxonomy** (feeds S6): Univariate (KS test, Jensen-Shannon Divergence, KL Divergence, Wasserstein Distance, Total Variation Distance) and multivariate (Energy Distance, Maximum Mean Discrepancy, reconstruction-error, Mahalanobis Distance) methods for data-drift detection, plus a separate five-method taxonomy for concept-drift detection (nearest-neighbour input-distribution control, performance monitoring over time, residual drift monitoring, retraining comparison, segment-level error tracking). Directly actionable technical content for any ongoing-monitoring obligation in the corpus (e.g., RBI FREE-AI's model-monitoring principles, DPDP Rules SDF algorithmic due-diligence).

5. **Explicit GenAI-extensibility claim** (feeds S1, forward-looking): The conclusion states "the principles for model validation discussed here are also applicable to validation of more complex models including Generative AI — though the detail testing approaches will be different." A direct, citable bridge from traditional predictive-model validation literature to GenAI validation, relevant to any argument that existing model-risk-management regimes (SR11-7, RBI's draft model-risk circular) are extensible to GenAI rather than requiring wholly new frameworks.

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The three-component validation framework (Finding 1) and the drift-detection method taxonomy (Finding 4) are directly reusable as a technical validation checklist for any AI/ML model-risk diagnostic engagement.
**Consulting connections:** Direct relevance to any BFSI AI-governance advisory work involving credit-scoring or predictive-model validation (AEGIS_OS-adjacent technical-governance conversations would also benefit from the drift-monitoring taxonomy).
**Teaching connection:** The explainability-methods taxonomy (Finding 3) is strong technical teaching material bridging governance-level "explainability is required" statements to the actual methods (SHAP/LIME/PDP/ALE) that satisfy them.

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S6, S1
**Concepts:** [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Transparency]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/Fed_OCC_SR11-7_Model_Risk_Management_2011]] (direct technical extension of the SR11-7 triad); [[07_Institutions/Corpus/RBI/RBI_3]] (India's draft model-risk circular — same-year technical-depth comparator); [[04_Knowledge_Products/Wiki_Intake/Kurshan_Shen_Chen_AI_Model_Governance_2020]] and [[04_Knowledge_Products/Wiki_Intake/Rao_Scepanovic_AI_Model_Risk_Catalog_2025]] (model-governance/model-risk-catalog cluster); [[04_Knowledge_Products/Wiki_Intake/F080_Mitchell_et_al_Model_Cards_for_Model_Reporting_2019]] and [[04_Knowledge_Products/Wiki_Intake/F081_Gebru_et_al_Datasheets_for_Datasets_2018]] (documentation-standard companions — this paper supplies the technical methods those standards report); [[04_Knowledge_Products/Wiki_Intake/Sejwal_Gupta_ADM_Indian_Credit_Scoring_2026]] (India credit-scoring ADM comparator to the CFPB/ECOA obligation)
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes
- [ ] Marked processed

---

## Log

- 2026-07-15: Wiki intake note created. NotebookLM extraction relay, PROMPT 0b. Duplicate check run against "Sudjianto," "Aijun Zhang," "PiML," "Model Validation Practice in Banking" — no prior match; confirmed new node. Classified Format B (High-tier academic/industry technical paper). No VERIFY flags required — extraction identified no ambiguous items.
