---
type: Method
tags:
  - type/method
  - status/active
  - paper/fsqca-primary
  - paper/p1
  - gate/open
  - engine/phd
---

# fsQCA

**Type:** Method **Status:** Active **Last Updated:** 2026-07-15

---

## Core Synthesis

Fuzzy-set Qualitative Comparative Analysis (fsQCA) is the primary causal inference method for the thesis empirical chapter — applied to derive sufficient configurations of governance conditions (EA × SR × RL × SI) for legitimate AI governance outcomes across 10 cases. This note records methodological intelligence accumulated through the research design process: what the method does, where it has been applied in the PRIS corpus, the design decisions made for the thesis chapter, and the open methodological questions. It is not a tutorial. The authoritative methodological source is Ragin (2008); the calibration architecture is in `fsqca_SOM_V2.docx`; and the coding protocol is in NVivo.

## Method Profile

- **Type:** Configurational comparative method; set-theoretic
- **Logic:** INUS — Insufficient but Non-redundant part of an Unnecessary but Sufficient condition
- **Software:** fsQCA 3.0 (Ragin & Davey); R package `QCA` (Dusa)
- **Key anchors in PRIS:** Ragin (1987, 2008); Fiss (2011) — typology-configuration logic; Dul (2016) — limited diversity; Andrews (2024) — see [[04_Knowledge_Products/Wiki_Intake/F087_Andrews_Beynon_Revolving_Door_UK_Government_fsQCA_2024|F087]], corpus node added 2026-07-15, Gong (2025) — robustness reporting precedents in target journals

## Design Decisions (Thesis Chapter — Locked)

|Decision|Choice|Rationale|
|---|---|---|
|Set type|Fuzzy sets (0.0–1.0)|Governance conditions are not binary; degree of presence is analytically meaningful|
|Calibration anchors|0.00 / 0.33 / 0.67 / 1.00|Four-anchor scheme; fully non-membership, more out than in, more in than out, fully in|
|Conditions|EA, SR, RL, SI|Four analytically independent dimensions confirmed by correlation matrix (Table S25)|
|Outcome|Legitimate AI governance outcome|Operationalisation via combined EA-principle calibration (pending TAC decision D4)|
|Case N|10 (from 20-candidate shortlist)|Mid-N fsQCA; diversity on jurisdiction, sector, maturity|
|Solution types|Complex, parsimonious, intermediate|All three reported per Ragin (2008); intermediate used for interpretation|
|Consistency threshold|≥ 0.80|Standard in governance literature; gatekeeping function|
|Coverage|Reported, not gatekept|Per Ragin (2008); coverage is explanatory scope, not validity criterion|
|INUS interpretation|Pending D4 decision|Whether INUS logic applied as robustness layer or primary interpretation|
|Limited diversity|Acknowledged per Dul (2016)|Counterfactual analysis reported for logically impossible configurations|

## Where I Am in Application

|Task|Status|
|---|---|
|Calibration architecture designed|✅ Complete — Tables S1, S3, S4 in `fsqca_SOM_V2.docx`|
|20-case shortlist with maturity scores|✅ Complete|
|Final 10-case list|🔴 Pending TAC confirmation (target: Q2 2026)|
|IG 2.0 coding of 10 cases|🔴 0% — begins after case list locked|
|Condition calibration scores|🔴 0% — depends on IG coding|
|Truth table construction|🔴 0% — Q3 2026|
|Boolean minimisation|🔴 0% — Q3 2026|
|INUS interpretation|🔴 Pending D4 decision|

## Methodological Tensions Encountered

**Truth table contradictions:** Multiple configurations mapping to both presence and absence of outcome are expected given limited N. Protocol: document contradiction sources; resolve by case-level evidence; report unresolved contradictions transparently.

**Calibration subjectivity:** Four-anchor calibration requires justification for anchor placement. Current approach: anchor placement driven by IG 2.0 coding distributions + literature benchmarks. TAC alignment required before Q3 2026.

**Limited diversity:** A 10-case design with four conditions (16 logical configurations) will produce remainder rows. Dul (2016) protocol for simplifying assumptions documented in `fsqca_SOM_V2.docx`.

**Robustness-over-time reporting (candidate addition, flagged 2026-07-15):** [[04_Knowledge_Products/Wiki_Intake/F087_Andrews_Beynon_Revolving_Door_UK_Government_fsQCA_2024|F087]] (Andrews & Beynon, *Regulation & Governance* 2024) demonstrates a concrete technique for this — re-running complex solutions separately across sub-periods of a panel and reporting per-period consistency (their COUT1 = 0.837, COUT2 = 0.812) — distinct from cross-sectional consistency/coverage. Worth evaluating as a robustness check for the thesis chapter if the 10-case design has any repeated-observation or temporal structure.

## Linked Projects

- [[fsQCA_Thesis_Chapter]]
- [[P1_SLR_RG]] _(future — Fiss 2011 typology-validation logic)_

## Linked Methods

- [[Institutional_Grammar_IG2]]
- [[SLR_Protocol]]

## Linked Frameworks

- [[EU_AI_Act]]
- [[OECD_AI_Principles]]
- [[IndiaAI_Framework]]
- [[NIST_AI_RMF]]
- [[UNESCO_Recommendations]]
- [[RBI_Free_AI]]
- [[SEBI_AI_Circular]]

## Linked Domains

- [[AI_Governance]]

---

_Back to [[_Methods_MOC]]_