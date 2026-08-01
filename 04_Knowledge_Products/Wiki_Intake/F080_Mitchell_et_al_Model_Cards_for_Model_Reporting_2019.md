---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - topic/model-documentation
  - topic/ai-fairness
  - topic/transparency
  - institution/google-research
---

# Model Cards for Model Reporting — Intake Note

**Source:** Google Research (+ University of Toronto — Raji)
**Year:** 2019 (FAT* '19, 29–31 January 2019)
**Full title:** Model Cards for Model Reporting
**File ID:** F080
**Zotero key:** [blank]
**Wiki section(s):** S6 (Implementation & Governance Artifacts — primary), S1 (Governance Fundamentals — secondary, bias/disaggregated-evaluation evidence)
**Confidence:** High (ACM peer-reviewed conference paper, FAT* '19; foundational, widely-cited standard; DOI 10.1145/3287560.3287596)
**Jurisdiction:** Global (technical documentation standard, not jurisdiction-specific)

**Note:** This is one of two papers deliberately sourced via a Perplexity Deep Research prompt to fill the vault's Domain III (AI Development Governance) gap identified in this session's AIGP BoK (F055) analysis — model documentation standards were previously referenced only as a taxonomy item inside International_20's AIIA Tool, never ingested as a primary source. Companion paper: Gebru et al., "Datasheets for Datasets" (pending, same sourcing pass).

---

## Classification

**Document type:** Academic Paper (ACM conference proceedings)
**Primary audience:** Researcher / Practitioner (ML engineers, model developers, AI governance/procurement reviewers)
**AI explicit:** Yes

---

## 3–5 Reusable Findings

1. **Nine-section Model Card template** (feeds S6): Model Details, Intended Use, Factors, Metrics, Evaluation Data, Training Data, Quantitative Analyses, Ethical Considerations, Caveats and Recommendations — the foundational model-documentation standard the vault's own International_20 (Australia AIIA Tool) references generically as "System factsheet/model card" without ever citing the source. This node closes that citation gap.

2. **Disaggregated and intersectional evaluation as a documentation requirement** (feeds S1/S6): The paper recommends performance metrics be broken down by individual and intersectional demographic/cultural/phenotypic groups, grounding this in Buolamwini's facial-recognition bias finding and the US FDA's 1998 mandate for disaggregated clinical-trial data by age/race/gender — a precedent-based argument for disaggregated AI evaluation reporting. Directly complements [[04_Knowledge_Products/Wiki_Intake/F076_CeRAI_IITM_Biased_LMs_Academic_Recommendations_2025]]'s empirical bias findings with the documentation-standard side of the same problem.

3. **Precise fairness-metric equivalence definitions** (feeds S6): "Equal false negative rates across groups is equivalent to fulfilling Equality of Opportunity, and equal false negative and false positive rates across groups is equivalent to fulfilling Equality of Odds" — technical-fairness vocabulary that bridges the corpus's legal/rights-based fairness framing (F039's rights-harm mapping) and ML technical evaluation metrics.

4. **Two fully worked model-card examples** (feeds S6): A "Smiling Detection in Images" card (CelebA dataset) and a "Toxicity in Text" card (Jigsaw/Perspective API), the latter explicitly used to argue that model cards must be versioned and updated as models drift over time ("the drastic ways that models can change over time"). Directly reusable teaching/consulting exemplars — a template a client can be walked through section-by-section.

5. **Model cards positioned as necessary but insufficient** (feeds S5/S6): The paper explicitly frames model cards as "one transparency tool among many," alongside third-party algorithmic auditing and adversarial testing — situating this documentation standard within a broader accountability ecosystem that includes [[04_Knowledge_Products/Wiki_Intake/F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations]]'s third-party evaluation standard.

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The nine-section template is directly reusable in any AI vendor-risk-assessment or AI procurement engagement requiring a documentation checklist.
**Consulting connections:** None of the three named inbounds map directly.
**Teaching connection:** The two worked examples (Smiling Classifier, Toxicity Scoring) are strong, ready-to-use classroom exemplars for a model-documentation/transparency module.

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S6, S1
**Concepts:** [[05_Concepts/05_Concepts_Standard/Transparency]], [[05_Concepts/05_Concepts_Standard/Accountability]]
**Corpus nodes:** [[07_Institutions/Corpus/International/International_20_Australia_DTA_AI_Impact_Assessment_Tool]] (cites model cards/datasheets as a documentation type — this node is the primary source that citation was missing); [[04_Knowledge_Products/Wiki_Intake/F076_CeRAI_IITM_Biased_LMs_Academic_Recommendations_2025]] (empirical bias evidence this documentation standard is designed to surface); [[04_Knowledge_Products/Wiki_Intake/F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations]] (complementary third-party evaluation standard)
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
| #223 | The paper's Toxicity Scoring example (Section 5.2) references "TOXICITY v.1" and "TOXICITY v.5" but the worked mock card itself only states "Developed by Jigsaw in 2017" without mapping that date to a specific version — minor internal ambiguity, low citation risk given this is illustrative rather than a factual claim about Jigsaw's actual product | LOW |

---

## Log

- 2026-07-15: Wiki intake note created. NotebookLM extraction relay, PROMPT 0b. Ad hoc pre-Batch 19 session. First of two papers sourced via Perplexity Deep Research to fill the S6/Domain III model-documentation-standards gap identified in this session's AIGP BoK (F055) analysis. Duplicate check run against "Model Cards," "Mitchell," "Model Cards for Model Reporting" — no prior match; confirmed new node.
