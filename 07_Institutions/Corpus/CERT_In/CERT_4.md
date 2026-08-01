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

# CERT_4 — Technical Guidelines on SBOM | QBOM & CBOM | AIBOM | HBOM (v2.0)

**Type:** Corpus Node  
**Vault path:** `07_Institutions/Corpus/CERT_In/CERT_4.md`  
**Institution:** [[07_Institutions/CERT_IN]]  
**Issuing body:** Indian Computer Emergency Response Team (CERT-In), Ministry of Electronics and Information Technology  
**Document date:** July 9, 2025 (Version 2.0)  
**Pages:** 65  
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]]  

---

## Instrument Identity

**Full title:** Technical Guidelines on SBOM | QBOM & CBOM | AIBOM | HBOM  
**Version:** 2.0 (July 09, 2025)  
**Issuer:** CERT-In / MeitY  
**Target scope:** Government entities, public sector, essential services organisations, software exporters, software services industry — Software Consumers, Developers, System Integrators  
**Authority basis:** CERT-In mandate under IT Act 2000 (Section 70B)

---

## Analytical Classification

**P3 corpus role:** Screening — not in canonical 91-RU analytical corpus (CERT-In = null AI-RU finding for P3). However, the AIBOM section (Chapter 9) constitutes substantive AI governance content for P4 and AI Governance Wiki.  
**P4 corpus relevance:** HIGH — AIBOM framework is directly relevant to AI supply chain governance and BFSI AI compliance.  
**AI Governance Wiki relevance:** HIGH — SBOM/AIBOM/HBOM framework represents India's most detailed technical AI transparency standard to date.  
**Tier classification:** Tier A (explicit AI-specific regulation — Chapter 9 AIBOM); Tier B (technology-neutral with AI application — SBOM/HBOM supply chain chapters)  
**RU count (estimated):** Not formally coded in P3 corpus. Requires fresh coding for future use.

---

## Substantive Content

### Chapter 9 — AIBOM (Artificial Intelligence Bill of Materials) [pp. 53–58]

**Definition:** Comprehensive list of components used in building, training, and deploying AI models — covering hardware (servers, sensors, GPUs), software (AI models, frameworks, development tools), data sources, and essential operational elements.

**Minimum AIBOM Elements (18 fields):**
- Model Name, Model Version, Model Type, Model Developer
- Model Licensing Information
- Software Dependencies
- ML Models and Algorithms (decision-making processes, input handling, learning mechanisms)
- Model Performance Metrics (accuracy, precision, recall, F1)
- Data Source (origin, provenance)
- Data Sets (names, versions, formats, limitations)
- Hardware (GPUs, TPUs, storage, memory)
- Security Requirements (encryption, access control)
- Input / Output type
- Intended Usage / Out of Scope Usage
- Environmental Impact (energy consumption, carbon footprint)
- Vulnerabilities (CVE references, severity ratings)
- Attestations (digital signature for model/AIBOM)

**AIBOM Recommendations (mandatory language):**
- All government/public sector AI procurements must include AIBOM requirement
- All AI solutions supplied to government must be accompanied by AIBOM
- Format: SPDX or CycloneDX
- VEX document required post-vulnerability discovery (Not Affected / Affected / Fixed / Under Investigation)
- AIBOM must be integrated with vulnerability databases and CERT-In advisories
- Consumer organisations must build internal AIBOM from supplier AIBOM
- Security teams must incorporate AIBOM into vulnerability management workflows
- Regular audits required; AIBOM data must be securely stored and transmitted

**AIBOM Best Practices:** Comprehensive inventory; standardised formats; automated generation; reproducibility (scripts, model weights, configuration settings); prioritise critical/high-risk models; track model lineage (versions, retraining, modifications)

### Chapter 8 — QBOM & CBOM (Quantum and Cryptographic BOM) [pp. 42–52]

**QBOM:** Quantum-safe inventory covering quantum algorithms, security frameworks, post-quantum cryptographic (PQC) components  
**CBOM:** Cryptographic asset inventory (algorithms, keys, protocols, certificates, dependencies)  
**PQC transition mandate:** RSA, ECC, Diffie-Hellman, DSA are vulnerable to Shor's algorithm → organisations must plan migration to lattice-based/code-based/multivariate polynomial primitives  
**Recommendation 8.4.1.1:** All government/public sector organisations shall mandate CBOM/QBOM in all cryptographic procurements  
**Format:** SPDX or CycloneDX; VEX required upon vulnerability discovery

### Chapter 10 — HBOM (Hardware Bill of Materials) [pp. 59–65]

**Definition:** Structured inventory of all physical components, sub-components, embedded devices — servers, networking equipment, storage, end-user systems, power backup, security infrastructure  
**Minimum Elements (18 fields):** Product Name/Version/Details, Warranty/AMC, Manufacturer Name/Location/Date, Supplier Information/Location, Model Number, Serial Number, Technical Specification, Technology Node, Compliance, Power Supply, License Information, Test Result, Sub-components  
**Mandate:** Government/public sector organisations must require HBOM in all hardware procurement contracts; HBOM must be accompanied with all hardware deliveries  
**Key governance provision:** HBOM must be integrated with CERT-In vulnerability notes, firmware advisories, threat intelligence platforms

### Chapters 1–7 — SBOM (Software Bill of Materials) [pp. 4–41]

**Target entities:** Software Consumer / Developer / System Integrator  
**Minimum data fields (21):** Component Name, Version, Description, Supplier, License, Origin, Dependencies, Vulnerabilities, Patch Status, Release Date, EOL Date, Criticality, Usage Restrictions, Checksums, Comments, SBOM Author, Timestamp, Executable/Archive/Structured Property, Unique Identifier (PURL format)  
**Standard formats:** SPDX, CycloneDX (machine-readable)  
**SBOM Levels:** Top-Level, N-Level, Delivery, Transitive, Complete  
**SBOM Classifications (aligned to SDLC):** Design, Source, Build, Analyzed, Deployed, Runtime  
**Adoption roadmap:** Phase 1 (Start) → Phase 2 (Progress) → Phase 3 (Advance)  
**Vulnerability management:** VEX + CSAF (Common Security Advisory Framework) integration required  
**Recommendation 7.1.1 (Government mandate):** All government/public sector/essential services organisations must include SBOM requirements in all software procurement  
**Recommendation 7.1.7:** Integration with CERT-In vulnerability notes and threat intelligence platforms mandatory

---

## Analytical Significance for PRIS Research

### For P3 (BFSI AI Governance / JEIM)
- CERT-In null finding for P3 corpus is confirmed (AIBOM is a July 2025 document; P3 corpus was finalised before this date)
- AIBOM appears as a downstream indicator of the governance gap P3 identifies — CERT-In now moving into AI supply chain territory that RBI/SEBI have not yet addressed
- Provides comparative evidence for the coordination gap between CERT-In's technical standards and SEBI/RBI's functional AI governance

### For P4 (BFSI Legal / IJLIT)
- AIBOM creates a new compliance obligation layer for financial entities deploying AI
- HBOM adds hardware supply chain governance that intersects with RBI IT governance directions
- CBOM/QBOM adds post-quantum cryptography compliance requirements for BFSI entities
- Creates doctrinal complexity: which regulator's obligation governs when AIBOM requirement conflicts with RBI IT outsourcing directions on vendor disclosure?

### For AI Governance Wiki
- AIBOM framework is the most detailed AI transparency and accountability standard India has issued
- Comparative significance: India's AIBOM aligns with EU AI Act's technical documentation requirements (Article 11) and NIST AI RMF's GOVERN function
- CERT-In is asserting jurisdiction over AI supply chain governance previously unaddressed in Indian regulatory space
- SBOM/AIBOM/HBOM/QBOM/CBOM together constitute a comprehensive "Digital Infrastructure Bill of Materials" framework — a significant regulatory innovation

### For fsQCA / Regulatory Parallelism
- AIBOM requirement from CERT-In and AI reporting requirements from SEBI/RBI create potential parallelism at the AI system transparency layer
- No cross-reference between CERT-In AIBOM and SEBI AI/ML reporting circulars despite functional equivalence on AI system inventory
- Coordination pattern: Unidirectional (CERT-In issues without referencing SEBI/RBI) or Unpaired (no cross-regulator equivalent in the 2019–2024 corpus)

---

## Coordination Pattern Analysis

| Pattern | Evidence |
|---------|----------|
| Parallelism (CERT-In ↔ SEBI) | AIBOM requires AI system documentation; SEBI AI/ML circulars require AI system reporting — functionally equivalent, issued without cross-reference |
| Unidirectional (CERT-In → SEBI/RBI) | CERT-In AIBOM cites SPDX/CycloneDX but does not reference SEBI AI/ML reporting regime or RBI IT directions |
| Gap (no BFSI-specific AIBOM) | RBI and SEBI have not issued AIBOM requirements specific to BFSI AI systems; CERT-In is general-purpose |

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/CERT_In/CERT_1]] | [[07_Institutions/Corpus/CERT_In/CERT_2]] | [[07_Institutions/Corpus/RBI/RBI_1]] | [[07_Institutions/Corpus/RBI/RBI_2]] | [[07_Institutions/Corpus/SEBI/SEBI_9]] | [[07_Institutions/Corpus/SEBI/SEBI_10]] | [[07_Institutions/Corpus/SEBI/SEBI_11]]  
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]]  
**Related frameworks:** [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]]  
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] | [[02_Projects/P4_Doctrinal_IJLIT]]  
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]  
**International comparators:** EU AI Act Article 11 (Technical Documentation) | NIST AI RMF GOVERN function | US EO 14028 SBOM mandate

---

## Coding Status

- **P3 NVivo coding:** Not in canonical corpus — CERT-In null finding confirmed
- **AI Governance Wiki coding:** Pending — Chapter 9 (AIBOM) should be coded for Wiki intake
- **P4 coding:** Flag for doctrinal analysis — AIBOM creates compliance gap in BFSI sector

---

## Log

- 2026-06-13: Corpus node created from source extraction. S5 session.
