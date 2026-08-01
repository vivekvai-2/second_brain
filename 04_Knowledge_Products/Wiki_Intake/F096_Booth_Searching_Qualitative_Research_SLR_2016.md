---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S7
  - tier/methodological-anchor
  - project/p1
  - method/slr-search-methodology
  - batch/adhoc-2026-07-15
  - engine/phd
---

# Booth: Searching for Qualitative Research for Inclusion in Systematic Reviews — A Structured Methodological Review (2016)

**Node ID:** F096
**Type:** Wiki Intake Note (Format B) — **Methodological Anchor** (no AI-governance content; opportunistic addition)
**Wiki Section:** S7 (Research Methods)
**Status:** Active
**Tier:** Methodological anchor — fills a documented gap in [[08_Methods/SLR_Protocol]]'s search-methodology detail
**Jurisdiction:** Method-general (healthcare/health-services research illustrative domain)

---

## Source

**Full Citation (APA):** Booth, A. (2016). Searching for qualitative research for inclusion in systematic reviews: a structured methodological review. *Systematic Reviews*, *5*(1), 74. https://doi.org/10.1186/s13643-016-0249-x — **published 4 May 2016** (confirmed 2026-07-31, see VERIFY #251 resolution)
**Document Type:** Academic paper — structured methodological review (BioMed Central, *Systematic Reviews* journal)
**Author:** Andrew Booth (School of Health and Related Research, ScHARR, University of Sheffield)
**Batch:** Ad hoc, pre-Batch-19 (NotebookLM relay, PROMPT 0b) | 2026-07-15
**Pages:** 23

---

## Scope Note — Why This Node Exists

This paper has **no AI-governance subject matter** — it is a methodological review of how systematic reviews should search for and identify qualitative research, illustrated primarily with health-services examples (MEDLINE/EMBASE/CINAHL/PsycINFO filters, breastfeeding-support and alternative-medicine review case studies). It does not back any pre-existing bare citation — it is added **opportunistically** because it directly addresses a gap in [[08_Methods/SLR_Protocol]]: that method note's "Protocol Decisions" table specifies inclusion/exclusion criteria, quality assessment, and coding unit for P1, but has **no documented search-strategy, search-filter, supplementary-search, or search-transparency-reporting detail** — exactly what this paper supplies a structured framework for.

**Domain-transferability caveat (important, not a VERIFY flag):** Booth's specific numeric findings (database sensitivity/specificity figures, filter performance statistics) are healthcare-database-specific (MEDLINE, EMBASE, CINAHL, PsycINFO) and **not directly transferable** to P1's AI-governance corpus (Scopus, Web of Science, SSRN, Google Scholar). The paper's value to PRIS is structural/methodological (the 7S framework, reporting-standard logic, supplementary-search-strategy evidence), not its specific figures.

---

## Key Findings and Framework

### The 7S Framework — directly reusable structure

Seven-part structure for systematic approaches to searching, used as this paper's own organising taxonomy and directly adoptable as a search-methodology reporting checklist:

1. **S**ampling — how many studies is "enough"; when to stop searching
2. **S**ources — database coverage, grey literature, books/chapters, theses
3. **S**tructured questions — formulating the review question (PICO-family notations)
4. **S**earch procedures — the search process itself
5. **S**earch **s**trategies and filters — validated search filters
6. **S**upplementary strategies — citation checking, hand searching, snowballing, expert contact
7. **S**tandards — reporting standards for search transparency

**Direct application to P1:** [[08_Methods/SLR_Protocol]]'s current documentation covers only a subset (roughly "Sources" and part of "Structured questions," via its inclusion-criteria table) — Sampling rationale, Search strategies/filters, Supplementary strategies, and Standards (search-reporting transparency) are all currently undocumented for P1's 49-instrument corpus. Adopting the 7S structure explicitly would strengthen P1's methods section, particularly given the prior GIQ desk rejection's emphasis on methodological rigor in framing.

### Structured Question Notations (Table 4) — candidate for P1's research-question formulation

Eleven named notations for formulating review questions, several of which extend beyond the standard PICO used in quantitative reviews: 3WH, BeHEMoTh, CIMO, ECLIPSe, PEICO(S), PICO, PICo, PICOC, PICOS, SPICE, SPIDER. **CIMO** (Context, Intervention, Mechanisms, Outcomes) and **SPICE** (Setting, Perspective, Intervention, Comparison, Evaluation) are the two most plausibly adaptable to an AI-governance-instrument review question, being less clinically-specific than the others — worth evaluating against P1's actual research question if the SLR is reactivated.

### Supplementary Search Strategies — strong empirical case for snowballing over pure database search

Repeatedly documented finding across multiple cited audits: database searching alone is insufficient. One audit found only 30% of included studies identified via databases/hand searches, ~50% via "snowballing," and 24% via personal knowledge/contact. Citation checking, reference checking, and expert contact yielded 11 of 41 included studies in another case study. **Bates' berry-picking approach** and the **CLUSTER approach** (Citations, Lead authors, Unpublished materials, Scholar/Google, Theories, Early examples, Related projects) are both named, structured supplementary-search methodologies — CLUSTER in particular is a readily adoptable checklist for P1's snowballing phase.

### Reporting Standards — PRISMA, STARLITE, ENTREQ

- **PRISMA** (already P1's adopted standard, per SLR_Protocol.md) — the quantitative-review reporting standard.
- **STARLITE** (Standards for Reporting Literature Searches) and **ENTREQ** (ENhancing Transparency in REporting the synthesis of Qualitative research) — qualitative-synthesis-specific reporting standards, mapped against each other in the paper's Table 6. Notable finding: only 1 of 19 papers published since ENTREQ's release actually used it — a low-adoption cautionary data point.
- Given P1's corpus mixes academic and policy-document literature (not purely qualitative synthesis), PRISMA remains the primary standard, but the paper's general principle — "make literature search processes as transparent as possible, even when complex" — and its emphasis on explicitly justifying sampling/stopping criteria are directly applicable regardless of quant/qual classification.

### Sampling Guidance (candidate answer to "how many is enough")

"Preferred number of between 6 and 14 studies" for tightly-scoped syntheses, "maximum of about 40 papers" for maintainable familiarity, with 81% of published meta-ethnographies using exhaustive (not purposive) search strategies. P1's 49-instrument corpus sits just above this "maintainable familiarity" ceiling — not a criticism, since P1's PRISMA/typology-building design differs structurally from meta-ethnography, but a useful benchmark if P1's methods section needs to justify corpus size.

---

### Additional Empirical Detail (added 2026-07-16, missed in original intake — second NotebookLM paste of the same source)

**Search yield and study composition:** 1717 references identified overall (654 from the author's own 7-year Cochrane Qualitative and Implementation Methods Group study register + citation searches seeded from 15 "citation pearls," Table 1, totalling 1063 citations across the 15 seed papers — individual counts range from 21 (Finfgeld-Connett & Johnson 2013) to 152 (Barroso et al. 2003)); 1299 records after de-duplication; **113 items** retained for the final methodological review. Composition of the 113: 46 overviews of QES methodology, 13 formal guidance documents, 3 narrative reviews of the QES search process specifically, 1 short general summary, 7 hybrid-design items, 43 formal study-design items (of which: case study 25, comparative study 7, literature surveys 5, multiple case studies 1, surveys 1, validation study 4).

**7S framework distribution across the 113 items:** Sampling n=47, Supplementary Strategies n=24, Sources n=22, Structured Questions n=17, Standards n=17, Search Strategies/Filters n=16, Search procedures n=6 — sampling is by a wide margin the most-studied 7S dimension in the methodological literature itself, a useful prioritisation signal if P1's methods section documents its own 7S dimensions in sequence.

**Table 3 — sampling method by synthesis-method taxonomy** (not previously captured): Critical interpretive synthesis (purposive + theoretical sampling); Grounded theory-based approaches (theoretical sampling); meta-aggregation (comprehensive sampling); meta-ethnography (purposive + theoretical sampling); meta-interpretation (maximal divergent/maximum variation + theoretical sampling); meta-narrative synthesis (purposive sampling of key papers); qualitative meta-synthesis (comprehensive/representative sampling); realist synthesis (comprehensive + purposive + theoretical + snowball sampling, the widest combination); scoping review (random sampling). Precedent worth citing if P1's methods section needs to justify its own sampling logic against a named synthesis-method family rather than asserting it de novo.

**Table 5 — validated qualitative search-filter performance** (not previously captured): sensitivity/specificity pairs for MEDLINE, EMBASE, PsycINFO, and CINAHL, each reported at three tuning settings (maximise sensitivity / maximise specificity / best balance) — e.g. MEDLINE best-balance 92/92, CINAHL maximise-sensitivity 99/54, PsycINFO maximise-specificity 50/99. Numerically confirms — rather than just asserting — the domain-transferability caveat already recorded above: these filters are healthcare-database-specific and not usable directly against P1's Scopus/WoS/SSRN corpus, but the sensitivity-vs-specificity tuning trade-off is a transferable design concept for any future P1 filter construction.

**Reporting standards, extended:** two further standards beyond STARLITE/ENTREQ (already captured) — **RAMESES** (Realist And Meta-narrative Evidence Syntheses: Evolving Standards) and **eMERGe** (Meta-Ethnography Reporting Guideline) — both named in the paper's "Towards a research agenda" discussion, rounding out the qualitative-synthesis reporting-standards landscape.

**Sources detail:** database-count distribution across a 2012–2013 QES sample — 37% searched 3–5 databases, 28% searched 6–8, 14% searched 9–11, 14% searched 12–14, 7% searched >16; a cautionary counter-example where 67 databases were searched yet 87% of included studies still came from PubMed alone; CINAHL's 4.5 million records cover roughly a quarter of MEDLINE's volume.

**Search-procedure precision figure:** "only 4% of papers proving to be relevant at full-text screening" cited as a low-precision-filter example, alongside "only 30 of 100 trials had associated qualitative work" as the underlying rationale for why qualitative literature is structurally harder to locate than quantitative literature — both reinforce (with numbers) the paper's core "qualitative searching is slow, labour-intensive, difficult to replicate" thesis already summarised in this node.

No new VERIFY flags required — the only uncertain items in this second extraction (exact publication day/month; absence of source page numbers beyond a single "Page 8 of 23" header) are the same items already covered by #251.

---

## Relevance to PRIS Research

### For [[08_Methods/SLR_Protocol]] / [[P1_SLR_RG]] (primary — direct methodological gap-fill)

Closes an identified documentation gap: P1's Protocol Decisions table has no search-strategy, filter, supplementary-search, or search-transparency-standard entries. The 7S framework, CLUSTER approach, and the transparency-reporting principle are all directly citable additions if P1's methods section is expanded when the paper is reactivated (Q3 2027 per the pipeline).

---

## Connections

**Related concepts:** None — pure methods paper, no PRIS concept links.

**Related corpus nodes:** None directly comparable — this is the corpus's first dedicated SLR-search-methodology node (distinct from the fsQCA-methods cluster F087–F093 and the theory-foundations node F095).

**Related methods:** [[08_Methods/SLR_Protocol]]

**Related projects:** [[P1_SLR_RG]]

---

## VERIFY Flags

**#251 — RESOLVED (2026-07-31, web search).** Confirmed published **4 May 2016** — High confidence, cross-referenced across BioMed Central/Springer Nature Link and the journal's own article page (DOI 10.1186/s13643-016-0249-x). Citation above updated with volume/issue (5(1)) and exact date.

---

## Log

- 2026-07-15: Node created. Ad hoc pre-Batch-19 NotebookLM relay session. PRIS v2.3.
- 2026-07-16: Enrichment. NotebookLM Ingestion Pipeline (PROMPT 0b) re-paste of the same source. Duplicate check against [[Corpus_Index_MOC]] confirmed exact match to this existing F096 node before any content was written. Added delta only (Table 1 citation-pearl counts, Table 3 sampling-by-synthesis-method taxonomy, Table 5 filter sensitivity/specificity figures, 113-item composition breakdown, 7S distribution counts, RAMESES/eMERGe standards, database-count distribution, precision figures) per the Bidirectional_Linking_Convention enrichment discipline — node not recreated, no rewrite. No new VERIFY flags; existing #251 already covers the residual publication-date uncertainty.
- 2026-07-31: VERIFY #251 resolved via web search — confirmed publication date 4 May 2016. Citation updated with volume/issue and exact date. This closes the final open item from the 2026-07-31 Cowork VERIFY-flag-resolution batch (Parts A–D, ~30 flags across two sessions).

---

*Node written: 2026-07-15 | Ad hoc pre-Batch-19 session | PRIS v2.3 | Methodological anchor node — opportunistic addition filling a documented search-methodology gap in SLR_Protocol.md; contains no AI-governance substantive content; healthcare-domain figures not directly transferable, structural framework is*
*Enriched: 2026-07-16 | NotebookLM Ingestion Pipeline*
