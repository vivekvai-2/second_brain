---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S1
  - section/S3
  - tier/high-medium
  - project/p1
  - project/p3
  - project/fsqca
---

# MIT AI Risk Initiative + FutureTech: Mapping AI Risk Mitigations — Evidence Scan and Draft Mitigation Taxonomy (July 2025)

**Node ID:** F043  
**Type:** Wiki Intake Note  
**Wiki Section:** S1 (Governance Fundamentals) / S3 (International Comparators)  
**Status:** Active  
**Tier:** High-Medium  
**Last Updated:** 2026-06-19  

---

## Source

**Full Citation (APA):** Slattery, P., Saeri, A. K., Grundy, E. A. C., Lewis, J., Noetel, M., Uuk, R., Dao, J., Pour, S., Casper, S., & Thompson, N. (2025, July). *Mapping AI risk mitigations: Evidence scan and draft mitigation taxonomy*. MIT AI Risk Initiative; FutureTech.  
**Document Type:** Technical report / systematic evidence scan (grey literature with academic methodology)  
**Issuing Institution:** MIT AI Risk Initiative (AIRI); FutureTech  
**Publication Date:** July 2025  
**URL / DOI:** Available via MIT AIRI and FutureTech repositories (⚠ VERIFY for stable DOI/URL)  

---

## Executive Summary

This report presents the first large-scale systematic mapping of AI risk mitigation measures drawn from 13 primary governance documents, extracting and classifying 831 individual mitigations into a four-category taxonomy. The taxonomy — covering Governance & Oversight, Technical & Security, Operational Process, and Transparency & Accountability — is designed to support evidence-based AI governance design, identify coverage gaps, and enable cross-jurisdiction comparability. A critical finding is that Model Alignment receives less than 1% of documented mitigations despite being identified by AI safety researchers as foundational to long-horizon AI risk. The document is intended for AI governance policymakers, standards bodies, and researchers seeking to map governance obligations to risk categories systematically. The MIT AIRI + FutureTech taxonomy directly links to the FLI AI Safety Index (F048), which cites this work as the Slattery et al. 2024/2025 MIT FutureTech AI Risk Repository.

---

## Key Frameworks and Findings

### Evidence Base

| Parameter | Value |
|---|---|
| Source documents reviewed | 13 |
| Individual mitigations extracted | 831 |
| Mitigations successfully classified | 815 (98%) |
| Unclassified / edge cases | 16 (2%) |
| Methodology | Systematic extraction; two-coder classification with inter-rater reliability protocol |

### Four-Category Mitigation Taxonomy

| Category | Share of All Mitigations | Description |
|---|---|---|
| **Governance & Oversight** | ~30% | Board/executive accountability, regulatory obligations, audit mandates, oversight bodies |
| **Technical & Security** | ~12% | Adversarial robustness, access controls, model testing, red-teaming, safety tooling |
| **Operational Process** | ~36% | Risk assessments, procurement controls, incident response, human-in-the-loop processes |
| **Transparency & Accountability** | ~21% | Disclosure obligations, explainability requirements, audit trails, documentation |

### Critical Gap: Model Alignment

The taxonomy's most significant finding is the **model alignment gap**: fewer than 1% of documented mitigations across all 13 source documents address Model Alignment — the technical and procedural question of ensuring AI systems pursue intended objectives. This gap exists despite model alignment being identified by leading AI safety researchers (Russell, Hadfield-Menell, and others) as the foundational challenge for advanced AI systems. The report does not explain or justify this gap; it documents it as an empirical finding across existing governance documents.

**Implication for governance design:** Current AI governance frameworks are heavily weighted toward process-level mitigations (Operational Process at 36%) and light on foundational technical safety measures (Technical & Security at 12%; alignment at <1%). This reflects a documentation/awareness bias: governance documents primarily articulate what organisations *must do* (process), not what AI systems *must be* (alignment).

### Source Documents in Scope

The 13 documents reviewed are not individually named in the available summary but include major international AI governance frameworks (EU AI Act, NIST AI RMF, ISO/IEC 42001, OECD AI Principles, and comparable documents — ⚠ VERIFY for complete source list in full document). This evidence base explains why the taxonomy skews toward process-level documentation.

### Taxonomy Architecture

The four-category taxonomy is designed for:
1. **Gap analysis:** identifying which risk types are under-mitigated in any given regulatory framework
2. **Cross-jurisdiction comparison:** enabling comparison of mitigation portfolios across governance regimes (e.g., India vs. EU vs. US)
3. **Evidence-based governance:** linking mitigations to supporting evidence (does this mitigation actually reduce the targeted risk?)

The taxonomy's categories map onto the PRIS vault's existing concept architecture: Governance & Oversight → [[Accountability]]; Technical & Security → [[Governance_Capacity]]; Operational Process → [[Governance_Capacity]] + [[Governance_Debt]]; Transparency & Accountability → [[Transparency]].

---

## India Relevance and Governance Gap Analysis

Applying the MIT/FutureTech taxonomy to India's AI governance landscape reveals a pattern consistent with global findings: India's existing instruments (NITI Aayog RAISE 2020, RBI CSCRF 2024, SEBI AI guidelines 2025) are heavily concentrated in the **Governance & Oversight** and **Operational Process** categories, with minimal contribution to **Technical & Security** or **Transparency & Accountability** as defined in the taxonomy.

**Specific gaps:**
1. **Model Alignment (<1% globally):** India has no instrument that addresses model alignment requirements for AI systems deployed in regulated sectors. This is the deepest structural governance gap — it exists globally, but India also lacks the evaluation infrastructure to even assess alignment (cf. F041 AEF-1 minimum operating conditions; F048 FLI finding that no frontier AI company scores above C+).
2. **Technical & Security (12% globally):** RBI CSCRF addresses cybersecurity broadly but not AI-specific adversarial robustness, model extraction protection, or AI red-teaming mandates. SEBI has no technical AI security requirements.
3. **Transparency & Accountability (21% globally):** India's DPDP Act 2023 addresses personal data transparency but not AI output transparency, algorithmic explainability, or audit trail requirements for AI decision-making systems.
4. **Taxonomy gap — India's regulatory documents not in the 13-document evidence base:** The report's source corpus is implicitly OECD/Western-centric. India's governance documents are not represented in the evidence scan, meaning India's existing mitigation coverage against the taxonomy is unmeasured.

Cross-reference: [[F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations]] (evaluation institution gap) and [[F048_FLI_AI_Safety_Index_Winter_2025]] (cites this taxonomy as foundational reference; confirms model alignment deficit at frontier AI developer level).

---

## Research Programme Applications

| Project | Application |
|---|---|
| P1 (SLR RG) | Primary — MIT/FutureTech taxonomy is a landmark governance literature contribution; directly citable as systematic evidence on mitigation coverage distribution; model alignment gap finding is a major conceptual anchor; 831 mitigation extraction methodology exemplifies evidence-scan approach usable in P1 |
| P3 (BFSI JEIM) | Operational Process (36%) and Governance & Oversight (30%) categories map directly onto BFSI AI governance implementation; India BFSI mitigation portfolio can be benchmarked against taxonomy distribution |
| P4 (Doctrinal IJLIT) | Taxonomy categories provide a doctrinal classification framework for analysing which AI governance obligations appear in Indian law vs. comparative jurisdictions; model alignment gap is relevant to liability doctrine discussion (if AI causes harm due to misalignment, which legal framework responds?) |
| fsQCA | OC/CC conditions — Governance & Oversight category distribution (30%) provides empirical basis for calibrating Organisational Commitment and Regulatory Commitment conditions across jurisdictions; EA condition — Technical & Security + Transparency shares calibrate accountability infrastructure scores |

---

## Concept Links

- [[Accountability]] — Governance & Oversight category (~30%) is the accountability-infrastructure component of the taxonomy; Transparency & Accountability category (~21%) adds disclosure and audit dimensions
- [[Transparency]] — Taxonomy's Transparency & Accountability category (21%) maps directly; model alignment gap means transparency at the *model level* is systematically absent from global governance documents
- [[Governance_Capacity]] — Technical & Security category (12%) directly measures governance capacity for AI-specific adversarial robustness; low share indicates systemic governance capacity deficit in technical AI safety
- [[Governance_Debt]] — Model alignment at <1% of mitigations is the most extreme instance of governance debt in the corpus: the foundational technical safety requirement is the most under-addressed by existing governance documentation
- [[Regulatory_Parallelism]] — 13-document source corpus draws from multiple uncoordinated international governance regimes; taxonomy implicitly demonstrates that parallel governance streams have independently arrived at similar Operational Process concentrations without coordination
- [[Institutional_Coherence]] — Taxonomy's cross-document extraction reveals coherence at the mitigation-category level (all documents emphasise process) but incoherence at the risk-priority level (alignment risk is high-priority but low-documentation)

---

## ⚠ VERIFY BEFORE PUBLISHING

No critical flags. The core statistical findings (831 mitigations, 4 categories, model alignment <1%) are the document's own outputs and are cited as document content. One precautionary note:

- **V-B14-03 / No number assigned (clean flag):** Confirm the complete list of 13 source documents in the evidence scan. If India instruments are among them, the governance gap analysis above requires revision. LOW priority — the document's framing and OECD context strongly imply Western-centric source corpus.

---

## Cross-Links to Corpus

- [[F048_FLI_AI_Safety_Index_Winter_2025]] — FLI cites this taxonomy (as "Slattery et al. 2024/2025 MIT FutureTech AI Risk Repository") as a foundational reference; confirms corpus coherence; FLI's Existential Safety domain scores corroborate the model alignment gap finding at the frontier AI developer level
- [[F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations]] — AEF-1 minimum conditions for AI evaluations addresses the evaluation infrastructure gap; MIT taxonomy's Technical & Security category (<1% alignment) is the design-level correlate of AEF-1's institutional implementation gap
- [[F038_ISACA_Agentic_AI_Security_Best_Practices]] — ISACA's ephemeral identity and least-privilege recommendations operationalise elements of the taxonomy's Technical & Security category for agentic AI contexts
- [[F047_BAIR_Berkeley_Responsible_GenAI_Playbook_2025]] — BAIR playbook's 10 plays largely operationalise Governance & Oversight and Operational Process categories; confirms dominant category distribution in practitioner guidance as well as in policy documents
