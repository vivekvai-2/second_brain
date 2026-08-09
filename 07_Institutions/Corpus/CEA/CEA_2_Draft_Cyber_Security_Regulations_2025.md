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

# CEA_2 — Draft Central Electricity Authority (Cyber Security in Power Sector) Regulations, 2025

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025.md`
**Institution:** [[07_Institutions/CEA]]
**Issuing body:** Central Electricity Authority, Ministry of Power
**Document date:** Released for public comment, deadline 7 November 2025 — supersedes an earlier August 2024 draft
**Pages:** Not independently paginated in this extraction
**Domain:** [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]]

---

## Instrument Identity

**Full title:** Draft Central Electricity Authority (Cyber Security in Power Sector) Regulations, 2025
**Type:** Draft subordinate regulation — **not yet finalised or notified**
**Target entities:** Generators, transmission/distribution companies, load despatch centres, power exchanges, vendors
**Legal basis:** Section 177, Electricity Act, 2003
**Companion documents:** Supersedes the Draft CEA (Cyber Security in Power Sector) Regulations, 2024 (August 2024, historical only, not separately noded); would formalise [[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]] into binding regulation once notified; closely tied to the CSIRT-Power establishment (below)

**Primary source link:** CEA draft regulations archive: https://cea.nic.in/regulations-category/draft-regulations/?lang=en (2024 draft text: https://cea.nic.in/wp-content/uploads/notification/2024/08/Draft_CEA_Cyber_Security_in_Power_Sectyor_Regulations_2024_English_Version.pdf)

> ## ✅ STATUS RESOLVED 2026-08-09 — SUPERSEDED BY NOTIFICATION
>
> **The draft was notified as the Central Electricity Authority (Cyber Security in Power Sector) Regulations, 2026 on 31 July 2026** (Gazette of India, Extraordinary, Part III—Section 4, No. 484). See **[[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]]** — the notified instrument, Tier A, in force 1 April 2027 with six regulations deferred to separate orders.
>
> **This node is retained as the draft-stage antecedent only.** For any current-law claim, cite CEA_3. Two draft-to-final deltas recorded below are now historical and should not be cited as current: the audit cadence (draft: bi-annual IT / annual OT → final: a single annual comprehensive audit across all critical systems, 9–15 month window, reg 5(22)) and commencement (draft: six months after Gazette publication → final: 1 April 2027, roughly eight months post-notification, with staggered commencement for the six costliest obligations).

~~**⚠ Status flag: this is a draft, not binding law.** Comment deadline passed 7 November 2025; not confirmed as finalised/gazetted as of this intake (2026-08-02). Any PRIS analysis must treat CEA_1 (2021 Guidelines) as the currently operative instrument and this draft as prospective only.~~ **Resolved — see above.**

---

## Analytical Classification

**Wiki section:** New — Critical Infrastructure / Power Sector
**Jurisdiction:** India
**Confidence:** Medium-High — primary CEA-hosted draft text, but explicitly not-yet-binding
**AI explicit:** No
**Tier classification:** Tier C (draft) — would become Tier B on finalisation
**AI Governance Wiki relevance:** MEDIUM — the clearest signal of where India's power-sector cyber-governance architecture is heading institutionally (centralisation via CSIRT-Power), though still silent on AI

---

## Substantive Content

### Proposed centralisation: CSIRT-Power under CEA
The draft proposes formal creation of a centralised CSIRT-Power under CEA as the nodal agency for cyber threat monitoring, incident response, and coordination with CERT-In/NCIIPC — **note this is the regulation-drafting side of an institution that was, in fact, already inaugurated administratively in September 2024** (see the Ministry of Power's own CSIRT-Power announcement, folded in below) — i.e., the institutional fact preceded the regulation meant to formalise it.

### Proposed obligations
Mandatory cybersecurity audits (bi-annual for IT systems, annual for OT systems); expanded CISO role definitions; expanded vendor/supply-chain security requirements; comes into effect six months after Gazette publication once finalised.

### CSIRT-Power — already operational, administratively established ahead of the regulation
**Ministry of Power PIB announcement (22 September 2024):** CSIRT-Power was inaugurated at the Northern Regional Power Committee, New Delhi, explicitly because "existing sub-sectoral CERTs lack the necessary legal mandate, resources, and skilled professionals to address cybersecurity incidents effectively." CERT-In is providing leadership to coordinate CSIRT-Power's incident and cybersecurity activities. This **replaces** the pre-existing six-sectoral-CERT structure (CERT-Thermal/NTPC, CERT-Hydro/NHPC, CERT-Transmission/POWERGRID, CERT-Distribution/CEA, CERT-Grid Operation/NLDC-Grid-India, CERT-Renewable Energy/MNRE-SECI), which operated under the Information Sharing and Analysis Center (ISAC-Power) framework with named CISOs per sub-sector.
Link: https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=2058001 | ISAC-Power six-CERT structure: https://cea.nic.in/power-sector-information-sharing-and-analysis-center-isac-power/?lang=en

### Confirmed absence
As with CEA_1, no provision in either the 2024 or 2025 draft addresses AI-based grid management or algorithmic decision systems specifically — the centralisation and audit-frequency changes are general cybersecurity governance improvements, not AI-specific extensions.

---

## Analytical Significance for PRIS Research

### Institution-before-regulation sequencing — a second instance of the pattern
CSIRT-Power's administrative inauguration (September 2024) preceding its regulatory formalisation (draft Regulations still pending as of November 2025 comment deadline) is structurally identical to the DPDP Board's "stand up the regulator before activating the regime" sequencing already documented in [[06_Frameworks/DPDP_Act_2023]] and [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]]. This is now a **second confirmed instance** of the same institutional-sequencing pattern in a completely different sector, strengthening the case that this is a general feature of Indian regulatory institution-building rather than a DPDP-specific idiosyncrasy — worth a note in [[05_Concepts/05_Concepts_Standard/Governance_Capacity]].

**Update 2026-08-09 — this instance is now closed and datable end-to-end.** Formal constitution came with [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] Chapter II (31 July 2026), which confers fourteen enumerated functions and binding authority over both entities and vendors. **The sequencing gap measures approximately 22 months** — September 2024 operational, July 2026 formal. This is the only one of the corpus's four institution-before-regulation instances (CSIRT-Power, the AA regime/DEPA, Sahamati, BIS/IS-ISO-IEC-42001 adoption) that can now be dated from both ends, which makes it the reference case for the pattern.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]], [[07_Institutions/Corpus/NCIIPC/NCIIPC_1_Guidelines_Protection_NCII_V2_2015]], [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]] (institution-before-regulation sequencing parallel)
**Related concepts:** [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] (institution-before-regulation sequencing), [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]
**Related frameworks:** [[06_Frameworks/DPDP_Act_2023]] (sequencing-pattern comparator)
**Related projects:** New domain, not yet assigned to a numbered project
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** Not applicable
- **Wiki intake status:** Pending — Normal priority; upgrade once finalised/notified

---

## Log

- 2026-08-02: Corpus node created. Sourced via Perplexity Deep Research per [[Sector_Gap_Audit_Perplexity_Prompts_2026-08-02]] Power Grid prompt. Folds in the 2024 draft (superseded) and the CSIRT-Power establishment as companion facts rather than separate nodes, per PRIS evidence-reuse threshold.
