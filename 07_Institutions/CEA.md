---
type: Institution
tags:
  - type/institution
  - status/active
  - engine/phd
  - gate/open
---

# CEA — Central Electricity Authority

**Type:** Institution **Status:** Active — created 2026-08-02 during Power Grid/Critical Infrastructure domain build **Last Updated:** 2026-08-02

---

## Core Synthesis

The Central Electricity Authority, under the Ministry of Power, is India's technical regulator for power-sector cybersecurity — the sole institution in this corpus with a binding, sector-specific cyber-governance instrument for critical energy infrastructure. CEA's 2021 Guidelines on Cyber Security in Power Sector predate the DPDP Act by two years and remain, as of this note, entirely OT/ICS/IT-security-scoped rather than AI-specific — no provision in either the binding 2021 Guidelines or the current 2025 draft Regulations addresses AI, ML, or algorithmic grid-management systems. This makes CEA analytically distinct from every other institution in the PRIS corpus: it is not a case of Regulatory Parallelism (multiple regulators covering the same ground independently) but of **regulatory silence on a specific technology** within an otherwise mature, binding governance architecture.

## Institutional Profile

- **Type:** Statutory technical authority under the Ministry of Power
- **Governing statute:** Electricity Act, 2003 (Section 177 — regulation-making power); Central Electricity Authority (Technical Standards for Connectivity to the Grid) (Amendment) Regulations, 2019 (Regulation 10 — cyber security)
- **Primary mandate:** Technical standards, grid connectivity, and — since 2021 — cybersecurity governance for the power sector
- **AI-relevant jurisdiction:** Generators, transmission companies (Transcos), distribution companies (Discos), State/Regional/National Load Despatch Centres (SLDCs/RLDCs/NLDC), power exchanges, System Integrators, Equipment Manufacturers, and Vendors
- **Enforcement mechanism:** Mandatory compliance for all "Responsible Entities"; CERT-In-empanelled OT auditors conduct annual audits

## Key Instruments (PRIS-relevant)

| Instrument | Date | Status | Role in PRIS |
|---|---|---|---|
| Guidelines on Cyber Security in Power Sector, 2021 ([[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]]) | 30 September 2021 | Current, binding | Primary anchor for the new Power Grid/Critical Infrastructure domain |
| Draft CEA (Cyber Security in Power Sector) Regulations, 2024 | August 2024 | Superseded by 2025 draft | Historical iteration only |
| Draft CEA (Cyber Security in Power Sector) Regulations, 2025 ([[07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025]]) | Comment deadline 7 November 2025 | ~~Draft, not yet notified~~ **Superseded — notified as CEA_3** | Draft-stage antecedent only |
| **CEA (Cyber Security in Power Sector) Regulations, 2026** ([[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]]) | **Notified 31 July 2026**; in force 1 April 2027 (six regs deferred to separate orders) | **Binding, gazetted — Tier A; the operative instrument** | Constitutes CSIRT-Power in binding text; 17 regulations, 40 definitions, 2 Schedules; **zero AI provisions**; mandates ISO 27001/TCC; seven retention horizons; binds vendors directly; MeitY concurrence on the face of the instrument |

> **Update 2026-08-09.** The "null case" characterisation below is retained but must now be read in its stronger form. CEA did not merely fail to extend an ageing instrument — it **legislated afresh in 2026**, after publishing a draft for comment in October 2025 and considering objections, with its own parent ministry having confirmed Grid-India's production ML on the record in a Rajya Sabha reply of 18 December 2023, and still issued zero AI provisions. Silence with notice is a different and more interesting finding than silence from lag. See [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] §S5.1.

## Institutional Logic (Research Relevance)

CEA's governing logic is **operational-resilience-first, technology-neutral** cybersecurity regulation — modelled on ISO 27001 ISMS principles, CII identification/reporting to NCIIPC, and legacy-system phase-out, with no risk-tiering by system type (AI vs. non-AI). This is structurally different from BFSI's regulators (RBI, SEBI), who have each independently begun inserting algorithm/AI-specific hooks into otherwise technology-neutral instruments (see [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]). CEA has not done this — its instruments remain silent on AI even as the sector visibly adopts AI/ML for load forecasting, demand response, and fault detection (confirmed absence — see [[07_Institutions/Corpus/International/International_26_NERC_CIP_ENISA_IEC62443_AI_Gap_2026]] for the cross-jurisdictional comparison). This makes CEA a useful **null case** for PRIS: a mature, binding, sector-specific cybersecurity regulator that has simply not yet extended its remit to the technology in question, rather than one actively building parallel or contradictory AI-specific obligations.

## Linked Domains

- [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]]

## Linked Institutions

- [[07_Institutions/NCIIPC]]
- [[07_Institutions/CERT_IN]]

## Linked Concepts

- [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (contrast case — silence, not parallelism)
- [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]

---

_Back to [[_Institutions_MOC]]_
