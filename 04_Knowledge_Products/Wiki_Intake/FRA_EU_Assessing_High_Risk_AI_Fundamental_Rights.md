---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S3
  - section/S2
  - tier/high
  - project/p1
  - project/p3
  - project/p4
  - project/fsqca
  - engine/phd
---

# FRA (EU Agency for Fundamental Rights): Assessing High-Risk AI — A Guide for Fundamental Rights Assessment (2025)

**Node ID:** F053
**Type:** Wiki Intake Note (Format B)
**Wiki Section:** S3 (International Regulatory Context) / S2 (India Regulatory — comparator)
**Status:** Active
**Tier:** High
**Last Updated:** 2026-07-14 (Batch 15 continuation)

---

## Source

**Full Citation (APA):** European Union Agency for Fundamental Rights. (2025). *Assessing high-risk artificial intelligence: A guide for fundamental rights assessment.* Publications Office of the European Union.
**Document Type:** Agency guidance / operational manual (FRIA implementation tool)
**Issuing Institution:** European Union Agency for Fundamental Rights (FRA)
**Batch:** 15 (continuation) | **Batch marker:** ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕
**Source corpus:** Policy Dump Future
**Note on corpus file:** File `_ENISA_Report_1765167800.pdf` in the source corpus is a mislabelled duplicate of this FRA document — it is NOT an ENISA report. Only the `ASSESSING_HIGH_RISK_ARTIFICIAL_INTELLIGENCE_1764937709.pdf` file is processed here.

---

## Summary

The FRA guide operationalises the Fundamental Rights Impact Assessment (FRIA) requirement under Article 9(9) and Annex III of the EU AI Act for deployers of high-risk AI systems. It provides a structured methodology — covering eight fundamental rights domains — for deployers to assess whether a specific AI system deployment creates risks to human dignity, non-discrimination, data protection, freedom of expression, right to an effective remedy, and related rights. The guide is addressed to EU deployers (public and private entities deploying high-risk AI systems listed in Annex III) and functions as a step-by-step operational guide rather than a legal commentary. It is the FRA's first AI Act implementation tool and positions fundamental rights assessment as a precondition for lawful deployment of high-risk AI, not a post-hoc compliance exercise.

---

## Key Findings and Framework

### FRIA Applicability and Trigger Conditions

The FRIA obligation under EU AI Act Article 9(9) is triggered for deployers (not providers/developers) of Annex III high-risk AI systems that:
1. Are public bodies, OR
2. Are private entities operating Annex III systems AND employ more than 250 persons or have annual turnover exceeding €50 million

This means SME deployers may be exempt from mandatory FRIA — a significant scope limitation the guide acknowledges.

### Eight-Domain Fundamental Rights Assessment Structure

| Rights Domain | Key Assessment Questions | Relevant EU AI Act Articles |
|---------------|-------------------------|-----------------------------|
| **Human dignity** | Does the system reduce persons to data points; does it dehumanise decision-making? | Art. 13 (transparency), Art. 14 (human oversight) |
| **Non-discrimination and equality** | Does the system produce differential outcomes by protected characteristic? | Art. 10 (data governance), Art. 9 (risk management) |
| **Privacy and data protection** | Does deployment comply with GDPR; is personal data used for AI training without lawful basis? | Art. 10(5), cross-reference GDPR Art. 35 DPIA |
| **Freedom of expression and information** | Does the system filter or suppress protected speech? | Particularly relevant for content moderation AI |
| **Right to effective remedy** | Can affected individuals challenge AI-assisted decisions? | Art. 26 (deployer obligations), Art. 85-86 (right to explanation) |
| **Right to a fair trial** | Does use in judicial/law enforcement contexts compromise procedural rights? | Annex III categories 6, 7 (law enforcement, justice) |
| **Children's rights** | Are specific protections in place for AI systems used in education or child-affecting contexts? | Annex III category 5 (education) |
| **Equality of access to public services** | Does AI-mediated public service delivery create or amplify access barriers? | Annex III category 5 (public administration) |

### Assessment Process — Six-Step Methodology

1. **Scoping:** Identify whether the AI system falls within Annex III categories and whether deployer threshold conditions are met
2. **System characterisation:** Document system functionality, data inputs, decision outputs, and human oversight mechanisms
3. **Stakeholder mapping:** Identify affected persons and groups; assess differential impact potential
4. **Rights impact analysis:** Systematic assessment against eight domains above
5. **Mitigation design:** For each identified risk, design mitigation — from technical controls (bias testing, data audits) to procedural safeguards (human review, override mechanisms)
6. **Documentation and review:** FRIA documentation to be maintained and updated when system or deployment context changes

### Relationship to DPIA (GDPR Art. 35) and AI Act Risk Management

The guide explicitly addresses the relationship between FRIA and GDPR Data Protection Impact Assessment (DPIA). FRA position: FRIA and DPIA are *complementary but distinct* — DPIA covers data processing risks; FRIA covers fundamental rights impacts beyond data. Where both are required, the guide recommends integrated assessment to avoid duplication. This has direct implications for deployers navigating simultaneous GDPR and AI Act compliance obligations.

---

## Relevance to Indian Context

India has no FRIA equivalent as of July 2026. The DPDP Act 2023 requires Data Protection Impact Assessment (DPIA equivalent) under draft DPDP Rules 2025 for significant data fiduciaries, but does not mandate a broader fundamental rights impact assessment for AI deployments. The FRA guide serves as:
- A **comparator framework** for evaluating India's AI impact assessment gap (relevant to P1 SLR S2 comparative analysis)
- A **methodology reference** for any future Indian AI Impact Assessment framework design
- A **contrast point** for fsQCA: EU's FRIA mechanism is a strong EA condition indicator; India's absence of FRIA is an EA gap

The Australian DTA AI Impact Assessment Tool (International_20) covers overlapping terrain from a different regulatory tradition — useful triangulation.

---

## Connections to Research

**[[P1_SLR_RG]]:** S3 (EU/international frameworks) and S2 (India regulatory comparators). Central document for FRIA literature in AI governance SLR.

**[[fsQCA_Thesis_Chapter]]:** Directly relevant to **EA condition** (Evaluative Authority) — FRIA is an EA mechanism; its mandatory status for Annex III deployers under EU AI Act represents a strong EA configuration. Comparison with jurisdictions lacking mandatory FRIA (India, ASEAN) generates configurational variation.

**[[P3_BFSI_JEIM]]:** Fundamental rights frame maps onto ethical AI governance; non-discrimination and dignity domains are core to ethical AI literature.

**Concept links:**
- [[Accountability]] — FRIA is a pre-deployment accountability mechanism; obligation to document and maintain assessment creates an accountability trail
- [[Transparency]] — right to effective remedy requires transparency about AI system operation; Art. 85-86 explanations are a transparency obligation
- [[Legitimacy]] — fundamental rights grounding of FRIA is a legitimacy-conferring mechanism; governance system predicated on rights is more legitimate than purely utilitarian risk frameworks
- [[Governance_Capacity]] — FRIA requires legal and technical capacity that smaller public sector deployers may lack; the guide's practical step-by-step format is a capacity-building intervention

**Related nodes:**
- [[04_Knowledge_Products/Wiki_Intake/International_20_Australia_DTA_AI_Impact_Assessment_Tool|International_20]] (Australian DTA AI Impact Assessment) — parallel instrument from common-law tradition; useful typological comparison
- [[04_Knowledge_Products/Wiki_Intake/RAND_GovAI_AI_Incident_Reporting_Institutional_Design|F051]] (RAND/GovAI Incident Reporting) — upstream-downstream relationship: FRIA is pre-deployment; AIIRS is post-deployment; together constitute a lifecycle governance architecture

---

## VERIFY Flags

*(No critical VERIFY flags for this node — FRA identity and EU AI Act Article references are confirmed from document face. Filing date and EU AI Act applicability timeline may shift post-August 2026 phased implementation — monitor.)*

---

*Node written: 2026-07-14 | Batch 15 continuation (rescued from staging; renumbered from staged F051 → F053) | PRIS v2.2*
