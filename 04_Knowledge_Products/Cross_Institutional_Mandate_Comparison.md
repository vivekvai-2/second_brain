---
type: Knowledge Product
tags:
  - type/knowledge-product
  - type/cross-institutional-comparison
  - status/active
  - paper/p3
  - paper/p4
  - paper/fsqca
  - engine/phd
  - engine/consulting
---

# Cross-Institutional Mandate Comparison: RBI, SEBI, MeitY, CERT-In, and IRDAI

**Type:** Knowledge Product | **Status:** Active | **Last Updated:** 2026-07-14

---

## 1. Purpose and Scope

### Domain Boundary

This cross-institutional comparison examines the overlapping, parallel, and intersecting regulatory mandates, instruments, and operational requirements governing artificial intelligence (AI), machine learning (ML), data protection, and cybersecurity in the Indian financial and digital ecosystems.

### Instruments Included

- **Reserve Bank of India ([[RBI]]):** Digital Lending Directions 2025 ([[07_Institutions/Corpus/RBI/RBI_7|RBI_7]]), Framework for Responsible and Ethical Enablement of AI Committee Report ([[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025|RBI_FREE_AI_2025]]), IT Outsourcing Master Directions 2023 ([[07_Institutions/Corpus/RBI/RBI_2|RBI_2]]), and IT Governance Master Directions 2023 ([[07_Institutions/Corpus/RBI/RBI_1|RBI_1]]).
- **Securities and Exchange Board of India ([[SEBI]]):** Intermediaries Amendment Regulations 2025 (Regulation 16C) ([[07_Institutions/Corpus/SEBI/SEBI_14|SEBI_14]]), AI/ML Reporting Circulars 2019 ([[07_Institutions/Corpus/SEBI/SEBI_9|SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10|SEBI_10]], [[07_Institutions/Corpus/SEBI/SEBI_12|SEBI_12]], [[07_Institutions/Corpus/SEBI/SEBI_17|SEBI_17]]), and Cybersecurity and Cyber Resilience Framework (CSCRF) 2024 ([[07_Institutions/Corpus/SEBI/SEBI_15|SEBI_15]]).
- **Ministry of Electronics and Information Technology ([[MEITY]]):** Digital Personal Data Protection Rules 2025 ([[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025|MeitY_4]]), Information Technology Rules 2021 (as amended 2026), and Draft IT Rules SGI Amendment 2025 ([[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025|MeitY_5]]).
- **Indian Computer Emergency Response Team ([[CERT_IN]]):** Directions 2022 (6-hour notification) and Comprehensive Cyber Security Audit Policy Guidelines 2025 ([[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025|CERT_In_1]]).
- **Insurance Regulatory and Development Authority of India ([[IRDAI]]):** Maintenance and Sharing of Information Regulations 2025 ([[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025|IRDAI_1]]).

### Instruments Excluded

- Non-binding state-level frameworks (e.g., [[07_Institutions/Corpus/TN_Govt/TN_Govt_1|TN_Govt_1]] Safe AI Policy) except as sub-national comparative context.
- Intellectual property copyright papers (e.g., [[DPIIT]] Copyright Working Paper 2025) unless used to highlight secondary IP-governance tracks.
- Offensive cyber intelligence frameworks operating outside civilian commercial regulatory compliance.

### Time Window and Unit of Analysis

- **Temporal Scope:** 2012 to 2026, capturing the qualitative transition from technology-neutral IT guidelines to explicit, binding AI accountability rules.
- **Unit of Analysis:** The "Requirement Unit" (RU)—individual, codeable regulatory statements containing specific obligations, deontic modalities, and enforcement sanctions.

### Intended Downstream Use

This comparison serves as the empirical and doctrinal baseline for:
1. **[[P3_BFSI_JEIM]]:** Quantifying the occurrence of [[Regulatory_Parallelism]] and [[Governance_Debt]] in dual-regulated entities.
2. **[[P4_Doctrinal_IJLIT]]:** Analyzing the legal coherence of liability attribution and non-delegable vendor risk.
3. **[[fsQCA_Thesis_Chapter]]:** Calibrating configuration pathways governing systemic regulatory trust.
4. **Consulting Frameworks:** Informing runtime control systems (e.g., AEGIS_OS) and purpose-limitation engines (e.g., PrivacyWeave).

---

## 2. Institutional Mandates

The statutory and administrative authority of India's digital and financial regulators is polycentric, fragmented, and vertically siloed. The table below maps their statutory boundaries across key regulatory functions:

### Functional Allocation of Authority

| Institution | Enabling Statute | Rule-Making Power | Supervision & Inspection | Incident Response | Technical Audit | Enforcement & Adjudication | Policy Formulation |
|---|---|---|---|---|---|---|---|
| **[[RBI]]** | RBI Act 1934; BR Act 1949; PSS Act 2007 | **Absolute** (sectoral directions) | **High** (on-site inspections, DAKSH portal) | **Sectoral** (DAKSH operational risk) | **Indirect** (prescribes IT audit baselines) | **High** (PCA, licensing, BR Act penalties) | **High** (FREE-AI committee, FinTech Dept) |
| **[[SEBI]]** | SEBI Act 1992; SCRA 1956; Depositories Act 1996 | **Absolute** (intermediary/MII regulations) | **High** (inspections, exchange monitoring) | **Sectoral** (CSCRF disruption logs) | **Indirect** (prescribes CSCRF audit cycles) | **High** (Chapter V inquiry, trading bans, fines) | **High** (Board memos, consultation papers) |
| **[[MEITY]]** | Business Allocation Rules; IT Act 2000; DPDP Act 2023 | **Absolute** (subordinate rules, IT/DPDP rules) | **None** (delegated to DPBI/CERT-In) | **None** (delegated to CERT-In) | **None** (delegated to STQC/CERT-In) | **None** (delegated to DPBI/adjudicators) | **Absolute** (national digital strategy, IndiaAI) |
| **[[CERT_IN]]** | IT Act 2000 (Section 70B) | **Limited** (binding directions/guidelines) | **Medium** (empannelled auditor oversight) | **National Nodal** (6-hour cyber triage) | **Absolute** (sets national cyber-audit standards) | **Medium** (penalties for non-compliance with directions) | **Medium** (cybersecurity standards advisory) |
| **[[IRDAI]]** | IRDA Act 1999; Insurance Act 1938 | **Absolute** (sectoral regulations) | **High** (solvency & conduct inspection) | **Sectoral** (operational incident reporting) | **Indirect** (prescribes data/IT audit baselines) | **High** (license suspension, solvency correction) | **Medium** (solvency & data governance advisory) |

### Key Institutional Interfaces & Logics

#### 1. [[RBI]] versus [[SEBI]]

- **RBI Logic:** *Prudential Stability and Credit Risk.* RBI approaches technology through the lens of capital adequacy, systemic contagion, and operational resilience. AI is governed as a "model risk" that could destabilise lending portfolios or as an "outsourcing risk" that threatens operational continuity.
- **SEBI Logic:** *Market Integrity and Investor Protection.* SEBI approaches technology through the lens of market conduct, fair access, and transaction transparency. AI is governed as an "accountability risk" (preventing algorithmic market manipulation and robo-advisory misrepresentation) and a "disclosure risk" (requiring granular asset registers).
- **Friction:** Dual-regulated financial institutions (e.g., commercial banks operating as SEBI-registered stockbrokers or investment advisers) are subjected to both logics simultaneously. RBI's FREE-AI framework and SEBI's Regulation 16C operate on parallel tracks with zero mutual cross-references, forcing entities to maintain duplicate compliance registries for identical AI models.

#### 2. [[MEITY]] versus [[CERT_IN]]

- **MeitY Logic:** *Ecosystem Development and Digital Sovereignty.* As a central ministry, MeitY is an executive policymaker focused on national compute capacity (IndiaAI Mission), horizontal data privacy (DPDP Act), and platform safety (IT Rules). It seeks to balance innovation with citizen protection.
- **CERT-In Logic:** *Reactive Incident Response and Technical Resilience.* As a statutory technical authority, CERT-In is an operational first-responder. Its focus is entirely on identifying, mitigating, and documenting technical vulnerabilities and security breaches.
- **Friction:** While CERT-In operates within MeitY's administrative portfolio, it exercises independent statutory authority under Section 70B of the IT Act. This produces a temporal friction: MeitY's DPDP Rules 2025 operate on a slow, ex-ante management-based compliance logic (DPIAs, Consent Managers), whereas CERT-In's Directions 2022 enforce a hyper-reactive, 6-hour ex-post notification window for security incidents, including algorithmic failures.

#### 3. [[RBI]] versus [[IRDAI]]

- **RBI Logic:** *Active, Prescriptive Tech Governance.* RBI actively intervenes in technology lifecycles, prescribing strict conditions for digital lending algorithms, non-delegable credit decisions, and detailed IT outsourcing audits.
- **IRDAI Logic:** *Siloed Data Governance through Omission.* IRDAI's technology posture is characterized by a significant lag. Its primary instrument, the Maintenance and Sharing of Information Regulations 2025, addresses basic data governance and localisation but contains zero explicit AI/ML or algorithmic-risk provisions.
- **Friction:** This creates a "fourth silo" in Indian financial regulation. While insurance companies are rapidly deploying AI for automated underwriting, algorithmic claims-denial, and fraud detection, they operate under a complete vacuum of sector-specific AI governance, while banks under RBI face highly prescriptive mandates.

#### 4. Central Digital Authority versus Sectoral Regulator

- **Central Digital Authority (MeitY/DPBI) Logic:** *Horizontal, Rights-Based Protection.* The Data Protection Board of India (DPBI) is designed to enforce individual privacy rights and algorithmic due diligence (Rule 13(3)) across all economic sectors uniformly, treating data fiduciaries identically.
- **Sectoral Regulators (RBI, SEBI, IRDAI) Logic:** *Vertical, Risk-Based Supervision.* Sectoral regulators enforce rules tailored to the specific risk profiles of their respective markets (e.g., credit risk, market manipulation, insurance solvency).
- **Friction:** The horizontal DPDP framework is layered directly on top of vertical sectoral mandates without a preemption or reconciliation mechanism. An SDF bank must execute a DPDP-compliant DPIA, an RBI-compliant IT outsourcing audit, and a SEBI-compliant CSCRF review. There is no cross-recognition of assurance artifacts, meaning an audit completed to satisfy CERT-In or DPBI cannot be reused to discharge RBI or SEBI obligations. This is the [[Assurance_Reuse_Gap]] documented in §13.

---

## 3. Instrument Inventory

The table below catalogs the primary regulatory instruments that comprise the active technology-governance corpus across these five institutions:

| Institution | Instrument | Date | Legal Force | Regulated Actor | Primary Objective | Enforcement Status |
|---|---|---|---|---|---|---|
| **[[RBI]]** | Digital Lending Directions, 2025 ([[07_Institutions/Corpus/RBI/RBI_7|RBI_7]]) | May 8, 2025 | **Binding** (Master Direction under BR Act/RBI Act) | Scheduled Commercial Banks, Co-op Banks, NBFCs, and LSPs | Regulate AI-driven creditworthiness scoring, training data, and LSP due diligence | Active. Non-compliance triggers BR Act penalties and lending restrictions. |
| **[[RBI]]** | FREE-AI Committee Report ([[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025|RBI_FREE_AI_2025]]) | August 2025 | **Aspirational** (Committee Report) | All RBI Supervised Entities | Establish principles-based model risk governance (Seven Sutras) | Non-enforceable. Recommendations use "should" language. |
| **[[RBI]]** | IT Outsourcing Directions, 2023 ([[07_Institutions/Corpus/RBI/RBI_2|RBI_2]]) | April 10, 2023 | **Binding** (Master Direction) | Banks, NBFCs, and Payment Operators | Regulate third-party technology risk and prescribe audit access | Active. Precludes delegation of core risk-management functions. |
| **[[SEBI]]** | Intermediaries Amendment Regulations, 2025 (Reg 16C) ([[07_Institutions/Corpus/SEBI/SEBI_14|SEBI_14]]) | February 6, 2025 | **Binding** (Statutory Regulation via Gazette) | All SEBI-registered Intermediaries (Brokers, Advisors, Portfolio Managers) | Impose sole, non-delegable responsibility for AI/ML outputs, data security, and compliance | Active. Enforcement via Chapter V (suspension, cancellation of registration). |
| **[[SEBI]]** | Cybersecurity Framework (CSCRF 2024) ([[07_Institutions/Corpus/SEBI/SEBI_15|SEBI_15]]) | August 20, 2024 | **Binding** (Consolidated Framework Direction) | All SEBI Regulated Entities | Prescribe tiered cybersecurity baselines, 24/7 SOCs, and quarterly board reviews | Active. Harmonises prior fragmented sector-specific cyber circulars. |
| **[[SEBI]]** | AI/ML Reporting Circulars ([[07_Institutions/Corpus/SEBI/SEBI_9|SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10|SEBI_10]], [[07_Institutions/Corpus/SEBI/SEBI_17|SEBI_17]]) | Jan/May 2019 | **Binding** (Regulatory Circular) | Market Infrastructure Institutions (MIIs), Mutual Funds, and Market Intermediaries | Establish mandatory quarterly reporting inventory of AI/ML applications | Active. First Indian regulatory attempt to define and catalogue AI. |
| **[[MEITY]]** | DPDP Rules, 2025 ([[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025|MeitY_4]]) | November 13, 2025 | **Binding** (Subordinate Legislation via Gazette) | Data Fiduciaries, Processors, and Significant Data Fiduciaries (SDFs) | Govern notice/consent, Consent Managers, and SDF algorithmic due diligence (Rule 13(3)) | **Staggered.** Board constitution live; substantive obligations in force May 13, 2027. |
| **[[MEITY]]** | Draft IT Rules SGI Amendment ([[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025|MeitY_5]]) | November 2025 | **Draft** (Proposed Amendment) | Social Media Intermediaries, AI Developers | Mandate metadata watermarking (C2PA) and labelling for synthetic media (SGI) | Pending finalisation. Currently drives speculative enterprise preparation. |
| **[[CERT_IN]]** | Directions under Sec 70B(6) | April 28, 2022 | **Binding** (Statutory Direction) | All Bodies Corporate, Intermediaries, and Service Providers | Mandate 6-hour reporting window for material cybersecurity incidents | Active. Non-compliance carries up to 1-year imprisonment under Sec 70B(7). |
| **[[CERT_IN]]** | Cyber Security Audit Policy Guidelines ([[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025|CERT_In_1]]) | July 25, 2025 | **Binding** (Statutory Guidelines) | Empannelled Auditing Organisations and Auditees | Standardize cyber audits; explicitly defines "AI System Audits" and "AIBOM Auditing" | Active. Binding on all empanelled auditors and covered auditee entities. |
| **[[IRDAI]]** | Maintenance & Sharing of Info Regulations ([[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025|IRDAI_1]]) | January 2025 | **Binding** (Statutory Regulations) | All Insurance Companies and Intermediaries | Establish Board-approved data governance, data lineage, and data localisation | Active. Contains no explicit AI/ML or algorithmic-risk provisions. |

---

## 4. Institutional Grammar Comparison

Applying the [[Institutional_Grammar_IG2]] syntax (ADICO: Attributes, Deontic, Aim, Conditions, Or-else) reveals the structural asymmetry and varying coercive force of the mandates across different regulatory silos.

### Coded Regulatory Statements

| Instrument & Clause | Attributes (A) | Deontic (D) | Aim (I) | Conditions (C) | Or-else (O) |
|---|---|---|---|---|---|
| **[[07_Institutions/Corpus/RBI/RBI_7|RBI_7]] (Digital Lending Directions 2025, RU1)** | Regulated Entity (RE) | **SHALL** | Conduct comprehensive due diligence on Loan Service Providers (LSPs), including a technical and risk assessment of AI/ML systems used for creditworthiness determination | Prior to onboarding and during periodic supervisory reviews | Supervisory audit escalation, restriction on digital lending activities, or administrative penalties under the Banking Regulation Act 1949 |
| **[[07_Institutions/Corpus/SEBI/SEBI_14|SEBI_14]] (Intermediaries Amendment 2025, Reg 16C)** | Registered Intermediary | **SHALL** | Assume sole and non-delegable responsibility for the privacy, security, data integrity, legal compliance, and all outputs derived from the use of AI/ML tools | When deploying any application, software, or executable system using AI/ML techniques | Enquiry and disciplinary action under Chapter V of the Intermediaries Regulations, including suspension or cancellation of registration |
| **[[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025|MeitY_4]] (DPDP Rules 2025, Rule 13(3))** | Significant Data Fiduciary (SDF) | **SHALL** | Verify and ensure that algorithmic software or automated systems used for hosting, processing, or displaying personal data do not pose a risk to the rights of Data Principals | During the conduct of the annual Data Protection Impact Assessment (DPIA) | Financial penalties up to INR 250 crores per violation category, adjudicated by the Data Protection Board of India (DPBI) |
| **[[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025|CERT_In_1]] (Audit Guidelines 2025, Sec 6)** | Auditee Organization | **SHALL** | Undergo a comprehensive cyber security audit, incorporating "Artificial Intelligence (AI) System Audits" and "AIBOM Auditing" conducted by a CERT-In empanelled auditor | At least once a year, covering all aspects of their ICT systems | Placement of the auditing organisation on a watch-list/suspension, or prosecution of the auditee under Section 70B(7) of the IT Act |
| **[[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025|IRDAI_1]] (Maintenance Regulations 2025, Board Policy)** | Regulated Insurance Entity | **SHALL** | Design, implement, and maintain a Board-approved data governance framework, and store all operational data in Indian data centres | For the maintenance and sharing of insurance-sector information | License review, restriction on underwriting activities, or monetary penalties under the Insurance Act 1938 |
| **[[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025|RBI_FREE_AI_2025]] (Responsible AI Framework, Chapter 4.4)** | Regulated Entity (RE) | *SHOULD* | Establish a board-approved AI policy covering governance structure, accountability, risk appetite, and human-in-the-loop oversight for autonomous systems | When deploying general-purpose AI/ML models across business functions | **None** (Explicitly classified as advisory/aspirational) |

---

## 5. Functional Equivalence Matrix

The matrix below evaluates potentially overlapping mandates across key control domains, testing whether independent instruments govern the same capabilities for similar actors:

| Control Domain | RBI Requirement | SEBI Requirement | MeitY / CERT-In Requirement | Equivalence Level | Cross-reference Present? | Coordination Evidence? |
|---|---|---|---|---|---|---|
| **Governance & Board Oversight** | Mandates Board-approved IT Outsourcing Policy ([[07_Institutions/Corpus/RBI/RBI_2|RBI_2]]) and recommends Board-approved AI Policy ([[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025|RBI_FREE_AI_2025]]). | Mandates Board-approved CSCRF Policy and quarterly cyber-AI risk reviews ([[07_Institutions/Corpus/SEBI/SEBI_15|SEBI_15]]). | Mandates Board-approved data protection policies under DPDP Rules ([[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025|MeitY_4]]). | **Substantial** (all require Board sign-off on technology risk) | **No** (0 references between financial and data instruments) | **No** (each Board policy must be separately drafted and approved) |
| **Algorithmic Accountability** | RE retains absolute accountability for credit decisions; cannot delegate to credit AI or LSP ([[07_Institutions/Corpus/RBI/RBI_7|RBI_7]], RU1/RU6). | Intermediary is "solely responsible" for all AI/ML outputs; cannot delegate to vendors ([[07_Institutions/Corpus/SEBI/SEBI_14|SEBI_14]], Reg 16C). | SDF must verify that algorithmic software does not risk Data Principal rights ([[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025|MeitY_4]], Rule 13(3)). | **Functional Equivalence** (unconditional attribution of liability to the regulated user) | **No** (SEBI_14 and RBI_7 do not acknowledge each other) | **No** (independent convergence on identical attribution logic) |
| **Technical Audit & Assurance** | Prescribes regular technical audits of outsourced IT and cloud systems ([[07_Institutions/Corpus/RBI/RBI_2|RBI_2]]). | Prescribes tiered CSCRF audit cycles and independent vulnerability testing ([[07_Institutions/Corpus/SEBI/SEBI_15|SEBI_15]]). | Mandates annual cyber security audits, explicitly defining "AI System Audits" and "AIBOM Auditing" ([[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025|CERT_In_1]]). | **Partial** (overlapping technical scopes; CERT-In standardizes the audit category) | **Yes** (SEBI_15 references CERT-In empanelled auditors) | **Yes** (SEBI utilizes CERT-In's auditor market; RBI operates independently) |
| **Incident Reporting** | Mandates immediate reporting of operational and IT failures via DAKSH portal ([[07_Institutions/Corpus/RBI/RBI_1|RBI_1]]). | Mandates immediate reporting of market disruptions and cyber incidents under CSCRF ([[07_Institutions/Corpus/SEBI/SEBI_15|SEBI_15]]). | Mandates 6-hour cybersecurity incident reporting (CERT-In Directions) and "without delay" breach reporting (DPDP Rules). | **Substantial Overlap** (same failure triggers multiple reports) | **No** (RBI has 0 references to CERT-In; SEBI has 3 references) | **Asymmetric** (SEBI coordinates cyber reporting with CERT-In; RBI operates a closed silo) |
| **Data Governance & Localisation** | Mandates strict payment data localisation (RBI 2018) and local storage for outsourced systems ([[07_Institutions/Corpus/RBI/RBI_2|RBI_2]]). | Prescribes strict data privacy, security, and integrity controls for AI tools ([[07_Institutions/Corpus/SEBI/SEBI_14|SEBI_14]], Reg 16C(a)). | Recommends targeted, committee-driven data localisation for specified SDF personal data ([[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025|MeitY_4]], Rule 13(4)). | **Adjacent** (different localisation thresholds and consent rules) | **No** (0 cross-references) | **No** (overlapping data-handling rules operate in isolation) |

---

## 6. Coordination Pattern

The overlapping mandates across these five institutions are classified below according to their dominant coordination patterns:

### 1. [[RBI]] ↔ [[SEBI]] AI Governance

- **Classification:** **Regulatory Parallelism**
- **Evidence:** SEBI notified Regulation 16C ([[07_Institutions/Corpus/SEBI/SEBI_14|SEBI_14]]) in February 2025, imposing a binding "sole responsibility for AI outputs" mandate. RBI notified its Digital Lending Directions ([[07_Institutions/Corpus/RBI/RBI_7|RBI_7]]) in May 2025, imposing a binding "sole credit accountability and LSP AI due diligence" mandate. Despite both instruments governing the algorithmic-attribution and data-integrity capabilities of dual-regulated NBFCs and commercial banks, there is **zero cross-referencing, mutual acknowledgement, or harmonisation** between them.

### 2. [[MEITY]] ↔ [[CERT_IN]] Cyber-AI Auditing

- **Classification:** **Incorporated Reference / Complementary Allocation**
- **Evidence:** CERT-In's Comprehensive Audit Guidelines ([[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025|CERT_In_1]]) explicitly incorporate by reference the 282-control-point cybersecurity checklist issued by MeitY's Cyber Security Division. Furthermore, MeitY's horizontal IT Rules and DPDP Rules rely on CERT-In's empanelled auditing organizations to verify technical compliance, representing a structured division of labor between executive rulemaking (MeitY) and technical standardisation (CERT-In).

### 3. [[RBI]] ↔ [[IRDAI]] Technology Oversight

- **Classification:** **Regulatory Parallelism through Omission**
- **Evidence:** While both are financial sector regulators governing information-asymmetric markets, RBI has built a highly sophisticated technology-governance stack (RBI_7, FREE-AI, RBI_2), whereas IRDAI's Maintenance and Sharing of Information Regulations ([[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025|IRDAI_1]]) remain entirely silent on AI/ML. This "fourth silo" omission forces insurance companies to deploy AI in a regulatory vacuum, while banks face prescriptive, high-capacity mandates.

### 4. Horizontal Data Authority ([[MEITY]]/DPBI) ↔ Sectoral Regulators ([[RBI]]/[[SEBI]]/[[IRDAI]])

- **Classification:** **Independent Convergence**
- **Evidence:** DPDP Rules (Rule 13(3)), SEBI Regulation 16C, and RBI Digital Lending Directions (RU1) have independently converged on a common regulatory design: **unconditional attribution of liability to the regulated entity for automated/algorithmic outputs**. Combined with IOSCO's non-delegable accountability principle documented in [[07_Institutions/Corpus/International/International_19_IOSCO_AI_Capital_Markets_CR_2025|International_19]], this constitutes a **four-way convergence** across global standard-setter + horizontal data authority + two sectoral regulators — the strongest cross-jurisdictional accountability-attribution convergence in the corpus. However, this convergence occurred without any central coordination, resulting in three independent, non-interoperable compliance and audit frameworks governing the same underlying software systems.

---

## 7. Regulatory Parallelism Assessment

The table below evaluates the candidate instances of [[Regulatory_Parallelism]] observed between **RBI (FREE-AI/RBI_7)** and **SEBI (Reg 16C/CSCRF)**:

### Parallelism Diagnostic Checklist

| Diagnostic Dimension | RBI (Digital Lending / FREE-AI) | SEBI (Reg 16C / CSCRF) | Parallelism Confirmed? |
|---|---|---|---|
| **1. Independent Issuance?** | Yes. Issued under Banking Regulation Act/RBI Act. | Yes. Issued under SEBI Act. | **Yes.** Both regulators acted within their respective statutory silos without joint consultation. |
| **2. Functionally Equivalent Capabilities?** | Yes. Both govern data integrity, model-output accountability, and third-party vendor due diligence. | Yes. Both govern data security, algorithmic-output liability, and vendor insulation. | **Yes.** The core control objectives—securing data and attributing liability for automated decisions—are identical. |
| **3. Explicit Cross-Reference?** | No. RBI FREE-AI and RBI_7 contain 0 references to SEBI. | No. SEBI_14 and CSCRF contain 0 references to RBI. | **No.** Absence of cross-reference is the primary indicator of uncoordinated parallelism. |
| **4. Shared Control Satisfaction?** | No. A single operational control (e.g., an AI inventory) cannot satisfy both. | No. SEBI requires a 6-category taxonomy; RBI requires a model-risk taxonomy. | **No.** Divergent definitions prevent the reuse of a single compliance control. |
| **5. Separate Evidence & Audit?** | Yes. Separate board sign-offs, separate audit trails, and separate regulatory filings. | Yes. CSCRF requires separate quarterly board reviews; DPDP requires annual DPIAs. | **Yes.** Evidentiary requirements are strictly segregated, multiplying administrative work. |
| **6. Substantive Protection Multiplied?** | No. Overlapping rules do not improve actual model security or explainability. | No. They merely duplicate the administrative paper trail. | **No.** Parallelism produces "governance theatre," not improved risk mitigation. |
| **7. Governance Work Multiplied?** | Yes. Dual-regulated entities must map, document, and audit the same systems twice. | Yes. Compliance teams must run parallel reporting cycles for the same tools. | **Yes.** Parallelism systematically generates substantial organizational burden. |

---

## 8. Governance Debt Assessment

The uncoordinated accumulation of parallel mandates across Indian regulators generates significant **[[Governance_Debt]]** for regulated enterprises. The table below evaluates and quantifies this burden:

| Parallel Mandate Interface | Additional Governance Work | Additional Control Value | Governance Debt Level | Rationale |
|---|---|---|---|---|
| **SEBI Reg 16C ↔ RBI Digital Lending (RBI_7)** | Dual-regulated NBFCs must maintain two independent AI asset registers, mapping the same models to SEBI's rigid 6-category taxonomy and RBI's model-risk classifications. | **None.** The underlying algorithmic risk is identical; separate registers add zero technical security. | **High** | Forces compliance teams to run parallel documentation streams and limits the reuse of model-validation artifacts. |
| **CERT-In 6-Hour Reporting ↔ RBI DAKSH ↔ SEBI CSCRF** | During a major cyber-AI failure, an enterprise must file three distinct incident reports with different taxonomies, formats, and escalation pathways within overlapping time windows. | **Low.** While rapid notification is valuable, the fragmented formats force the entity to duplicate triage effort during a crisis. | **High** | Divergent incident taxonomies and short reporting windows systematically transfer the coordination burden to the victim. |
| **DPDP SDF Audit ↔ SEBI CSCRF Quarterly Review ↔ CERT_In_1 Audit** | An enterprise must undergo three separate, non-aligned audit cycles (annual DPIA, quarterly board cyber-AI reviews, and annual CERT-In cyber audits), using different auditors. | **Moderate.** CERT-In's standardized "AI System Audit" category adds value, but the inability to reuse audit artifacts across forums is inefficient. | **Moderate** | Lack of cross-recognition of audits prevents the enterprise from leveraging a single technical evaluation to satisfy multiple regulators. This is the canonical [[Assurance_Reuse_Gap]] instance in the corpus. |
| **RBI Outsourcing (RBI_2) ↔ SEBI Reg 16C Vendor Clause** | Intermediaries must negotiate separate, highly complex liability-shifting contracts with global AI cloud and SaaS providers to satisfy conflicting sectoral non-delegation rules. | **Low.** The contract-heavy focus insulates the regulators but does not address the underlying technical supply-chain risk (e.g., model drift). | **High** | Sectoral non-delegation clauses insulate vendors while placing the entire, unmanageable technical burden on the enterprise. |

---

## 9. Institutional Coherence Assessment

Evaluating the Indian regulatory landscape against the dimensions of **[[Institutional_Coherence]]** reveals a system characterized by high administrative complexity but low structural integration. A key analytical distinction that emerges from this assessment is between **horizontal infrastructure coherence** (which CERT-In achieves by standardizing the cyber-auditor market via its empanelment scheme) and **vertical substantive incoherence** (where RBI, SEBI, and MeitY maintain parallel, non-aligned rules sitting atop that shared infrastructure). Coherence is not a binary state; it can exist at the technical infrastructure layer while being absent at the rule-making layer.

- **Clear Role Allocation:** **Low.** While sectoral boundaries are clear for traditional activities (lending vs. securities trading), they collapse in digital-first environments. A single AI-driven robo-advisory tool that also facilitates credit lines falls simultaneously under RBI, SEBI, and DPBI jurisdiction, with no clear lead regulator.
- **Consistent Terminology:** **Low.** There is no harmonised definition of "AI," "machine learning," or "algorithmic decision system" across Indian regulators. SEBI's 2019 circulars rely on a rigid, six-category taxonomy; RBI's FREE-AI uses a broad "model risk" framing; MeitY's draft IT Rules focus on synthetic media; and CERT_In_1 defines "AI System Audits" broadly without technical standards.
- **Interoperable Reporting:** **Absent.** Sectoral incident reporting channels (RBI DAKSH, SEBI CSCRF, CERT-In, DPBI) are completely non-interoperable. There is no shared reporting template (such as the international FSB FIRE format), forcing entities to manually translate technical incident data into multiple regulatory vocabularies.
- **Shared Assurance & Cross-Recognition of Audits:** **Absent.** No financial regulator accepts an audit certificate issued under another regulator's framework as discharging its own requirements. An audit completed by a CERT-In empanelled auditor to satisfy CERT_In_1 does not discharge an RBI IT outsourcing audit obligation or a DPDP SDF audit requirement, preventing the reuse of assurance artifacts. This is the canonical [[Assurance_Reuse_Gap]] pattern.
- **Coordinated Enforcement:** **Low.** Sectoral regulators enforce compliance through independent, isolated channels (RBI's PCA framework, SEBI's Chapter V enquiry, DPBI's financial penalties). There is no permanent, cross-authority enforcement coordination mechanism comparable to the UK's Digital Regulation Cooperation Forum (DRCF).

---

## 10. Contradictions and Ambiguities

The polycentric technology-governance landscape produces several unresolved legal and operational frictions:

### 1. Direct Legal Contradiction — The DLT-Privacy Conflict (TRAI vs. MeitY)

TRAI's UCC Spam Direction 2026 mandates that telecom access providers deploy AI spam detection and share flagged numbers via Distributed Ledger Technology (DLT) within 2 hours. However, the DPDP Act 2023 enforces a strict "right to erasure" (Rule 8) and purpose limitation. Because DLT architectures are structurally immutable, a telecom provider cannot erase a flagged number from the ledger without breaking the TRAI mandate, creating a direct legal contradiction between sectoral telecom rules and horizontal data protection law. This is the sharpest direct-legal-contradiction instance in the corpus and warrants a standalone doctrinal analysis feed into [[P4_Doctrinal_IJLIT]].

### 2. Implementation Inconsistency — Data Localisation Thresholds

IRDAI_1 reports a blanket data-localisation mandate ("all data... in Indian data centres"), whereas MeitY's DPDP Rules (Rule 13(4)) restrict cross-border transfer only for government-specified SDF personal data, and the RBI enforces payment-specific localisation. An enterprise operating across banking, insurance, and digital services must segment its database architecture into multiple, non-aligned regional storage pools to satisfy these varying thresholds.

### 3. Definitional Ambiguity — The "AI Vendor" Liability Gap

SEBI Regulation 16C declares that the registered intermediary is "solely responsible" for AI outputs, effectively insulating third-party AI vendors from direct regulatory accountability. However, MeitY's draft IT Rules 2025 seek to hold AI developers and platforms directly liable for synthetic media outputs. This creates a severe definitional ambiguity regarding liability allocation in the AI supply chain for financial services.

### 4. Temporal Inconsistency — Ex-Ante Approval vs. Ex-Post Incident Response

Regulated entities must navigate conflicting temporal tracks simultaneously. RBI's model-validation expectations (RBI_3) and SEBI's Regulatory Sandbox ([[07_Institutions/Corpus/SEBI/SEBI_13_Regulatory_Sandbox_Framework_2021|SEBI_13]]) require extensive, slow ex-ante testing. Conversely, CERT-In's Directions enforce a hyper-reactive, 6-hour ex-post incident notification window. This mismatch forces enterprises to divert technical resources away from thorough pre-deployment safety testing to maintain expensive, hyper-reactive notification infrastructures.

---

## 11. India-Centric Governance Implications

The structural frictions of India's technology-governance landscape produce distinct national implications:

- **Whole-of-Government Coordination:** The absence of a permanent coordinating body (like the UK's DRCF) prevents the Indian state from presenting a unified technology-policy posture. While NITI Aayog proposed a "Council for Ethical Technology" (CET) in 2021 to drive convergence, the proposal remains unimplemented as of mid-2026, allowing sectoral silos to deepen.
- **Ease of Compliance:** The accumulation of [[Regulatory_Parallelism]] and [[Governance_Debt]] acts as a significant regulatory tax on Indian enterprises. Dual-regulated financial firms and digital startups must allocate substantial capital to administrative paper-mapping and duplicate audit cycles, diverting resources away from actual technical R&D and core model-safety engineering.
- **Regulatory Capacity:** Both the regulators and the panellist auditors exhibit a severe deficit in AI-specific technical capacity. While CERT_In_1 defines "AI System Audits" and "AIBOM Auditing," there are no standardized technical audit playbooks (such as the EU's mapping of ISO 42001 controls documented in [[04_Knowledge_Products/Wiki_Intake/F034_Buscemi_Assessing_High_Risk_AI_2025|F034]]) to verify compliance. This capacity gap forces regulators to rely on "paper-heavy" processual compliance, generating administrative forms that satisfy bureaucrats but fail to secure actual operational systems.
- **Sovereign Digital Rails (DPI):** India's Digital Public Infrastructure (Aadhaar, UPI, Account Aggregator) is built on state-backed, population-scale digital rails. In this ecosystem, citizens are heavily represented as data records but structurally excluded from enforceable rule-bearing structures (the [[Records_Rules_Asymmetry]]). If an AI-enabled eligibility algorithm or biometric authentication fails, there is a complete absence of legally mandated, citizen-facing fallback procedures or localized grievance redressal, systematically transferring the procedural burden of system failure to the citizen.
- **Strategic Autonomy and the Compute Gap:** India's technology policy is driven by a commitment to strategic autonomy and localized data storage. However, this sovereignty claim is structurally constrained by a deep domestic "compute gap"—a reliance on foreign compute hardware and global cloud providers. Systemic technology governance must navigate this tension, balancing localized compliance mandates with the practical necessity of accessing global frontier models.

---

## 12. Recommendations

### Institutional Level (Regulators & Government)

1. **Establish a Financial Technology Joint Coordination Committee (FT-JCC):** RBI, SEBI, IRDAI, and the DPBI should execute a formal Memorandum of Coordination establishing a permanent joint committee. The FT-JCC should harmonise AI/ML taxonomies, align incident reporting timelines, and establish a unified digital registry for AI assets.
2. **Implement Cross-Recognition of Technical Audits:** Sectoral regulators should formally agree to cross-recognize audit certificates. A technical AI system audit or AIBOM audit conducted by a CERT-In empanelled auditor using standardized guidelines (such as ISO 42001) should be accepted as discharging the equivalent technical audit obligations under RBI's outsourcing rules and DPDP's Significant Data Fiduciary rules — directly addressing the [[Assurance_Reuse_Gap]].
3. **Draft a Joint "AI Explanability and Consumer Protection" Circular:** RBI and SEBI should issue joint guidance defining clear, sector-aligned standards for algorithmic explainability and consumer recourse, closing the "explainability gap" in digital lending and investment advisory.

### Enterprise Level (Regulated Entities)

1. **Build a Unified Controls Framework (UCF):** Dual-regulated financial entities should abandon siloed compliance mapping. They should design a UCF—a many-to-many control library where a single operational activity (e.g., executing a standardized model-drift validation test) simultaneously generates the evidentiary artifacts required to satisfy RBI's FREE-AI, SEBI's CSCRF, and DPDP's Significant Data Fiduciary audit cycles.
2. **Establish a Common Evidence Repository (CER):** Implement a centralized, write-once-read-many (WORM) digital repository for all technical audits, model documentations, and board attestation artifacts, allowing multiple internal compliance teams to reuse the same assurance documents.
3. **Implement Automated Runtime Decision Enforcement (e.g., AEGIS_OS):** Deploy technical guardrails at the API and model execution layer to log AI outputs, detect hallucinations, and enforce purpose-limitation rules in real-time, converting passive "paper compliance" into active technical enforcement.

### Research Level (Academic & Policy)

1. **Quantify the Cost of Governance Debt:** Conduct structured compliance-cost surveys across dual-regulated financial institutions in India to empirically measure and mathematically operationalise the financial burden of regulatory parallelism.
2. **Map the Sub-National Regulatory Interface:** Expand the PRIS corpus to analyze how sub-national technology policies (such as Tamil Nadu's ethics-first framework) interface with central sectoral mandates, testing for vertical regulatory parallelism.
3. **Conduct Longitudinal Analysis of AI Audit Quality:** Track the performance of CERT-In empanelled auditors executing the new "AI System Audit" and "AIBOM Auditing" categories under CERT_In_1, evaluating whether the empanelment model successfully builds actual technical capacity over time.

---

## 13. Conceptual Contribution

This cross-institutional comparison provides strong empirical grounding that:

- **Supports and Extends [[Regulatory_Parallelism]]:** The Indian case proves that the absence of a horizontal, centralizing AI law systematically drives independent sectoral regulators to insert uncoordinated, parallel algorithmic-governance clauses into pre-existing sectoral frameworks. We extend the concept by proposing the construct of [[Deontic_Bifurcation]] — the structural coexistence of highly coercive, binding sectoral "shall" rules alongside flexible, principles-based horizontal "should" guidelines, which systematically drives enterprises to prioritize rigid compliance over ethical principles.
- **Supports and Grounds [[Governance_Debt]]:** The comparison demonstrates that uncoordinated parallelism directly translates into a measurable organizational burden. We ground this concept by documenting the [[Assurance_Reuse_Gap]] — the systematic inability of enterprises to reuse technical audit artifacts across different regulatory forums, which multiplies "governance theatre" without improving substantive system security.
- **Refines [[Institutional_Coherence]]:** Our findings refine the concept of institutional coherence by distinguishing **horizontal infrastructure coherence** (which CERT-In achieves by standardizing the cyber-auditor market) from **vertical substantive incoherence** (where RBI, SEBI, and MeitY maintain parallel, non-aligned rules sitting atop that shared infrastructure). Coherence is not a binary state; it can exist at the technical infrastructure layer while being absent at the rule-making layer.

---

## 14. Compounding Loop

This comparative analysis directly feeds the PRIS continuous compounding loop:

```
[Regulatory Evidence (Corpus Nodes: RBI_7, SEBI_14, SEBI_15, CERT_In_1)]
                           │
                           ▼
[Cross-Institutional Comparison (This Knowledge Product Note)]
                           │
                           ▼
[Refined Signature Concepts (Deontic_Bifurcation & Assurance_Reuse_Gap)]
                           │
                           ▼
[Academic Manuscripts (P3_BFSI_JEIM & P4_Doctrinal_IJLIT Submissions)]
                           │
                           ▼
[Consulting Control Frameworks (AEGIS_OS & PrivacyWeave Implementations)]
                           │
                           ▼
[Enterprise Implementation Evidence (Quantified Compliance Cost Savings)]
                           │
                           ▼
[Revised Academic Concepts & Policy Briefs (MeitY / FSDC Submissions)]
```

---

## 15. Related PRIS Notes

- [[Systemic_Regulatory_Governance]]
- [[AI_Governance]]
- [[BFSI_Governance]]
- [[DPI_Governance]]
- [[Privacy_DataProtection]]
- [[Cybersecurity_Governance]]
- [[Regulatory_Parallelism]]
- [[Governance_Debt]]
- [[Institutional_Coherence]]
- [[Accountability]]
- [[Legitimacy]]
- [[Deontic_Bifurcation]]
- [[Assurance_Reuse_Gap]]
- [[Records_Rules_Asymmetry]]
- [[RBI]]
- [[SEBI]]
- [[MEITY]]
- [[CERT_IN]]
- [[IRDAI]]
- [[Institutional_Grammar_IG2]]
- [[fsQCA]]

---

*Knowledge product prepared: 2026-07-14 | PRIS v2.3 | Cowork session (companion to [[Systemic_Regulatory_Governance]])*
