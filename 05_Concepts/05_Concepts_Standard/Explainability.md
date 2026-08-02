---
type: Standard Concept
tags:
  - type/concept-standard
  - status/active
  - paper/p3
  - paper/p4
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - content/carousel-ready
---

# **Explainability**

**Type:** Standard Concept
**Status:** Active — created 2026-08-02 (EA-principle cluster intake)
**Last Updated:** 2026-08-02
**Theoretical Lineage:** XAI/HCI measurement; IS governance; regulatory governance
**Role in fsQCA:** Candidate constituent of the EA (Ethical Alignment) outcome condition — see [[fsQCA_Thesis_Chapter]] decision D4

---

## **Definition**

Explainability is defined in this research programme as the property of an AI system whereby a representation of the mechanisms underlying its operation can be produced, at a fidelity and in a register appropriate to the recipient and the decision's consequence. It is deliberately held apart from two neighbouring constructs. It is distinct from [[Transparency]], which concerns the *visibility and availability* of governance information about a system — an opaque model can be highly transparent in this sense, with published model cards, audit trails and documented controls, while remaining unexplainable. It is also distinct from **interpretability**, which per NIST concerns whether a human can derive *meaning* from an output relative to the system's designed functional purpose. Explainability is about mechanism; interpretability is about meaning; transparency is about disclosure. Instruments in the corpus routinely collapse all three, and that collapse is itself a coding observable.

## **Application in This Research**

Within [[P3_BFSI_JEIM]], explainability appears as a coded obligation in RBI and SEBI instruments, almost always bundled with transparency rather than specified separately — the bundling is analytically significant because it means Indian instruments impose no independent explainability standard that could be audited against. Within [[P4_Doctrinal_IJLIT]], explainability is the doctrinal hinge of the India/EU divergence: the EU AI Act Article 86 creates a right to explanation of individual decision-making, while no Indian BFSI instrument creates a corresponding statutory entitlement (see the HCJP finding recorded in [[Transparency]]). Within [[fsQCA_Thesis_Chapter]], explainability is a candidate constituent of the EA condition, and is the construct in the cluster with the *best-developed* measurement literature — which makes it the natural calibration reference case against which the weaker constructs are benchmarked.

## **Measurement & Calibration**

Two validated instruments exist, both user-facing and Likert-based:

| Instrument | Source | Structure | Calibration use |
|---|---|---|---|
| **System Causability Scale (SCS)** | Holzinger, Carrington & Müller, *KI – Künstliche Intelligenz*, Jan 2020 | 10-item Likert; measures "causability" — the degree to which an explanation achieves causal understanding with effectiveness, efficiency and satisfaction in a specified context of use | Continuous, bounded → direct fuzzy-set membership after anchor selection |
| **XAI Trust Scale** | Hoffman et al., *Frontiers in Computer Science*, Feb 2023 | Likert; confidence, predictability, reliability, efficiency, believability | Secondary/triangulating instrument |

**Critical caveat for D4:** both instruments measure *received* explanation quality from a human subject. Neither measures the explainability of a **governance regime**, which is the unit of analysis in this thesis. Applying SCS to a regulatory instrument is a category error. What is transferable is its underlying construct decomposition (effectiveness / efficiency / satisfaction), which can be re-specified at the regime level as: does the instrument specify *what must be explained*, *to whom*, and *at what fidelity*. Recommend calibrating on that three-part specification rather than importing SCS wholesale.

NIST AI RMF sub-function **MEASURE 2.9** provides the closest regime-level anchor: "The AI model is explained, validated and documented, and AI system output is interpreted within its context to inform responsible use and governance," with named artifacts including SHAP/LIME explainability reports.

## **Regulatory Definitions (Operative Text)**

| Instrument | Locus | Operative text / status |
|---|---|---|
| **NIST AI RMF 1.0** (Jan 2023) | Trustworthiness characteristic 5 of 7 | "Explainability refers to a representation of the mechanisms underlying AI systems' operation, whereas interpretability refers to the meaning of AI systems' output in the context of their designed functional purposes." **The only framework that formally separates the two constructs** |
| **OECD AI Principles** (2019, amended 3 May 2024) | Principle 1.3(iii) | "where feasible and useful, to provide plain and easy-to-understand information on the sources of data/input, factors, processes and/or logic that led to the prediction, content, recommendation or decision, to enable those affected by an AI system to understand the output" — note the double hedge, "where feasible and useful" |
| **UNESCO Recommendation** (Nov 2021) | Art. 42, Transparency & Explainability | "The level of T&E should be appropriate to the context, as there may be tensions between T&E and other principles such as privacy, safety and security" — explainability is expressly made defeasible |
| **EU AI Act** | No dedicated article | Distributed across Art. 13 (information to deployers), Art. 86 (right to explanation of individual decision-making), Recital 27; bias-side via Art. 10(2)(f)–(g) |
| **India** | — | No instrument defines explainability independently. NCAIC bundles it as "Transparency and Explainability" (model cards, datasheets, provenance metadata); MeitY's seven sutras render it as "Understandable by Design"; RBI FREE-AI treats it as a barrier to Gen-AI adoption rather than an obligation |

**Deontic observation for [[Deontic_Bifurcation]]:** OECD 1.3(iii) and UNESCO Art. 42 both attach explicit defeasibility conditions ("where feasible and useful"; "appropriate to the context") to an otherwise advisory deontic. This is a second-order bifurcation — not merely should-vs-shall, but a *should* qualified by a feasibility test that the obligated party itself evaluates. Worth coding as a distinct ADICO condition type.

## **Boundary Conditions**

- Explainability is not transparency and not interpretability; see Definition. Where an instrument uses the terms interchangeably, code the bundling, not the intent.
- Post-hoc explanation methods (SHAP, LIME, PDP, ALE) are *techniques for producing* explanations, not evidence that explainability obligations are met — the CFPB Circular 2022-03 explanation-accuracy requirement is the corpus's clearest statement of this gap.
- Explainability obligations directed at supervisors differ in kind from those directed at affected individuals. India has the former, not the latter.

## **Measurement Risk**

*Investigating the Duality of Interpretability and Explainability* (arXiv, 26 Mar 2025) states there is "a lack of comprehensive quantitative evaluation metrics for various explainable ML techniques" and "a lack of standardized quantitative measures to facilitate their comparison." Treating explainability as a stable cross-case-comparable fsQCA input without acknowledging this heterogeneity is not defensible. Declare the measurement basis explicitly in the methodology chapter.

## **Literature Anchors**

Per PRIS convention, references live in Zotero; recorded here for coding continuity only.

- Phillips, Hahn, Fontana, Yates, Greene, Broniatowski & Przybocki (2021). *Four Principles of Explainable Artificial Intelligence.* NIST IR 8312. — Explanation, Meaningful, Explanation Accuracy, Knowledge Limits. Positions explainability as measurable, not merely normative.
- Broniatowski et al. (2021). *Psychological Foundations of Explainability and Interpretability in AI.* NIST IR 8367. — Source of the explainability/interpretability separation later carried into AI RMF 1.0.
- Holzinger, Carrington & Müller (2020). *The System Causability Scale.* KI – Künstliche Intelligenz.
- Hoffman, Mueller, Klein & Litman (2023). *Measures for Explainable AI.* Frontiers in Computer Science.
- *Investigating the Duality of Interpretability and Explainability* (2025). arXiv 2503.21356.

## **Instances in Corpus**

- [[04_Knowledge_Products/Wiki_Intake/F085_Sudjianto_Zhang_Model_Validation_Practice_Banking_2024]] — the corpus's most granular explainability-*methods* taxonomy (SHAP/LIME/PDP/ALE, interpretable architectures, fANOVA decomposition). Supplies the techniques that would satisfy a post-hoc explanation-accuracy requirement. Previously unwired to any concept.
- [[04_Knowledge_Products/Wiki_Intake/F040_ELI_Guiding_Principles_ADM_EU]] — Principles 5 (Traceable Decisions) and 6 (Reasoned Decisions): traceability is necessary but not sufficient for explanation; opacity is not a valid ground for an unreasoned decision. The corpus's sharpest statement that logging ≠ explaining.
- [[04_Knowledge_Products/Wiki_Intake/International_12_HCJP_Legal_AI_BFSI_2025]] — right to explanation in financial services as a statutory consumer entitlement under EU AI Act + MiFID II/CRD, against which India's supervisory-only framing is the contrast case.
- [[04_Knowledge_Products/Wiki_Intake/F046_UK_LawCommission_AI_and_Law_DiscussionPaper_2025]] — Theme 5 (Opacity): courts cannot establish causation without understanding AI decisions. The doctrinal consequence of unexplainability.
- [[04_Knowledge_Products/Wiki_Intake/F115_Verma_Sentiment_Analysis_Smart_Society_2022]] — sub-symbolic vs symbolic framing (Calegari, Ciatto & Omicini 2020); practitioner-register account of the transparency/performance trade-off.
- [[04_Knowledge_Products/Wiki_Intake/Tammenga_AI_3LoD_Banks_2020]] and [[04_Knowledge_Products/Wiki_Intake/Eisenberg_Gamboa_Sherman_Unified_Control_Framework_2025]] — explainability as a second-line validation obligation within three-lines architectures.
- [[04_Knowledge_Products/Wiki_Intake/Sejwal_Gupta_ADM_Indian_Credit_Scoring_2026]] — India-side ADM credit scoring; the nearest thing to an Indian explainability case study in the corpus.
- [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] — "Transparency and Explainability" as one of eight foundational design principles (model cards, datasheets, provenance metadata). India's most explicit explainability specification, in a non-binding framework.
- [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] — explainability appears as a *reason for non-adoption* (67% of surveyed entities reluctant on customer-facing Gen AI partly on explainability grounds), not as an obligation. Analytically inverted framing.

- **(2026-08-02)** [[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]] — Explainability is one of only three principles AI Verify subjects to **technical testing** (with Fairness and Robustness), the other eight of eleven being process checks. Practitioner-side corroboration of this note's finding that explainability has the best-developed measurement literature of the EA cluster.
- **(2026-08-02)** [[07_Institutions/Corpus/International/International_34_MAS_FEAT_Veritas_AI_MRM]] — MAS FEAT Transparency principles 12–14 and **Veritas Doc 3C** supply a regime-level transparency/explainability assessment methodology; note that FEAT bundles the two constructs, consistent with this note's finding that instruments routinely collapse them.

## **Future Reuse Opportunities**

- The explainability / interpretability / transparency triad, with NIST as the only framework that separates them, is a publishable short piece and a clean carousel.
- The "second-order defeasibility" observation (OECD 1.3(iii), UNESCO Art. 42) feeds directly into [[Deontic_Bifurcation]] as a new condition type — designed defeasibility, distinct from designed and emergent bifurcation already recorded there.
- Regime-level re-specification of SCS (what / to whom / at what fidelity) is a methodological contribution in its own right if the thesis needs one.

## **Linked Projects**

[[P3_BFSI_JEIM]]

[[P4_Doctrinal_IJLIT]]

[[fsQCA_Thesis_Chapter]]

## **Linked Domains**

[[AI_Governance]]

[[BFSI_Governance]]

## **Linked Standard Concepts**

[[Transparency]]

[[Accountability]]

[[Fairness]]

[[Human_Oversight]]

[[Contestability_Redress]]

## **Linked Signature Concepts**

[[Deontic_Bifurcation]]

[[Evidentiary_Governance]]

## **Linked Frameworks**

[[NIST_AI_RMF]]

[[EU_AI_Act]]

[[OECD_AI_Principles]]

[[UNESCO_Recommendations]]

[[RBI_Free_AI]]

## **Linked Methods**

[[fsQCA]]

---

_Back to [[_Concepts_MOC]]_
