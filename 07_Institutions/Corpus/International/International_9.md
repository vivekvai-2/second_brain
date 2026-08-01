---
type: corpus-node
node-id: International_9
institution: International
date: 2024-12
wiki-section: S4
tier: B
ai-explicit: true
tags:
  - type/corpus-node
  - institution/International
  - wiki-section/S4
  - tier/B
  - batch/9
  - concept/Governance_Debt
  - concept/Institutional_Coherence
  - concept/Governance_Capacity
  - concept/Accountability
  - concept/Transparency
  - concept/Regulatory_Parallelism
  - project/P1
  - project/P3
  - project/fsQCA
---

# International_9 — BIS/FSI: Regulating AI in the Financial Sector: Recent Developments and Main Challenges (FSI Insights No. 63, December 2024)

**Node ID:** International_9  
**Institution:** Bank for International Settlements (BIS) / Financial Stability Institute (FSI)  
**Document type:** FSI Insights on policy implementation — cross-jurisdictional regulatory review and implementation guidance  
**Date:** December 2024  
**Series:** FSI Insights on policy implementation, No. 63  
**Jurisdictions reviewed:** Brazil, China, EU, Qatar, Singapore, United Kingdom, United States (+ referenced: Qatar Central Bank)  
**Wiki Section:** S4 — International Standard Setters / BIS-FSI Analytical Reports  
**Tier:** B (BIS/FSI authorship; December 2024; directly cited by FSI Insights No. 73 as predecessor; widely circulated among financial supervisors)

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | Regulating AI in the financial sector: recent developments and main challenges |
| Series | FSI Insights on policy implementation, No. 63 |
| Date | December 2024 |
| Publisher | Financial Stability Institute (FSI), Bank for International Settlements |
| Authors | Juan Carlos Crisanto (BIS); Cris Benson Leuterio (Bangko Sentral ng Pilipinas/BSP); Jermy Prenio (BIS); Jeffery Yong (BIS) |
| ISBN | 978-92-9259-822-8 (online) |
| ISSN | 2522-249X (online) |
| JEL | C60, G29, G38, O30 |
| Keywords | Artificial intelligence, machine learning, corporate governance, risk management, risk modelling |
| Authorised by | Fernando Restoy, Chair of FSI |
| Focus jurisdictions | Brazil, China, EU, Qatar, Singapore, UK, US |
| Predecessor | Prenio and Yong (2021): "Humans keeping AI in check — emerging regulatory expectations in the financial sector", FSI Insights No. 35, August 2021 |
| Successor | Crisanto et al (2026): FSI Insights No. 73 "In data we trust?" (International_8) — extends this document's data governance section |
| Source URL | bis.org/fsi |

---

## S2. Governance Context

International_9 is the BIS-FSI's 2024 synthesis of the global regulatory landscape for AI in financial services — updating the 2021 predecessor (Prenio and Yong) and situating financial sector AI governance within the broader cross-sectoral AI policy evolution. It provides the most comprehensive multi-jurisdiction comparison of AI regulatory approaches available at the time of publication (December 2024), covering both the **cross-sectoral** AI governance layer (national AI laws/principles) and the **financial sector-specific** layer (MRM frameworks, conduct rules, consumer protection).

The document's central diagnostic: the common themes of cross-sectoral AI guidance are already broadly reflected in existing financial regulations, yet AI presents implementation challenges that may require sector-specific guidance in six specific areas. This nuanced position — "not new risks, but new implementation challenges" — is analytically significant for P1 (SLR) and P3 (BFSI).

---

## S3. AI Use Cases in Financial Services (Section 2)

### Quantitative Context

| Indicator | Figure | Source |
|---|---|---|
| Financial sector AI spending 2023 | USD 35 billion | Statista 2024 |
| Financial sector AI spending 2027 (forecast) | USD 97 billion | Statista 2024 |
| Banking gen AI spending 2023 | USD 3.86 billion | — |
| Banking gen AI spending 2030 (forecast) | ~USD 85 billion | — |
| Gen AI value added to banking annually | USD 200–340 billion (2.7–4.7% revenues) | McKinsey 2024 |
| Third-party AI model usage (cross-sector) | 78% of organisations (53% exclusively) | MIT-BCG 2023 (87 jurisdictions) |
| US population interacting with bank chatbot (2022) | 37% | CFPB 2023 |
| Foundation model hallucination rate (LLMs) | 1.4–4.2% | Stanford/BIS cited estimate |

### Use Case Taxonomy (Table 1)

Three primary use case clusters in banking and insurance:

1. **Customer support chatbots** — AML/CFT alert reduction; 24/7 customer interaction (Bank of America Erica: 1.5B interactions, 37M clients)
2. **Fraud detection / AML/CFT** — HSBC: 2–4x more suspicious activities detected vs. previous system; 60% alert reduction
3. **Credit and insurance underwriting** — ML for credit scoring, collateral valuation, loan personalisation; gen AI for insurance underwriting (unstructured data processing); EU AI Act classifies both as high-risk AI uses

**Structural observation:** Most reviewed use cases are for internal operational efficiency; gen AI use in customer-facing and high-risk activities remains limited due to: regulatory uncertainty, third-party model dependency, customer acceptance concerns, and internal accountability gaps.

---

## S4. Cross-Sectoral AI Guidance — Common Themes (Section 3)

### Seven Themes Framework (Figure 2)

Building on Prenio and Yong (2021) which identified five themes, International_9 documents the evolved framework:

| Theme | Status (2024) | Key developments since 2021 |
|---|---|---|
| Transparency / Explainability | Core; unchanged | More concrete guidance on post-hoc explainability techniques (SHAP, LIME); NIST 4 principles of explainable AI |
| Accountability / Governance | Core; unchanged | Human-in-the-loop → human-on-the-loop → human-in-control evolution |
| Reliability / Soundness | Core; unchanged | Framed as harm-avoidance (customer outcomes), not just model performance |
| Fairness and Ethics | Core; less explicit | Ethics increasingly folded into governance/accountability |
| Data Privacy / Security | More prominent in newer guidance | GDPR/data minimisation for AI training; data poisoning; breach notification |
| Safety | More prominent in newer guidance | UK and US AI Safety Institutes; EU AI Office safety unit |
| Intellectual Property + Sustainability | Emerging (gen AI specific) | Licensing; copyright; energy consumption |

**Increasingly common expectations (across all newer guidance):** Consumer redress channels; AI literacy/awareness training; international interoperability; public-private partnerships.

### Two Policy Approach Archetypes (para 23)

| Archetype | Jurisdictions | Characteristics |
|---|---|---|
| Principles-based | Singapore, UK, US | Non-binding principles; voluntary commitments; technology-neutral; defers regulation pending AI evolution |
| Rules-based | Brazil, China, EU, Qatar | AI legislation enacted or in process; regulatory clarity; legal enforcement powers; consumer rights protection focus |

This dichotomy is the primary cross-jurisdictional configurational data for the fsQCA paper.

---

## S5. Financial Sector Guidance Status (Section 4)

### Who Has Issued AI-Specific Financial Regulations?

Among the seven jurisdictions examined, **only Qatar Central Bank (QCB) and several US state insurance regulators** have issued financial sector regulations specifically addressing AI use. All other authorities have issued either:
- High-level principles (EBA, EIOPA, HKMA, MAS), or
- Clarifications of how existing regulations apply to AI (UK authorities)

**Key finding (para 4):** "Majority of respondents to an OECD survey do not plan to introduce new regulations on AI use in finance in the near future." Survey: Q1 2024; 49 OECD and non-OECD jurisdictions.

### Credit and Insurance Underwriting — Focus Analysis (Section 4)

The document anchors practical implementation analysis in credit and insurance underwriting — the two use cases classified as high-risk under the EU AI Act. Four challenge areas:

**1. Governance and accountability:**
- Three accountability roles: model owner, model developers, model users (credit officers / underwriters)
- Board and senior management accountable for entire AI lifecycle
- AI expertise gap: insufficient AI familiarity at board level for effective challenge of AI-driven decisions
- Human oversight trade-off: autonomous AI acceptance of loan/insurance applications conflicts with human-in-the-loop requirements

**2. Transparency and explainability:**
- Performance-explainability trade-off: more complex models → higher accuracy → lower explainability
- Post-hoc techniques in use: SHAP (40%), graphical tools (20%), enhanced documentation (28%), sensitivity analysis (8%) (EBA survey)
- Gen AI exacerbates: billions of parameters; non-deterministic outputs; novel content generation
- Singapore MAS Veritas Initiative — FEAT assessment methodology tested in financial institutions

**3. Third-party AI services, data security, operational resilience:**
- 78% of organisations use third-party AI models (53% exclusively)
- Shared responsibility model: third-party controls foundation model documentation; financial institution controls deployment/retraining
- Data poisoning, prompt injection, model theft as AI-specific cyber attack vectors
- Cloud-AI convergence: same providers supply both → systemic concentration risk
- Indirect oversight (via financial institution due diligence) insufficient for systemic risk management

**4. New players and new business arrangements:**
- BaaS (Banking-as-a-Service): bank makes credit decision; customer relationship with non-bank intermediary; accountability attribution unclear
- Embedded insurance / big tech insurance intermediaries: no clear accountable party for AI explainability obligations
- Big techs simultaneously: lenders + cloud providers + AI service providers to other banks

---

## S6. Six Areas for Regulatory Action (Section 5 — Conclusions, para 70)

The document's normative contribution — the six areas where financial authorities should examine existing regulations and consider clarifications/new guidance:

| # | Area | Core Recommendation |
|---|---|---|
| (i) | Governance framework | Specify AI lifecycle accountability; define human intervention role for harmful-outcome minimisation |
| (ii) | AI expertise and skills | Clarify expectations for board/senior management AI competency for AI-active financial institutions |
| (iii) | Model risk management | Extend MRM guidance to AI explainability; define explainability technique standards; consider comprehensive MRM covering all AI models |
| (iv) | Data governance and management | Assess whether existing model risk / consumer privacy / information security regulations are sufficient; consider AI-specific data governance guidance |
| (v) | New/non-traditional players and new business models | Assess regulatory coverage gaps for FinTech/BigTech lenders; address multi-layer BaaS accountability |
| (vi) | Regulatory perimeter — third parties | Strengthen case for direct oversight of cloud/AI service providers as concentration risk becomes systemic |

---

## S7. Analytical Significance

### Governance_Debt — Financial sector AI regulation gap
The document's core diagnosis is that financial AI regulation has not caught up to cross-sectoral AI governance frameworks, and most financial authorities explicitly decline to issue sector-specific AI rules in the near term. This is a policy-level Governance_Debt: the institutional awareness is present (six areas identified; three further research areas proposed) but the regulatory instruments have not been issued. The OECD finding that most jurisdictions don't plan new financial AI regulations compounds this: the debt is structural, not transitional.

For P1 SLR: anchor the "financial sector AI governance gap" finding in this document (December 2024 data; 49-jurisdiction OECD survey).

### Institutional_Coherence — Cross-sectoral vs. sector-specific governance parallelism
The document empirically documents the Institutional_Coherence failure: cross-sectoral AI guidance (national AI bodies) and financial sector AI guidance (financial authorities) operate on parallel tracks without systematic translation mechanisms. In Singapore and the UK, partial coherence is achieved through industry co-creation (MAS Veritas) and existing-regulation clarification (UK authorities). In the EU, the EU AI Act creates the horizontal layer but EBA/EIOPA have not yet issued financial-sector-specific implementation guidance. In the US, the fragmentation is most severe: multiple federal bodies (FRB-OCC, CFPB, SEC) plus state-level insurance regulators, without a unified financial AI governance architecture.

For P3: map this pattern onto India — NITI Aayog (cross-sectoral) + RBI/SEBI/IRDAI (sector-specific) with no coordination mechanism — as a direct example of the Institutional_Coherence gap documented here.

### Regulatory_Parallelism — Principles vs. rules dichotomy
The most important fsQCA contribution: the document provides the empirical basis for the primary condition of interest in the comparative regulatory analysis — principles_based vs. rules_based approach — with explicit jurisdiction assignment. Singapore/UK/US = principles-based configuration (voluntary, non-binding, technology-neutral). Brazil/China/EU/Qatar = rules-based configuration (legislative, binding, risk-classified). This two-configuration baseline is the empirical anchor for the fsQCA cross-jurisdictional comparison.

India maps as: mixed/transitional — NITI Aayog guidance (principles-based); DPDP 2023 (rules-based for data); RBI AI guidance (principles-based + existing regulation extension) → an incoherent configuration that doesn't cleanly fit either archetype.

### Governance_Capacity — AI expertise and skills gap
The document identifies the AI expertise gap at board and senior management level as a foundational governance capacity failure: without adequate AI literacy, governance frameworks (however well-designed) cannot be effectively implemented. This is a distinct dimension of Governance_Capacity — institutional human capital capacity — separate from regulatory instrument capacity. For P3: RBI has issued MRM guidance extending to AI but has not yet addressed the board-level AI expertise requirement.

---

## S8. Research Project Linkages

| Project | Relevance |
|---|---|
| **P1 (SLR)** | December 2024 global baseline on financial sector AI regulation; seven-jurisdiction comparative; six-areas framework for gap analysis; OECD survey on regulatory intentions |
| **P3 (BFSI)** | Financial sector-specific AI governance diagnostic; India absence from seven-jurisdiction comparison analytically significant; RBI governance gap identification |
| **fsQCA** | Primary jurisdictional configuration data: principles-based (SG, UK, US) vs. rules-based (Brazil, China, EU, Qatar); condition set construction; India configuration analysis |

---

## S9. Key Concepts

- [[Governance_Debt]] — "majority of jurisdictions don't plan new financial AI regulations" (OECD Q1 2024 survey); structural financial sector AI governance gap
- [[Institutional_Coherence]] — cross-sectoral vs. sector-specific governance parallelism; MAS Veritas as partial coherence model; BaaS accountability gap
- [[Governance_Capacity]] — AI expertise gap at board level; third-party model opacity limiting independent validation
- [[Accountability]] — six-area framework; AI lifecycle accountability; human-in-the-loop requirements; BaaS attribution problem
- [[Transparency]] — explainability-performance trade-off; SHAP/LIME techniques; NIST four principles of explainable AI; CFPB adverse action notifications
- [[Regulatory_Parallelism]] — principles-based vs. rules-based; cross-sectoral vs. sector-specific tracks; financial sector AI governance lag

---

## ⚠ VERIFY Flags

| # | Flag | Priority |
|---|---|---|
| ⚠V-I9-1 | Confirm OECD Q1 2024 survey (49 jurisdictions): "majority do not plan new AI financial regulations in near future" — verify exact phrasing and data | High |
| ⚠V-I9-2 | Confirm BSP (Bangko Sentral ng Pilipinas) co-authorship — verify Leuterio's institutional affiliation as BSP | Low |
| ⚠V-I9-3 | Confirm Qatar Central Bank AI Guideline (September 2024) — verify date and content (human-in-control; stop button requirement) | Medium |
| ⚠V-I9-4 | Confirm that only QCB + US state insurance regulators have issued specific financial AI regulations — verify whether any other authority has since done so | High |
| ⚠V-I9-5 | Confirm FSB (2024) "Financial stability implications of AI" — November 2024 date; whether in PRIS corpus | Medium |
| ⚠V-I9-6 | Confirm HKMA GenA.I. Sandbox — verify launch date and programme scope | Low |
| ⚠V-I9-7 | Verify India's configuration classification — confirm RBI's AI governance posture as "principles-based + existing regulation extension" with no AI-specific rules as of December 2024 | High |

---

## S10. Connections

**Corpus nodes:**
- [[International_8]] — FSI Insights No. 73 (March 2026); successor document; AI data governance specifics
- [[International_7]] — BIS/IFC Report No. 18 (April 2025); central bank deployer-side governance
- [[RBI_1]] through [[RBI_4]] — India BFSI AI regulation; compare to seven-jurisdiction framework
- [[SEBI_14]] — India BFSI AI governance; SEBI principles-based approach
- [[NITI_1]], [[NITI_3]], [[NITI_7]] — India cross-sectoral AI strategy; compare to international cross-sectoral vs. sector-specific architecture

**Concepts:**
- [[Governance_Debt]]
- [[Institutional_Coherence]]
- [[Governance_Capacity]]
- [[Accountability]], [[Transparency]]
- [[Regulatory_Parallelism]]

**Institutions:**
- [[_Institutions_MOC]] — International row (BIS/FSI publication)

**Projects:**
- [[02_Projects/P1_SLR_RG]]
- [[02_Projects/P3_BFSI_JEIM]]
- [[fsQCA_Regulatory_Configurations]]

---

_Added: Batch 9 — 2026-06-18 | FSI Insights No. 63 (December 2024) | Predecessor to International_8; primary fsQCA configuration data for principles-based vs. rules-based AI regulatory approach | ⚠V-I9-7 priority: confirm India configuration classification_
