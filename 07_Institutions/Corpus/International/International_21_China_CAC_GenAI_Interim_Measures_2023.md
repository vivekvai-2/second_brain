---
type: Corpus Node
tags:
  - type/corpus-node
  - status/active
  - series/format-a
  - section/S3
  - section/S1
  - tier/high
  - project/p1
  - project/p3
  - project/fsqca
  - institution/CAC
  - jurisdiction/China
  - engine/phd
---

# International_21 — China (CAC et al.): Interim Measures for the Management of Generative Artificial Intelligence Services (2023)

**Type:** Corpus Node (Format A)
**Vault path:** `07_Institutions/Corpus/International/International_21_China_CAC_GenAI_Interim_Measures_2023.md`
**Institution:** Cyberspace Administration of China (CAC), jointly with NDRC, Ministry of Education, MOST, MIIT, MPS, NRTA
**Issuing body:** Cyberspace Administration of China (lead) — seven-ministry joint promulgation
**Document date:** Approved 10 July 2023 (12th CAC Office Affairs Meeting) / published 13 July 2023 / effective **15 August 2023**
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/International_Comparators]]
**Batch:** Ad hoc — gap-directed sourcing (Perplexity Deep Research → China Law Translate primary text → NotebookLM PROMPT 0b), pre-Batch 19 session
**Source corpus:** Gap-fill for AIGP BoK (F055) Domain II (Laws & Standards) gap — the vault's first primary-source China AI regulatory instrument, closing a citation gap that [[04_Knowledge_Products/Wiki_Intake/F048_FLI_AI_Safety_Index_Winter_2025]] had already flagged generically ("Interim Measures for GenAI") without ingesting the source.

---

## Instrument Identity

**Chinese title:** 生成式人工智能服务管理暂行办法
**Translated title:** Interim Measures for the Management of Generative Artificial Intelligence Services
**Translation source:** China Law Translate (crowdsourced, not CAC-certified); cross-referenced against the Air University/CASI ITOW translation
**Type:** Departmental regulatory instrument (部门规章) — binding but sub-statutory; sits below administrative regulations (行政法规) and laws (法律) in China's legislative hierarchy
**Structure:** 5 chapters, 24 articles, ~2,200–2,500 words in English translation — a notably short, principles-plus-obligations instrument compared to the EU AI Act's length
**Legal basis cited:** Cybersecurity Law of the PRC; Data Security Law; Personal Information Protection Law; Law on Scientific and Technological Progress
**Applicability:** GenAI services provided to the (mainland) public within the PRC, including via APIs; excludes non-public-facing R&D by enterprises/research institutions and sector-specific carve-outs (news/publishing, film/TV, artistic creation) where other state provisions apply

---

## Scope and Purpose

The Measures are the PRC's first dedicated, binding regulatory instrument governing generative AI specifically (as distinct from the earlier Deep Synthesis Provisions, effective January 2023, which govern synthetic-media techniques more broadly). Article 3 states the governing philosophy explicitly: **"the state is to adhere to the principle of placing equal emphasis on development and security... carrying out tolerant and cautious graded management by category of generative AI services"** — a development-security balance and tiered/categorised management doctrine that recurs throughout the instrument's enforcement design (Art. 16's "regulation by type and grade," Art. 17's risk-triggered security-assessment threshold).

Article 4 imposes five categories of mandatory content and process obligations on **both providers and users** (a deliberate broadening from the April 2023 draft, which applied only to providers): (1) prohibition on content violating core socialist values / national security; (2) anti-discrimination measures across race, ethnicity, faith, nationality, region, sex, age, profession, health; (3) IP and fair-competition protection; (4) protection of personal rights (image, reputation, privacy); (5) transparency and accuracy obligations.

---

## Framework Architecture

### Five-Chapter, Twenty-Four-Article Structure

| Chapter | Title | Articles | Core content |
|---|---|---|---|
| **I** | General Provisions | 1–4 | Legal basis, scope, development-security philosophy, five mandatory provider/user obligations |
| **II** | Development and Governance of Technology | 5–8 | State encouragement of innovation; infrastructure/international-cooperation provisions; training-data lawful-source and quality obligations (truth/accuracy/objectivity/diversity); human-annotation quality controls |
| **III** | Service Specifications | 9–15 | Producer/personal-information-handler liability; service agreements; minor-protection (anti-addiction); data minimisation; content labelling (cross-references Deep Synthesis Provisions); service continuity; two-tier content/user-violation response; complaint mechanisms |
| **IV** | Oversight Inspections and Legal Responsibility | 16–21 | Multi-regulator enforcement (7 named departments); security-assessment and algorithm-filing trigger for services with "public opinion properties or capacity for social mobilization"; user complaint right; cooperation-with-inspection duties; **extraterritorial technical-measures enforcement**; penalty regime (cross-referenced, not self-contained) |
| **V** | Supplementary Provisions | 22–24 | Definitions (GenAI technology / provider / user — API providers explicitly included); permit and foreign-investment carve-outs; effective date (15 Aug 2023) |

### Enforcement Design — Three Load-Bearing Features

1. **No self-contained monetary penalty.** The April 2023 draft included a fine of up to CNY 100,000; this was deleted before promulgation. Article 21 instead cross-references penalties under the Cybersecurity Law, Data Security Law, PIPL, and the S&T Progress Law, falling back to warnings/circulated criticism/corrections/service suspension where those laws are silent. This is a materially lighter direct-sanction architecture than the EU AI Act's turnover-based fines.
2. **Risk-triggered security assessment (Art. 17).** Services with "public opinion properties or the capacity for social mobilization" must undergo security assessment and algorithm filing. **Corrected 2026-07-31 (see VERIFY #224 resolution):** the operationalizing instrument is not the Algorithmic Recommendations Provisions (2022) as originally stated here, but the earlier, purpose-built CAC/Ministry of Public Security "Provisions on the Security Assessment of Internet Information Services with Public Opinion Properties or Capacity for Social Mobilization" (effective 30 November 2018), incorporated by cross-reference. That 2018 instrument defines the trigger functionally (Art. 2: forums/blogs/livestreaming/information-sharing-type services, plus any other service providing public-opinion-expression channels or mobilization capacity) rather than quantitatively — no user-count threshold exists in any instrument. Per 2023–2025 legal-practice commentary, this functional test is broad enough that most consumer-facing GenAI services are treated as presumptively in-scope.
3. **Extraterritorial enforcement via access-blocking, not fines (Art. 20).** Where an overseas GenAI service fails to meet the Measures, CAC "shall notify the relevant organs to employ technical measures and other necessary measures" — the standard PRC formulation for network-level blocking, not a claim of extraterritorial monetary jurisdiction. This is a structurally distinct enforcement model from the EU AI Act's extraterritorial-fine approach and from India's DPDP Act (which has no equivalent blocking mechanism).

---

## Regulatory Significance

### Comparison with EU AI Act, RBI FREE-AI, and DPDP Act

| Dimension | China GenAI Measures (2023) | EU AI Act | RBI FREE-AI (2025) | India DPDP Act (2023) |
|---|---|---|---|---|
| Legal form | Departmental regulation (sub-statutory) | Regulation (directly binding, statutory) | Regulatory framework/principles (RBI statutory authority) | Statute |
| Direct AI-specific fine | None (deleted from draft) | Up to 3%/EUR 35m (prohibited practices) | No specified AI-specific fine; supervisory action | No AI-specific fine (data-processing focus) |
| Extraterritorial mechanism | Technical measures (blocking) against non-compliant overseas services | Extraterritorial application + fines | N/A (domestic BFSI) | Extends to processing of Indian residents' data by any entity |
| Enforcement trigger | Multi-regulator (7 departments), risk-graded by "public opinion/social mobilization" capacity | Risk-tiered (prohibited/high-risk/limited/minimal) | Principles-based ("should") | DPIA-triggered for significant data fiduciaries |
| Training-data obligations | Lawful source + IP + consent + quality (truth/accuracy/objectivity/diversity) — Art. 7 | Data governance obligations for high-risk systems (Art. 10) | No codified training-data standard | No AI-specific training-data provision |
| Content labelling | Mandatory, cross-referenced to Deep Synthesis Provisions; later layered by GB 45438-2025 (Sept 2025) | Art. 50 transparency/labelling obligations for GPAI | N/A | N/A |

### Layered Instrument Architecture

The Measures are the base layer of a now four-instrument Chinese GenAI regulatory stack, per the user's own research pass: (1) these Interim Measures (2023, general obligations); (2) Deep Synthesis Provisions (2023, synthetic-media labelling, cross-referenced at Art. 12); (3) AI Labelling Measures + GB 45438-2025 (effective September 2025, elaborating the Art. 12 labelling obligation into a binding national standard); (4) Anthropomorphic AI Interactive Services Measures (effective 15 July 2026, the same day as this extraction). This layering pattern — a short principles-based base instrument progressively elaborated by binding technical standards — is itself a distinct regulatory-design configuration worth tracking against the EU's single-instrument-plus-delegated-acts model and India's currently single-layer (no elaboration) advisory model.

---

## Implications for Indian Governance

China is the corpus's first primary-source instance of a **mandatory, multi-regulator, sub-statutory GenAI regime with graded risk triggers but no self-contained fine** — a fourth configuration alongside the EU's binding-statute-with-fines model, Australia's voluntary-government-as-deployer model (International_20), and India's own advisory/principles-based posture (NITI_7, MeitY_2, RBI FREE-AI). For fsQCA calibration, China's Evaluative Authority (EA) score is a mixed case: mandatory obligations exist (high nominal EA) but enforcement is deliberately softened (no fine, corrections-first) relative to the EU (high EA, hard sanction). This nuance is analytically useful for avoiding a binary "mandatory vs voluntary" EA coding and supports a graded EA operationalisation.

India has no equivalent to: (a) the Art. 7 training-data quality mandate (truth/accuracy/objectivity/diversity); (b) the Art. 17 risk-triggered security-assessment/algorithm-filing mechanism; (c) the Art. 20 extraterritorial technical-measures enforcement against non-compliant overseas GenAI services (DPDP Act's extraterritorial reach is data-processing-scoped, not service-blocking-scoped).

---

## Connections

**[[P1_SLR_RG]]:** S3 (international frameworks) — closes a citation gap the SLR corpus has carried since Batch 14 (F048's generic "Interim Measures for GenAI" reference); this node is the primary source.

**[[fsQCA_Thesis_Chapter]]:** Adds a fourth EA/SR configuration point (mandatory-but-softened enforcement) distinct from EU (mandatory-hard), Australia (voluntary-internal, International_20), and India (advisory, EA≈0). Supports graded rather than binary EA coding.

**[[P3_BFSI_JEIM]]:** Indirect — China's multi-regulator (7-department) enforcement architecture is a comparator for India's own multi-silo (RBI/SEBI/MeitY/TRAI/ICMR) fragmentation, though China's instrument at least names all seven regulators within a single text rather than issuing seven uncoordinated instruments.

**Concept links:**
- [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — directly completes the citation [[04_Knowledge_Products/Wiki_Intake/F048_FLI_AI_Safety_Index_Winter_2025]]'s Batch 14 entry left open ("Chinese mandatory reporting... Interim Measures for GenAI" — this is that instrument, now primary-sourced). Also a new instance in its own right: Art. 12's labelling obligation and the later GB 45438-2025 standard are a domestic (intra-China) instrument-layering case, not cross-jurisdictional parallelism — worth distinguishing from the corpus's usual cross-regulator parallelism pattern.
- [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] — the 7-department joint promulgation (single instrument, multiple named enforcement agencies) is a coherence-by-design counterpoint to India's coherence-by-absence pattern (separate uncoordinated instruments from RBI/SEBI/MeitY).
- [[05_Concepts/05_Concepts_Standard/Accountability]] — Art. 9's producer-liability + personal-information-handler dual accountability framing.
- [[05_Concepts/05_Concepts_Standard/Transparency]] — Art. 4(5) and Art. 12 labelling obligations.

**Related nodes:**
- [[04_Knowledge_Products/Wiki_Intake/F048_FLI_AI_Safety_Index_Winter_2025]] — the instrument this node's ingestion was specifically sourced to primary-cite (Batch 14 flagged this as a gap).
- [[07_Institutions/Corpus/International/International_9]] (BIS/FSI Insights No. 63) — China is one of seven jurisdictions in that comparative financial-AI-governance study; this node now gives that comparator a primary-source anchor.
- [[07_Institutions/Corpus/International/International_18_UNESCO_Recommendation_Ethics_AI_2021]] (UNESCO Recommendation, 2021) — China is one of 193 adopting states; this node is China's binding domestic instrument, contrasted against the non-binding global norm.
- [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]] — Supreme Court's 13-jurisdiction comparative survey names China among its comparators without primary-sourcing the instrument; this node fills that gap.
- [[04_Knowledge_Products/Wiki_Intake/NITI_8_DeepSeek_AI_Shifts_2025]] — positions China as the "security-sensitive" comparator against India's "sovereign and ethical AI" and the US's "capital-dominant" models; this node gives that framing a primary regulatory-text basis.

---

## VERIFY Flags

**#224 — RESOLVED (2026-07-31, Perplexity Deep Research), Medium confidence overall.**

**(1) Article 17 threshold — operationalized, Medium-High confidence.** The trigger phrase is operationalized not by a new CAC document for GenAI specifically, but by cross-reference to the pre-existing CAC/MPS "Provisions on the Security Assessment of Internet Information Services with Public Opinion Properties or Capacity for Social Mobilization" (effective 30 Nov 2018) — see corrected framework summary above. The test remains qualitative/functional (service-category based), not quantitative — no user-count threshold exists anywhere in the applicable instruments. No 2025/2026 CAC guidance introducing numeric thresholds was found. Practical effect: most consumer-facing GenAI services are presumptively in-scope given the functional categories' breadth. **EA coding implication: this strengthens rather than weakens China's nominal EA score — the trigger is broad and low-bar, not narrow/rarely-invoked as an undefined-threshold framing might suggest.**

**(2) Article 2 B2B/API exclusion — Medium confidence.** Converging legal-practice consensus: pure enterprise-internal API deployments (no downstream public-facing product) are excluded; but a B2B API vendor whose enterprise client resells the capability to consumers does not escape the regime — obligations attach further up/down the supply chain based on who ultimately "provides" the service to the public, consistent with "technical supporter" treatment under the related Algorithm/Deep Synthesis Provisions. No definitive CAC enforcement precedent found on this specific edge case — remains legal-practice interpretation, not settled CAC ruling.

**(3) Fine-deletion rationale — Low confidence, genuinely unresolved.** Deletion of the draft CNY 100,000 fine is independently confirmed as fact by multiple law-firm bulletins, but no official CAC statement or authoritative source explains *why*. Vivek's working hypothesis (enforcement deferred to Cybersecurity Law/Data Security Law/PIPL/S&T Progress Law rather than a self-contained penalty) is plausible and consistent with general PRC tech-regulation drafting patterns, and is in fact already the framing used in this node's own Key Findings §1 (Art. 21 cross-references those exact statutes) — but this should be treated as **informed inference, not a sourced fact**. No academic paper on the Measures' legislative history was found that addresses this directly.

Flag closed — item (1) resolved into the node text above; items (2) and (3) retained as standing interpretive caveats for any scope-boundary or fine-severity comparative claims.

**#225 — CLOSED, standing caveat (2026-07-31).** Self-resolving by design: (1) date question already resolved in-node (13 July treated as publication, 10 July as approval, consistent with corroborating sources) — no change needed. (2) and (3) are already-correct standing caveats — CLT's non-certified status and the Art. 3 translation-phrasing divergence — that should be retained verbatim and re-checked only if this node is ever used for direct-quote publication-track material. No further action needed.

---

*Node written: 2026-07-15 | Gap-directed sourcing (Gap #2, China AI regulation) — Perplexity Deep Research confirmation → NotebookLM PROMPT 0b extraction → PRIS classification | PRIS v2.2*
