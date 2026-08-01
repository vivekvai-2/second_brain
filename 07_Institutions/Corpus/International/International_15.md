---
type: corpus-node
node-id: International_15
institution: FSB
date: 2025-04
wiki-section: S3
tier: A
ai-explicit: false
tags:
  - type/corpus-node
  - institution/FSB
  - wiki-section/S3
  - tier/A
  - batch/11
  - concept/Institutional_Coherence
  - concept/Regulatory_Parallelism
  - concept/Governance_Capacity
  - concept/Accountability
  - project/P3
  - project/P4
---

# International_15 — FSB FIRE: Format for Incident Reporting Exchange (April 2025)

**Node ID:** International_15  
**Institution:** Financial Stability Board (FSB)  
**Document type:** International Standard — Technical Format/Framework  
**Date:** April 2025 (⚠V-I15-1: confirm precise April 2025 publication date and FSB reference)  
**Jurisdiction:** Global (applicable to FSB member jurisdictions including India)  
**Wiki Section:** S3 — International Regulatory  
**Tier:** A (FSB publication; machine-readable standard with India-specific implications explicitly mapped in source document)  
**Source PDF:** FSB FIRE Format for Incident Reporting Exchange.pdf

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | FIRE: Format for Incident Reporting Exchange |
| Issuing Authority | Financial Stability Board (FSB) |
| Date | April 2025 |
| Jurisdiction | Global — FSB member jurisdictions |
| Scope | Financial sector cyber and operational incident reporting; cross-border incident data exchange between national financial regulators |
| Key deliverable | Machine-readable standard for incident reports (initial/interim/final phases); JSON/XML-compatible data schema |
| Authority level | High: FSB is the G20-mandated financial stability oversight body; FIRE is the FSB's first machine-readable incident reporting standard |
| India applicability | RBI (DAKSH incident reporting), CERT-In notifications, SEBI CSCRF — all are named or mappable as India-domestic implementations of the FIRE framework |

---

## S2. Governance Context

International_15 (FSB FIRE) arrives in April 2025 as a technical standard rather than a principles document — the FSB's first attempt to create machine-readable interoperability for incident reporting across national financial regulators. Its significance for PRIS:

**Pre-FIRE landscape:** India's financial sector incident reporting operates across three independent regulator-specific channels:
- **RBI DAKSH** — RBI's centralised IT incident reporting system for Regulated Entities
- **CERT-In Notifications** — National-level cyber incident notifications to the Computer Emergency Response Team India (MeitY oversight)
- **SEBI CSCRF** — Securities sector cyber incident reporting under SEBI's Cyber Security and Cyber Resilience Framework

These three channels are not interoperable: a single cyber incident affecting a bank's securities trading operations may require three independent notifications in three formats with three different timelines. FIRE provides the technical architecture to collapse this fragmentation — but India's adoption of FIRE is unconfirmed. (⚠V-I15-2)

**Relationship to International_11 (FSB TPRM Toolkit):** International_11 established the governance policy for third-party risk in financial services. International_15 provides the operational layer for what happens *after* an incident occurs — the reporting mechanism. Together: governance policy (TPRM) + incident response standard (FIRE) = the FSB's complete third-party AI/cyber risk management architecture.

---

## S3. Regulatory Units (RUs) — FIRE Framework

| RU# | Provision | Deontic | Key Obligation |
|---|---|---|---|
| RU1 | Machine-readable incident reporting format | SHOULD | FSB member jurisdictions SHOULD adopt the FIRE format for financial sector cyber/operational incident reporting to enable cross-border data exchange (⚠V-I15-3: confirm deontic — SHOULD vs. SHALL in FSB standards) |
| RU2 | Phased reporting structure | SHALL | FIRE mandates a three-phase reporting structure: (a) Initial Report — early notification within defined hours; (b) Interim Report — updated situational assessment; (c) Final Report — root cause, impact, and remediation; format applies consistently across all three phases |
| RU3 | Data field standardisation | SHALL | Specific mandatory data fields across all FIRE reports: incident identifier, affected entity, incident type, onset date/time, discovery date/time, geographic scope, estimated financial impact, operational impact, regulatory notifications triggered |
| RU4 | Cross-border coordination mechanism | SHOULD | FIRE enables national regulators to share incident data in a common format; the mechanism supports the FSB's cross-border crisis coordination mandate without requiring real-time data sharing (asynchronous exchange architecture) |
| RU5 | India mapping — RBI DAKSH interface | N/A (aspirational) | FSB FIRE maps to RBI DAKSH reporting architecture; DAKSH → FIRE format compatibility is technically feasible; no RBI notification mandating FIRE adoption identified (⚠V-I15-2) |
| RU6 | India mapping — SEBI CSCRF interface | N/A (aspirational) | FSB FIRE maps to SEBI CSCRF cyber incident reporting fields; CSCRF → FIRE compatibility assessment needed |

---

## S4. Key Verbatim Quotes

> "The FSB has developed the Format for Incident Reporting Exchange (FIRE) to support cross-border communication and information sharing to address cyber incidents in financial services." — Executive Summary

> "FIRE is a technical format that defines the data to be exchanged when reporting cyber and operational incidents between financial authorities globally, in a consistent machine-readable way." — Executive Summary

> "Three phases of reporting: initial report, interim report, and final report — each captures different information relevant to the time of submission." — FIRE Architecture Overview

---

## S5. Analytical Notes

**India's multi-regulator fragmentation and FIRE:**

The FIRE framework is structurally designed to solve exactly the fragmentation problem that the Indian BFSI sector exhibits:

| India challenge | FIRE solution |
|---|---|
| Three independent reporting channels (DAKSH, CERT-In, SEBI CSCRF) | Single machine-readable format applicable to all channels |
| Different timelines per regulator (RBI 6-hour, CERT-In 6-hour, SEBI CSCRF varies) | Standardised phased reporting (Initial/Interim/Final) |
| Non-interoperable formats — an incident reported to RBI cannot be forwarded to SEBI in a compatible format | Machine-readable JSON/XML schema enabling regulator-to-regulator forwarding |
| No cross-border template for cyber incidents affecting foreign counterparties of Indian banks | FSB cross-border coordination mechanism |

India's adoption of FIRE would represent the single highest-leverage governance action for reducing the Institutional_Coherence deficit in financial sector incident reporting. However, no RBI/SEBI/CERT-In notification mandating FIRE adoption has been identified in the corpus. (⚠V-I15-2)

**FIRE and AI-specific incidents:**

International_15 is not explicitly an AI governance document — FIRE applies to all cyber and operational incidents, not only AI-related ones. However, three relevance pathways exist:

1. *GenAI cyber incidents* (International_14's four risk categories) require incident reporting; FIRE would standardise how those AI-specific incidents are reported cross-border
2. *AI model failure as operational incident* — SEBI CSCRF and RBI DAKSH both cover operational incidents, which would include AI model failures; FIRE would standardise the format for these
3. *AI-driven attack detection* — as Indian financial institutions increasingly use AI for threat detection, FIRE's standardised incident format enables cross-institutional learning from AI-detected incidents

**FIRE as Institutional_Coherence evidence:**

International_15 is the corpus's strongest international *prescriptive* evidence for Institutional_Coherence in financial sector governance — it operationalises coherence as a technical interoperability standard rather than a principles aspiration. Combined with International_10 (BoE multi-authority coordination model as descriptive evidence), these two nodes constitute the strongest international coherence architecture findings in the corpus.

**RBI DAKSH — FIRE relationship:**

The source document explicitly maps FIRE fields to RBI DAKSH reporting fields. This is analytically significant: the FSB has pre-validated FIRE's compatibility with India's domestic incident reporting infrastructure. India's adoption barrier is regulatory mandate, not technical compatibility. This distinction matters for fsQCA: the EA (Enforcement Architecture) condition for India in cyber incident reporting is not constrained by technical incapacity (DAKSH is FIRE-compatible) but by regulatory will (no adoption mandate). A high technical readiness + low institutional mandate configuration.

---

## S6. Concept Linkages

| Concept | Evidence from International_15 |
|---|---|
| [[Institutional_Coherence]] | Core document for the Institutional_Coherence concept's incident-reporting dimension. FIRE is the international standard for what inter-regulator coherence looks like in operational form: machine-readable, phased, cross-border compatible. India's three-channel fragmentation (DAKSH/CERT-In/CSCRF) is the absence of FIRE-level coherence. Combined with International_10 (BoE coordination model), International_15 completes the corpus's international prescriptive evidence for institutional coherence as a measurable design objective. |
| [[Regulatory_Parallelism]] | India's three incident reporting channels (DAKSH, CERT-In, SEBI CSCRF) are a Regulatory_Parallelism instance operating at the incident-response layer. FIRE's design rationale — reducing cross-regulator reporting fragmentation — confirms that India's incident reporting fragmentation is a specific expression of the broader India BFSI Regulatory_Parallelism pattern. Extends the Regulatory_Parallelism finding from ex-ante governance (rule-making fragmentation) to ex-post governance (incident response fragmentation). |
| [[Governance_Capacity]] | The gap between FIRE's technical feasibility (DAKSH is FIRE-compatible) and India's regulatory mandate (none identified) is a Governance_Capacity finding: the technical infrastructure exists but the institutional will and regulatory authority to mandate adoption have not been exercised. This is the "capacity-without-deployment" configuration — distinct from the "architecture-without-enforcement" pattern (ICMR_1) and the "aspirational-without-operative" pattern (TRAI_2). |
| [[Accountability]] | FIRE's phased reporting structure (Initial/Interim/Final) establishes a temporal accountability architecture: who reports what to whom, when, and in what format. This is the incident accountability complement to the ex-ante accountability architectures (SEBI_14 sole-responsibility, RBI_7 LSP due diligence chain). Together, these nodes show that accountability in AI/cyber governance has two dimensions: ex-ante obligation assignment and ex-post incident reporting. The corpus now has evidence for both. |

---

## S7. Project Relevance

| Project | Relevance |
|---|---|
| P3 (BFSI — JEIM) | Core corpus: FIRE's India mapping (DAKSH/CERT-In/CSCRF compatibility) directly feeds the BFSI governance fragmentation analysis; the three-channel incident reporting parallelism is a concrete operational manifestation of the P3 core thesis; International_15 provides the international standard against which India's incident reporting deficit can be measured |
| P4 (Doctrinal — IJLIT) | FIRE's RU2 (phased reporting structure) and RU3 (mandatory data fields) are ADICO-codeable; the India mapping (DAKSH/CERT-In/CSCRF as parallel channels without FIRE interoperability) is a doctrinal gap finding — three separate legal bases for incident reporting with no harmonisation instrument |
| P1 (SLR — RG/GIQ) | Incident reporting standards as a distinct sub-category of AI governance; FIRE demonstrates that international governance operates at both principles and operational/technical levels; SLR typology should include technical standard as a governance instrument type |

---

## S8. ⚠ VERIFY Flags

| Flag | Claim | Action |
|---|---|---|
| ⚠V-I15-1 | Exact FSB FIRE publication date — April 2025; confirm month and FSB reference number | fsb.org → Publications → 2025 |
| ⚠V-I15-2 | Has RBI, SEBI, or CERT-In issued any notification/circular mandating or recommending adoption of FSB FIRE format as of Batch 11 (June 2026)? | rbi.org.in, sebi.gov.in, cert-in.org.in → 2025-2026 notifications; also check IFSCA (GIFT City) for any FIRE adoption |
| ⚠V-I15-3 | FSB FIRE deontic level — does the standard use "shall" (mandatory for FSB member jurisdictions) or "should" (recommended)? | Primary text: FIRE document; also FSB standards-setting methodology |
| ⚠V-I15-4 | Does FIRE include explicit GenAI-specific incident categories, or does it use technology-neutral incident classification? | Primary text: FIRE data field specification section |

---

## Backlinks

← [[07_Institutions/Corpus/International/International_11]] (FSB TPRM Toolkit — policy governance layer; FIRE is the operational/incident-response layer; together = FSB's complete third-party risk architecture)  
← [[07_Institutions/Corpus/International/International_14_BIS_GenAI_Financial_Services]] (BIS GenAI Working Paper — GenAI-specific cyber risks that FIRE incident reporting would cover)  
← [[07_Institutions/Corpus/International/International_10]] (BoE multi-authority coordination model — descriptive coherence evidence; FIRE is the prescriptive coherence standard)  
← [[07_Institutions/Corpus/RBI/RBI_1]] (IT Governance — RBI DAKSH is the India domestic implementation context for FIRE)  
← [[05_Concepts/Institutional_Coherence]]  
← [[05_Concepts/Regulatory_Parallelism]]  
← [[05_Concepts/Governance_Capacity]]  
← [[05_Concepts/Accountability]]
