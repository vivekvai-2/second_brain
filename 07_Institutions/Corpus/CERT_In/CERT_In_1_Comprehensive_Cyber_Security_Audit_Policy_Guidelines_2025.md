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

# CERT_In_1 — Comprehensive Cyber Security Audit Policy Guidelines

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025.md`
**Institution:** [[07_Institutions/CERT_IN]] ⚠ VERIFY BEFORE PUBLISHING — first CERT-In corpus node; new institution folder `07_Institutions/Corpus/CERT_In/` created this batch. Confirm whether `07_Institutions/CERT_In.md` institution file exists or needs creation as part of the indexing pass.
**Issuing body:** Indian Computer Emergency Response Team (CERT-In), Ministry of Electronics and Information Technology, Government of India
**Document date:** Version 1.0, 25.07.2025
**Pages:** 69
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/Cybersecurity_Governance]]

---

## Instrument Identity

**Full title:** Comprehensive Cyber Security Audit Policy Guidelines, Version 1.0
**Type:** Statutory guidelines issued by CERT-In in exercise of its powers under Section 70B of the Information Technology Act, 2000 — explicitly stated to be "binding on all CERT-In empanelled auditing organizations and auditee entities covered under the relevant provisions" (Section 2, "Authority for Issuance of Guidelines")
**Target entities:** (i) CERT-In empanelled Information Security Auditing Organizations; (ii) Auditee Organizations — public and private sector entities subject to or seeking cyber security audits
**Legal basis:** Section 70B(1) IT Act 2000 (CERT-In's statutory establishment, notified 27.10.2009); Section 70B(4)(e) (CERT-In's function to "issue guidelines, advisories, vulnerability notes and whitepapers relating to information security practices, procedures, prevention, response and reporting of cyber incidents"); Section 70B(5) read with the Information Technology (The Indian Computer Emergency Response Team and Manner of performing functions & duties) Rules, 2013, specifically Rule 9 (prescribing "Information security assurance and audit" as a CERT-In activity); Section 70B(6)/(7) (CERT-In's power to call for information/give directions, with punitive consequences for non-compliance).
**Companion documents:** References multiple companion CERT-In policy documents published on its website and incorporated by reference: "Policy Guidelines for Handling Audit related Data," "Cyber Security Audit Baseline Requirements" (forms the basis for audit programs), "Guidelines for Secure Application Design, Development, Implementation & Operations," "Guidelines for applying for Empanelment," the NDA template, the "Deter and Punish Framework" (RoD_Interaction_session_website.pdf), and "Directions under sub-section (6) of section 70B... for Safe & Trusted Internet" dated 28 April 2022 (the well-known "CERT-In Directions 2022" — 6-hour incident reporting). Cross-references the "Guidelines on Mandatory Features of Cybersecurity Architecture to be Ensured in all Ministries/Departments" (282-control-point checklist) issued by MeitY's Cyber Security Division.

---

## Analytical Classification

**Wiki section:** S5 (Data, Privacy & Security) / S6 (Implementation & Governance Artifacts) / S4 (Agentic AI Governance — AI System Audits as a defined audit category)
**Jurisdiction:** India
**Confidence:** HIGH — primary CERT-In document, version-controlled (v1.0, 25.07.2025), with explicit statutory authority citation (Section 70B IT Act 2000)
**AI explicit:** YES — Section 6 ("Scope of Engagements Covered") explicitly enumerates "Artificial Intelligence (AI) System Audits" (item xxiii: "Evaluation of AI systems for security, ethical alignment, transparency, data integrity, and resilience to adversarial manipulation") and "AIBOM (Artificial Intelligence Bill of Materials) Auditing" (item xxvi) as defined, in-scope audit types — making this the corpus's first instrument to establish **AI system audits as a named category within India's binding cyber-audit regime**.
**Tier classification:** Tier A — explicitly names AI system audits and AIBOM auditing as defined audit categories within a binding national cyber-audit framework, with direct relevance to assurance/certification regimes (cf. ISO/IEC 42001 referenced in NCAIC_1)
**AI Governance Wiki relevance:** VERY HIGH — this is the corpus's clearest instance of an **existing, binding, statutorily-grounded Indian regulatory instrument incorporating AI-specific audit categories** into its scope — distinct from NCAIC_1 (a proposed/unverified framework) and from MeitY_4/MeitY_5 (algorithmic-governance provisions embedded in data-protection/intermediary instruments). CERT-In_1 demonstrates that AI system audits are *already* part of India's operative cyber-audit ecosystem, at least as a defined scope category, even absent a horizontal AI law.

---

## Substantive Content

### Statutory Authority and Binding Character
Section 2 ("Authority for Issuance of Guidelines") reproduces the full chain of statutory authority: Section 70B(1) (CERT-In's establishment as the national agency), Section 70B(4) (CERT-In's six enumerated functions, including issuing binding guidelines), Section 70B(5) read with the 2013 CERT-In Rules (Rule 9 specifically assigning "Information security assurance and audit" to CERT-In), and Section 70B(6)/(7) (CERT-In's information-calling/direction powers with punitive backing). The guidelines conclude this chain with "Now, therefore, these guidelines are herein issued by CERT-In in discharge of its statutory authority... which are binding on all CERT-In empanelled auditing organizations and auditee entities covered under the relevant provisions." This is a notably explicit and self-contained statutory-authority recitation — more elaborate than the authority statements in MeitY_4 (DPDP Rules) or MeitY_5/MeitY_6, and establishes CERT-In_1 as binding subordinate guidance with direct enforcement teeth (Section 70B(7) penal consequences for non-compliance with CERT-In directions).

### Scope of Engagements — AI, AIBOM, QBOM, and Emerging-Technology Audit Categories (Section 6)
Section 6 enumerates 26 categories of cyber security audits/assessments falling within scope, "including but not limited to" the list. Of direct AI-governance relevance: item (xxiii) **"Artificial Intelligence (AI) System Audits"** — defined as "Evaluation of AI systems for security, ethical alignment, transparency, data integrity, and resilience to adversarial manipulation" — and item (xxvi) **"SBOM, QBOM, and AIBOM Auditing"** — evaluation of Software/Quantum/AI Bills of Materials "to ensure transparency, traceability, and integrity of components used in software, quantum computing, and AI systems," focused on "identifying known vulnerabilities, licensing issues, and supply chain risks associated with open-source and third-party components." ⚠ VERIFY BEFORE PUBLISHING — while these categories are *named* and *defined*, the guidelines do not specify a mandatory AI-audit methodology, AI-specific standards reference, or AI-audit frequency distinct from the general annual cyber-audit requirement (Section 6 preamble: "comprehensive audit covering all aspects of their ICT systems at least once a year"). The inclusion appears to be **scope-expansion by definitional enumeration** rather than a fully operationalised AI-audit regime — i.e., AI systems are *brought within* the existing audit framework's net, but no AI-specific audit standard (analogous to OWASP for web apps) is mandated.

### CVSS/EPSS Mandatory Dual-Scoring Requirement (Sections 5, 16.2)
A notable methodological mandate: "Auditors are required to implement both CVSS and Exploit Prediction Scoring System (EPSS) frameworks within their audit reports" — vulnerabilities must be scored for severity (CVSS, 0.0–10.0) *and* supplemented with EPSS (0–100% real-world exploitation probability), with every observation mapped to CWE and CVE identifiers. This dual-scoring requirement is a precise, internationally-aligned (CVSS/EPSS/CWE/CVE are all US-NIST/MITRE/FIRST-maintained standards) technical mandate — a strong example of India's cyber-audit regime incorporating global technical standards by direct reference rather than developing India-specific scoring systems, in contrast to NCAIC_1's claim of "90%+ ISO 42001 alignment" (a framework-level rather than scoring-level alignment).

### Independence and Anti-Conflict-of-Interest Provisions (Section 7)
Section 7(i) ("Independence") contains an unusually explicit anti-conflict provision: "payments to the auditing organization should not be contingent upon the outcome of the audit—whether favorable or unfavorable—nor should they be tied to the submission or approval of any closure reports," with escalation to CERT-In if the auditee applies "pressure tactics, coercion, or undue influence." This directly addresses a structural conflict-of-interest risk (outcome-contingent audit fees) that is rarely codified explicitly in audit-governance instruments — a notable **governance-design innovation** worth flagging for any comparative analysis of audit-independence regimes (cf. statutory-auditor independence rules in company law/SEBI LODR contexts, which Vivek's secondary BFSI/legal interests may find relevant).

### Mandatory Three-Tier Sign-Off and Maker-Checker Structure (Sections 9.5, 10.3, 16.1)
Audit reports must be signed by (1) the Auditors who conducted the audit, (2) a designated mid-management Reviewer "who is not part of audit team" (independent review), and (3) the Head of the Auditing Organization (Director/Partner/CEO) — with the audit certificate additionally requiring both Lead Auditor and Head-of-Organization signatures. Section 15.2.5(iii) further mandates a "maker-checker concept" with "a separate verification team (checker)" reviewing the audit team's ("maker") work. This three/four-layer sign-off and maker-checker structure is one of the corpus's most elaborate **internal-control-over-audit-quality** mechanisms — directly analogous to financial-audit quality-control structures (engagement partner/EQCR review in statutory audit), and a strong ADICO/Institutional Grammar candidate (explicit Attributes: Auditor/Reviewer/Head of Organization; Deontic: "shall be signed only by"; Conditions: role-based exclusion — Reviewer "not part of audit team").

### Auditee Responsibility — Top Management Accountability and Risk Ownership (Section 9)
Section 9.1–9.2 places ultimate accountability with the auditee's top management: the "responsibility for maintaining an efficient and robust cyber security posture ultimately rests with the auditee organization, not the auditor"; risk-treatment decisions (retain/avoid/transfer/reduce) and exceptions to findings "must be authorized & accepted by the head of the auditee organization." Section 9.6(i) further mandates that the *entire* audit process — scope definition, auditor selection, infrastructure access, observation closure — "must be carried out by the owner of the information infrastructure" and "must not be delegated," except where mandated by a Regulator/Government. This non-delegation principle is structurally significant for any organization (including BFSI entities already subject to RBI_6/SEBI/IRDAI_1 audit-adjacent obligations) attempting to outsource cyber-audit governance — it establishes a **non-delegable accountability floor** analogous to the Board-approval requirements seen across MeitY_4, RBI_6, and IRDAI_1.

### Data Localisation and Secure Handling of Audit Data (Section 10.3)
Auditee-related audit data "should be stored only on systems located in India," kept encrypted on auditor laptops during engagement, wiped with forensic-irretrievability certification post-engagement, and retained for a default **1 year** absent a specific contractual/regulatory period. Cross-border disclosure of auditee data is prohibited "unless specifically authorized in writing by the auditee organization" (Section 16.6) — though disclosures mandated by Indian law/regulators (including CERT-In itself) require no additional consent. This is **another instance of India's recurring sector-by-sector data-localisation pattern** (cf. IRDAI_1's "all data... in Indian data centres" claim and DPDP Rule 13(4) SDF-localisation), here applied specifically to *audit-related data* rather than the auditee's primary business data — a narrower, audit-process-specific localisation requirement.

### Empanelment, Quality Control, and Graded Deter-and-Punish Framework (Sections 11, 19)
CERT-In maintains an empanelment register of auditing organizations with published "snapshot information" (skills, manpower, audit history by sector/category). Section 19 sets out a **four-tier graded enforcement ladder** for auditing-organization non-compliance: (1) watch-list placement with warning and written corrective-action commitment, (2) suspension (revocable on satisfactory corrective action), (3) withdrawal of empanelment per General Financial Rules (GFR) and a named Department of Expenditure Office Memorandum (O.M. F.1/20/2018-PPD dated 2 Nov 2021), and (4) penal/legal action for breach of trust, digital break-in, or damage to auditee infrastructure. ⚠ VERIFY BEFORE PUBLISHING — the indicative-parameters table (e.g., "First adverse report includes missing of maximum 2 vulnerabilities" as a Grade-1 trigger) provides unusually granular, almost rubric-like enforcement criteria; confirm whether this level of granularity is typical of CERT-In's other empanelment-governance documents or is a notable innovation specific to this v1.0 guideline.

---

## Analytical Significance for PRIS Research

### For P1 (AI Governance SLR) — AI Audit as an Operative (vs. Proposed) Category
CERT_In_1 provides the corpus's clearest evidence that "AI System Audits" and "AIBOM Auditing" are **already named, binding scope categories** within an operative Indian cyber-audit regime grounded in explicit statutory authority (Section 70B IT Act) — a materially different evidentiary status from NCAIC_1's proposed AIREC/CARO/AIBOM framework (whose issuing body's institutional status is itself ⚠VERIFY-flagged). For P1's comparative regulatory-configuration analysis, CERT_In_1 and NCAIC_1 form an instructive **operative-vs-proposed pairing** on the same substantive concept (AIBOM auditing, AI system evaluation): CERT-In's binding guideline establishes the *category* without prescribing AI-specific *methodology*, while NCAIC's proposal supplies a more elaborate *methodology* (evaluation gates, AIBOM content specification, ISO 42001 mapping) without confirmed *institutional authority*. A mature Indian AI-audit ecosystem would plausibly require CERT-In's binding categories to be filled in with NCAIC-style (or ISO 42001-aligned) methodological content — a "form without content / content without form" complementarity worth noting in any framework-gap analysis.

### For Regulatory Parallelism / Institutional Coherence
CERT_In_1 functions as the **horizontal technical-audit backbone** that several sectoral instruments explicitly or implicitly rely upon: RBI_6 (AIFI outsourcing — IT/cloud audits), SEBI's AI/ML reporting circulars, and the 282-control-point MeitY "Mandatory Features of Cybersecurity Architecture" checklist (referenced directly in Section 8(v)) all presuppose CERT-In-empanelled audit infrastructure. Unlike the MeitY_4/RBI_6/SEBI_9-11 "parallelism" pattern (independent, non-cross-referencing algorithmic-governance insertions), CERT-In_1 is explicitly **cross-referenced by name** within other instruments (e.g., MeitY_6's SOP references CERT-In's Sahyog Portal; the 282-point checklist is incorporated by reference here) — suggesting CERT-In occupies a more genuinely **horizontal/coordinating role** for cyber-audit infrastructure than any single sectoral regulator, even though no horizontal *AI* law exists. This nuances the Regulatory_Parallelism thesis: parallelism characterises *AI/algorithmic-specific* governance insertions, while *generic cyber-audit* infrastructure (CERT-In empanelment, CVSS/EPSS, audit methodology) is comparatively more horizontally coordinated — a useful scope qualification for any policy-recommendation output ("India's AI governance parallelism sits atop a more coherent generic cyber-audit substrate").

### Governance Capacity and Audit-Market Structure
The empanelment/snapshot/deter-and-punish architecture represents a mature, decades-refined (CERT-In established 2009, this is "Version 1.0" of a *consolidated* guideline implying prior less-formalised practice) regulatory-market-structuring mechanism — CERT-In does not itself audit; it certifies and polices a market of private auditing organizations. This "certify-and-police-the-market" model is a distinct [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] archetype, differing from DPDP's "stand up a new Board" model (MeitY_4) or NCAIC's "propose a new coordinating body" model (NCAIC_1) — a third institutional-design archetype for AI/cyber governance capacity-building worth adding to any typology developed for P1.

### Coordination / Parallelism Pattern
**Existing nodes:** [[07_Institutions/Corpus/MeitY/MeitY_6_SOP_NCII_Takedown_2025]] (Sahyog Portal/I4C cross-reference), [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] (IT/cloud outsourcing audit requirements presuppose CERT-In-empanelled auditors), [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] (AIBOM/evaluation-gate methodology — operative-vs-proposed pairing on AI audit).
**Pattern:** **Horizontal infrastructure underpinning vertical/sectoral instruments** — CERT-In_1 is the auditing infrastructure layer that RBI_6, SEBI circulars, and MeitY's 282-point checklist all build upon by reference, even as those instruments' *substantive* AI/algorithmic provisions remain parallel/uncoordinated. This is a distinct pattern from pure parallelism: **shared horizontal infrastructure + parallel vertical substantive obligations**.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] (AI System Audits/AIBOM — operative-vs-proposed pairing; also NCAIC_1 explicitly references CERT-In-aligned 6-hour incident reporting and IndiaAI Safety Institute red-teaming), [[07_Institutions/Corpus/MeitY/MeitY_6_SOP_NCII_Takedown_2025]] (Sahyog Portal/I4C — CERT-In coordination role), [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] (IT outsourcing audit presupposes CERT-In empanelment), [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (breach-notification 72-hour timeline — compare to CERT-In Directions 2022's 6-hour reporting referenced here)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] (CERT-In as horizontal audit-infrastructure coordinator), [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (scope-qualification — horizontal infrastructure vs. parallel substantive AI provisions), [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] (certify-and-police-the-market archetype), [[05_Concepts/05_Concepts_Standard/Accountability]] (non-delegable auditee accountability; maker-checker; three-tier sign-off), [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] (AI System Audits/AIBOM as named categories)
**Related frameworks:** Strong candidate reference point for a future "India Cyber Audit Infrastructure" framework synthesis node, and for cross-referencing against NCAIC_1's AIBOM/evaluation-gate proposals
**Related projects:** [[02_Projects/P1_SLR_RG]] (AI Governance SLR — operative vs. proposed AI-audit categories), [[02_Projects/P3_BFSI_JEIM]]/[[02_Projects/P4_Doctrinal_IJLIT]] (BFSI entities' cyber-audit obligations under CERT-In empanelment intersect with RBI/SEBI/IRDAI sectoral audit requirements), [[08_Methods/Institutional_Grammar_IG2]] (three-tier sign-off / maker-checker — strong ADICO candidate), [[08_Methods/fsQCA]] (CERT-In as a "horizontal infrastructure" configurational variable distinct from "sectoral substantive AI provision" variables)
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] (S4/S5/S6 — first CERT-In entry, AI System Audits/AIBOM categories)
**Related consulting:** **AEGIS_OS** — directly relevant; CERT-In empanelment requirements, the independence/anti-conflict provisions (Section 7), and the three-tier sign-off/maker-checker structure are highly relevant if AEGIS_OS engagements involve cyber-audit governance advisory for Indian enterprise/BFSI/Defence clients, or if AEGIS_OS itself operates as (or alongside) a CERT-In-empanelled auditing organization.

---

## Coding Status

- **P3 NVivo:** High priority — first CERT-In entry; AI System Audits/AIBOM categories are direct cross-regulator AI-governance evidence
- **Wiki intake status:** Pending — HIGH priority for S4/S5/S6, opens new CERT-In institutional section

---

## Log

- 2026-06-15: Corpus node created. Batch 7. Cowork session. Document 8 of 9. First CERT-In corpus entry — new institution folder `07_Institutions/Corpus/CERT_In/` created. Source: 69-page "Comprehensive Cyber Security Audit Policy Guidelines," Version 1.0, 25.07.2025.
