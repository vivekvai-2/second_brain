---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/ncaic
---

# NCAIC_1 — AI Governance Framework for India 2025-26 (National Cyber and AI Center)

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26.md`
**Institution:** [[07_Institutions/NCAIC]] ⚠ VERIFY BEFORE PUBLISHING — **CRITICAL institutional-identity flag**. This document was sourced for Batch 7 under the working filename "AI_governace_Framework_2025_for_india" and was originally slated for **NITI_8** (i.e., assumed to be a NITI Aayog publication). On reading, the issuing body is explicitly the **"National Cyber and AI Center (NCAIC)"** (www.ncaic.in), described as publishing "A National Policy Report." NCAIC is **not** one of the institutions previously tracked in this corpus (RBI, SEBI, MeitY, NITI Aayog, IRDAI, CERT-In) and does not correspond to any GoI ministry/statutory body known from prior batches. ⚠ Before treating this as an official Government of India instrument, verify: (a) whether NCAIC is a registered/recognised GoI body, a proposed/under-formation entity, an industry consortium, or a private think-tank publishing under a national-sounding name; (b) whether www.ncaic.in resolves to an official `.gov.in` or `.nic.in` domain (the cited domain is `.in`, not `.gov.in`); (c) whether NITI_8 should instead be reserved for a genuine NITI Aayog document not yet sourced. Pending verification, this node is filed under a **new, provisional NCAIC institution folder** rather than NITI_8 — **do not renumber NITI_8 to this document** until the institutional identity of NCAIC is confirmed.
**Issuing body:** National Cyber and AI Center (NCAIC) — self-described as coordinating across "National Cyber and AI Center (NCAIC), Ministry of Electronics and Information Technology, CERT-In, IndiaAI Mission, various sectoral regulators, leading technology companies, premier academic institutions, and civil society advocacy groups" (Acknowledgments section)
**Document date:** Published September 1, 2025
**Pages:** 36 (whitepaper/national policy report format, with infographics)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/Cybersecurity_Governance]]

---

## Instrument Identity

**Full title:** AI Governance Framework for India 2025-26 — Whitepaper for the National Cyber and AI Center (NCAIC), "A National Policy Report"
**Type:** Whitepaper / proposed national framework (non-binding as presented — ⚠ VERIFY whether this has any formal regulatory status, or is a policy-advocacy/framework-proposal document analogous to a model law or industry-association template)
**Target entities:** Ministries, regulatory bodies, public sector undertakings (PSUs), and large enterprises operating in India — i.e., a cross-sectoral framework intended for voluntary or eventually-mandated adoption, not a binding regulation on its own terms
**Legal basis:** None cited directly — the document positions itself as synthesising and operationalising existing legal instruments (DPDP Act 2023 + Draft DPDP Rules 2025, CERT-In Directions 2022, sectoral regulator mandates, IndiaAI Mission) rather than deriving authority from a specific statutory provision. ⚠ VERIFY — no enabling notification, executive order, or Cabinet approval is cited for the framework itself.
**Companion documents:** Explicitly cross-references [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (cited as "Draft DPDP Rules 2025" — note the source document predates or was drafted concurrent with the final notified DPDP Rules 2025 of Nov 13, 2025, and refers to them as still "Draft" as of Sept 1, 2025 publication — internally consistent with MeitY_4's commencement timeline), CERT-In Directions 2022 (6-hour incident reporting, 180-day log retention — cf. [[07_Institutions/CERT_IN]] nodes), IndiaAI Mission, and international standards (ISO/IEC 42001, ISO/IEC 23894, NIST AI RMF 1.0, EU AI Act).

---

## Analytical Classification

**Wiki section:** S3 (AI Governance Frameworks — India) / S4 (Agentic AI Governance) / S6 (Implementation & Governance Artifacts)
**Jurisdiction:** India (national, cross-sectoral)
**Confidence:** MEDIUM — primary-source document (full 36-page whitepaper read directly), but ⚠ institutional provenance/authority is unverified (see Institution flag above). Confidence in the **content's internal consistency and cross-referencing accuracy** (DPDP, CERT-In, IndiaAI Mission alignment) is HIGH; confidence in the **document's formal regulatory status or binding effect** is LOW pending verification.
**AI explicit:** YES — this is the most comprehensive, explicitly AI-focused framework document in the corpus to date. Unlike MeitY_4 (DPDP Rules) or RBI_6 (outsourcing directions), which contain AI-relevant provisions embedded within broader instruments, this document is **wholly and exclusively** an AI governance framework.
**Tier classification:** Tier A — comprehensive, dedicated AI governance framework with explicit risk taxonomy, lifecycle controls, and institutional architecture
**AI Governance Wiki relevance:** VERY HIGH — this is the single most structurally complete "model AI governance framework for India" document in the corpus, directly comparable to NIST AI RMF, ISO/IEC 42001, and the EU AI Act in scope and ambition, while explicitly adapting to the Indian regulatory landscape (DPDP, CERT-In, sectoral regulators, IndiaAI Mission). High priority for S3/S4/S6 wiki sections regardless of the institutional-provenance question, given the framework's substantive content can be analysed on its own terms as a "proposed national AI governance template."

---

## Substantive Content

### Foundational Design Principles (8 principles)
The framework is built on eight principles: Human-Centric Approach (human oversight, opt-out, appeal mechanisms), Risk Proportionality (prohibited/high/medium/low-risk tiers), Privacy by Design (DPDP-aligned consent, minimisation, retention, deletion), Security by Design (adversarial robustness, prompt-injection defences, secrets isolation, immutable audit trails), Transparency and Explainability (model cards, data sheets, provenance metadata), Inclusivity and Fairness (bias testing across Indian demographics/languages/cultures), Accountability and Traceability (named ownership, immutable logging), and Continuous Assurance (pre-deployment and ongoing evaluation).

### Risk Classification Taxonomy
Four-tier taxonomy explicitly adapted to "India's public interest priorities":
- **Prohibited AI systems**: social scoring of citizens for public benefit access; biometric categorisation by sensitive personal attributes; emotion inference for employment/education/credit decisions; subliminal manipulation targeting vulnerable populations. ⚠ VERIFY BEFORE PUBLISHING — this prohibited list closely mirrors EU AI Act Article 5 prohibited practices; the framework explicitly states EU AI Act taxonomy "informs" its risk classification while adapting to "Indian constitutional principles" — useful comparative datapoint for fsQCA, but the degree of genuine adaptation vs. direct transposition should be assessed before citing as an "Indian-specific" innovation.
- **High-risk**: financial services (credit scoring/underwriting), employment/education (hiring algorithms, admissions, performance evaluation), critical infrastructure (power grid, telecom core, transport safety, medical devices), law enforcement (biometric ID, risk scoring, predictive policing).
- **Medium-risk**: fraud detection, content moderation, customer-support copilots with sensitive data access, remote proctoring with biometric verification.
- **Low-risk**: code assistants, content generation without personal data, general chatbots, internal automation.

### Governance Model and Organisational Structure
Four-tier model: Board & Apex Leadership (risk appetite approval, quarterly reporting) → AI Risk and Ethics Committee (AIREC — cross-functional, maintains AI System Inventory, risk classification, deployment approvals) → Chief AI Risk Officer (CARO — single-threaded ownership, regulatory coordination) → Operational Roles (model owners, data stewards, security leads, evaluation specialists). A RACI table assigns System Inventory (Model Owner/CARO/Data Steward), Risk Classification (Eval Lead/AIREC/Legal-Privacy), Production Approval (AIREC/Board Delegate/Security-Legal), and Incident Reporting (Security Lead/CARO/Legal-Privacy-PR).

### AI System Inventory and Registration
Mandatory registration of **every** AI system regardless of risk tier, covering use case, business/technical owners, data sources, model lineage/provenance, third-party dependencies, risk classification, deployment environment, and operational status. High-risk systems require enhanced AIREC registration with technical documentation, risk assessment, mitigation measures, and monitoring plans, with potential regulatory notification for regulated sectors.

### Data Governance, Secure Development, and AIBOM
Data governance operationalises DPDP requirements across the AI lifecycle (collection/processing/storage/sharing/deletion), explicitly invoking DPDP data-subject rights (access, rectification, deletion) even for decommissioned AI systems. Secure model development mandates an **AI Bill of Materials (AIBOM)** — documenting training datasets, pre-trained models, software libraries, dev tools, third-party APIs, and cryptographic attestations — plus model cards/data sheets initiated at design time and threat modelling for prompt injection, data poisoning, model extraction, and inference-time manipulation.

### Pre-Deployment Evaluation Gates and Production Operations
Five mandatory evaluation gates: Safety (jailbreak resistance, harmful content), Security (adversarial robustness, model extraction resistance, RAG hardening), Privacy (membership inference, PII leakage), Fairness (demographic parity across Indian linguistic/regional/socioeconomic segments), Performance (accuracy, latency, cost). Production operations require environment hardening (network isolation, MFA, kill-switches), **content provenance via C2PA manifests** for AI-generated content, audit logging aligned to CERT-In and DPDP, human-in-the-loop workflows for high-risk decisions, and an **operational requirement for automated rollback within 15 minutes** of detecting safety/security/performance issues. ⚠ VERIFY BEFORE PUBLISHING — the 15-minute rollback requirement and the "99.7% safety compliance / <0.1% jailbreak rate / 15-minute incident response / 100% inventory coverage" metrics presented in the Performance Metrics section (p.23) appear to be **illustrative target figures or aspirational benchmarks**, not empirically reported statistics — do not cite as measured outcomes from any actual Indian AI deployment.

### Assurance, Certification, and International Standards Alignment
Three-tier certification ladder (Basic Compliance/self-certification → Enhanced Assurance/biennial independent audit → Premium Certification/ISO 42001 + annual audit), explicitly mapped to ISO/IEC 42001 (AIMS), ISO/IEC 23894 (AI risk management), NIST AI RMF 1.0 (Govern/Map/Measure/Manage), and EU AI Act taxonomy/conformity assessment. Independent testing is positioned to leverage **IndiaAI Safety Institute** laboratories for red-teaming and conformance testing — a direct institutional linkage to the IndiaAI Mission infrastructure.

### Sectoral Implementation Blueprints
Dedicated guidance for BFSI (credit-scoring fairness, explainability, audit trails, stress testing — directly relevant to [[02_Projects/P3_BFSI_JEIM]]), Healthcare (clinical safety officer authority, post-market surveillance, medical device regulation interface), Telecommunications (5G core security, lawful intercept, supply-chain assurance), and Manufacturing/OT (Purdue model segmentation, safety interlocks, firmware integrity for edge ML).

### Implementation Roadmaps (100-day / 12-month / 24-month)
A phased adoption roadmap: 100-day "quick start" (appoint CARO, constitute AIREC, board approval, complete AI system inventory, halt shadow IT, draft AIPIA templates); 12-month "maturity" (ISO 42001-aligned AIMS, evaluation harness development, content-provenance/watermarking implementation, advanced monitoring); 24-month "strategic excellence" (external ISO 42001 certification, transparency reporting, ecosystem participation, advanced red-teaming).

### Enforcement, Incident Response, and Case Studies
Enforcement framework proposes graduated sanctions "aligned with DPDP Act," sector-specific enforcement by existing regulators, safe-harbour protections for proactive/transparent reporting, and grievance redressal with ombudsperson mechanisms. Incident response integrates **CERT-In's 6-hour reporting requirement** with DPDP breach notification, with a four-phase timeline (0-1hr immediate response, 1-6hr assessment/reporting, 6-24hr remediation, 24+hr recovery/learning). Two illustrative case studies — a payment-fraud-detection data-drift incident (with RBI/CERT-In notification) and a healthcare radiology AI demographic-performance-degradation incident — demonstrate the framework's incident-response and fairness-monitoring mechanisms in practice (presented as **illustrative scenarios**, not documented real incidents — ⚠ VERIFY if either case study is later found to reference an actual reported incident).

### NCAIC's Proposed National Role
The document positions NCAIC itself as the coordinating body for: national conformance programmes (certification, technical standards, evaluation frameworks), sectoral coordination across regulators (RBI, SEBI, IRDAI, DoT, NCIIPC, state authorities — explicitly named as maintaining "cyber and risk mandates that intersect with AI assurance"), capacity building, and international representation — i.e., NCAIC is proposed as a **functional analogue to a national AI regulator/coordination body**, which is precisely why its institutional status (per the flag above) is the single most important verification item arising from this document.

---

## Analytical Significance for PRIS Research

### For P1 (AI Governance SLR)
This document is the corpus's most direct primary source for "what a comprehensive, dedicated Indian AI governance framework could look like" — as distinct from the amendment-based, sector-by-sector approach evidenced in MeitY_4, MeitY_5, RBI_6, SEBI_9-13, and IRDAI_1. If NCAIC's institutional status is confirmed as a genuine (even if nascent/proposed) GoI coordination body, this document becomes a **central counter-example** to the [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] thesis — i.e., evidence that India is *also* pursuing (or at least has a credible proposal for) a horizontal, NIST/ISO/EU-AI-Act-aligned coordinating framework alongside the parallel sectoral insertions. If NCAIC's status is *not* confirmed as official, the document instead becomes evidence of a **third-party/industry-proposed model framework** filling the perceived gap left by regulatory parallelism — itself a relevant data point about how the absence of a horizontal AI law generates non-governmental framework proposals.

### For Institutional Grammar / ADICO and fsQCA
The risk-classification taxonomy (prohibited/high/medium/low) and the AIREC/CARO governance architecture are highly ADICO-codeable — explicit Attributes (AIREC, CARO, Board), Deontics ("must register," "shall implement," "must report within 6 hours"), Aims (registration, evaluation, reporting), and Conditions (risk tier, deployment status). This is a strong candidate for fsQCA as a **configurational template** — i.e., a hypothetical "what full AI-specific institutional coherence would look like" configuration against which the actual fragmented landscape (MeitY/RBI/SEBI/IRDAI parallel insertions) can be compared.

### Coordination / Parallelism Pattern
**Existing nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]], [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]], [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]], [[07_Institutions/Corpus/SEBI/SEBI_9]]/[[07_Institutions/Corpus/SEBI/SEBI_10]]/[[07_Institutions/Corpus/SEBI/SEBI_11]], [[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025]].
**Pattern:** This document explicitly **names and cross-references** the parallel regulatory tracks (DPDP/MeitY, CERT-In, RBI/SEBI/IRDAI/DoT/NCIIPC) as the "Regulatory Landscape Alignment" this framework must integrate with — making it the **first corpus document to explicitly acknowledge and attempt to bridge the cross-regulator parallelism** identified across MeitY_4, RBI_6, SEBI_9-13, and IRDAI_1. Whether NCAIC has the institutional standing to actually perform this bridging function is the open verification question; but the *aspiration* to bridge is itself a notable [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] data point — either as an emerging coherence mechanism (if NCAIC is real/credible) or as evidence that the *absence* of such a mechanism is widely recognised as a gap (if NCAIC is a private/proposed body filling a perceived vacuum).

### Governance Debt
The framework itself, if implemented as proposed, would represent a **significant net-new compliance layer** on top of (not replacing) the existing DPDP/CERT-In/sectoral-regulator obligations — AIREC, CARO, AI System Inventory, AIBOM, AIPIA, evaluation gates, and ISO 42001 certification are all **additional** structures alongside DPDP SDF obligations (MeitY_4), RBI cloud/outsourcing governance (RBI_6), and SEBI AI/ML reporting (SEBI_9-11). This is a further [[05_Concepts/05_Concepts_Signature/Governance_Debt]] consideration: even a well-designed horizontal framework, if layered onto rather than integrated with existing sectoral obligations, could compound rather than resolve the parallelism-driven compliance burden — a point worth raising in any policy-recommendation output building on this corpus.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (explicitly cross-referenced — DPDP/CERT-In alignment), [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]] (content provenance/C2PA, deepfake crisis management — strong thematic overlap), [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] (cloud/IAM controls parallel to "Security by Design" principle), [[07_Institutions/Corpus/SEBI/SEBI_9]]/[[07_Institutions/Corpus/SEBI/SEBI_10]]/[[07_Institutions/Corpus/SEBI/SEBI_11]] (BFSI AI/ML reporting — direct sectoral blueprint overlap), [[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025]] (data governance/Board-policy template parallel)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (explicit cross-regulator bridging attempt), [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] (NCAIC as proposed coordination body), [[05_Concepts/05_Concepts_Signature/Governance_Debt]] (net-new compliance layer), [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] (comprehensive AI lifecycle governance — central reference document), [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Transparency]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Related frameworks:** **Strong candidate for a new `06_Frameworks/NCAIC_AI_Governance_Framework_2025.md` synthesis node** given the document's comprehensive, standalone-framework character — pending institutional-status verification
**Related projects:** [[02_Projects/P1...]] (AI Governance SLR — central comparative reference), [[02_Projects/P3_BFSI_JEIM]] (BFSI sectoral blueprint), [[08_Methods/fsQCA]] (configurational template candidate)
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] (S3/S4/S6 — high priority)
**Related consulting:** **AEGIS_OS** — the AIREC/CARO governance model, AI System Inventory, AIBOM, and AIPIA templates are directly reusable as a consulting methodology/toolkit reference if AEGIS_OS engagements involve AI governance maturity assessments for Indian enterprise clients, regardless of NCAIC's institutional status (the *content* is reusable even if the *provenance* is uncertain).

---

## Coding Status

- **P3 NVivo:** High priority — primary reference for "comprehensive framework" comparator class; flag institutional-status caveat in any coding memo
- **Wiki intake status:** Pending — HIGH priority for S3/S4/S6; institutional-status verification should be resolved or explicitly caveated before wiki publication

---

## Log

- 2026-06-15: Corpus node created. Batch 7. Cowork session. **Filed under new provisional institution "NCAIC" rather than the originally-planned NITI_8** due to explicit issuing-body mismatch discovered on full-text reading — flagged as the batch's highest-priority institutional-identity verification item. NITI_8 numbering remains unused/available pending a genuine NITI Aayog document.
