---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S7
  - tier/methodological-anchor
  - project/fsqca
  - method/fsqca-robustness
  - batch/adhoc-2026-07-15
  - engine/phd
---

# Andrews & Beynon: The Revolving Door in UK Government Departments — A Configurational Analysis (2024)

**Node ID:** F087
**Type:** Wiki Intake Note (Format B) — **Methodological Anchor** (not AI-governance content; see scope note below)
**Wiki Section:** S7 (Research Methods)
**Status:** Active
**Tier:** Methodological anchor (fsQCA robustness-reporting precedent)
**Jurisdiction:** UK (substantive case); method is jurisdiction-agnostic

---

## Source

**Full Citation (APA):** Andrews, R., & Beynon, M. J. (2024). The revolving door in UK government departments: A configurational analysis. *Regulation & Governance*, *18*(2), 590–611. https://doi.org/10.1111/rego.12550 (DOI inferred from journal/volume convention — ⚠VERIFY)
**Document Type:** Academic paper (peer-reviewed, *Regulation & Governance*, Wiley) — ABDC ranking not yet confirmed for this specific title ⚠VERIFY
**Authors:** Rhys Andrews & Malcolm J. Beynon — Cardiff Business School, Cardiff University, UK
**Batch:** Ad hoc, pre-Batch-19 (NotebookLM relay, PROMPT 0b) | 2026-07-15
**Pages:** 22 (pp. 590–611)

---

## Scope Note — Why This Node Exists Despite Zero AI Content

This paper has **no AI-governance subject matter** — it is a configurational (fsQCA) study of civil-service-to-private-sector revolving door appointments across 17 UK government departments (2015–2018). It does not feed any AI Governance Wiki section in the substantive sense (S1–S6, S8–S9 do not apply). It is admitted to the corpus solely as a **methodological anchor**, on the same basis as [[04_Knowledge_Products/Wiki_Intake/Frantz_Siddiki_Institutional_Grammar_2_2021|F056]] (Institutional Grammar 2.0): it is already cited by name in [[08_Methods/fsQCA]]'s Method Profile ("Andrews (2024) — robustness reporting precedent in target journals") without a dedicated corpus entry backing that citation. This node closes that gap.

---

## Key Findings and Framework

### fsQCA Design Choices (directly comparable to PRIS's own design)

| Element | Andrews & Beynon (2024) | PRIS fsQCA_Thesis_Chapter (for comparison) |
|---|---|---|
| Case N | 17 departments × 4 years (department-year observations) | 10 cases |
| Calibration | Fuzzy membership scores, "<0.5 or ≥0.5" thresholds → 0/1 crisp anchors for some steps | Four-anchor scheme (0.00/0.33/0.67/1.00) |
| Truth table size | 32 (= 2⁵) possible configurations | Determined by 4 conditions (16 logical configurations) |
| Necessity consistency threshold | 0.9 | ≥ 0.80 (Design Decisions table) |
| Truth table frequency threshold | At least two cases | Typically 1 for N=10 |
| Truth table consistency threshold | 0.811 | ≥ 0.80 |
| Solutions reported | Complex only (per department-year results tables) | Complex, parsimonious, intermediate (all three, per Ragin 2008) |
| **Robustness/temporal check** | **Consistency of pathways through time** (Section 4.4) — solutions re-run separately for presence and absence of the outcome across sub-periods; complex-solution consistency reported per period (COUT1 = 0.837; COUT2 = 0.812) | Not yet designed — candidate addition |

### Substantive Results (for completeness, not for AI-governance reuse)

- Necessity analysis: no single condition individually necessary for high revolving-door activity.
- Sufficiency analysis: **3 configurations** sufficient for presence of high revolving-door activity (12 cases); **15 configurations** sufficient for absence (50 cases) — together 91.176% of department-year observations covered.
- Core executive departments (Cabinet Office, Defence, HM Treasury, Home Office) drive the bulk of revolving-door activity; Lowi's (1964) tripartite policy typology (constituent/redistributive/regulatory) organizes the department-level predictors — constituent departments show a significant positive association (0.22) with private-sector appointments; distributive departments a significant negative association (−0.29).
- 213 ACOBA applications (2015–2018) against ~4,572 senior civil servants (~5%) form the dependent-variable base.

### "Bureaucratic Capital" (Brezis & Cariolle, 2019, as cited)

Defined as the specific knowledge of over-complex or ill-designed regulations built by a regulator, plus the special relationships with government and peer bureaucrats accumulated during public office — a candidate construct if PRIS ever extends into regulator-capture/revolving-door dimensions of BFSI AI governance (currently out of scope for P1–P4/fsQCA, noted here only for completeness).

---

## Relevance to PRIS Research

### For [[fsQCA_Thesis_Chapter]] (primary — methods, not substance)

The paper's **Section 4.4 "Consistency of pathways through time"** is the most directly transferable element: it demonstrates a concrete technique for reporting fsQCA solution stability across sub-periods of a panel, distinct from and complementary to the standard consistency/coverage reporting already locked into the thesis chapter's Design Decisions table. If Vivek's 10-case design has any temporal or repeated-observation structure, this section is a citable precedent for how to report robustness-over-time rather than only cross-sectional consistency. It also demonstrates department-level (organizational) case selection and typology-based condition derivation (Lowi 1964) as an alternative case-structuring logic to jurisdiction/sector-based case selection.

### For [[08_Methods/fsQCA]] (backing an existing citation)

This node is the corpus record for the "Andrews (2024)" citation already present in the fsQCA method note's Key Anchors line. See enrichment logged there.

---

## Connections

**Related concepts:** None of PRIS's signature or standard concepts (Regulatory_Parallelism, Governance_Debt, Institutional_Coherence, Accountability, Transparency, Governance_Capacity, Legitimacy) are substantively instantiated by this paper's UK civil-service subject matter. No "Instances in Corpus" entries added — this is a deliberate exception, consistent with F056's treatment (methodological anchors are cited from method notes and project files, not from concept "Instances in Corpus" sections, since they are not evidence of a governance construct).

**Related corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/Frantz_Siddiki_Institutional_Grammar_2_2021|F056]] (Institutional Grammar 2.0 — the other pure-methods anchor node in the corpus); [[04_Knowledge_Products/Wiki_Intake/F086_Almeida_dosSantos_AI_Governance_Public_Organizations_QCA_2025|F086]] (Almeida & dos Santos — the corpus's other QCA-methodology precedent, but substantively AI-governance content, unlike this node).

**Related methods:** [[08_Methods/fsQCA]]

**Related projects:** [[fsQCA_Thesis_Chapter]]

**Related knowledge products:** None (does not feed [[04_Knowledge_Products/AI_Governance_Wiki]])

---

## Methodological Notes

**Why a Format B / S7 slot rather than exclusion:** Per [[PRIS_Cowork_Context]] Section 6, out-of-scope criteria name military doctrine, pure PM methodology, quantum crypto, drone regulation, and social-media policy without an AI component — this paper does not fall under any of those exclusion categories, and it is affirmatively useful (already cited in a live method note). The F056 precedent establishes that pure-methods academic papers with no AI-governance substance are captured under Wiki Section S7 rather than excluded outright.

**Fuzzy calibration technique:** Note the paper's simpler 0/1 crisp-anchor step for some variables ("<0.5 or ≥0.5") alongside genuine fuzzy scores elsewhere — a lighter-weight calibration approach than PRIS's four-anchor scheme, useful as a contrast case if a reviewer questions why PRIS uses four anchors rather than a simpler binary/crisp calibration for any condition.

---

## VERIFY Flags

**#233 — RESOLVED (2026-07-31, editorial convention).** Standard academic practice cites the year of the printed volume/issue of record, not the earlier acceptance/online-first year, unless explicitly citing "forthcoming"/"in press" work. This node's own Full Citation line already correctly uses **2024** (matching "*Regulation & Governance* (2024) 18, 590–611"). No change needed — flag closed as already-compliant.

**#234 — RESOLVED (2026-07-31).** Immaterial per the flag's own text (this node does not cite department-level findings substantively). Closed without further action.

---

*Node written: 2026-07-15 | Ad hoc pre-Batch-19 session | PRIS v2.3 | Methodological anchor node — backs an existing bare citation in [[08_Methods/fsQCA]]; contains no AI-governance substantive content*
