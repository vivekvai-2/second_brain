---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S1
  - section/S2
  - tier/high
  - project/p1
  - project/p3
  - project/fsqca
  - engine/phd
  - engine/linkedin
---

# IAPP: AIGP Body of Knowledge and Exam Blueprint — Version 2.1 (February 2026)

**Node ID:** F055
**Type:** Wiki Intake Note (Format B)
**Wiki Section:** S1 (Governance Fundamentals) / S2 (India Regulatory — comparator)
**Status:** Active
**Tier:** High
**Last Updated:** 2026-07-14 (Batch 15 continuation)

---

## Source

**Full Citation (APA):** International Association of Privacy Professionals. (2026). *AIGP body of knowledge and exam blueprint — Version 2.1.* IAPP (effective 2 February 2026).
**Document Type:** Professional certification body of knowledge / competency framework
**Certification:** AI Governance Professional (AIGP)
**Issuing Institution:** International Association of Privacy Professionals (IAPP)
**Version:** 2.1
**Batch:** 15 (continuation) | **Batch marker:** ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕
**Source corpus:** Policy Dump Future

---

## Summary

The IAPP AIGP Body of Knowledge (BoK) v2.1 defines the competency framework for the Certified AI Governance Professional (AIGP) credential — IAPP's primary AI governance certification. It specifies four governance domains with associated task statements, knowledge areas, and exam weightings, and functions simultaneously as a professional competency standard and an implicit consensus view of what "AI governance" comprises as a practitioner discipline. Version 2.1 (effective February 2026) updates the prior BoK to expand coverage of agentic AI, generative AI-specific governance, and recent regulatory developments (EU AI Act implementation, emerging national AI strategies). The BoK is significant for PRIS research purposes primarily as a *mapping instrument* — it provides a consensus practitioner-level taxonomy of AI governance competencies that can be used to evaluate the coverage and gaps of research-focused AI governance frameworks.

---

## Four-Domain Competency Architecture

### Domain I: Foundations of AI Governance (Exam Weighting: 20%)

Core competencies:
- AI system lifecycle understanding (data collection → training → deployment → monitoring → decommissioning)
- AI risk types: technical risks (bias, hallucination, robustness), operational risks, legal/compliance risks, reputational risks
- AI ethics principles and frameworks: fairness, transparency, accountability, privacy, human oversight
- Governance structures for AI: roles and responsibilities (CAIO, AI Ethics Committee, AI Risk Owner, AI product teams)
- Difference between traditional software governance and AI governance (non-determinism, emergent behaviour, continuous learning)

### Domain II: Laws, Standards, and Frameworks (Exam Weighting: 30%)

Core competencies:
- EU AI Act: risk tiers, Annex III high-risk categories, conformity assessment, notified bodies, prohibited practices
- US regulatory landscape: NIST AI RMF, FTC AI guidance, sector-specific (FDA, CFPB, EEOC), White House EO 14110 status
- Global frameworks: ISO/IEC 42001, OECD AI Principles, G7 Hiroshima Process, Singapore FEAT/MAS guidelines
- Data protection intersection: GDPR Art. 22 (automated decision-making), CCPA, India DPDP Act (brief reference)
- Standards bodies: ISO/IEC JTC1/SC42, IEEE, NIST, BSI, CEN/CENELEC
- Sector-specific AI regulation: financial services (DORA, MAS Guidelines), healthcare (FDA SaMD), employment (EU AI Act Annex III cat. 4)

### Domain III: AI Development Governance (Exam Weighting: 25%)

Core competencies:
- Data governance for AI: training data quality, bias testing in datasets, data lineage, synthetic data governance
- Model development standards: documentation (Model Cards, Datasheets for Datasets), version control, reproducibility
- Safety and alignment techniques: RLHF, Constitutional AI, adversarial testing, red-teaming
- Third-party AI and foundation model governance: vendor risk assessment, API usage policies, model cards review
- GenAI-specific development risks: hallucination, copyright/IP in training data, dual-use capability risks

### Domain IV: AI Deployment Governance (Exam Weighting: 25%)

Core competencies:
- Algorithmic impact assessment and fundamental rights impact assessment (FRIA) — methodology and applicability
- Human oversight mechanisms: human-in-the-loop, human-on-the-loop, meaningful human control
- Incident management for AI: incident definition, response protocols, post-incident review
- AI auditing and conformity assessment: third-party audits, self-assessment, regulatory audit requirements
- Agentic AI governance: autonomous action risk, tool-use governance, multi-agent system oversight
- Transparency and explainability obligations: right to explanation, recourse mechanisms, contestability

---

## Research Significance

### As a Competency Mapping Instrument

The AIGP BoK's value for PRIS research is not primarily its content (which synthesises rather than originates) but its function as a *practitioner consensus document*. The BoK reveals what the AI governance profession, as of February 2026, collectively considers the essential knowledge base for AI governance practice. This provides:
1. A reference taxonomy for evaluating completeness of regulatory frameworks (do national AI governance frameworks cover all four domains?)
2. A competency gap indicator for institutional capacity assessment (jurisdictions without AIGP-trained practitioners face Domain I-IV capacity deficits)
3. A comparative lens for evaluating Indian AI governance capacity: which AIGP competency domains are covered by India's regulatory infrastructure?

### Indian AI Governance Competency Gap Assessment

| AIGP Domain | India Coverage Assessment |
|-------------|--------------------------|
| **Domain I (Foundations)** | Partial — MeitY AI Advisory (2024) covers principles; NASSCOM AI governance materials; no formal practitioner competency standard |
| **Domain II (Laws/Standards)** | Partial — DPDP Act 2023, IT Act, sector-specific (RBI, SEBI, IRDAI); no comprehensive AI-specific legislation equivalent to EU AI Act |
| **Domain III (Development Governance)** | Minimal — no mandatory model documentation standards; no AI dataset governance regulation; CERT-In guidelines address security but not AI development |
| **Domain IV (Deployment Governance)** | Minimal — no mandatory AIA/FRIA equivalent; no AIIRS; no formal AI audit requirement; agentic AI governance absent |

The Domain III and IV deficits are the most actionable research findings.

---

## Connections to Research

**[[P1_SLR_RG]]:** S1 (governance fundamentals) — AIGP BoK provides the practitioner-consensus taxonomy against which academic AI governance frameworks can be mapped; useful for SLR scoping and gap analysis.

**[[fsQCA_Thesis_Chapter]]:** Relevant to **SR condition** (Structural Readiness) — presence/absence of AI governance professional certification ecosystem is a proxy for structural readiness; AIGP certification availability and uptake is an SR indicator.

**[[P3_BFSI_JEIM]]:** Domain IV competency gaps (deployment governance, FRIA, AIIRS) directly correspond to the governance gaps identified in the Indian e-governance context.

**Concept links:**
- [[Governance_Capacity]] — the AIGP BoK defines what governance capacity means at the practitioner level; a jurisdiction whose regulatory and institutional staff cannot pass a Domain I-IV competency assessment is governance-capacity constrained
- [[Accountability]] — Domain IV's emphasis on audit, conformity assessment, and incident management are accountability instantiations
- [[Transparency]] — Domain IV's explainability and transparency obligations module is a transparency competency domain
- [[Agentic_AI_Governance]] — v2.1's expanded agentic AI coverage (Domain IV) reflects the profession's recognition of agentic AI as a distinct governance challenge; minimal footprint, tool-use governance, multi-agent oversight are AIGP competency areas

**Related nodes:**
- [[04_Knowledge_Products/Wiki_Intake/FRA_EU_Assessing_High_Risk_AI_Fundamental_Rights|F053]] (FRA FRIA) — Domain IV assessment/FRIA module in AIGP BoK maps directly to FRA's FRIA guide; practitioner competency grounded in FRA methodology
- [[04_Knowledge_Products/Wiki_Intake/F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations|F041]] (AEF-1) — Domain III development governance (pre-deployment testing, red-teaming) aligns with AEF-1's minimum operating conditions; AIGP BoK is the competency layer, AEF-1 is the technical standard layer
- [[04_Knowledge_Products/Wiki_Intake/RAND_GovAI_AI_Incident_Reporting_Institutional_Design|F051]] (RAND/GovAI AIIRS) — Domain IV incident management module aligns with Wei/Heim AIIRS framework; AIGP practitioners expected to understand AIIRS design principles

---

## VERIFY Flags

*(No critical VERIFY flags for this node — IAPP identity and BoK version 2.1 effective date confirmed from document cover. IAPP AIGP is an established professional credential; no uncertain institutional claims.)*

---

*Node written: 2026-07-14 | Batch 15 continuation (rescued from staging; number unchanged as F055) | PRIS v2.2*
