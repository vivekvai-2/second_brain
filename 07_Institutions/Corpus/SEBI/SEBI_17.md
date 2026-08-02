---
type: corpus-node
node-id: SEBI_17
institution: SEBI
date: 2019-01-04
wiki-section: S2
tier: A
ai-explicit: true
tags:
  - type/corpus-node
  - institution/SEBI
  - wiki-section/S2
  - tier/A
  - batch/11
  - concept/Regulatory_Parallelism
  - concept/Accountability
  - concept/Transparency
  - concept/Governance_Debt
  - project/P3
  - project/P4
  - project/fsQCA
---

# SEBI_17 — Reporting for AI/ML Applications by Market Intermediaries (SEBI, 2019)

**Node ID:** SEBI_17  
**Institution:** Securities and Exchange Board of India (SEBI)  
**Document type:** Regulatory — SEBI Circular  
**Date:** January 4, 2019  
**Jurisdiction:** India  
**Wiki Section:** S2 — India Regulatory  
**Tier:** A (primary SEBI circular; verbatim quotes extracted)  
**Source PDF:** Reporting for Artificial Intelligence (AI) and Machine Learning (ML) applications and systems offered and used by market intermediaries.pdf

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | Reporting for AI/ML Applications by Market Intermediaries |
| Issuing Authority | Securities and Exchange Board of India (SEBI) |
| Date | January 4, 2019 |
| Legal basis | SEBI Act 1992; SEBI (Stock Brokers and Sub-Brokers) Regulations 1992 |
| Scope | Stock brokers, depository participants, and all other SEBI-registered market intermediaries (not MIIs, not Mutual Funds — separate circulars govern those) |
| Reporting mechanism | Quarterly reports consolidated by Stock Exchanges and Depositories; submitted to SEBI within 30 days of quarter-end |

> **Trilogy Note:** This circular completes the SEBI 2019 AI/ML reporting trilogy:
> - **SEBI_9** (January 2019): Reporting for AI/ML Applications by Market Infrastructure Institutions (MIIs)
> - **SEBI_10** (May 2019): Reporting for AI/ML Applications by Mutual Funds
> - **SEBI_17** (January 4, 2019): Reporting for AI/ML Applications by Market Intermediaries (stock brokers, DPs)
>
> All three circulars share the identical six-category AI/ML taxonomy (Cluster C09 intra-SEBI convergence). SEBI_17's node completes the Cluster C09 documentation.

---

## S2. Governance Context

SEBI_17 is the earliest dated of the three 2019 circulars (January 4, 2019 — slightly predating SEBI_9's January 2019 MII circular). Like SEBI_9 and SEBI_10, it establishes a mandatory quarterly inventory-and-reporting regime for AI/ML systems. The three circulars were issued within a five-month window (January–May 2019), applying the identical taxonomy across three distinct SEBI-regulated entity categories:

- **MIIs** (exchanges, depositories, clearing corporations) — SEBI_9
- **Market Intermediaries** (brokers, DPs) — SEBI_17
- **Mutual Funds / AMCs** — SEBI_10

The background rationale in SEBI_17 states the purpose explicitly: creating "an inventory of the AI/ML landscape in the Indian financial markets" and preventing "misrepresentation" of AI-driven financial benefits in investor-facing products. This inventory-before-accountability sequence (2019 reporting → 2024-25 accountability via SEBI_11/SEBI_14) is the core SEBI governance architecture arc in P3.

**IOSCO connection:** The circular title references IOSCO — SEBI's AI/ML reporting regime is framed within the IOSCO mandate for securities regulators to understand AI/ML adoption by market participants. SEBI is an IOSCO member; this circular operationalises IOSCO principles at the India securities-market level. (⚠V-SEBI17-1: confirm IOSCO instrument cited)

---

## S3. Regulatory Units (RUs) — AI-Relevant

| RU# | Provision | Deontic | Key Obligation |
|---|---|---|---|
| RU1 | Mandatory quarterly AI/ML reporting | SHALL | All market intermediaries using AI/ML systems in investor-facing or compliance functions must report quarterly via Annexure A format to Stock Exchanges/Depositories |
| RU2 | Scope of AI/ML systems covered | SHALL | Reporting covers: robo-advisors, algorithmic order execution, compliance automation, sentiment analysis, NLP-based advisory, and any system using AI/ML for investment or compliance functions |
| RU3 | Misrepresentation prevention | SHALL NOT | Intermediaries SHALL NOT misrepresent financial benefits of AI-driven products to investors; advertised claims must be substantiated |
| RU4 | Control safeguards documentation | SHALL | Intermediaries must document control safeguards implemented for each AI/ML system, including safeguards against abnormal behaviour |
| RU5 | Abnormal behaviour prevention | SHALL | Systems must include mechanisms to detect and prevent abnormal AI/ML system behaviour; these mechanisms must be disclosed in quarterly reports |

---

## S4. Key Verbatim Quotes

> "There is increasing usage of AI (Artificial Intelligence) and ML (Machine Learning) as product offerings by market intermediaries and participants (eg: robo advisors) in investor and consumer facing products." — Background

> "SEBI is conducting a survey and creating an inventory of the AI / ML landscape in the Indian financial markets to gain an in-depth understanding of the adoption of such technologies in the markets." — Background

> "As most AI / ML systems are black boxes and their behavior cannot be easily quantified, it is imperative to ensure that any advertised financial benefit owing to these technologies in investor facing financial products offered by intermediaries should not constitute to misrepresentation." — Background

> "Any set of applications / software / programs / executable / systems (cumulatively called application and systems) that are offered to investors... OR to disseminate investments strategies and advice, OR to carry out compliance operations / activities" — Scope Definition 3

---

## S5. Analytical Notes

**Cluster C09 — SEBI 2019 AI/ML trilogy completion:**

SEBI_9 and SEBI_10 were identified in earlier batches as the Cluster C09 intra-SEBI convergence evidence. SEBI_17 confirms the convergence extends across all three entity categories. The identical AI/ML taxonomy across MIIs, Mutual Funds, and Market Intermediaries represents SEBI's deliberate system-wide inventory architecture — rare within the corpus as an example of coordinated within-regulator coverage.

| Circular | Entity category | Date | Taxonomy |
|---|---|---|---|
| SEBI_17 (this node) | Market Intermediaries (brokers, DPs) | Jan 4, 2019 | Identical 6-category |
| SEBI_9 | Market Infrastructure Institutions (MIIs) | Jan 2019 | Identical 6-category |
| SEBI_10 | Mutual Funds / AMCs | May 2019 | Identical 6-category |

**Governance arc: inventory → accountability (2019–2025):**
The six-year SEBI sequence: **2019** mandatory AI/ML reporting (SEBI_9/10/17 — know what exists) → **2024–25** SEBI_11 (assign responsibility) → **August 2024** SEBI_15 CSCRF (consolidated cybersecurity + cyber-resilience substrate, Circular SEBI/HO/ITD-1/ITD_CSC_EXT/P/CIR/2024/113) → **February 2025** SEBI_14 Reg.16C (statutory sole-responsibility for AI outputs, F. No. GN/2025/226 dated 6 Feb 2025 — this is the same Gazette notification previously duplicated as SEBI_16, now redirected to SEBI_14 following 2026-07-14 OCR-based duplicate identification). The completion of the 2019 trilogy in this batch closes the documentation of the arc's starting point; SEBI_14 + SEBI_15 together form the complete SEBI cyber+AI governance stack.

**Cross-regulator parallelism context:**
As of January 2019, SEBI had mandatory AI/ML reporting for all three regulated entity categories. RBI's equivalent AI-specific governance (RBI_FREE_AI_2025) did not arrive until November 2025 — a **six-year gap** between SEBI's operationalisation and RBI's principles framework. This is the corpus's longest dated instance of the SEBI-RBI parallelism timeline.

---

## S6. Concept Linkages

| Concept | Evidence from SEBI_17 |
|---|---|
| [[Regulatory_Parallelism]] | Extends the Cluster C09 intra-SEBI convergence finding across all three SEBI entity categories; confirms SEBI's AI/ML reporting architecture was system-wide by January 2019 — six years before RBI_FREE_AI_2025. The six-year SEBI-RBI gap is now documentable with a precise start date (January 4, 2019) and end date (November 2025). |
| [[Governance_Debt]] | 5-year gap between SEBI_17's inventory obligation (2019) and SEBI_11's accountability obligation (2024) — intermediaries reported AI/ML systems for five years without being held accountable for their outputs. The inventory-without-accountability configuration is the clearest governance debt arc in the corpus: governance form preceded governance substance by five years. |
| [[Accountability]] | RU3 (misrepresentation prevention) and RU4 (control safeguards documentation) establish pre-accountability governance obligations — but accountability for AI outputs is not assigned until SEBI_11 (2024) and SEBI_14 (2025). SEBI_17 is the earliest SEBI instrument in the accountability-without-enforcement chain. |
| [[Transparency]] | RU1/RU4/RU5: quarterly reporting to Stock Exchanges → SEBI is a regulator-facing transparency mechanism — earliest SEBI instance of structured AI transparency obligations. User-facing transparency (disclosure to investors about AI-driven decisions) is not required; only regulator-facing inventory transparency is mandated. |

---

## S7. Project Relevance

| Project | Relevance |
|---|---|
| P3 (BFSI — JEIM) | Completes the Cluster C09 trilogy documentation; confirms the SEBI 2019 AI/ML reporting system covered all three entity categories from inception — relevant to the regulatory-evolution timeline and the inventory-to-accountability arc |
| P4 (Doctrinal — IJLIT) | RU3 (misrepresentation prevention) is the earliest SEBI explicit AI/ML consumer-protection obligation — predates SEBI_11's accountability framework by five years; relevant to the doctrinal analysis of how SEBI built AI consumer protection step by step |
| fsQCA | Provides January 4, 2019 as the precise start date for SEBI's AI/ML governance arc — enables a longitudinal configurational analysis of how SEBI's governance configuration evolved from inventory (2019) to accountability (2025) while RBI's equivalent configuration remained at zero |

---

## S8. ⚠ VERIFY Flags

| Flag | Claim | Action |
|---|---|---|
| ⚠V-SEBI17-1 | IOSCO citation — does SEBI_17 explicitly cite an IOSCO instrument (resolution, report, or consultation paper) as the basis for the AI/ML reporting framework? | Primary text; also check IOSCO.org for 2018-2019 AI in securities markets documents |
| ⚠V-SEBI17-2 | Is SEBI_17's January 4, 2019 date confirmed as preceding or simultaneous with SEBI_9's MII circular? Establish precise chronological sequence | Primary circulars; SEBI.gov.in circular archive |
| ⚠V-SEBI17-3 | Has SEBI issued a subsequent circular updating or superseding the SEBI_17 quarterly reporting format for market intermediaries (analogous to how SEBI_11 updated the accountability framework)? | SEBI.gov.in → Circulars → 2023-2025 |

---

## Backlinks

← [[07_Institutions/Corpus/SEBI/SEBI_9]] (SEBI_9 — MII-facing sister circular, January 2019; Cluster C09)  
← [[07_Institutions/Corpus/SEBI/SEBI_10]] (SEBI_10 — Mutual Fund-facing sister circular, May 2019; Cluster C09)  
← [[07_Institutions/Corpus/SEBI/SEBI_11]] (SEBI_11 — 2024-25 accountability arc successor)  
← [[07_Institutions/Corpus/SEBI/SEBI_14]] (SEBI_14 — 2025 statutory accountability arc culmination)  
← [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]  
← [[05_Concepts/05_Concepts_Signature/Governance_Debt]]  
← [[05_Concepts/05_Concepts_Standard/Accountability]]  
← [[05_Concepts/05_Concepts_Standard/Transparency]]
