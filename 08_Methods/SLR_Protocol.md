---
type: Method
tags:
  - type/method
  - status/active
  - paper/p1-primary
  - gate/open
  - engine/phd
---

# SLR Protocol

**Type:** Method **Status:** Active **Last Updated:** 2026-07-15

---

## Core Synthesis

Systematic Literature Review (SLR) is the foundational method for P1 and the evidence-synthesis scaffold for the theoretical front-ends of P2, P3, and P4. In PRIS, SLR is not applied uniformly — P1 uses a PRISMA-informed full SLR to build the AI governance typology; P2/P3/P4 use structured literature intake to establish theoretical scaffolding without generating a standalone SLR contribution. This distinction matters for both methodology reporting and journal positioning: P1's contribution is the typology derived from SLR; the other papers' contributions are empirical and do not depend on SLR as a method per se. This note records the SLR protocol decisions made for P1 and the lessons learned from the GIQ desk rejection.

## Method Profile

- **Type:** Secondary research synthesis; evidence-based literature analysis
- **Standard:** PRISMA 2020 (Preferred Reporting Items for Systematic Reviews and Meta-Analyses)
- **Scope (P1):** AI governance frameworks — ethical, regulatory, institutional; 2015–2025; English language; peer-reviewed journals and major policy documents
- **Database coverage:** Scopus, Web of Science, SSRN, Google Scholar supplementary
- **Key anchors:** Page et al. (2021) — PRISMA 2020; Tranfield et al. (2003) — SLR in management research; Fiss (2011) — typology-building from SLR logic

## Application in PRIS

### P1 — AI Governance SLR (R&G, deferred to Q3 2027)

- **Purpose:** Generate the AI governance archetype typology (9 archetypes × 3 dimensions: RL, SR, SI) that feeds the fsQCA chapter as theoretical scaffolding
- **Corpus:** 49-instrument PRISMA-informed corpus (F1–F49 in `V12_SOM.docx`) — coded at rule level using IG 2.0
- **Status:** Corpus assembled and coded; typology derived; standalone P1 paper deferred post-defence
- **Lesson from GIQ desk rejection:** The desk rejection on narrative architecture failure (not substance) established that SLR-generated typology requires a contribution framing that foregrounds the typology's explanatory power, not the SLR process itself. The Fiss (2011) typology-validation logic — SLR builds the typology; fsQCA validates configurations — is the correct framing for R&G submission.

### P2/P3/P4 — Structured Literature Intake (not standalone SLR)

- **Purpose:** Establish theoretical scaffolding (Institutional Theory, Agency Theory, Regulatory Governance Theory, IS theory) without PRISMA-level systematic process
- **Method:** Targeted database searches + snowballing from key anchor papers + Perplexity-assisted recent literature scanning
- **Output:** Theoretical framework sections in each paper — not a reported SLR

## Protocol Decisions (P1-specific)

|Decision|Choice|Rationale|
|---|---|---|
|Inclusion criteria|Peer-reviewed + major policy documents (OECD, UNESCO, NIST, EU AI Act)|AI governance literature spans academic and policy registers equally|
|Exclusion|Pre-2015, non-English, grey literature below policy-document tier|Manageability; post-2015 captures the post-OECD-Principles generation|
|Quality assessment|Methodological quality assessment per Tranfield et al. (2003)|ABDC-A publication standard requirement|
|Coding unit|Framework / instrument as unit; rule as sub-unit|Matches IG 2.0 coding granularity|
|Synthesis method|Configurational (Fiss 2011 typology logic)|Produces typology contribution, not narrative synthesis|
|Search strategy / filters / supplementary search / search-transparency reporting|**Not yet documented** — flagged gap, 2026-07-15|See gap note below|

**Documented gap, flagged 2026-07-15:** this table covers inclusion/exclusion, quality assessment, coding unit, and synthesis method, but has no entry for search strategy, search filters, supplementary search methods (snowballing/citation-checking), or a search-transparency reporting standard. [[04_Knowledge_Products/Wiki_Intake/F096_Booth_Searching_Qualitative_Research_SLR_2016|F096]] (Booth, 2016, *Systematic Reviews*) supplies a directly adoptable structure for closing this gap: the **7S framework** (Sampling, Sources, Structured questions, Search procedures, Search strategies/filters, Supplementary strategies, Standards), the **CLUSTER** supplementary-search checklist (Citations, Lead authors, Unpublished materials, Scholar/Google, Theories, Early examples, Related projects), and the empirical case for snowballing (multiple audits found 50%+ of included studies come from snowballing/personal contact, not database search alone). Booth's paper is healthcare-domain-illustrated and its specific filter-performance figures are not transferable to an AI-governance corpus, but its structural framework is domain-general. Evaluate before P1 is reactivated (Q3 2027) and before the methods section is finalised.

**Screening-efficiency candidate, added 2026-07-16:** [[04_Knowledge_Products/Wiki_Intake/F113_Kempeneer_Pirannejad_Wolswinkel_OGD_Legal_Perspective_AI_SLR_2023|F113]] (Kempeneer, Pirannejad & Wolswinkel, 2023, *Government Information Quarterly*) used **ASReview**, an open-source active-learning screening tool, to triage a 2,598-record title/abstract candidate pool after a 30-record "prior knowledge" training set — reaching its stopping criterion (top 100 relevant records) after reviewing only ~522 records, roughly 20% of the full pool (~80% screening-burden reduction). This addresses a different sub-problem than F096's search-strategy gap-fill: F096 covers *finding* candidate studies; F113 covers *triaging* a large candidate pool once found. Worth evaluating for P1's SLR reactivation if the candidate pool (post-search) proves large — not yet trialled or committed to.

## Lessons Learned

**GIQ desk rejection (14 April 2026):** The paper was rejected on narrative architecture failure, not substance quality. The typology content was sound; the failure was in framing SLR findings as an intrinsically valuable literature contribution rather than as the scaffolding for a typology claim. The DDP (Drafting Discipline Protocol) directly addresses this: contribution claim before 500 words; typology as the output, SLR as the method.

**Implication for P1 (Q3 2027):** When P1 is reactivated, the R&G submission must frame the SLR as the evidence base for a typology that the fsQCA chapter then validates — Fiss (2011) logic applied explicitly, not implicitly.

## Linked Projects

- [[P1_SLR_RG]]
- [[P2_DPI_JSIS]] _(structured intake only)_
- [[P3_BFSI_JEIM]] _(structured intake only)_
- [[P4_Doctrinal_IJLIT]] _(structured intake only)_

## Linked Methods

- [[fsQCA]]
- [[Institutional_Grammar_IG2]]

## Linked Domains

- [[AI_Governance]]

---

_Back to [[_Methods_MOC]]_