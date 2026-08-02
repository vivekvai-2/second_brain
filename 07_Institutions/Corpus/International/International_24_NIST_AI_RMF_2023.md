---
type: Corpus Node
status: active
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/us
  - institution/international
  - theme/ai-risk-management
---

# International_24 — NIST AI Risk Management Framework (AI RMF 1.0) and Companion Materials

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/International/International_24_NIST_AI_RMF_2023.md`
**Institution:** [[07_Institutions/International]]
**Issuing body:** National Institute of Standards and Technology (NIST), U.S. Department of Commerce
**Document date:** AI RMF 1.0 published January 2023 (released 26 January 2023); Generative AI Profile (NIST AI 600-1) published July 2024
**Pages:** Not independently paginated in this extraction
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]]

---

## Instrument Identity

**Full title:** Artificial Intelligence Risk Management Framework (AI RMF 1.0), NIST AI 100-1
**Type:** Voluntary framework / risk-management standard
**Target entities:** U.S. organisations designing, developing, deploying, or using AI systems; increasingly expected (not mandated) for federal agencies and contractors
**Legal basis:** NIST authoring authority under its standards-development mandate; voluntary, non-regulatory
**Companion documents:**
- **NIST AI 600-1 — Generative Artificial Intelligence Profile** (final, published 26 July 2024, superseding an April 2024 public draft; developed pursuant to Executive Order 14110 §4.1(a)(i)(A))
- **NIST AI RMF Playbook** (first complete version 30 March 2023; living document — NIST states it "will be updated after the AI RMF 1.0 is revised," implying a pending future revision not yet issued)
- **NIST AIRC Crosswalk index** (rolling, most recently updated 14 April 2026) — includes an "OECD/EU/EO13960" crosswalk mapping AI RMF trustworthiness characteristics to the OECD AI Recommendation, the EU AI Act, US Executive Order 13960, and the Blueprint for an AI Bill of Rights; and a Microsoft-contributed ISO/IEC 42001 crosswalk (14 August 2025)

**Primary source link:** https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf (DOI 10.6028/NIST.AI.100-1) | landing page https://www.nist.gov/itl/ai-risk-management-framework
**Generative AI Profile:** https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf (DOI 10.6028/NIST.AI.600-1)
**Playbook:** https://www.nist.gov/itl/ai-risk-management-framework/nist-ai-rmf-playbook
**Crosswalk index:** https://airc.nist.gov/airmf-resources/crosswalks/

---

## Analytical Classification

**Wiki section:** S3 (International Regulatory Context)
**Jurisdiction:** United States (voluntary internationally; widely referenced in India, Singapore, Australia per the parent framework note)
**Confidence:** High — primary NIST-hosted text and DOI-registered publications, cross-confirmed
**AI explicit:** Yes
**Tier classification:** Tier A for the RMF itself (dedicated AI risk-management standard); the crosswalk index is a Tier A comparative-methodology resource
**AI Governance Wiki relevance:** HIGH — this corpus previously had zero primary-source citation for NIST despite the framework node's SR-high/RL-low fsQCA prior resting entirely on the RMF's four-function architecture

---

## Substantive Content

### Four-function core
**Govern** (organisational policies, processes, accountability structures — the strategic/cultural layer); **Map** (context, stakeholders, risk categories for a specific system); **Measure** (quantitative/qualitative risk assessment — bias testing, benchmarking, impact assessment); **Manage** (risk prioritisation and response, incident response, residual-risk acceptance). Cyclical, not a sequential checklist.

### Generative AI Profile (NIST AI 600-1)
Extends the four-function core specifically to generative AI and foundation-model risks; issued under Executive Order 14110's direct instruction to NIST, making it the clearest textual link in this corpus between a binding US executive action and a nominally "voluntary" NIST output — relevant to the framework note's "voluntary but increasingly expected" tension.

### Crosswalks — direct evidentiary value for fsQCA/comparative work
The NIST AIRC crosswalk index is a NIST-maintained (not third-party) resource explicitly mapping AI RMF trustworthiness characteristics against the OECD Recommendation, the EU AI Act, and US Executive Order 13960/Blueprint for an AI Bill of Rights. This is the single most directly reusable primary source in this batch for **fsQCA cross-case comparability** — NIST itself, not an external researcher, has already produced a structured mapping between three of the ten candidate fsQCA cases (NIST, OECD, EU AI Act).

### Federal adoption evidence (GAO)
**GAO-25-107653** (28 July 2025, direct primary link confirmed) explicitly cites the AI RMF as "a resource to organizations designing, developing, deploying, or using AI systems," and documents federal agency AI use cases nearly doubling from 571 (2023) to 1,110 (2024) across 11 reviewed agencies — concrete adoption-trajectory evidence for the framework note's "voluntary but increasingly expected" argument.
Link: https://www.gao.gov/assets/gao-25-107653.pdf
**GAO-25-107933** (September 2025, mapping 94 AI-related federal requirements/executive orders/governance structures) and an earlier December 2023 GAO compliance review are referenced only via secondary summaries in this search round (LinkedIn and EPIC.org respectively) — **flagged for direct GAO.gov confirmation before citing figures from either.**

### NIST AI RMF vs. India's IndiaAI/RBI FREE-AI — confirmed gap
No formal, peer-reviewed, or government-issued comparative analysis explicitly juxtaposing the NIST AI RMF against India's IndiaAI Governance Guidelines or RBI's FREE-AI framework was identified. Available material is limited to practitioner commentary noting structural parallels ("India's soft-law, sector-led path similar to the U.S. NIST RMF"). This is a **confirmed open research gap** — a genuine opportunity for original comparative work (P1/P4/fsQCA) rather than a citable existing source. The two India-side primary documents themselves were independently confirmed in this search:
- RBI FREE-AI Committee Report (13 August 2025) — primary RBI.org.in link not independently confirmed in this search round; only a secondary-hosted copy (Khaitan & Co) was located. Flag for direct retrieval from rbi.org.in before citing as a primary source.
- India AI Governance Guidelines (PIB-circulated, 4 November 2025) — confirmed to explicitly adapt "seven guiding principles or sutras" from the RBI FREE-AI Committee Report. Link: https://static.pib.gov.in/WriteReadData/specificdocs/documents/2025/nov/doc2025115685601.pdf

---

## Analytical Significance for PRIS Research

### For fsQCA and P4 (Doctrinal Analysis)
The NIST-authored crosswalk (OECD/EU/EO13960) directly supports the framework note's SR-high/RL-low prior by giving an independent, non-PRIS-authored confirmation that these frameworks are commensurable on trustworthiness characteristics despite differing enforcement postures — strengthening the methodological defensibility of treating them as comparable fsQCA cases.

### Confirmed research gap for original contribution
The absence of any existing NIST RMF vs. IndiaAI/RBI FREE-AI comparative study is a genuine white space — worth flagging explicitly in [[contribution-framing]] work as a defensible original-comparison claim, since the primary documents on both sides are now independently confirmed and coded in this corpus.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/International/International_23_OECD_AI_Principles_2019_2024]] (crosswalk target), [[07_Institutions/Corpus/International/International_18_UNESCO_Recommendation_Ethics_AI_2021]], [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]], [[07_Institutions/Corpus/MeitY/MeitY_2]] (India AI Governance Guidelines)
**Related concepts:** [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] (Govern function — role/accountability specification), [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Transparency]]
**Related frameworks:** [[06_Frameworks/NIST_AI_RMF]] (parent framework/synthesis node — this Corpus Node supplies its primary-source grounding), [[06_Frameworks/OECD_AI_Principles]], [[06_Frameworks/EU_AI_Act]], [[06_Frameworks/RBI_Free_AI]], [[06_Frameworks/IndiaAI_Framework]]
**Related projects:** [[02_Projects/P1_SLR_RG]], [[02_Projects/P4_Doctrinal_IJLIT]], [[08_Methods/fsQCA]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** Screening corpus — BFSI-adjacent via crosswalk/comparative value, not a direct Indian BFSI instrument
- **Wiki intake status:** Pending — HIGH priority for S3 update

---

## Log

- 2026-08-02: Corpus node created. Sourced via Perplexity Deep Research per [[Thin_Node_Perplexity_Prompts_2026-08-02]] NIST prompt. Closes the "framework has zero evidence links" gap flagged in the 2026-08-02 thin-node audit. GAO-25-107933 and the December 2023 GAO compliance review are flagged pending direct GAO.gov verification — not yet cited as confirmed primary sources.
