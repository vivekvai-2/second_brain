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

**EA outcome calibration — D4 dependency resolved to a decision, 2026-08-02.** The outcome is operationalised as "combined EA-principle calibration (pending TAC decision D4)," but until 2026-08-02 the constituent principles had no concept notes, no operational definitions and no measurement basis in the vault. That gap is now closed: [[Explainability]], [[Fairness]], [[Human_Oversight]], [[Contestability_Redress]] and [[Proportionality]] were created from a dedicated sourcing pass. Four consequences bear directly on D4:

1. **Fairness cannot be calibrated as a scalar without declaring a metric family.** Kleinberg's impossibility theorem (restated as Thm 2.1, *CACM* Jan 2024) proves calibration-within-groups, positive-class balance and negative-class balance cannot jointly hold except under perfect prediction or equal base rates. A composite EA score that silently averages over fairness embeds an undisclosed normative choice. Bell et al. (2023) show the constraint binds loosely in practice, but the theoretical objection stands for a reviewer.
2. **Human oversight has no validated instrument.** Unlike explainability (SCS) and contestability (CAS), nothing exists to adopt. A bespoke five-item scheme derived from EU AI Act Art. 14(4) is recommended, and must be disclosed as constructed rather than adopted.
3. **Proportionality should not enter EA.** It is a regime-level property governing how the other principles are allocated, and belongs with RL. Folding it into EA mixes levels of analysis.
4. **Recommended resolution — calibrate on specification, not satisfaction.** Score each case's *instrument* on whether it names the principle, specifies a test, and attaches a consequence, rather than scoring whether the deployed system achieves the principle. This sidesteps the impossibility problem, matches an institutional-design thesis rather than a technical-audit one, is consistent across all four EA constituents, and answers the reviewer question "are you measuring rules or reality?" before it is asked. It also produces a substantively striking result, since Indian instruments score at or near zero on the "specifies a test" item across every constituent.

**D4 — third calibration option located 2026-08-02 (Singapore pass).** The EA-principle notes recorded that the available instruments (SCS, XAI Trust Scale, CAS) are *subject-perception* scales measuring received explanation quality, and cannot be applied to a governance regime without category error. **MAS's Veritas Documents 3A (Fairness), 3B (Ethics and Accountability) and 3C (Transparency) are the missing instrument class** — published assessment methodologies that assess the *deploying institution's process*, with open-source toolkits (v1.0 2022, v2.0 2023) and documented pilots across seven financial institutions. Evaluate as a third D4 option alongside "declare the metric family" and "calibrate on specification." Caveat: Veritas ended at Phase 3 (June 2023) and covers neither generative nor agentic systems. See [[Singapore_AI_Governance]].

**Convergent evidence on the Human Oversight weakness.** Singapore's AI Verify operationalises eleven principles but runs **technical tests on only three — Fairness, Explainability, Robustness** — assessing the remaining eight, including Human Agency and Oversight, by documented process check. This independently corroborates the conclusion reached from the academic literature at [[Human_Oversight]]: no validated instrument exists and it is the least technically measurable EA constituent. Two independent routes to the same finding; state as convergent evidence in the methodology chapter rather than as a single-source claim.

**Two RL-low / SR-high cases now identified.** [[Singapore_AI_Governance]] (no binding instrument, highly developed assessment infrastructure) and [[DEPA]] (never-enacted draft, operative licensed-intermediary regime). Cases where RL and SR diverge sharply carry the configurational information; if both enter the 10-case set the design gains real leverage on whether structural readiness can substitute for regulatory logic in producing legitimate governance outcomes — close to the thesis's central question. Flag both for TAC discussion.

**Configurational precedent for RAI principles (located 2026-08-02):** Akbarighatar et al., *Enacting Responsible AI: A Configurational Analysis of AI Principles in Practice*, **Information Systems Frontiers** 28(1), 2026, DOI 10.1007/s10796-025-10618-x — uses fsQCA to examine how AI experts view Responsible AI principles and the relations among them, treating multiple RAI principles as configurational rather than additive conditions. This is the **only confirmed fsQCA study applying the method to an RAI principle set** and is the closest methodological precedent to this chapter. Two implications: it is a template for calibration and solution reporting, and it is a **positioning risk** — the contribution claim must be specified against it, since the obvious framing ("first configurational analysis of AI governance principles") is no longer available. Read before finalising the contribution statement. No fsQCA study was located using any of the five EA constituents individually as a calibrated condition, which leaves that space open.

**⚠ IG-QCA precedent CORRECTED, 2026-08-02 — the design is not methodologically first.** The methods sourcing pass asked whether any published study combines Institutional Grammar coding with QCA. **One does.** Schlager, Bakkensen, Olivier & Hanlon, *Institutional Design for a Complex Commons*, **Public Administration** (19 Jan 2021), DOI 10.1111/padm.12715 — and the field states the priority explicitly: Siddiki & Frantz's companion symposium introduction (*Public Administration*, 2021, DOI 10.1111/padm.12753) says **"Schlager et al.'s (2021) study is the first to use QCA to analyze institutional statements coded using the Institutional Grammar."**

No subsequent IG-QCA study appears in the citation trail or on institutionalgrammar.org's published-research index. Consequences:

- **Cannot claim** first to combine IG and QCA. That priority is Schlager et al. (2021) and must be cited and built on, not contested.
- **Can claim** first application to AI governance / regulatory-institution comparison — Schlager et al. is domain-distinct (commons and public-goods governance).
- The chapter's stated contribution (§6.4) is **substantive-configurational**, not methodological, so it survives intact. The correction bites only on any framing that presents IG-QCA as a methodological innovation. **Second contribution-claim correction of 2026-08-02**, after the Akbarighatar precedent above — both from the same cause: assuming novelty without searching for the incumbent.
- Schlager et al. is also a **reporting template**: it engaged the kappa-vs-Gwet's-AC1 reliability debate directly. See [[Coding_Reliability_Protocol]].

**Calibration source located — the one this design actually needs.** **Basurto, X. & Speer, S.**, *Structuring the Calibration of Qualitative Data as Sets for Qualitative Comparative Analysis*, states the problem exactly: "Existing direct and indirect calibration techniques for quantitative data (Ragin 2008) cannot be applied to qualitative data as such data need to be coded and summarized before fuzzy-set values can be assigned." Six-step procedure built for qualitative/textual/institutional data: operationalise conditions and outcome → develop anchor points → apply content analysis → summarise code output → determine the fuzzy-set scale → assign and revise values. Its central rule — set values "should be based on a researcher's theoretical and substantive knowledge and not on internal criteria such as the mean or the mode" — settles the theoretical-vs-data-driven anchor question in favour of theory, and matches the locked four-anchor scheme. **This is the single most directly applicable calibration source for an IG-coded → fsQCA design and should anchor the calibration section.** Pair with Ragin, *Fuzzy Sets: Calibration Versus Measurement* (direct vs indirect) and Ragin's April 2024 *QCA Research Notes* (anchors as 0.95/0.05/0.50).

**Robustness protocol — current standard located.** **Oana, I.-E. & Schneider, C.Q.**, *A Robustness Test Protocol for Applied QCA*, **Sociological Methods & Research** 53(1), 2024 — three-part protocol: (1) **sensitivity ranges** (parameter range within which the solution formula is unchanged); (2) **fit-oriented** robustness; (3) **case-oriented** robustness, classifying cases as robust / shaky / possible. Introduces the **"test set"** and **"robust core"** concepts; implemented in the **SetMethods** R package — an addition to the locked software list (fsQCA 3.0; R `QCA`). Pair with **Skaaning (2011, SMR)** as the foundational precedent, whose rule is that robustness checks should vary anchors "only within ranges small enough so as not to undermine the theoretical arguments underpinning the original choice." Citing both shows lineage.

**⚠ Gap in the locked design: negation analysis.** Schneider & Wagemann's *Standards of Good Practice* (2010, 2,133 citations) requires that "the outcome and the negation of the outcome should always be analyzed in two separate analyses," and that sufficiency analysis "always be performed with and without simplifying assumptions… Both solution formulas should be reported." The locked Design Decisions table covers all three solution types but **does not mention analysing the negated outcome**. Add it — omission is a standard reviewer catch. Also relevant: "the number of conditions should be kept moderate" (four conditions is fine at N=10) and Thomann (2020, SMR) on reducing limited diversity *a priori* through case selection rather than only correcting post hoc via solution type — directly applicable while the 10-case list is still open. Glaesser (2023, *Quality & Quantity*) frames the three solution types as "endpoints of a single continuum" differing in tolerance for counterfactuals, rather than one being superior.

**Robustness-over-time reporting (candidate addition, flagged 2026-07-15):** [[04_Knowledge_Products/Wiki_Intake/F087_Andrews_Beynon_Revolving_Door_UK_Government_fsQCA_2024|F087]] (Andrews & Beynon, *Regulation & Governance* 2024) demonstrates a concrete technique for this — re-running complex solutions separately across sub-periods of a panel and reporting per-period consistency (their COUT1 = 0.837, COUT2 = 0.812) — distinct from cross-sectional consistency/coverage. Worth evaluating as a robustness check for the thesis chapter if the 10-case design has any repeated-observation or temporal structure.

## Linked Projects

- [[fsQCA_Thesis_Chapter]]
- [[P1_SLR_RG]] _(future — Fiss 2011 typology-validation logic)_

## Linked Methods

- [[Institutional_Grammar_IG2]]
- [[SLR_Protocol]]
- [[Coding_Reliability_Protocol]]
- [[Comparative_Regulatory_Analysis]]

## Linked Frameworks

- [[EU_AI_Act]]
- [[OECD_AI_Principles]]
- [[IndiaAI_Framework]]
- [[NIST_AI_RMF]]
- [[UNESCO_Recommendations]]
- [[RBI_Free_AI]]
- [[SEBI_AI_Circular]]
- [[Singapore_AI_Governance]]
- [[ISO_IEC_42001]]
- [[DEPA]]

## Linked Standard Concepts

- [[Explainability]] — EA constituent; best-instrumented (SCS)
- [[Fairness]] — EA constituent; ⚠ calibration blocked pending metric-family declaration
- [[Human_Oversight]] — EA constituent; ⚠ highest construct-validity risk, bespoke instrument required
- [[Contestability_Redress]] — EA constituent; CAS is the most calibration-ready instrument located
- [[Proportionality]] — **RL property, not EA** — see D4 note above

## Linked Domains

- [[AI_Governance]]

---

_Back to [[_Methods_MOC]]_