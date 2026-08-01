---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S5
  - tier/medium
  - project/p3
  - project/p1
---

# Microsoft Security (ATML): AI Security Risk Assessment — Best Practices and Guidance

**Node ID:** F044  
**Type:** Wiki Intake Note  
**Wiki Section:** S5 (Data, Privacy & Security)  
**Status:** Active  
**Tier:** Medium  
**Last Updated:** 2026-06-19  

---

## Source

**Full Citation (APA):** Microsoft Security. (c. 2021–2022). *AI security risk assessment: Best practices and guidance*. Microsoft Corporation. [⚠ VERIFY #167 — document is undated; date estimated from content references]  
**Document Type:** Technical white paper / practitioner guidance  
**Issuing Institution:** Microsoft Security — AI/ML Threat & Research (ATML)  
**Publication Date:** Undated — ⚠ VERIFY #167 (estimated c. 2021–2022 based on ISO 27001:2013 reference and absence of NIST AI RMF 2023 or EU AI Act references; document may be updated without explicit versioning)  
**URL / DOI:** Microsoft Security blog / ATML repository (⚠ VERIFY #167 for canonical URL)  

---

## Executive Summary

Microsoft's AI Security Risk Assessment framework adapts the ISO 27001:2013 information security risk management standard across the AI/ML system lifecycle, providing a structured methodology for identifying, assessing, and mitigating AI-specific security risks. The document is authored by Microsoft's ATML (AI, ML, and Threat Research) team and is intended for enterprise security architects and AI/ML practitioners deploying machine learning systems. A key empirical anchor is a survey finding that 25 of 28 (89%) businesses report lacking adequate tools to secure their ML systems — a figure that, while undated, remains relevant as a baseline for enterprise AI security maturity. The framework introduces a severity-likelihood attack matrix covering five AI-specific attack categories. This document predates the NIST AI RMF (2023) and EU AI Act (enacted 2024) and should be read as a practitioner reference rather than a current policy standard; its technical taxonomy retains analytical value independent of its publication date.

---

## Key Frameworks and Findings

### ISO 27001-Adapted AI Risk Assessment Lifecycle

Microsoft maps AI security risk assessment across four AI lifecycle phases:
1. **Data Collection & Preparation** — data poisoning, supply chain integrity
2. **Model Training & Development** — training data attacks, model extraction during development
3. **Model Deployment & Serving** — inference-time attacks, adversarial inputs
4. **Monitoring & Operations** — model drift exploitation, evasion at scale

### ML Attack Severity Matrix

Five AI-specific attack categories assessed across severity and likelihood dimensions (⚠ VERIFY #168 — matrix ratings are Microsoft's internal classification; independently verifiable against MITRE ATLAS and NIST AIRC):

| Attack Type | Description | Primary Phase |
|---|---|---|
| **Model Extraction** | Querying a model to reconstruct its parameters or architecture | Deployment |
| **Evasion** | Crafting adversarial inputs to cause misclassification at inference time | Deployment / Operations |
| **Model Inversion** | Reconstructing training data from model outputs | Training / Deployment |
| **Inference** | Extracting membership or property information about training data | Training / Deployment |
| **Data Poisoning** | Corrupting training data to degrade or manipulate model behaviour | Data Preparation / Training |

### Survey Finding

> "25 out of 28 businesses don't have the right tools in place to secure their machine learning systems."

This is the document's headline empirical finding. Source and methodology of the underlying survey are not disclosed in the document (⚠ VERIFY #168). The 89% figure is used to motivate the framework rather than as a primary research finding.

### Risk Assessment Components

The framework recommends a structured risk assessment covering:
- **Asset identification** — model artefacts, training data, inference endpoints, pipelines
- **Threat modelling** — adversary profiles, attack vectors (using the attack matrix above)
- **Vulnerability assessment** — model robustness testing, adversarial input probing
- **Impact analysis** — financial, reputational, regulatory, safety consequences of model compromise
- **Mitigation selection** — aligned to ISO 27001 control categories adapted for AI context

### Alignment with ISO 27001:2013

The framework explicitly extends ISO 27001:2013 Annex A controls to AI contexts. For practitioners using ISO 27001 as their primary security management standard (as most Indian BFSI entities do for IT security), this provides a direct bridge to AI-specific security risk management without requiring adoption of a new framework.

---

## India Relevance and Governance Gap Analysis

The ISO 27001 alignment is the primary India relevance vector. Indian BFSI entities subject to RBI CSCRF are required to maintain information security management systems aligned with ISO 27001 or equivalent standards. Microsoft's extension of ISO 27001 to AI/ML security provides a practitioner bridge that Indian BFSI entities could apply within their existing compliance frameworks.

**Specific governance gaps:**

1. **No India-specific AI security assessment standard:** RBI CSCRF (2024) addresses cybersecurity broadly; there is no RBI, SEBI, or MeitY instrument that specifically mandates ML attack surface assessment (model extraction, adversarial robustness, data poisoning) as a distinct security requirement for AI systems deployed in regulated financial services.

2. **Model security vs. data security bifurcation:** India's regulatory instruments protect *data* (DPDP Act 2023) and *IT systems* (IT Act 2000, CSCRF) but have no framework specifically addressing *model security* — the integrity, confidentiality, and availability of AI model artefacts themselves. Microsoft's taxonomy makes this distinction explicit.

3. **Survey baseline (89% lacking ML security tools):** If this figure is even approximately applicable to Indian enterprises, it implies acute vulnerability in the Indian BFSI AI deployment context, where AI adoption has accelerated post-2024 without commensurate security governance.

**Important caveat:** This document is estimated at c. 2021–2022 and predates NIST AI RMF (2023), EU AI Act (2024), and Microsoft's own subsequent AI security guidance (e.g., Responsible AI Impact Assessments, Copilot security guidance). For current practice guidance, F042 (IBM breach report), F043 (MIT mitigation taxonomy), and F047 (BAIR playbook) provide more current frameworks.

---

## Research Programme Applications

| Project | Application |
|---|---|
| P1 (SLR RG) | Technical AI security risk taxonomy — provides the security/adversarial dimension of the AI governance literature that is often absent from policy-focused SLRs; ISO 27001 bridge makes it relevant to institutional governance literature |
| P3 (BFSI JEIM) | ML attack taxonomy is directly relevant to BFSI AI security governance; Indian BFSI entities using ISO 27001 can use this framework to extend to AI-specific security; 89% lacking tools baseline is useful context for Indian BFSI maturity assessment |
| P4 (Doctrinal IJLIT) | Limited — technical reference providing attack surface taxonomy that can inform liability analysis for AI system compromise |
| fsQCA | Limited — document is undated and not a regulatory instrument; useful as technical context for EA/CC calibration but not as a direct condition anchor |

---

## Concept Links

- [[Accountability]] — ISO 27001-based risk assessment framework operationalises accountability through structured documentation of identified risks, owner assignments, and mitigation tracking; the AI lifecycle extension makes AI-specific accountability traceable
- [[Governance_Capacity]] — 89% lacking ML security tools directly measures (approximately) the governance capacity deficit in enterprise AI security; the framework itself is a capacity-building instrument
- [[Governance_Debt]] — Undated nature of the document (c. 2021–2022) and absence in current Indian regulatory instruments illustrate governance debt: a technically available mitigation framework has not been adopted into India's regulatory compliance architecture
- [[Transparency]] — Model inversion and inference attacks (two of five attack types) are threats *to* transparency — they can reconstruct training data or extract membership information; conversely, transparency requirements (audit logs, model documentation) are part of the ISO 27001 control set

---

## ⚠ VERIFY BEFORE PUBLISHING

- **V-B14-04 / #167 — Undated document — LOW.** The document carries no publication date, version number, or revision history. The c. 2021–2022 estimate is based on: (a) ISO 27001:2013 reference (not updated to ISO 27001:2022 edition); (b) absence of NIST AI RMF 2023, EU AI Act, or Microsoft Responsible AI Impact Assessment references; (c) ATML team nomenclature. Verify: search Microsoft Security blog and ATML GitHub for any dated version of this paper; note estimation basis in any citation.
- **V-B14-05 / #168 — Survey source and ML attack severity ratings — LOW.** The "25 of 28 businesses" finding is unsourced. The attack matrix severity ratings (e.g., Model Extraction rated as high severity/medium likelihood) are Microsoft's internal assessment without disclosed methodology. Verify: do not treat severity ratings as externally validated; treat the 25/28 figure as anecdotal unless a source study can be identified.

---

## Cross-Links to Corpus

- [[F043_MIT_AI_Risk_Mitigation_Taxonomy_2025]] — MIT taxonomy's Technical & Security category (12% of all mitigations) maps directly to the Microsoft ML attack framework; F044 provides the attack-surface detail that populates F043's security category
- [[F042_IBM_Cost_Data_Breach_Report_2025]] — IBM's 97% lacking AI access controls finding corroborates Microsoft's 89% lacking ML security tools finding from a different instrument and period; together they establish a sustained enterprise AI security governance deficit
- [[F038_ISACA_Agentic_AI_Security_Best_Practices]] — ISACA's ephemeral identity and lateral movement controls address the Evasion and Model Extraction attack categories in agentic AI deployment contexts
- [[F036_NIST_NCCoE_Agent_Identity_Authorization]] — NIST NCCoE authentication and access delegation framework addresses access control failures that enable Model Extraction and Inference attacks
