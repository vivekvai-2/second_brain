---
type: Corpus Node
status: active
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/cea
---

# CEA_1 — Guidelines on Cyber Security in Power Sector, 2021

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021.md`
**Institution:** [[07_Institutions/CEA]]
**Issuing body:** Central Electricity Authority, Ministry of Power
**Document date:** Released 30 September 2021
**Pages:** 14 Articles (not independently paginated beyond article count in this extraction)
**Domain:** [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]]

---

## Instrument Identity

**Full title:** Guidelines on Cyber Security in Power Sector, 2021
**Type:** CEA Guidelines (binding directive under regulatory authority)
**Target entities:** All "Responsible Entities" — generators, Transmission companies (Transcos), Distribution companies (Discos), SLDCs/RLDCs/NLDC — plus System Integrators, Equipment Manufacturers, and Vendors
**Legal basis:** Regulation 10 on Cyber Security, Central Electricity Authority (Technical Standards for Connectivity to the Grid) (Amendment) Regulations, 2019
**Companion documents:** PIB press release announcing the Guidelines (30 September 2021); superseded/updated by [[07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025]] once finalised (currently draft only)

**Primary source link:** https://cea.nic.in/wp-content/uploads/notification/2021/10/Guidelines_on_Cyber_Security_in_Power_Sector_2021-2.pdf
**PIB announcement:** https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=1761862

---

## Analytical Classification

**Wiki section:** New — Critical Infrastructure / Power Sector (no existing wiki section covers this; recommend a new S9 or subsection)
**Jurisdiction:** India
**Confidence:** High — primary CEA-hosted PDF, cross-confirmed via PIB
**AI explicit:** No — general OT/ICS/IT cybersecurity, no AI/ML-specific provision anywhere in the 14 Articles
**Tier classification:** Tier B — mature, binding, sector-specific cybersecurity regime with zero AI-specific extension
**AI Governance Wiki relevance:** MEDIUM — the sole binding cyber-governance anchor for a sector that is a confirmed AI-governance blank spot; high value as the "closest available anchor" despite not itself addressing AI

---

## Substantive Content

### Core architecture (14 Articles)
ISMS requirements modelled on ISO 27001; mandatory CISO appointment per Responsible Entity; Critical Information Infrastructure (CII) identification and reporting to NCIIPC; Electronic Security Perimeter definition; cyber risk assessment; legacy-system phase-out requirements; mandatory staff training; cyber supply-chain risk management via a "Trusted Sources/Trusted Products" list; incident reporting to CERT-In; a Cyber Crisis Management Plan requirement; sabotage reporting; and annual audits by CERT-In-empanelled OT auditors.

### Described by Ministry of Power as "first-of-its-kind"
The PIB announcement (30 September 2021) frames these Guidelines as establishing "a cyber assurance framework, threat early-warning mechanisms, and secure remote operations for Control Systems, Communication Systems, and Secondary Automation/Tele-control technologies" — i.e., the OT layer of grid operations specifically, not the IT/data layer that DPDP or CERT-In's general 2022 Directions address.

### Confirmed absence
No provision anywhere in the 14 Articles references AI, ML, or algorithmic decision systems. The "Trusted Sources/Trusted Products" supply-chain mechanism is the closest analog to an algorithmic-accountability hook (comparable in spirit to DPDP Rule 13(3)'s algorithmic-software due-diligence clause — see [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]]) but is not framed around AI-specific risk and predates the sector's AI/ML load-forecasting and demand-response adoption documented in the technical (non-governance) literature.

---

## Analytical Significance for PRIS Research

### For a new Power Grid/Critical Infrastructure domain
This is the **sole primary anchor** for the domain and the clearest available evidence that India's power-sector cyber-governance architecture, while mature and binding (unlike insurance's IRDAI gap or telecom's TRAI gap), has simply not yet extended to AI-specific risk — a distinct governance-gap type from Regulatory_Parallelism (multiple regulators, uncoordinated) or Governance_Debt (overlapping obligations): this is **regulatory silence within a single, otherwise-comprehensive regime**.

### Comparative significance
Confirmed via [[07_Institutions/Corpus/International/International_26_NERC_CIP_ENISA_IEC62443_AI_Gap_2026]] that this silence is not an India-specific capacity gap — NERC CIP (US), ENISA/NIS2 (EU), and IEC 62443 (international) all show the identical pattern: mature OT/ICS cybersecurity frameworks with explicitly acknowledged-but-unaddressed AI-specific gaps. This is a rare instance in the PRIS corpus where India is not lagging global peers but moving in lockstep with an as-yet-unsolved global regulatory problem.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025]], [[07_Institutions/Corpus/NCIIPC/NCIIPC_1_Guidelines_Protection_NCII_V2_2015]], [[07_Institutions/Corpus/International/International_26_NERC_CIP_ENISA_IEC62443_AI_Gap_2026]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (contrast — silence vs. parallelism), [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Related frameworks:** None yet — no Framework-tier node exists for power-sector cybersecurity
**Related projects:** New domain, not yet assigned to a numbered project
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] (candidate new section)

---

## Coding Status

- **P3 NVivo:** Not applicable (not a BFSI instrument)
- **Wiki intake status:** Pending — new sector, High priority as the sole binding anchor

---

## Log

- 2026-08-02: Corpus node created. Sourced via Perplexity Deep Research per [[Sector_Gap_Audit_Perplexity_Prompts_2026-08-02]] Power Grid prompt. First node in a new CEA institution folder and the anchor for a new Power Grid/Critical Infrastructure domain.
