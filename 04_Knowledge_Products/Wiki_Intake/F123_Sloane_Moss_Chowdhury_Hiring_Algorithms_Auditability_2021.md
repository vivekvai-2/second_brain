---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - section/S1
  - section/S4
  - section/S6
---

# Sloane, Moss & Chowdhury: A Silicon Valley Love Triangle — Hiring Algorithms, Pseudo-Science, and the Quest for Auditability (2021) — Intake Note

**Source:** Mona Sloane (New York University); Emanuel Moss (Cornell Tech / Data & Society Research Institute); Rumman Chowdhury (Director of ML Ethics, Transparency and Accountability, Twitter)
**Year:** 2022 — published *Patterns* (Cell Press), Volume 3, Issue 2, **11 February 2022** (confirmed 2026-07-31, see VERIFY #285 resolution; note the DOI string embeds "2021" per Elsevier's online-first-registration convention, but the formal volume/issue date is 2022 — cite as 2022)
**Full title:** A Silicon Valley love triangle: Hiring algorithms, pseudo-science, and the quest for auditability
**Journal:** *Patterns* (Cell Press), DOI 10.1016/j.patter.2021.100425
**File ID:** F123
**Zotero key:** [leave blank — to be added manually]
**Wiki section(s):** S1 (Foundational Landscape), S4 (Agentic/Algorithmic Governance), S6 (Implementation & Audit)
**Confidence:** High
**Jurisdiction:** US primary (NYC bias-audit law, US Algorithmic Accountability Act), with EU AI Act comparison

---

## Classification

**Document type:** Academic paper (Perspective), peer-reviewed, *Patterns* (Cell Press) — same journal as [[04_Knowledge_Products/Wiki_Intake/F121_Correa_Kluge_Worldwide_AI_Ethics_200_Guidelines_2023|F121]]
**Primary audience:** Researcher / Regulator / Practitioner (auditors, HR-tech vendors)
**AI explicit:** Yes — algorithmic decision systems (ADSs) in hiring; NLP, computer vision, supervised ML.

---

## Scope Note — Why This Node Exists

Genuinely AI-governance-substantive, unlike much of this session's GIQ e-government batch. Supplies a **directly reusable audit framework** (the socio-technical matrix) for a specific, high-stakes AI application domain (hiring) that the PRIS corpus has not previously covered in depth, and explicitly cites two existing corpus nodes — [[04_Knowledge_Products/Wiki_Intake/F080_Mitchell_et_al_Model_Cards_for_Model_Reporting_2019|F080]] (Model Cards) and [[04_Knowledge_Products/Wiki_Intake/F081_Gebru_et_al_Datasheets_for_Datasets_2018|F081]] (Datasheets for Datasets) — as direct methodological precedents, making this a confirmed citation-chain extension of existing PRIS documentation-standard evidence rather than an isolated addition.

---

## Key Findings and Framework

### The socio-technical matrix — seven-element audit tool

A structured evaluative tool combining: (1) Hiring ADS [name], (2) Funnel stage, (3) Goal, (4) Data, (5) Function, (6) Assumption, (7) Epistemological roots. Applied to four commercial hiring ADS products in a worked example table: Hiretual (experience matching), Codility (skill/coding testing), Pymetrics (ability/gameplay performance), Humantic (personality profiling). The matrix's explicit design lineage cites "datasheets for datasets" and "model cards for model reporting" as precedent documentation standards — directly extending [[04_Knowledge_Products/Wiki_Intake/F080_Mitchell_et_al_Model_Cards_for_Model_Reporting_2019|F080]] and [[04_Knowledge_Products/Wiki_Intake/F081_Gebru_et_al_Datasheets_for_Datasets_2018|F081]] from general-purpose model/dataset documentation into a domain-specific (hiring) audit application.

### The hiring funnel — four stages (Bogen & Reike)

Sourcing → screening → interviewing → selection. Each stage carries a distinct ADS type and distinct auditability challenge; the matrix is designed to be applied per-stage rather than to a hiring pipeline as an undifferentiated whole — a directly transferable disaggregation principle for auditing any multi-stage algorithmic pipeline (equally applicable to India's DPI multi-stage verification/eligibility pipelines, e.g. Aadhaar authentication → eligibility determination → benefit disbursement).

### Epistemological roots — the paper's sharpest conceptual contribution

Defined as "the claims to knowledge that the system is making — specifically, that there is a way to 'know' the interior emotional state of a subject based on externally discernable attributes like facial expressions, pupil dilation, or other physiological characteristics." The paper's central normative argument: audits "cannot be limited merely to the degree to which they promote demographic parity" but "must also contend with claims that such ADSs can reveal aptitude, future performance, and cultural fit" — i.e., audits must interrogate the underlying scientific/pseudo-scientific validity claim, not merely the output distribution. This is a distinct audit dimension from the corpus's existing bias/fairness-metric-focused evidence (e.g. F085's model validation taxonomies) — validity/construct-validity as a freestanding audit target, citing the OCEAN Big-5 personality model as a worked example of a contested-validity construct widely deployed in commercial hiring ADS (Humantic) despite significant psychometric controversy over its predictive validity for job performance.

### Regulatory landscape cited — NYC, US federal, EU

Three named instruments: NYC bill A1894-2020 (mandatory annual bias audits of hiring ADS — a binding, enacted sub-national US instrument); the proposed US Algorithmic Accountability Act (calls for algorithmic impact assessments — not enacted at time of writing); the EU AI Act proposal ("calls for audits and 'conformity assessments' without providing instruction on what these practices ought to entail" — the paper's own explicit criticism, corroborating [[04_Knowledge_Products/Wiki_Intake/F106_Edwards_EU_AI_Act_Summary_Significance_Scope_2022|F106]]'s documentation of the 2021-22 proposal-stage EU AI Act's comparative underspecification relative to the final Regulation). The paper's call for "an interdisciplinary group of experts... because of the range of expertise needed" (social scientists, psychologists, historians of science) to conduct audits is a specific, actionable audit-governance-design recommendation not yet present elsewhere in the PRIS corpus's audit-framework evidence base.

---

## Relevance to PRIS Research

### Institutional_Coherence — regulatory audit-standard fragmentation (light instance)

NYC's binding local bias-audit mandate, the non-enacted federal Algorithmic Accountability Act, and the EU AI Act's underspecified conformity-assessment requirement together constitute a US-multi-level-plus-EU parallelism/incoherence pattern in *audit methodology specification* — none of the three cited instruments specifies what an adequate hiring-ADS audit must actually examine, a gap this paper's own socio-technical matrix is explicitly designed to fill.

### Transparency / Accountability — direct documentation-standard extension

See Instances in Corpus additions below — extends F080/F081's general documentation-standard evidence into a domain-specific audit application.

---

## Connections

**Related concepts:** [[05_Concepts/05_Concepts_Standard/Transparency]], [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]]

**Related corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/F080_Mitchell_et_al_Model_Cards_for_Model_Reporting_2019|F080]] (direct cited precedent), [[04_Knowledge_Products/Wiki_Intake/F081_Gebru_et_al_Datasheets_for_Datasets_2018|F081]] (direct cited precedent), [[04_Knowledge_Products/Wiki_Intake/F106_Edwards_EU_AI_Act_Summary_Significance_Scope_2022|F106]] (corroborates proposal-stage EU AI Act audit/conformity-assessment underspecification), [[04_Knowledge_Products/Wiki_Intake/F124_Viljanen_Parviainen_AI_Regulatory_Strata_2022|F124]] (same-batch companion — Finnish hiring-AI regulatory mapping from a doctrinal rather than audit-practice angle; both papers independently select hiring AI as their worked domain)

**Related projects:** [[P1_SLR_RG]]

**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] (S6 — audit frameworks)

---

## VERIFY Flags

**#285 — RESOLVED (2026-07-31, Perplexity Deep Research).** Confirmed published in *Patterns* (Cell Press), Volume 3, Number 2, **11 February 2022** — High confidence. Year field above corrected from 2021 to 2022 (the DOI's embedded "2021" reflects Elsevier's online-first registration year, not the formal volume/issue date).

---

## Log

- 2026-07-16: Node created. NotebookLM Ingestion Pipeline (PROMPT 0b relay), per [[Session_Handoff_NotebookLM_Ingestion_20260715]]. Duplicate check against [[Corpus_Index_MOC]], `04_Knowledge_Products/Wiki_Intake/`, and `_Institutions_MOC.md` (searched "Sloane," "Moss," "Chowdhury," "hiring algorithm," "socio-technical matrix," "hiring ADS") found no existing vault node — three incidental keyword false-positives (F070, F047, NCAIC_1, all unrelated generic uses of "hiring") ruled out on inspection. Confirmed genuinely new. Classified Format B, full treatment given genuine AI-governance substance and direct citation chain to F080/F081. One new VERIFY flag (#285). New institution row (New York University + Cornell Tech/Data & Society Research Institute + Twitter META) added to `_Institutions_MOC.md`. "Instances in Corpus" additions to Transparency and Accountability.
