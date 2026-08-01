---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/sebi
---

# SEBI_15 — Cybersecurity and Cyber Resilience Framework (CSCRF) for SEBI Regulated Entities

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/SEBI/SEBI_15.md`
**Institution:** [[07_Institutions/SEBI]]
**Issuing body:** Securities and Exchange Board of India (SEBI), Information Technology Department–1 (ITD-1)
**Document date:** 20 August 2024
**Circular reference:** **SEBI/HO/ITD-1/ITD_CSC_EXT/P/CIR/2024/113**
**Pages:** 165 (consolidated framework, including Parts I–IV + annexures)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]] | [[03_Domains/Cybersecurity_Governance]]
**Source:** SEBI website — [circular index page](https://www.sebi.gov.in/legal/circulars/aug-2024/cybersecurity-and-cyber-resilience-framework-cscrf-for-sebi-regulated-entities-res-_85964.html); [attached PDF](https://www.sebi.gov.in/sebi_data/attachdocs/aug-2024/1724326790365.pdf)

---

## Instrument Identity

**Full title:** Cybersecurity and Cyber Resilience Framework (CSCRF) for SEBI Regulated Entities (REs)
**Type:** Consolidated cybersecurity framework circular; supersedes and harmonises fragmented cybersecurity circulars issued by SEBI to individual RE categories since 2015
**Legal basis:** Sections 11(1), 11(2)(g), and 11A of the SEBI Act 1992, read with the powers of SEBI to specify prudential requirements for regulated entities
**Target entities:** All SEBI regulated entities (REs), categorised into four tiers:

| Category | Description | Examples |
|---|---|---|
| **Market Infrastructure Institutions (MIIs)** | Stock exchanges, depositories, clearing corporations | NSE, BSE, MCX, NSDL, CDSL, ICCL, NSCCL |
| **Qualified REs** | Large REs meeting specified size / activity thresholds | Large stock brokers, top-tier merchant bankers, large mutual funds |
| **Mid-size REs** | Intermediate-tier REs | Mid-tier stock brokers, PMS providers, investment advisers above threshold |
| **Small REs** | Smaller intermediaries | Small stock brokers, sub-brokers, small investment advisers, sub-threshold entities |

Applies to: Stock Brokers and Depository Participants; KYC Registration Agencies (KRAs); Merchant Bankers; Portfolio Managers; Investment Advisers; Designated Depository Participants (DDPs); Registrars & Transfer Agents; Custodians; Mutual Funds; Debenture Trustees; Alternative Investment Funds; other categories per Section 16 applicability schedule.

**Effective / Compliance timeline:**
- Publication: 20 August 2024
- For REs where a cybersecurity framework circular already exists: compliance by **1 January 2025**
- For REs where no prior cybersecurity framework circular exists: compliance by **1 April 2025**
- Market SOC (M-SOC, hosted by NSE + BSE): operational by **1 January 2025**

**Companion documents:**
- [[07_Institutions/Corpus/SEBI/SEBI_14]] — SEBI (Intermediaries) (Amendment) Regulations 2025 (Reg 16C AI/ML sole responsibility) — cross-cuts CSCRF at the AI/ML technology governance layer
- [[07_Institutions/Corpus/SEBI/SEBI_11]] — SEBI Board memo on AI responsibility assignment
- [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] — CERT-In Audit Policy — parallel cyber framework at a distinct regulator
- [[04_Knowledge_Products/Wiki_Intake/FIDC_SEBI_NBFCSector_Representation_2025]] — practitioner testimony citing CSCRF as one of three fragmented cyber standards
- [[07_Institutions/Corpus/RBI/RBI_5_Operational_Risk_Management_Resilience_NBFC_Guidance_2024]] — RBI Operational Risk Management / Resilience (NBFC) — cross-regulator cyber-resilience comparator
- Referenced standards: ISO/IEC 27000 series (ISO 27001 certification mandatory for MIIs and Qualified REs); NIST SP 800-53; NIST Cybersecurity Framework (functions mapping); CIS Controls Version 8; BIS Financial Stability Institute guidelines; CPMI-IOSCO principles

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S5 (Data, Privacy & Security) / S6 (Model Risk & Implementation)
**Jurisdiction:** India
**Confidence:** HIGH — primary-source SEBI circular retrieved from sebi.gov.in official URL
**AI explicit:** NO in the CSCRF instrument itself (predates SEBI_14 Reg 16C by six months); AI/ML systems are covered via technology-neutral cybersecurity + cyber-resilience obligations. The AI-specific layer is added by [[SEBI_14]] Reg 16C (February 2025), which sits on top of the CSCRF baseline.
**Tier classification:** Tier A — Binding, primary-source consolidated cybersecurity framework
**AI Governance Wiki relevance:** HIGH — CSCRF is the *cybersecurity substrate* on which SEBI's subsequent AI accountability layer (Reg 16C) rests. Together, SEBI_14 + SEBI_15 form the complete SEBI cyber+AI governance stack for capital markets.

---

## Substantive Content

### Framework Architecture

The CSCRF is a **consolidated, outcome-based framework** organised into four parts:

| Part | Content | Approximate page range |
|---|---|---|
| **Part I** | CSCRF Objectives and Standards | pp. 53–79 |
| **Part II** | CSCRF Guidelines (operational requirements) | pp. 79–133 |
| **Part III** | Structured Formats for CSCRF Compliance | pp. 133–152 |
| **Part IV** | CSCRF Annexures and References (including VAPT Report Format) | pp. 152–165 |

### Five Cyber Resilience Goals (NIST-aligned)

The framework operationalises **five cyber resilience goals** mapped onto the NIST Cybersecurity Framework functions:

| Cyber Resilience Goal | Mapped NIST Cybersecurity Function |
|---|---|
| **1. Anticipate** | Governance + Identify + Protect + Detect |
| **2. Withstand** | Respond (in combination with Contain) |
| **3. Contain** | Respond (in combination with Withstand) |
| **4. Recover** | Recover |
| **5. Evolve** | Continuous improvement / adaptive governance |

### Tiered Applicability

Obligations scale with RE category. Key differentials:

| Requirement | MIIs | Qualified REs | Mid-size REs | Small REs |
|---|---|---|---|---|
| ISO/IEC 27001 certification | **Mandatory** | **Mandatory** | Not mandatory | Not mandatory |
| Cyber Capability Index (CCI) — half-yearly third-party assessment | **Mandatory** | **Mandatory** | Self-assessment | Not required |
| Cyber risk assessment plans | **Mandatory** | **Mandatory** | **Mandatory** | Not required |
| Red Teaming exercises | **Mandatory** | **Mandatory** | Not required | Not required |
| Security Operations Centre (SOC) | Own / group / Market SOC | Own / group / Market SOC / third-party | Market SOC / third-party | Market SOC / third-party |
| VAPT (Vulnerability Assessment & Penetration Testing) | **Mandatory** with specified comprehensive scope | **Mandatory** | **Mandatory** | **Mandatory** |
| SOC functional efficacy check (half-yearly) | **Mandatory** | **Mandatory** | Obtained from SOC provider | Obtained from SOC provider |
| Board / Partners / Proprietor approval of critical systems list | **Mandatory** | **Mandatory** | **Mandatory** | **Mandatory** |

### Market SOC (M-SOC)

To enable smaller REs to comply without independently building SOC capability, the framework provides for a **Market SOC (M-SOC)**, to be set up by NSE and BSE and operational from **1 January 2025**. Mid-size and Small REs can onboard the M-SOC as a compliance-satisfying option, alongside using their own SOC, group SOC, or third-party managed SOC.

### Board and Governance Structure

- Cybersecurity and cyber-resilience policy shall be documented and implemented with **Board / Partners / Proprietor approval**
- The Board / Partners / Proprietor shall approve the list of critical systems
- IT Committee governance and executive accountability structures scale with RE category
- Cyber audit is mandated to verify compliance with CSCRF

### VAPT Requirements

A comprehensive VAPT scope is specified (Annexure-A of the CSCRF supplies the VAPT Report Format). VAPT is mandatory across all four RE categories, with the scope and frequency scaling by tier.

### SBOM (Software Bill of Materials)

CSCRF references SBOM requirements as part of the software supply-chain integrity dimension of cyber-resilience — cross-linking with [[07_Institutions/Corpus/CERT_In/CERT_4]] (CERT-In SBOM Technical Guidelines v2.0) at the technical standards layer.

---

## Analytical Significance for PRIS Research

### For P3 — BFSI AI Governance / Regulatory Parallelism (JEIM)

CSCRF is the **cybersecurity substrate** on which SEBI's later AI-specific accountability layer (SEBI_14 Reg 16C) is built. Together:

- **SEBI_15 (Aug 2024, CSCRF)** — technology-neutral cybersecurity resilience framework applicable to all REs
- **SEBI_14 (Feb 2025, Reg 16C)** — AI/ML-specific sole responsibility clause

form the **complete SEBI capital-markets cyber + AI governance stack**. Compared to RBI's parallel stack (RBI_5 Operational Risk NBFC + RBI_FREE_AI_2025 committee report + RBI_3 Model Risk draft + RBI_7 Digital Lending 2025), the two regulators have now each enacted binding cyber + AI governance frameworks for overlapping BFSI entities without mutual cross-reference — extending the P3 Regulatory Parallelism finding from AI-specific instruments alone to the full cyber+AI regulatory stack.

CSCRF also cross-cuts with [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] (CERT-In Audit Policy) and [[07_Institutions/Corpus/CERT_In/CERT_4]] (CERT-In SBOM/AIBOM Technical Guidelines) — three parallel cybersecurity frameworks (SEBI CSCRF, CERT-In Audit Policy, CERT-In SBOM) for the same regulated entity population without a single coordination mechanism. Practitioner testimony via [[FIDC_SEBI_NBFCSector_Representation_2025]] confirms that NBFC-BL entities perceive this as a **triple compliance burden**.

### For P4 — Doctrinal (IJLIT)

CSCRF's outcome-based approach (five cyber resilience goals + tiered applicability + NIST CSF alignment) is doctrinally distinct from the input-based approach of earlier fragmented circulars. It is the corpus's clearest instance of a **consolidated, outcome-based cybersecurity regulation in the Indian securities market** — a doctrinal model that Reg 16C's terse "sole responsibility" approach does *not* follow. The doctrinal contrast between SEBI's outcome-based cybersecurity regulation (SEBI_15) and simple-attribution AI regulation (SEBI_14) is analytically significant.

### For P1 — SLR (Regulation & Governance)

Provides the India-securities-sector data point for cyber-resilience regulation in the global SLR comparators (alongside RBI cybersecurity master directions, EU DORA — see [[F045_PwC_TPRM_Digital_Geopolitical_Era_2025]] — and CPMI-IOSCO principles referenced within the CSCRF itself).

### For fsQCA — Regulatory Configurations for Trustworthy AI

CSCRF adds the *cybersecurity governance capacity* dimension to the SR (Structural Readiness) condition calibration for India. High SR requires operative cybersecurity infrastructure; CSCRF's mandatory ISO 27001 + CCI + Red Teaming for MIIs and Qualified REs represents a substantive SR investment at the capital-markets layer. Contrast with RBI's less prescriptive cybersecurity governance for banks and TRAI's telecom-sector approach.

### Regulatory Parallelism Pattern

**Instruments in same BFSI cybersecurity + AI governance space:**
- SEBI_15 (CSCRF, Aug 2024) ↔ [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] (CERT-In Audit Policy, Jul 2025) ↔ [[07_Institutions/Corpus/RBI/RBI_5_Operational_Risk_Management_Resilience_NBFC_Guidance_2024]] (RBI ORM NBFC, 2024) — three parallel cybersecurity frameworks with no mutual cross-reference
- SEBI_15 (CSCRF cybersecurity substrate) → SEBI_14 (Reg 16C AI accountability layer) — SEBI's own two-layer stack (six-month interval)

Pattern: **Sequential parallelism** — SEBI_15 → SEBI_14 is a self-consistent two-layer stack within SEBI; but the SEBI stack operates in parallel to the RBI stack and the CERT-In stack without coordination. A textbook instance of Regulatory_Parallelism at the cyber + AI governance interface.

---

## Connections

**Related corpus nodes:**
- [[07_Institutions/Corpus/SEBI/SEBI_14]] — companion AI-accountability layer (Reg 16C) built on the CSCRF cybersecurity substrate
- [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] — parallel cyber audit framework at CERT-In
- [[07_Institutions/Corpus/CERT_In/CERT_4]] — CERT-In SBOM/AIBOM Technical Guidelines v2.0
- [[07_Institutions/Corpus/RBI/RBI_5_Operational_Risk_Management_Resilience_NBFC_Guidance_2024]] — RBI Operational Risk Management (NBFC) — cross-regulator cyber-resilience comparator
- [[04_Knowledge_Products/Wiki_Intake/FIDC_SEBI_NBFCSector_Representation_2025]] — practitioner testimony on triple compliance burden
- [[04_Knowledge_Products/Wiki_Intake/F045_PwC_TPRM_Digital_Geopolitical_Era_2025]] — EU DORA + NIS2 + AI Act comparator; CSCRF is India's closest analogue to DORA at the sector level

**Related concepts:**
- [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — sequential SEBI stack + cross-regulator (SEBI/CERT-In/RBI) parallelism at the cybersecurity + AI layer
- [[05_Concepts/05_Concepts_Signature/Governance_Debt]] — six-year cyber-standard fragmentation resolved by CSCRF consolidation (positive Governance_Debt closure instance)
- [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] — CSCRF's within-SEBI harmonisation is a positive IC finding; SEBI/CERT-In/RBI cross-regulator gap is a negative IC finding
- [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] — mandatory ISO 27001 + CCI + Red Teaming for MIIs/Qualified REs is a substantial SR-condition capacity investment

**Related projects:**
- [[02_Projects/P3_BFSI_JEIM]]
- [[02_Projects/P4_Doctrinal_IJLIT]]
- [[02_Projects/P1_SLR_RG]]
- [[02_Projects/fsQCA_Thesis_Chapter]]

**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Log

- 2026-06-18 (Batch 8): SEBI_15_TEMPLATE.md created as shell; source PDF (46MB) could not be read by prior intake agent
- 2026-07-14 (Batch 15 continuation): Local PDF found corrupted (trailer dictionary error; `pdftotext`/`pdfimages`/`qpdf` all failed). WebSearch + WebFetch retrieved the primary-source SEBI circular from sebi.gov.in (Circular SEBI/HO/ITD-1/ITD_CSC_EXT/P/CIR/2024/113 dated 20 August 2024). Node populated with primary-source content. Template file `SEBI_15_TEMPLATE.md` retained as artefact.

---

## Later Amendments and Clarifications

Subsequent SEBI circulars clarified or amended the CSCRF (tracked for currency but not separate corpus nodes at this time):
- December 2024 — *Clarifications to Cybersecurity and Cyber Resilience Framework (CSCRF) for SEBI Regulated Entities (REs)* (circular reference to be confirmed)
- August 2025 — *Technical Clarifications to Cybersecurity and Cyber Resilience Framework (CSCRF) for SEBI Regulated Entities (REs)* (circular reference to be confirmed)

⚠ Consider spawning SEBI_18 for the consolidated Aug 2025 technical clarifications in a future batch.

---

_Back to [[07_Institutions/SEBI]] | [[Corpus_Index_MOC]]_
