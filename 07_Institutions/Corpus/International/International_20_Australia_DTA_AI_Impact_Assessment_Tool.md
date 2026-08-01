---
type: Corpus Node
tags:
  - type/corpus-node
  - status/active
  - series/format-a
  - section/S3
  - section/S1
  - tier/high
  - project/p1
  - project/p3
  - project/p4
  - project/fsqca
  - institution/DTA
  - jurisdiction/Australia
  - engine/phd
---

# International_20 — Australian Government DTA: AI Impact Assessment Tool v1.0

**Type:** Corpus Node (Format A)
**Vault path:** `07_Institutions/Corpus/International/International_20_Australia_DTA_AI_Impact_Assessment_Tool.md`
**Institution:** Digital Transformation Agency (DTA), Australian Government
**Issuing body:** Digital Transformation Agency (DTA)
**Document date:** 01 December 2025 (Version 1.0)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/Systemic_Regulatory_Governance]]
**Batch:** 15 (continuation) | **Batch marker:** ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕
**Source corpus:** Policy Dump Future

---

## Instrument Identity

**Full title:** Artificial Intelligence Impact Assessment Tool
**Version:** 1.0
**Type:** Mandatory Government Tool / Policy Instrument
**Applicability:** All Australian Government entities deploying AI systems
**Alignment:** Australian Government Voluntary AI Safety Standard; Australian AI Ethics Framework (8 principles)
**Note:** Two files in source corpus (`AI_Impact_Assessment_Tool_1765037667.pdf` and `AI_impact_assessment_and_guidance_DTA_1764755745.pdf`) contain the same DTA document; only one node is created.

---

## Scope and Purpose

The Australian Government AI Impact Assessment (AIIA) Tool establishes a structured pre-deployment assessment process for AI systems used by Commonwealth entities. It is designed to ensure that government AI deployments comply with the AI Ethics Principles, address risks to individuals and communities, and maintain public trust. The tool is positioned as mandatory for all Australian Government agencies when acquiring, developing, or significantly modifying AI systems used in administrative decision-making or service delivery contexts.

The AIIA Tool operates within Australia's broader AI governance architecture, which includes the Voluntary AI Safety Standard (for high-risk AI; released separately), the National AI Strategy, and the mandatory guardrails issued by the Department of Industry, Science and Resources. It is the operational implementation instrument for the government-as-deployer dimension of Australian AI governance — distinct from, and complementary to, Australia's regulatory oversight of private sector AI deployments.

**#185 — RESOLVED (2026-07-31, Perplexity Deep Research).** (1) **Mandatory status confirmed, High confidence:** the DTA's "Policy for the Responsible Use of AI in Government," Version 2.0, took effect 15 December 2025 and is explicitly a **mandatory whole-of-government policy** for non-corporate Commonwealth entities — not departmental guidance. (2) **Deadline confirmed, High confidence:** the AI Impact Assessment requirement for in-scope use cases applies by **15 December 2026**, matching this node's original figure exactly. A separate, earlier mandatory milestone (AI use-case register with accountable owner) took effect 15 June 2026, with remaining requirements phased through December 2026. (3) **No later Tool version found, Medium confidence:** sources describe "Policy v2.0" but do not evidence a distinct "Tool v2.0" versioning scheme beyond the v1.0 referenced in this node — the policy and the tool appear to be versioned somewhat independently; worth a light re-check in a future session rather than treated as fully closed.

---

## Framework Architecture

### Twelve-Section Assessment Structure

The tool is organised as a sequential 12-section assessment workbook, designed to be completed by the responsible agency official prior to deployment (or as part of procurement for externally developed AI):

| Section | Assessment Domain | Key Questions |
|---------|------------------|---------------|
| **S1: System Information** | Basic identification — system name, purpose, deploying agency, responsible official | What does this system do? Who is accountable? |
| **S2: Decision Context** | Is AI involved in administrative decision-making? Degree of human oversight in the decision loop? | Fully automated vs. human-in-the-loop vs. human-on-the-loop |
| **S3: Inherent Risk — Individual Impact** | Potential harm to individuals from incorrect/biased decisions | False positive/negative consequences; severity of harm |
| **S4: Inherent Risk — Community Impact** | Systemic or population-level effects | Disproportionate impacts on vulnerable groups |
| **S5: Inherent Risk — Safety** | Physical safety implications | Deployment in safety-critical contexts |
| **S6: Inherent Risk — Privacy** | Personal information handling | Privacy Act 1988 compliance; data minimisation |
| **S7: Inherent Risk — Security** | Cybersecurity risk | Adversarial manipulation; model poisoning |
| **S8: Inherent Risk — Transparency** | Explainability of AI outputs | Ability to explain decisions to affected individuals |
| **S9: Inherent Risk — Reliability** | System accuracy, consistency, and performance degradation | Testing requirements; monitoring obligations |
| **S10: Inherent Risk — Accountability** | Governance and responsibility chain | Who is accountable when AI causes harm? |
| **S11: Cumulative Risk Assessment** | Aggregated risk rating (High/Medium/Low) across S3–S10 | Composite risk score determines required mitigations |
| **S12: Mitigation and Controls** | Required actions for each risk dimension identified | Specific controls mapped to identified risks |

### Risk Rating and Decision Logic

The AIIA Tool generates a cumulative risk rating of High, Medium, or Low based on scores across S3–S10:
- **High risk:** Mandatory additional approval (SES Band 2 minimum); independent expert review required; AIIA to be published proactively
- **Medium risk:** Agency head or SES Band 1 approval; AIIA retained on record; public disclosure on request
- **Low risk:** Responsible official approval; AIIA retained on record; streamlined assessment acceptable

### Integration with Australian AI Ethics Framework

The tool explicitly maps each section to one or more of the 8 Australian AI Ethics Principles:
1. Human, societal and environmental wellbeing
2. Human-centred values
3. Fairness
4. Privacy protection and security
5. Reliability and safety
6. Transparency and explainability
7. Contestability
8. Accountability

Each principle has associated assessment questions, enabling agencies to demonstrate ethics compliance as part of the AIIA process.

---

## Regulatory Significance

### Government-as-Deployer Model

The AIIA Tool represents a "government-as-deployer" governance model — where the government disciplines its own AI use through mandatory internal processes rather than through external legislation. This contrasts with:
- **EU model (FRIA / F053):** Mandatory pre-deployment fundamental rights assessment for all Annex III deployers, including public bodies; externally enforceable
- **India (no equivalent):** No mandatory pre-deployment AI impact assessment for government AI systems as of July 2026; DPDP Act DPIA requirement under draft Rules is narrow (data processing focus) and not yet in force

The Australian AIIA Tool occupies a middle position: formally mandatory for Commonwealth entities, but enforcement is through internal APS governance rather than external regulatory sanction.

### Comparison with EU FRIA (F053)

| Dimension | Australian AIIA | EU FRIA (FRA Guide, F053) |
|-----------|----------------|--------------------------|
| Legal basis | Mandatory APS policy / Finance guidance | EU AI Act Art. 9(9) (externally enforceable) |
| Scope | Government entities only | Public bodies + private deployers above threshold |
| Assessment domains | 8 risk categories + 8 ethics principles | 8 fundamental rights domains |
| Rights framework | Ethics principles (voluntary) | Fundamental rights (legally binding under EU Charter) |
| Sanction for non-compliance | Internal APS accountability; no external fine | EU AI Act penalties (up to 3% global turnover) |
| Public disclosure | Proactive for High risk; on-request for Medium | Varies by member state; FRA recommends proactive |

---

## Implications for Indian Governance

India's absence of an equivalent AIIA instrument for government AI deployments is a governance gap finding with direct research implications:
- **DPDP Act 2023:** Draft Rules propose DPIA for significant data fiduciaries; scope does not extend to all government AI systems
- **MeitY AI Advisory (March 2024):** Voluntary; no mandatory assessment process
- **Ministry-level AI policies:** No whole-of-government AI impact assessment mandate

The Australian AIIA Tool serves as a policy design template for any future Indian government AI impact assessment framework. The 12-section structure and cumulative risk rating methodology are transferable with adaptation.

---

## Connections

**[[P1_SLR_RG]]:** S3 (international frameworks) and S1 (governance fundamentals) — the Australian AIIA is a primary comparator for pre-deployment assessment frameworks; essential for the SLR's impact assessment literature section.

**[[fsQCA_Thesis_Chapter]]:** Central to **EA condition** (Evaluative Authority). Australia's mandatory government AIIA represents a high EA score for the government-as-deployer dimension; India's absence represents EA=0 for this dimension. The government-only scope means EA is partial even in the Australian case — private sector AI is separately governed.

**[[P3_BFSI_JEIM]]:** Australian model is the most directly relevant comparator for what an Indian government AI impact assessment could look like; the 12-section structure and ethics-principles mapping are directly applicable analysis frameworks.

**[[P4_Doctrinal_IJLIT]]:** Government-as-deployer model provides comparative institutional design for doctrinal analysis of AI accountability in public administration.

**Concept links:**
- [[Accountability]] — S10 (accountability section) and cumulative risk rating directly instantiate accountability; High risk systems require elevated approval chain
- [[Transparency]] — S8 (transparency/explainability) and proactive disclosure requirement for High risk AIIA are transparency mechanisms
- [[Governance_Capacity]] — mandatory AIIA requires agency capacity to complete assessment; DTA's guidance materials are capacity-building instruments
- [[Legitimacy]] — public disclosure of High risk AIIA assessments is a legitimacy mechanism; allows external scrutiny of government AI decisions
- [[Institutional_Coherence]] — AIIA integrates with Privacy Act DPIA, Cyber Security Framework, and Procurement Framework; IC question is whether agencies navigate multi-framework requirements coherently

**Related nodes:**
- [[04_Knowledge_Products/Wiki_Intake/FRA_EU_Assessing_High_Risk_AI_Fundamental_Rights|F053]] (FRA FRIA) — EU parallel; fundamental rights vs. ethics-principles framing comparison
- [[04_Knowledge_Products/Wiki_Intake/F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations|F041]] (AEF-1) — technical evaluation complement; AIIA is the governance assessment; AEF-1 is the technical safety evaluation standard; together they define full pre-deployment governance lifecycle
- [[04_Knowledge_Products/Wiki_Intake/MindForge_MAS_AI_Risk_Management_Executive_Handbook|F054]] (MindForge) — private sector complement; AIIA covers government; MindForge covers BFSI; together they illustrate the public/private split in AI governance
- [[07_Institutions/Corpus/International/International_16_Australia_National_AI_Plan_2025]] — sits within Australia's broader AI governance architecture; AIIA is the government-as-deployer operational instrument for the National AI Plan's framework posture

---

## VERIFY Flags

**#185 — RESOLVED (2026-07-31)** — see full resolution note above (this was a duplicate flag instance within this same file; both now closed together). **New follow-up item:** confirmed mandatory status strengthens (does not weaken) this node's "government-as-deployer" comparative framing in the Regulatory Significance section above — the "enforcement through internal APS governance rather than external regulatory sanction" distinction still holds; what's newly confirmed is that the internal mechanism is a hard mandatory policy, not discretionary departmental guidance.

---

*Node written: 2026-07-14 | Batch 15 continuation (rescued from staging; number unchanged as International_20) | PRIS v2.2*
