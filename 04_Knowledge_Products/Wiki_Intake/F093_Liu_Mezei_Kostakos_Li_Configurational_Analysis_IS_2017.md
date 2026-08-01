---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S7
  - tier/methodological-anchor
  - project/fsqca
  - method/fsqca-tutorial
  - method/sem-fsqca-mixed
  - journal/isj
  - batch/adhoc-2026-07-15
  - engine/phd
---

# Liu, Mezei, Kostakos & Li: Applying Configurational Analysis to IS Behavioural Research — A Methodological Alternative for Modelling Combinatorial Complexities (2017)

**Node ID:** F093
**Type:** Wiki Intake Note (Format B) — **Methodological Anchor** (no AI-governance content; opportunistic addition)
**Wiki Section:** S7 (Research Methods)
**Status:** Active
**Tier:** Methodological anchor — general fsQCA/SEM methods tutorial, direct Fiss (2011) citation
**Jurisdiction:** Finland (authors) / Zhejiang, China (worked example); method is jurisdiction-agnostic

---

## Source

**Full Citation (APA):** Liu, Y., Mezei, J., Kostakos, V., & Li, H. (2017). Applying configurational analysis to IS behavioural research: A methodological alternative for modelling combinatorial complexities. *Information Systems Journal*, *27*(1), 59–89. https://doi.org/10.1111/isj.12086 (DOI inferred from journal/volume convention — ⚠VERIFY)
**Document Type:** Academic paper (peer-reviewed, *Information Systems Journal*, Wiley) — methods tutorial with worked empirical example
**Authors:** Yong Liu (Aalto University); József Mezei (Åbo Akademi University + RiskLab Finland); Vassilis Kostakos (University of Oulu); Hongxiu Li (University of Turku)
**Batch:** Ad hoc, pre-Batch-19 (NotebookLM relay, PROMPT 0b) | 2026-07-15
**Pages:** 31 (pp. 59–89)

---

## Scope Note — Why This Node Exists Despite Zero AI Content

This paper has **no AI-governance subject matter** — it is a general fsQCA methods tutorial for IS behavioural research, with a worked example on rural Chinese citizens' adoption of mobile government services. Unlike F087–F092, it does not back any pre-existing bare citation in the vault — it is added **opportunistically** for its direct methodological value: it is the clearest single-source tutorial in the corpus explaining the RBM (regression-based method) vs. fsQCA symmetric/asymmetric distinction, and it directly cites and applies [[02_Projects/Shared_Anchors/Fiss_2011|Fiss (2011)]]'s core/peripheral-conditions framework — reinforcing the enrichment made to that Shared Anchor note earlier this session.

---

## Key Findings and Framework

### Definitions and Taxonomy

- **Configuration theory:** combinations of varying initial conditions can lead to the same outcome; the outcome-precondition relationship is asymmetric, not symmetric.
- **Regression-based methods (RBMs):** multiple regression/SEM, positing a predictor as both necessary *and* sufficient — the explicit methodological contrast class against which fsQCA is defined throughout the paper.
- **Configuration:** a specific set of causal variables that, working together, brings about an outcome of interest.
- **Core conditions:** appear in both parsimonious and intermediate solutions. **Peripheral conditions:** appear in intermediate but not parsimonious solutions. (Directly cites [[02_Projects/Shared_Anchors/Fiss_2011|Fiss (2011)]] for this distinction.)
- **Solution coverage / raw coverage / unique coverage:** clearly defined and distinguished — the clearest single explanatory table for these three coverage metrics found in the corpus to date (Table 2, p. 74).

### Worked Empirical Example (Mobile Government Adoption, Rural Zhejiang)

A fully worked SEM + FsQCA pipeline: 433 survey responses (409 retained) from rural Chinese citizens on mobile government service adoption, testing perceived ease of use, near-term/long-term usefulness, benevolence, and image as predictors of behavioural intention. SEM measurement/structural model reported in full (fit statistics, path coefficients: Image β=0.228, long-term usefulness β=0.225, ease-of-use β=0.178, benevolence β=0.151), followed by FsQCA calibration of the same latent SEM constructs into fuzzy sets (Likert-to-fuzzy breakpoints: 1→0, 3→0.4, 4→0.70, 5→1) and solution analysis (consistency >0.92, combined coverage ~66%). This SEM-first-then-fsQCA-on-the-same-latent-constructs sequencing is methodologically the clearest and most fully-specified example in the corpus of exactly this pipeline (compare F089's similar but less granularly-documented SEM+fsQCA sequencing).

### Practitioner Guidance (When to Use fsQCA Over RBMs)

The paper's explicit three-condition recommendation for choosing fsQCA over RBMs — (i) symmetric approaches cannot satisfactorily explain the phenomenon, (ii) evidence suggests asymmetric relationships, (iii) the research goal is full interpretation of the phenomenon rather than isolated effect-testing — is a directly citable methods-section justification template for [[fsQCA_Thesis_Chapter]] §4 (method justification).

---

## Relevance to PRIS Research

### For [[fsQCA_Thesis_Chapter]] (primary — method-justification and calibration-from-latent-constructs template)

Two direct uses: (1) the RBM-vs-fsQCA justification criteria for §4; (2) a fully worked example of converting SEM-validated latent constructs into fsQCA calibration inputs — relevant if any of PRIS's four conditions (EA/SR/RL/SI) are ever operationalised via a measurement-model step before calibration, rather than directly from ADICO-coded rule counts.

### For [[08_Methods/fsQCA]] (secondary — coverage-metric reference)

The Table 2 (p. 74) definitions of core/peripheral conditions and the three coverage metrics are the clearest single reference table in the corpus and worth citing directly if the method note ever needs a canonical definitions source beyond Ragin (2008) itself.

---

## Connections

**Related concepts:** None substantively instantiated. No "Instances in Corpus" entries added.

**Related corpus nodes:** [[02_Projects/Shared_Anchors/Fiss_2011|Fiss (2011)]] (directly cited by this paper for core/peripheral conditions — cross-reference now bidirectional); [[04_Knowledge_Products/Wiki_Intake/F089_Chen_Cao_Liang_Open_Government_Data_Usage_2023|F089]] (the corpus's other SEM+fsQCA mixed-design precedent).

**Related methods:** [[08_Methods/fsQCA]]

**Related projects:** [[fsQCA_Thesis_Chapter]]

---

## VERIFY Flags

**#245 — RESOLVED (2026-07-31, editorial convention).** Standard academic practice cites the year of the printed volume/issue of record, not the earlier acceptance/online-first year. This node's own Full Citation line already correctly uses **2017** (matching "Info Systems J (2017) 27, 59–89"). No change needed — flag closed as already-compliant.

**#246 — CLOSED, standing caveat (2026-07-31).** Self-resolving by design: its own text already correctly instructs not to assume Appendix D's content and to re-source it if ever needed. No further action needed unless the fuzzy-membership visualisation itself becomes required — in which case this note directs the re-extraction step already.

---

*Node written: 2026-07-15 | Ad hoc pre-Batch-19 session | PRIS v2.3 | Methodological anchor node — opportunistic addition (no pre-existing bare citation to resolve); direct Fiss (2011) cross-reference; contains no AI-governance substantive content*
