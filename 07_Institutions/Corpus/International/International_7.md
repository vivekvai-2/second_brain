---
type: corpus-node
node-id: International_7
institution: International
date: 2025-04
wiki-section: S4
tier: B
ai-explicit: true
tags:
  - type/corpus-node
  - institution/International
  - wiki-section/S4
  - tier/B
  - batch/9
  - concept/Governance_Capacity
  - concept/Governance_Debt
  - concept/Accountability
  - concept/Transparency
  - project/P1
  - project/P3
  - project/fsQCA
---

# International_7 — BIS/IFC: Governance and Implementation of Artificial Intelligence in Central Banks (IFC Report No. 18, April 2025)

**Node ID:** International_7  
**Institution:** Bank for International Settlements (BIS) / Irving Fisher Committee on Central Bank Statistics (IFC)  
**Document type:** Survey Report — empirical cross-jurisdictional survey of central bank AI governance practices  
**Date:** April 2025  
**Series:** IFC Report No. 18  
**Survey scope:** 60 IFC member central banks across all continents (survey window: September–November 2024)  
**Wiki Section:** S4 — International Standard Setters / BIS-IFC Empirical Reports  
**Tier:** B (BIS/IFC authorship; 60-jurisdiction empirical survey; high credibility; not standard-setting but analytically foundational for P3)

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | Governance and implementation of artificial intelligence in central banks |
| Series | IFC Report No. 18 |
| Date | April 2025 |
| Publisher | Bank for International Settlements / Irving Fisher Committee on Central Bank Statistics |
| Authors | Douglas Araujo (BIS); Rafael Schmidt (BIS); Olivier Sirello (BIS); Bruno Tissot (BIS & IFC); Ricardo Villarreal (Central Bank of Chile) |
| ISBN | 978-92-9259-847-1 |
| Survey instrument | Questionnaire distributed to 60 IFC member central banks, September–November 2024 |
| Respondent coverage | 60 jurisdictions: ~48% Europe; ~28% Asia & Oceania; ~18% Americas; ~6% Africa |
| ⚠VERIFY | Whether RBI is among the 60 respondents (IFC membership; India is likely but confirm) |
| Source URL | bis.org/ifc |

---

## S2. Governance Context

This survey report provides the most current (2024 data) cross-jurisdictional empirical evidence on AI governance maturity and implementation practices in central banks globally. It is the IFC's first comprehensive survey dedicated specifically to AI governance — distinguished from earlier BIS publications (International_2 on generative AI; the FSI Insights series) by its exclusive focus on central bank institutional governance rather than regulatory frameworks for financial sector firms.

**PRIS corpus positioning:** International_7 operates at a different analytical layer than the regulatory frameworks (RBI_x, SEBI_x, IRDAI_x nodes). Where those nodes document regulatory instruments directed at regulated entities, this document surveys how central banks govern AI internally — as institutions deploying AI themselves. This creates a critical distinction for P3: the RBI is simultaneously a regulator of BFSI AI (regulator-role) and a central bank deploying AI (deployer-role). International_7 addresses the deployer-role governance dimension.

The companion publication is CGRM (2025), "Governance of AI adoption in central banks," BIS Representative Office for the Americas — cited in International_7 as a parallel study. (**⚠VERIFY** whether CGRM 2025 is in the PRIS corpus or pending acquisition.)

---

## S3. Core Findings

### AI Adoption Status (60 central banks, 2024)

| Status | Share |
|---|---|
| AI/ML in full production | ~25% |
| AI/ML in development/piloting | ~33% |
| Small-scale production | ~30% |
| No AI/ML in use | ~12% |

**Key tension:** 45% rate AI/ML as "high priority" in strategic planning; 62% are extensively discussing AI/ML internally. Yet only 25% have reached full production. This "expectation-deployment gap" is a governance signal: institutional and governance constraints, not technical capability, are the binding constraint in most central banks.

### Generative AI Adoption
- 88% of respondent central banks use generative AI (text and code generation are dominant use cases)
- Despite near-universal GenAI use, full production deployment remains low — suggesting most use is experimental or staff-level rather than institutionally governed

### AI Policy Status

| Policy Status | Share |
|---|---|
| Publicly available AI policy | ~5% |
| Internally available AI policy | ~28% |
| Currently elaborating AI policy | ~33% |
| No AI policy (no plans) | ~32% |
| No AI policy (planning to elaborate) | ~2% ⚠VERIFY |

**Key finding:** Only ~33% of central banks have any form of AI policy (public or internal). ~32% have no AI policy and no active elaboration plans. This is the empirical basis for the global Governance_Debt claim in P3 and P1.

**Restriction landscape:** 75% restrict AI tool use for confidentiality and security reasons — the most common operational governance measure. This indicates risk management precedes policy formalisation in most institutions.

### Organisational Governance Structures

| Characteristic | Finding |
|---|---|
| Centralised AI governance (CDO or equivalent) | ~20% |
| Decentralised (business-area led) | ~68% |
| CDO-coordinated hybrid | ~12% |
| Established AI-specific central governance structure | ~39% |

Advanced Economies (AEs) are significantly more likely to have centralised or CDO-led governance. Emerging Market Economies (EMEs): ~72% manage AI decentrally (business-area level); ~50% of EMEs have no AI governance policy or plans. This **AE–EME governance gap** is a structurally significant finding for P1 (global AI governance literature) and P3 (India as an EME central banking jurisdiction).

### IT Architecture (selected)

| Dimension | Finding |
|---|---|
| On-premises self-deployed preference | ~40%+ (majority preference) |
| Cloud allowance (full or partial) | ~35% |
| Cloud not allowed or experimental only | ~65% |
| Hybrid open+closed source model | ~63% |
| Python as dominant language | ~73% |

---

## S4. AI Governance Framework (Box A — Four Components)

The report presents a 4-component AI governance framework applicable to central banks:

| Component | Description |
|---|---|
| **Data governance** | Data quality; metadata documentation; FAIR principles (Findable, Accessible, Interoperable, Reusable); data provenance and lineage |
| **Organisational structures** | Responsibility allocation (CDO, AI steering committees, business-area AI leads); three-lines-of-defence (3LoD) adaptation for AI risk |
| **Guidelines and policies** | AI ethics principles; acceptable use policies; procurement standards; model documentation requirements |
| **Risk management** | Bias assessment; explainability requirements; cyber risk; model risk management (extending existing MRM frameworks to AI); audit protocols |

This 4-component model is the report's analytical scaffold — used to benchmark where individual jurisdictions fall on each dimension. It is consistent with but not identical to NIST AI RMF (Govern/Map/Measure/Manage) and EU AI Act governance requirements.

---

## S5. Roadmap — Four Priority Areas

IFC's recommended roadmap for central bank AI governance improvement:

1. **Act as data curators** — improve internal data quality, metadata, lineage documentation, and FAIR-compliance; treat data governance as prerequisite for AI deployment
2. **Improve global data infrastructure** — adopt SDMX standards; contribute to G20 Data Gaps Initiative (DGI); build cross-border data sharing frameworks
3. **Modernise data processes and systems** — data pipeline modernisation; legacy system integration; real-time data ingestion capabilities
4. **Advance user literacy in AI and data science** — structured upskilling; AI literacy programmes at board and senior management levels; reduce dependence on external vendors for AI interpretation

---

## S6. Analytical Significance

### Governance_Debt — Global empirical baseline
International_7 provides the 2024 empirical baseline for the claim that AI Governance_Debt is not India-specific but globally prevalent even in the most institutionally sophisticated financial sector organisations (central banks). The finding that ~32% of central banks have no AI policy — including some EME central banks with sophisticated existing IT and risk management frameworks — grounds the Governance_Debt concept in cross-jurisdictional empirical evidence rather than theoretical argument alone.

For the P1 SLR: cite this as the quantitative anchor for the global AI governance gap in central banking (2024 data point). For the P3 thesis: use the AE–EME gap as the comparative framework within which RBI's AI governance trajectory can be positioned.

### Governance_Capacity — AE vs. EME structural divergence
The systematic governance capacity gap between Advanced Economies and Emerging Market Economies — more centralised governance, more policy formalisation, higher CDO presence in AEs — provides empirical structure for the Governance_Capacity concept. The gap is not merely a resource difference; it reflects institutional complexity and legacy system constraints that are higher in EMEs. The 72% decentralised AI management rate in EMEs (vs. much lower in AEs) is a measurable governance capacity indicator.

### India (RBI) positioning — EME deployer-role governance
If RBI is among the 60 respondents (⚠VERIFY), India appears in the aggregated data as one of the EME governance cases. Given India's mixed profile — sophisticated payment system AI (UPI) but early-stage AI policy — RBI likely falls in the "AI policy elaborating" or "internally available" category rather than "publicly available." The deployer-role governance gap at RBI thus mirrors the global EME pattern. This dual framing (regulator-role: RBI circulars on BFSI AI; deployer-role: EME governance gap) is a novel analytical contribution for P3.

### fsQCA — Global configuration evidence
For the fsQCA paper: International_7 provides cross-jurisdictional empirical evidence on configuration diversity in central bank AI governance. The AE–EME split corresponds to distinct condition sets (centralised_governance, policy_formalisation, CDO_presence). This empirical baseline supports the fsQCA claim that AI governance configurations are not uniformly distributed across jurisdictions.

### Three-Lines-of-Defence (3LoD) adaptation
The report documents that central banks adapting 3LoD to AI risk is the most common risk governance mechanism (where any AI risk governance exists). This links to the existing PRIS concept track and connects International_7 to the 3LoD dimension in BFSI AI governance frameworks.

---

## S7. Research Project Linkages

| Project | Relevance |
|---|---|
| **P1 (SLR)** | 2024 empirical baseline on global central bank AI governance maturity; AE–EME gap; expectation-deployment gap |
| **P3 (BFSI)** | RBI as EME central bank deployer of AI; dual-role (regulator + deployer) governance complexity; international comparator for Indian BFSI AI governance |
| **fsQCA** | Cross-jurisdictional configuration evidence; AE vs. EME as distinct condition sets in AI governance dataset |

---

## S8. Key Concepts

- [[Governance_Debt]] — ~32% of central banks have no AI policy and no plans; global empirical baseline; EME-concentrated
- [[Governance_Capacity]] — AE–EME governance gap documented empirically; CDO presence; policy formalisation rate; 3LoD adaptation
- [[Accountability]] — 3LoD adaptation for AI risk; CDO accountability structures; organisational responsibility allocation
- [[Transparency]] — FAIR data principles; model documentation; explainability requirements in risk management component
- [[Regulatory_Parallelism]] — indirect: decentralised AI governance within central banks = internal parallelism (business-area silos); maps to external regulatory parallelism pattern

---

## ⚠ VERIFY Flags

| # | Flag | Priority |
|---|---|---|
| ⚠V-I7-1 | Confirm RBI is among the 60 IFC member respondents; identify any India-specific data point in the survey | High |
| ⚠V-I7-2 | Confirm exact percentage breakdown of AI policy status (5% public / 28% internal / 33% elaborating / 32% no plans) — read primary text | Medium |
| ⚠V-I7-3 | Confirm CGRM (2025) "Governance of AI adoption in central banks" (BIS Americas) — check if in PRIS corpus or to be acquired | High |
| ⚠V-I7-4 | Confirm exact AE–EME breakdown for decentralised management (72% EME figure) and no-policy rate (50% EME) | Medium |
| ⚠V-I7-5 | Confirm whether "expectation-deployment gap" language is document's own or PRIS analytical label | Low |
| ⚠V-I7-6 | Cross-reference 4-component Box A framework text verbatim against NIST AI RMF and EU AI Act governance requirements | Medium |

---

## S9. Connections

**Corpus nodes:**
- [[International_2]] — BIS Working Paper on Generative AI (already in corpus); companion to International_7 on AI adoption
- [[International_8]] — next BIS corpus node (BIS In data we trust)
- [[International_9]] — next BIS corpus node (BIS Regulating AI in the financial sector)
- [[RBI_1]] through [[RBI_4]] — RBI regulatory instruments; cross-reference deployer-role vs. regulator-role governance distinction
- [[SEBI_14]] — SEBI AI framework; India BFSI side; connects to central bank governance gap documented here

**Concepts:**
- [[Governance_Debt]] — global empirical baseline instance
- [[Governance_Capacity]] — AE–EME gap; CDO presence; policy formalisation
- [[Accountability]] — 3LoD adaptation for AI
- [[Transparency]] — FAIR principles; explainability in risk management

**Institutions:**
- [[_Institutions_MOC]] — International row (BIS/IFC publication)

**Projects:**
- [[02_Projects/P1_SLR_RG]]
- [[02_Projects/P3_BFSI_JEIM]]
- [[fsQCA_Regulatory_Configurations]]

---

_Added: Batch 9 — 2026-06-18 | IFC Report No. 18 (April 2025) | 60-jurisdiction survey, Sep–Nov 2024 data | ⚠V-I7-1 priority: confirm RBI respondent status_
