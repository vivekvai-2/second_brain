---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/cert-in
---

# CERT_In_2 — Cyber Security Framework and Guidelines for Space Including Satellite Communication

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/CERT_In/CERT_In_2.md`
**Institution:** [[07_Institutions/CERT_IN]]
**Issuing body:** Indian Computer Emergency Response Team (CERT-In), Ministry of Electronics and Information Technology, in collaboration with SIA-India (Satellite Industry Association of India)
**Document date:** February 2026
**Document reference:** CIGU-2026-0001
**Pages:** ~50
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]]

---

## Instrument Identity

**Full title:** Cyber Security Framework and Guidelines for Space Including Satellite Communication
**Document reference:** CIGU-2026-0001
**Type:** Cyber Security Framework / Technical Guideline (CERT-In)
**Target entities:** Entire SatCom ecosystem — space segment operators (satellite manufacturers/operators), ground segment operators (gateway stations, TT&C, mission control), user segment operators (Very Small Aperture Terminal/VSAT network operators, terminal device manufacturers), and supply chain entities
**Legal basis:** CERT-In Act (IT Act 2000, Section 70B); CERT-In Directions dated April 28, 2022; DPDP Act 2023 (referenced)
**Companion documents:** [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] (parent audit policy framework), [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (DPDP Act compliance interface)

---

## Analytical Classification

**Wiki section:** S5 (Data, Privacy & Security) / S2 (India Regulatory Framework) / S6 (Implementation & Governance Artifacts)
**Jurisdiction:** India
**Confidence:** High — primary CERT-In issued framework document; co-branded with SIA-India
**AI explicit:** Partial — AI-enabled satellite capabilities implied but the framework is primarily sector-specific cyber governance; AI governance relevance is via critical infrastructure protection and supply chain security
**Tier classification:** Tier B — Technology-neutral with AI application: SatCom infrastructure is increasingly AI-enabled; the framework governs cyber risk in infrastructure where AI is embedded rather than governing AI directly
**AI Governance Wiki relevance:** MEDIUM — Extends CERT-In's regulatory footprint to the space/SatCom sector; contributes to S5 (cyber resilience for critical infrastructure) and signals CERT-In's expanding operational perimeter beyond traditional ICT

---

## Substantive Content

### Framework Structure

The document covers three segments of the SatCom ecosystem in distinct chapters:

| Segment | Coverage |
|---|---|
| Space Segment | Satellite (on-orbit), launch vehicle, satellite manufacturing supply chain |
| Ground Segment | Gateway stations, TT&C (Telemetry, Tracking & Control) centres, mission control facilities |
| User Segment | VSAT networks, terminal devices, customer-premises equipment |

### Key Obligations and Requirements

**Incident Reporting:**
- **6-hour mandatory reporting timeline** to CERT-In for cyber security incidents affecting SatCom infrastructure
- Applies to space segment operators, ground segment operators, and user segment operators
- Aligns with CERT-In Directions 2022 (general 6-hour cyber incident reporting mandate)

**Risk Management:**
- Mandatory risk assessment framework for all three segments
- Threat modelling required covering: jamming, spoofing, uplink/downlink interception, supply-chain compromise, and ground station attacks
- Risk register maintenance requirement

**Supply Chain Security:**
- Explicit supply chain security obligations — covers hardware and software components from third-party vendors
- Covers satellite components, launch systems, ground control software
- Background checks and vendor assessment requirements for critical component suppliers

**Security Governance:**
- Designated Chief Information Security Officer (CISO) or equivalent for SatCom operators
- Board-level / senior management accountability for cyber security programme
- Annual cyber security audit requirement (consistent with CERT_In_1 audit policy framework)

**Technical Controls (selected):**
- End-to-end encryption for command/control links
- Multi-factor authentication for ground station access
- Air-gap / network segmentation for mission-critical systems
- Patch management and vulnerability disclosure programme
- Penetration testing of ground segment systems

**DPDP Act Interface:**
- Document explicitly references DPDP Act 2023 for data collected through user-segment SatCom services (e.g., broadband internet via satellite)
- Personal data processed by VSAT operators subject to Data Fiduciary obligations under DPDP Rules 2025 (MeitY_4)

### Regulatory Significance

This is the **first CERT-In framework specifically governing space/SatCom cyber security** in India, coinciding with the liberalisation of India's space sector post-IN-SPACe (Indian National Space Promotion and Authorisation Centre) and the entry of private satellite operators (Eutelsat OneWeb, Starlink, Tata Sky, etc.). It extends CERT-In's mandatory-reporting infrastructure to a previously unregulated critical-infrastructure domain.

---

## Analytical Significance for PRIS Research

### For P3 — BFSI AI Governance / Regulatory Parallelism (JEIM)

Secondary relevance. CERT_In_2 extends the pattern documented in CERT_1, CERT_2, CERT_4 and CERT_In_1: CERT-In continues to issue sector-specific cyber security governance frameworks **without cross-reference to SEBI's CSCRF or RBI's IT governance directions**, even where regulated BFSI entities use SatCom infrastructure (e.g., VSAT-based banking connectivity in rural branch networks). The 6-hour reporting timeline is consistent with CERT-In Directions 2022 but has not been harmonised with SEBI's or RBI's own incident-reporting requirements — another instance of [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] in critical-infrastructure cyber governance.

### For P1 — SLR (Regulation & Governance)

Documents India's extension of cyber governance to the space sector — a gap in most global AI governance SLRs. Useful as a note on jurisdictional expansion of regulatory perimeter.

### For AI Governance Wiki (S5)

Provides the SatCom-sector cyber security framework content for Wiki S5. Pairs with CERT_In_1 (general audit policy) to complete CERT-In's governance architecture coverage.

### Coordination / Parallelism Pattern

**Pattern: Parallel Silo (Sector Extension)**
CERT-In issues SatCom-specific framework without coordination with: (a) DoT (telecom regulator for satellite communications), (b) IN-SPACe (space sector regulator), (c) MeitY on DPDP interface. The reference to DPDP Act in the framework is a citation, not a coordination mechanism. [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] manifests as multi-regulator coverage of SatCom (DoT, IN-SPACe, CERT-In) without formal coordination.

---

## Connections

**Related corpus nodes:**
- [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] — parent audit policy; CERT_In_2 is a sector application of CERT_In_1's audit architecture
- [[07_Institutions/Corpus/CERT_In/CERT_4]] — SBOM/AIBOM/HBOM guidelines; supply chain security overlap
- [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] — DPDP Act interface (user-segment personal data)

**Related concepts:**
- [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — multi-regulator SatCom governance without coordination
- [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] — CERT-In expanding institutional perimeter to space sector
- [[05_Concepts/05_Concepts_Standard/Accountability]] — CISO designation, Board-level accountability requirements
- [[05_Concepts/05_Concepts_Standard/Transparency]] — audit and vulnerability disclosure requirements

**Related projects:**
- [[02_Projects/P3_BFSI_JEIM]] (secondary — cyber infrastructure for BFSI)
- [[02_Projects/P1_SLR_RG]] (sector coverage note)

**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** Screening corpus — secondary relevance; not canonical corpus unless SatCom-BFSI infrastructure angle is developed
- **Wiki intake status:** Pending

---

## Log

- 2026-06-18: Corpus node created. Batch 4 (Policy Dump intake). Cowork session.
