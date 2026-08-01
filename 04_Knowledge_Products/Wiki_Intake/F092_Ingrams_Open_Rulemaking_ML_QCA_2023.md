---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S7
  - tier/methodological-anchor
  - project/fsqca
  - project/p4
  - method/fsqca-robustness
  - method/ml-qca-mixed
  - journal/giq
  - batch/adhoc-2026-07-15
  - engine/phd
---

# Ingrams: Do Public Comments Make a Difference in Open Rulemaking? Insights from Information Management Using Machine Learning and QCA Analysis (2023)

**Node ID:** F092
**Type:** Wiki Intake Note (Format B) — **Methodological Anchor** (no AI-governance content; backs a pre-existing bare citation)
**Wiki Section:** S7 (Research Methods)
**Status:** Active
**Tier:** Methodological anchor — resolves the vault's standing "Ingrams 2023" citation
**Jurisdiction:** United States (US Dept. of Education rulemaking); method is jurisdiction-agnostic

---

## Source

**Full Citation (APA):** Ingrams, A. (2023). Do public comments make a difference in open rulemaking? Insights from information management using machine learning and QCA analysis. *Government Information Quarterly*, *40*(1), Article 101778. https://doi.org/10.1016/j.giq.2022.101778 (DOI inferred from article-number convention — ⚠VERIFY)
**Document Type:** Academic paper (peer-reviewed, *Government Information Quarterly*, Elsevier)
**Author:** Alex Ingrams (Institute of Public Administration, Leiden University)
**Batch:** Ad hoc, pre-Batch-19 (NotebookLM relay, PROMPT 0b) | 2026-07-15
**Pages:** Not sequentially numbered (article no. 101778)

---

## Scope Note — Resolves an Existing Bare Citation Gap

This paper has **no AI-governance subject matter** in the sense of AI regulation — it studies whether public comments influence US Department of Education rulemaking, using machine learning (LDA topic modelling) combined with fsQCA. Machine learning is the *analytical instrument*, not the *regulatory subject*. It is admitted as a **methodological anchor**: this is the confirmed source behind the bare "Ingrams 2023" citation already present in `01_Strategy/VV_Publication_Pipeline_v3.md`'s P1 skill-mapping line ("gap analysis between existing fsQCA studies (Almeida 2025, Ingrams 2023, Gong 2025)"), now updated to link here. (Correction, logged 2026-07-15: this node's first draft incorrectly attributed this citation to `P4_Doctrinal_IJLIT.md` — corrected.)

---

## Key Findings and Framework

### Mixed ML + fsQCA Design — the distinctive methodological contribution

Ingrams combines **Latent Dirichlet Allocation (LDA)**, an unsupervised topic-modelling method, with fsQCA: LDA extracts latent topics from public comment text and measures topic-overlap ("degree of change," Δcontent = |FRk − PRk|·θwt) between proposed and final rules; these text-analytic measures then become fsQCA conditions alongside political/media variables. This is the corpus's **first text-analytics-plus-configurational mixed design** — a genuinely different combination from F089's SEM+fsQCA and F093's (below) SEM+fsQCA, and directly relevant if PRIS ever wants to run topic-modelling over a large corpus of regulatory comments/submissions (e.g., MeitY/SEBI/RBI public consultation responses) as an fsQCA condition.

| Element | Ingrams (2023) | PRIS fsQCA_Thesis_Chapter (for comparison) |
|---|---|---|
| Case N | 25 US Dept. of Education regulations, 2008–2016 (min. 30 comments per case) | 10 cases |
| Calibration | 90th/50th/10th percentile bounds, cross-over adjusted to 45th percentile to avoid dropping contradictory cases | Four-anchor scheme (0.00/0.33/0.67/1.00) |
| Necessity threshold | 0.80 (conventional) | ≥0.80 |
| Sufficiency consistency threshold | 0.75 | ≥0.80 |
| Configurations (4 conditions) | 24 (= 4!) — note: text describes 24 "possible configurations," distinct from the standard 2^k truth-table row count, likely reflecting a different condition-counting convention — flagged, not resolved | 16 logical configurations (4 conditions) |
| Intermediate solution | Coverage 0.778, consistency 0.753 | To be determined |

### Definitions

- **Democratic legitimacy perspective:** policymakers and public constitute a forum for information-sharing/monitoring of government promises.
- **Political pluralism perspective:** participation as competitive interest-group influence-seeking.
- **Alpha (α) (LDA hyperparameter):** measures whether comment topics are densely clustered or broadly dispersed.
- **Necessity / Consistency / Coverage / Logical remainders:** standard QCA definitions, consistent with Ragin (2008) usage elsewhere in the corpus.

### Worked Example (Violence Against Women Act rulemaking)

A fully worked qualitative deep-dive: 100 public comments (30% from professional organizations) on the VAWA regulation, cross-referenced against 730 media articles (Factiva), yielding 11 substantive changes in the final rule attributable to public input — a concrete illustration of the ML+QCA pipeline applied end-to-end on one case, useful as a template if PRIS ever wants a similarly fully-worked single-case illustration alongside a cross-case fsQCA.

---

## Relevance to PRIS Research

### For [[fsQCA_Thesis_Chapter]] / [[08_Methods/fsQCA]] (primary — resolves existing citation, mixed ML+QCA design template)

Closes the "Ingrams 2023" placeholder in P4's skill-mapping line. The LDA+fsQCA combination is a candidate technique if PRIS's future work (post-thesis, consulting, or P1 extensions) involves large public-comment or submission corpora requiring both topic extraction and configurational analysis.

### For [[P4_Doctrinal_IJLIT]] (peripheral — public-participation angle)

India's AI-governance rulemaking processes (e.g., MeitY consultation rounds referenced elsewhere in the corpus, such as DPIIT_1's 171-comment/80-counter-comment record) could in principle be analysed with this paper's method — noted as a possible future extension, not current P4 evidence.

---

## Connections

**Related concepts:** None substantively instantiated. No "Instances in Corpus" entries added.

**Related corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/F089_Chen_Cao_Liang_Open_Government_Data_Usage_2023|F089]], [[04_Knowledge_Products/Wiki_Intake/F091_Gong_Yang_Digital_Government_Partnerships_fsQCA_2025|F091]] (the corpus's other GIQ QCA precedents); [[07_Institutions/Corpus/DPIIT/DPIIT_1|DPIIT_1]] (India's own public-consultation-record instrument, a peripheral comparator for the VAWA worked example's comment-count/change-count structure).

**Related methods:** [[08_Methods/fsQCA]]

**Related projects:** [[fsQCA_Thesis_Chapter]]; peripheral note in [[P4_Doctrinal_IJLIT]]

---

## VERIFY Flags

**#242 — RESOLVED (2026-07-31, WebSearch/ScienceDirect).** DOI confirmed independently: ScienceDirect record pii/S0740624X22001149 matches https://doi.org/10.1016/j.giq.2022.101778 exactly. Flag closed.

**#243 — PARTIALLY RESOLVED, Medium confidence (2026-07-31, Perplexity Deep Research).** Standard QCA/fsQCA convention (Ragin terminology) confirms **PRI = Proportional Reduction in Inconsistency**, **SYM consist. = Symmetric Consistency** (applying the same consistency standard to an outcome's presence and its negation). This was verified against general fsQCA methodology sources, not against Ingrams' actual Table 4/methods text directly (paywalled, full text not accessible). Reasonably safe to cite under standard-usage assumption, but not independently confirmed this paper doesn't redefine the terms idiosyncratically — retain as a residual Low-risk caveat if institutional access to the paper becomes available.

⚠ VERIFY BEFORE PUBLISHING #244: The Δcontent formula's θwt (word-similarity score) component is described only abstractly in the source, without precise operational calculation steps — do not attempt to reproduce the formula without the full methods appendix — LOW. **Attempted 2026-07-31 (Perplexity Deep Research): unresolved.** No open-access methods appendix found; genuinely needs manual re-extraction with direct/institutional PDF access.

---

*Node written: 2026-07-15 | Ad hoc pre-Batch-19 session | PRIS v2.3 | Methodological anchor node — resolves the vault's standing "Ingrams 2023" placeholder citation; contains no AI-governance substantive content; machine learning is the analytical instrument, not the regulatory subject*
