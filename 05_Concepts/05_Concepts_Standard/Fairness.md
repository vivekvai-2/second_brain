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

# **Fairness**

**Type:** Standard Concept
**Status:** Active — created 2026-08-02 (EA-principle cluster intake)
**Last Updated:** 2026-08-02
**Theoretical Lineage:** Algorithmic fairness (statistical); anti-discrimination law; regulatory governance
**Role in fsQCA:** Candidate constituent of the EA (Ethical Alignment) outcome condition — see [[fsQCA_Thesis_Chapter]] decision D4
**Calibration status:** ⚠ **Blocked pending metric-family declaration — see Measurement Risk**

---

## **Definition**

Fairness is defined here as the property of an AI-supported decision process whereby differential treatment or differential outcome across protected or salient groups is either absent or justified by a legitimate, stated and reviewable ground. The definition deliberately admits both a *treatment* limb and an *outcome* limb, because the corpus's instruments split along exactly that line and the split is a coding observable. Bias is treated as subordinate to fairness in this ontology — bias is a mechanism producing unfairness, not a separate construct, and does not receive its own note.

The construct's defining feature, and the reason it is handled differently from every other concept in this vault, is that its principal formalisations are **provably mutually incompatible**. Fairness is simultaneously the best-instrumented and the most formally contested construct in the EA cluster.

## **Application in This Research**

Within [[P3_BFSI_JEIM]], fairness appears in RBI FREE-AI's consumer-protection pillar and in the recommended amendment to the Digital Lending Directions requiring fairness audits of AI-driven credit assessments — recommendations, not operative obligations. Within [[P4_Doctrinal_IJLIT]], fairness is the clearest instance of an Indian instrument naming a principle without specifying a test: no Indian instrument states which fairness criterion applies, which means no Indian fairness obligation is presently auditable. Within [[fsQCA_Thesis_Chapter]], fairness is a candidate EA constituent whose calibration cannot proceed until a metric family is declared — see below.

## **Measurement & Calibration**

Three metric families, following Barocas, Hardt & Narayanan's standard taxonomy:

| Family | Criterion | Typical metric |
|---|---|---|
| **Independence** | Prediction independent of protected attribute | Demographic / statistical parity |
| **Separation** | Prediction independent of attribute *given* the true outcome | Equalized odds; equality of opportunity |
| **Sufficiency** | True outcome independent of attribute *given* the prediction | Calibration within groups |

Two anchors with unusual calibration value:

- **The four-fifths rule** — a legally codified numeric threshold: the selection rate for the protected group must be at least 80% of that for the comparison group. This is one of very few fairness thresholds with statutory force anywhere, which makes it a defensible crisp-set anchor or fuzzy crossover point. ⚠ **Provenance correction:** the Perplexity return attributed this to Romei et al. (2013). It is not theirs. It originates in the US EEOC *Uniform Guidelines on Employee Selection Procedures* (1978), 29 CFR §1607.4(D); Romei & Ruggieri's survey merely cites it. Cite the regulation, not the survey.
- **Speicher et al. (2018) fairness index** — decomposable into between-group and within-group components, rooted in economic inequality-index literature. The decomposability is the useful property: it yields a continuous bounded score suitable for direct fuzzy calibration, unlike binary parity tests.

## **Measurement Risk — the impossibility results (read before calibrating)**

This is the single most consequential finding from the EA-cluster sourcing pass.

**Kleinberg, Mullainathan & Raghavan's impossibility theorem** (restated as Theorem 2.1 in *Communications of the ACM*, Jan 2024) proves that calibration within groups, balance for the positive class, and balance for the negative class **cannot simultaneously hold**, except in two degenerate cases: perfect prediction, or equal base rates across groups. Neither holds in any realistic governance setting. *Philosophy & Technology* (Oct 2024) restates the general result: an error-prone predictive model cannot simultaneously satisfy two plausible fairness criteria.

**Direct consequence for D4:** a single scalar "fairness" membership score is not theoretically coherent unless the metric family is declared in advance. Calibrating fairness without that declaration would embed an undisclosed normative choice into the outcome variable — precisely the kind of move a *Regulation & Governance* or GIQ reviewer is equipped to catch. Three defensible options, in descending order of preference:

1. **Declare the family.** Calibrate on separation (equalized odds) and state that independence and sufficiency criteria are thereby not satisfied by construction. Defensible, transparent, and requires only a sentence of justification.
2. **Calibrate on specification rather than satisfaction.** Score the *instrument*, not the system: does the instrument name a fairness criterion at all? This sidesteps the impossibility problem entirely and is better aligned with an institutional-design thesis than a technical-audit one. **Recommended** — and it produces a striking finding, since on this measure every Indian instrument scores at or near zero membership.
3. Drop fairness from EA and retain it as a descriptive domain property.

**Counter-source, for balance:** Bell et al. (arXiv 2302.06347, 2023) empirically show across five real-world datasets that many models satisfy multiple fairness criteria simultaneously within small error margins — the impossibility result binds tightly in theory and loosely in practice. The critique is itself contested. Note both.

## **Regulatory Definitions (Operative Text)**

| Instrument | Locus | Operative text / status |
|---|---|---|
| **EU AI Act** | Art. 10(2)(f) | "examination in view of possible biases that are likely to affect the health and safety of persons, have a negative impact on fundamental rights or lead to discrimination prohibited under Union law, especially where data outputs influence inputs for future operations" |
| | Art. 10(2)(g) | "appropriate measures to detect, prevent and mitigate possible biases identified according to point (f)" |
| | Art. 10(3) | datasets "shall be relevant, sufficiently representative, and to the best extent possible, free of errors and complete" |
| **NIST AI RMF 1.0** | Characteristic 7 of 7 | "Fair with Harmful Bias Managed — The system addresses equality and equity, and manages systemic, computational/statistical and human-cognitive biases across the lifecycle" |
| **OECD** | Principle 1.2 | Subsumed within "human-centred values and fairness"; no standalone measurement clause |
| **UNESCO** | Named value | "Fairness and non-discrimination"; no operative test |
| **India — NCAIC** | Principle 6 of 8 | "Inclusivity and Fairness (bias testing across Indian demographics/languages/cultures)"; Fairness is also one of five mandatory evaluation gates — "demographic parity across Indian linguistic/regional/socioeconomic segments." **The only Indian instrument that names a specific criterion (demographic parity = independence family), and it is non-binding** |
| **India — MeitY** | Sutra 4 of 7 | "Fairness & Equity" |
| **India — RBI FREE-AI** | Consumer Protection pillar | Board-approved framework "prioritising transparency and fairness for AI-driven decisions"; recommended amendment to Digital Lending Directions 2025 adds "fairness audits" — Committee recommendation, not operative |

**Note the asymmetry:** the EU AI Act imposes a *process* obligation (examine, detect, mitigate) without specifying a criterion; NCAIC specifies a *criterion* (demographic parity) without binding force. No instrument in the corpus does both. That gap is a clean P4 finding.

## **Boundary Conditions**

- Fairness in this programme is a property of decision processes and of the instruments governing them, not of model artifacts in isolation.
- Bias folds into Fairness; do not create a separate Bias note.
- Fairness obligations phrased as dataset-quality requirements (AI Act Art. 10(3)) are analytically distinct from those phrased as outcome tests, and should be coded separately.

## **Literature Anchors**

- Chen, R.J. et al. (2023). *Algorithm Fairness in Artificial Intelligence for Medicine and Healthcare.* Nature Biomedical Engineering. — formal probability-notation definitions of demographic parity, equalized odds, equality of opportunity.
- Barocas, Hardt & Narayanan (2023). *Fairness and Machine Learning: Limitations and Opportunities.* MIT Press. — independence / separation / sufficiency taxonomy. ⚠ Perplexity returned this via a LinkedIn explainer; cite the book (fairmlbook.org), not the intermediary.
- Kleinberg, Mullainathan & Raghavan — impossibility theorem, as restated in *Communications of the ACM* (Jan 2024), "What Should We Do When Our Ideas of Fairness Conflict?"
- *What's Impossible About Algorithmic Fairness?* (2024). Philosophy & Technology.
- Bell, A. et al. (2023). *Revisiting the Impossibility Theorem in Practice.* arXiv 2302.06347.
- Speicher et al. (2018). *A Unified Approach to Quantifying Algorithmic Unfairness.* KDD. ⚠ returned via a personal blog; verify against the KDD proceedings before citing.
- EEOC (1978). *Uniform Guidelines on Employee Selection Procedures*, 29 CFR §1607.4(D) — four-fifths rule.

## **Instances in Corpus**

- [[04_Knowledge_Products/Wiki_Intake/F076_CeRAI_IITM_Biased_LMs_Academic_Recommendations_2025]] — CeRAI/IIT Madras: fully disclosed LLM fairness-audit methodology (DRS/GRS formulae, hyperparameters, prompt templates) with the recommendation that deployers compare new model versions against fairness baselines pre-deployment. **The corpus's only Indian-authored empirical fairness measurement work.** Previously fully isolated — zero inbound and zero outbound links.
- [[04_Knowledge_Products/Wiki_Intake/F123_Sloane_Moss_Chowdhury_Hiring_Algorithms_Auditability_2021]] — introduces epistemological-roots auditing: interrogate not merely output distribution but the validity of what the system claims to measure (the contested OCEAN Big-5 example). Fairness auditing that goes beneath parity metrics.
- [[04_Knowledge_Products/Wiki_Intake/Sejwal_Gupta_ADM_Indian_Credit_Scoring_2026]] — India-side automated credit scoring; the applied setting for RBI's recommended fairness audits.
- [[04_Knowledge_Products/Wiki_Intake/F127_Masiero_Biometric_Infrastructures_Indian_PDS_2020]] — exclusion effects of biometric authentication in the Indian PDS. Fairness as *access* rather than as prediction parity — a DPI-side framing not captured by any statistical metric. Links to [[DPI_Governance]].
- [[04_Knowledge_Products/Wiki_Intake/F121_Correa_Kluge_Worldwide_AI_Ethics_200_Guidelines_2023]] — fairness across 200 global AI ethics guidelines; the base rate against which India's specification gap can be quantified.
- [[04_Knowledge_Products/Wiki_Intake/F039_ICAAD_KWM_AI_Harm_Human_Rights]] — fairness recast as human-rights harm rather than statistical disparity.
- [[04_Knowledge_Products/Wiki_Intake/Hadley_Algorithm_Review_Boards_RAI_2025]] — algorithm review boards as an institutional (rather than metric) fairness mechanism.
- [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] — Principle 6 plus the Fairness evaluation gate specifying demographic parity across Indian linguistic/regional/socioeconomic segments. India's only named fairness criterion.
- [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] — fairness audits recommended for AI-driven credit assessment; not yet operative.

- **(2026-08-02 — the missing instrument class)** [[07_Institutions/Corpus/International/International_34_MAS_FEAT_Veritas_AI_MRM]] — **Veritas Document 3A, FEAT Fairness Principles Assessment Methodology** (MAS, 2022; open-source toolkit v1.0/v2.0; piloted on credit risk scoring and customer marketing). Assesses the *deploying institution's process*, not a human subject's perception — the level at which this thesis calibrates. Offers a **third route past the impossibility problem**: rather than declaring a metric family or scoring specification, assess whether the institution has run a defensible fairness assessment process. Evaluate against the two options above before D4 is settled.
- **(2026-08-02)** Fairness is one of only **three principles AI Verify tests technically** (with Explainability and Robustness), consistent with its status here as the best-instrumented but most formally contested construct.

## **Future Reuse Opportunities**

- "Every Indian instrument names fairness; none specifies a test" is a one-line finding with a carousel, a LinkedIn post, and a P4 section behind it.
- The specification-vs-satisfaction calibration move (option 2 above) is methodologically transferable to every other EA constituent and may be the cleanest general solution to D4 across the whole cluster.
- The EU-process / NCAIC-criterion asymmetry is a candidate figure for P4.

## **Linked Projects**

[[P3_BFSI_JEIM]]

[[P4_Doctrinal_IJLIT]]

[[fsQCA_Thesis_Chapter]]

## **Linked Domains**

[[AI_Governance]]

[[BFSI_Governance]]

[[DPI_Governance]]

## **Linked Standard Concepts**

[[Explainability]]

[[Human_Oversight]]

[[Contestability_Redress]]

[[Proportionality]]

[[Accountability]]

## **Linked Frameworks**

[[EU_AI_Act]]

[[NIST_AI_RMF]]

[[OECD_AI_Principles]]

[[UNESCO_Recommendations]]

[[RBI_Free_AI]]

## **Linked Methods**

[[fsQCA]]

---

_Back to [[_Concepts_MOC]]_
