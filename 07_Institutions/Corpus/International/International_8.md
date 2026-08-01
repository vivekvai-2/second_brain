---
type: corpus-node
node-id: International_8
institution: International
date: 2026-03
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
  - concept/Governance_Capacity
  - concept/Institutional_Coherence
  - concept/Accountability
  - concept/Transparency
  - project/P1
  - project/P3
  - project/fsQCA
---

# International_8 — BIS/FSI: In Data We Trust? Emerging Policy and Supervisory Approaches to AI Data Use in Financial Services (FSI Insights No. 73, March 2026)

**Node ID:** International_8  
**Institution:** Bank for International Settlements (BIS) / Financial Stability Institute (FSI)  
**Document type:** FSI Insights on policy implementation — analytical review and supervisory guidance synthesis  
**Date:** March 2026  
**Series:** FSI Insights on policy implementation, No. 73  
**Jurisdictions reviewed:** China (NFRA), EU (EBA/EIOPA/ECB), Singapore (MAS), UK (BoE-PRA, FCA), US (FRB-OCC, CFPB, NYDFS)  
**Wiki Section:** S4 — International Standard Setters / BIS-FSI Analytical Reports  
**Tier:** B (BIS/FSI authorship; March 2026 — most recent in the corpus; policy-relevant to P3; widely cited by financial supervisors)

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | In data we trust? Emerging policy and supervisory approaches to AI data use in financial services |
| Series | FSI Insights on policy implementation, No. 73 |
| Date | March 2026 |
| Publisher | Financial Stability Institute (FSI), Bank for International Settlements |
| Authors | Juan Carlos Crisanto (BIS); Adrien Currat (BIS); Johannes Ehrentraud (BIS); Wenguang Wu (People's Bank of China/PBC) |
| ISBN | 978-92-9259-943-0 (online) |
| Authorised by | Fernando Restoy, Chair of FSI |
| Jurisdictions | China (NFRA), EU (EBA/EIOPA/ECB), Singapore (MAS), UK (BoE-PRA/FCA), US (FRB-OCC/CFPB/NYDFS) |
| Predecessor | Crisanto et al (2024) = FSI Insights No. 63, December 2024 — same lead author team; No. 73 extends No. 63's governance coverage into AI data governance specifically |
| Source URL | bis.org/fsi |

---

## S2. Governance Context

This document is the FSI's dedicated treatment of AI data governance in financial services — a topic identified as structurally underserved in FSI Insights No. 63 (December 2024), which noted that "data governance and management" was one of six areas needing specific supervisory attention. International_8 addresses that gap with a cross-jurisdictional policy synthesis.

The document's framing is explicit: 79% of financial institutions identify data quality as a key barrier to AI production deployment (IIF-EY 2025 ⚠VERIFY exact figure and survey scope). The document synthesises how financial authorities in five jurisdictions have addressed AI data risks and proposes five priority areas for supervisors globally. India is not among the five jurisdictions — constituting an analytically significant absence given DPDP 2023 and RBI's evolving AI governance posture.

**PRIS corpus positioning:** International_8 is the second document in the BIS-FSI AI governance series at S4 (after International_9 = FSI No. 63). Together the two FSI Insights papers (No. 63 on general AI regulation, No. 73 on AI data governance) form a two-paper BIS-FSI diagnostic series on regulating AI in financial services, published within 15 months of each other by overlapping author teams.

---

## S3. Core Framework — AI Data Risks

### Three Categories of AI Data Risk

| Risk Category | Description | Examples |
|---|---|---|
| **Data quality** | Accuracy, completeness, representativeness of training and input data | Data drift; biased training sets; stale data; alternative/synthetic data quality |
| **Data privacy** | Lawful basis for collection; purpose limitation; data minimisation; data subjects' rights | Right to erasure challenges in LLMs; GDPR compliance in model training |
| **Data security** | Confidentiality, integrity, availability of AI systems and their data | Data poisoning; prompt injection; breach notification; unauthorised access |

**Fourth dimension (cross-cutting):** Third-party data dependencies — financial institutions relying on external data providers and AI service providers face compounded versions of all three risks.

### Cross-Sectoral Guidance — Four Themes

The document maps cross-sectoral (non-financial) AI governance guidance across four themes:

| Theme | Key regulatory instruments covered |
|---|---|
| **Data privacy** | GDPR (EU); China Personal Information Protection Law (PIPL); PDPA (Singapore); UK GDPR |
| **Data quality** | EU AI Act Article 10 (data governance for high-risk AI); MAS FEAT Principles; EBA MRM guidelines |
| **Data security** | CIA triad (Confidentiality, Integrity, Availability); NYDFS 72-hour breach notification; cyber security frameworks |
| **Data governance** | BCBS 239 (banking sector baseline); board accountability frameworks; GPA (Global Privacy Assembly) resolutions |

---

## S4. Financial Sector Guidance — Jurisdiction Matrix (Table 1 Summary)

| Jurisdiction | Key Authority/Instrument | Approach | Binding? |
|---|---|---|---|
| China | NFRA — AI MRM + data governance guidance | Sector-specific; binding | Yes |
| EU | EBA (2020 big data report); EIOPA (2021 AI principles); EU AI Act Article 10 | Tiered — high-risk AI binding; otherwise principles | High-risk: binding |
| Singapore | MAS FEAT Principles (2018); MAS Veritas Initiative; MAS Consultation Paper on AI Risk Management (2025a) | Principles-based + industry co-creation | Voluntary principles |
| UK | BoE-PRA SS1/23 (MRM); FCA; DRCF (Digital Regulation Cooperation Forum — ICO + FCA) | Existing regulation application + inter-regulator coordination | Principles-based |
| US | FRB-OCC 2011 MRM; CFPB adverse action notification; NYDFS 72-hour breach rule; NYDFS Insurance Circular Letter No. 7 (July 2024) | Fragmented by function; existing frameworks extended | Mixed — binding at state level for insurance |

**Key finding:** "Existing policy responses are often piecemeal, with guidance typically focusing on either MRM or general data management, neither of which is necessarily tailored to AI" (document conclusion).

### BCBS 239 — Box 3 (Implementation Status)

BCBS 239 (Principles for effective risk data aggregation and risk reporting, 2013) represents the international baseline standard for banking data governance. Status as of International_8's publication:
- **Only 2 of 31 G-SIBs** report full compliance with all BCBS 239 principles (⚠VERIFY exact figure)
- Implementation remains uneven after a decade
- This reveals that the foundational data governance standard for global systemically important banks has not achieved compliance even at the top tier — a structural Governance_Capacity failure that precedes and constrains AI data governance

---

## S5. Five Priority Areas for Supervisory Guidance (Section 5 — Conclusions)

The document recommends financial supervisors develop tailored guidance in five priority areas:

| # | Priority Area | Core Gap Identified |
|---|---|---|
| 1 | **Data governance frameworks** | Clear roles, accountability, board oversight; adapt BCBS 239 principles to AI context |
| 2 | **Data quality management** | Accuracy, completeness, timeliness, representativeness of AI training and input data; address data drift |
| 3 | **Data security** | Incident response; breach notification; cyber security integration for AI-specific attack vectors (poisoning, prompt injection) |
| 4 | **Third-party dependencies** | Contractual safeguards; data lineage transparency; shared responsibility model for AI-as-a-service |
| 5 | **Data privacy in AI context** | Lawful basis for training data; purpose limitation; privacy-enhancing technologies (PETs); right to erasure in LLM context |

---

## S6. Analytical Significance

### Governance_Debt — Piecemeal policy architecture
The document's core empirical finding is that AI data governance in financial services is a structurally piecemeal landscape: existing MRM frameworks were not designed for AI data risks; data privacy laws were not designed for financial institutions' AI use cases; and there is no single integrated instrument addressing all five priority areas in any jurisdiction examined. This is the definitional condition of Governance_Debt: governance apparatus exists (MRM frameworks, BCBS 239, GDPR) but is not calibrated to the AI-era governance challenge. The five-priority-areas framework is the document's prescription for closing this debt.

For P1 SLR: cite as the 2026 empirical baseline for the claim that AI data governance in BFSI remains structurally incomplete across five major jurisdictions.

### Governance_Capacity — BCBS 239 compliance gap
The Box 3 finding that only 2/31 G-SIBs are fully compliant with BCBS 239 — a standard published in 2013 — demonstrates that governance capacity for data governance in banking has not been achieved even where comprehensive standards exist and a decade of supervisory pressure has been applied. This is the empirical anchor for the Governance_Capacity concept in the data dimension: institutional capacity to implement data governance standards lags regulatory aspiration by a decade-plus even in the most supervised institutions globally.

India dimension: India's large public sector banks (SBI, Bank of Baroda, PNB) are not G-SIBs but are subject to RBI's own data governance and MRM requirements. The BCBS 239 compliance gap at G-SIBs is directionally predictive of the compliance gap in Indian PSBs.

### Institutional_Coherence — Cross-authority collaboration gap
The document explicitly identifies that financial authorities and data protection authorities (DPAs) operate in institutional silos: financial AI regulation and data privacy regulation proceed on parallel tracks without systematic coordination. The UK's DRCF (Digital Regulation Cooperation Forum) — bringing together ICO, FCA, CMA, and Ofcom — is cited as the exception and model for inter-regulatory coherence. No other jurisdiction has a comparable permanent coordination structure.

This is a direct empirical instantiation of the Institutional_Coherence gap concept: two regulatory tracks (financial AI → FCA/PRA; data privacy → ICO/DPA) converge on the same technology (AI data use in financial services) without integrated governance. For P3: apply this framework to India, where RBI (financial AI regulation) and MeitY/DPDP authority (data protection) are structurally separate with no coordination mechanism analogous to DRCF.

### fsQCA — Cross-jurisdictional regulatory configurations
The five-jurisdiction comparison provides direct empirical data for fsQCA condition-set construction:

| Configuration | Jurisdictions | Conditions |
|---|---|---|
| Binding sector-specific + integrated data governance | China (NFRA) | sector_specific=1, binding=1, integrated_DG=1 |
| Principles + industry co-creation + inter-regulator coordination | Singapore (MAS) + UK (DRCF) | voluntary=1, industry_co_design=1, inter_regulator_coord=1 |
| Horizontal legislation (high-risk binding) + sectoral pending | EU | horizontal_law=1, sector_specific=0.5 |
| Fragmented principles + state-level binding | US | fragmented=1, state_binding=partial |
| India (absent — gap) | India | No equivalent BFSI AI data governance instrument identified |

The India absence is analytically productive: it defines a null condition set for the fsQCA that can be tested against governance outcomes (DPDP 2023 enacted; RBI AI guidance partial; no equivalent to MAS FEAT or NFRA data governance guidance).

---

## S7. Research Project Linkages

| Project | Relevance |
|---|---|
| **P1 (SLR)** | 2026 baseline on cross-jurisdictional AI data governance gap; piecemeal policy architecture as structural finding; five-priority-areas framework for literature positioning |
| **P3 (BFSI)** | Direct BFSI AI data governance evidence; India absence from five-jurisdiction comparison; RBI vs. NFRA/MAS comparison; DPDP 2023 and AI data governance intersection |
| **fsQCA** | Five-jurisdiction regulatory configuration data; binding vs. principles-based; sector-specific vs. cross-sectoral; inter-regulator coordination as condition |

---

## S8. Key Concepts

- [[Governance_Debt]] — piecemeal policy landscape; "existing policy responses are often piecemeal"; 2026 cross-jurisdictional empirical baseline
- [[Governance_Capacity]] — BCBS 239: only 2/31 G-SIBs fully compliant decade after publication; data governance capacity gap in banking
- [[Institutional_Coherence]] — financial authority vs. DPA parallel tracks; DRCF as exception model; India gap
- [[Accountability]] — board accountability for data governance; shared responsibility model for third-party AI data; GPA accountability definition
- [[Transparency]] — GPA transparency requirements; model documentation; data lineage disclosure; right to explanation for AI-driven decisions
- [[Regulatory_Parallelism]] — cross-sectoral data privacy + sector-specific financial AI governance operating in parallel without integration

---

## ⚠ VERIFY Flags

| # | Flag | Priority |
|---|---|---|
| ⚠V-I8-1 | Confirm "79% of financial institutions identify data quality as key barrier to AI production" — verify IIF-EY 2025 as source (vs. IIF-EY 2023 cited in Int'l_9) and exact survey scope | High |
| ⚠V-I8-2 | Confirm BCBS 239 Box 3: "only 2 of 31 G-SIBs fully compliant" — verify exact figure and reference date | High |
| ⚠V-I8-3 | Confirm 144 countries have national data privacy laws (IAPP 2025) — verify figure and IAPP source | Medium |
| ⚠V-I8-4 | Confirm MAS 2025a consultation paper on AI risk management — verify publication status and title | High |
| ⚠V-I8-5 | Verify DRCF composition (ICO + FCA confirmed; verify CMA and Ofcom as members) | Low |
| ⚠V-I8-6 | Confirm that India (RBI/MeitY) has no coordination mechanism analogous to DRCF — check for any MoU or bilateral arrangement | Medium |

---

## S9. Connections

**Corpus nodes:**
- [[International_9]] — FSI Insights No. 63 (Dec 2024); predecessor document by same lead author; general AI regulation in finance
- [[International_7]] — IFC Report No. 18 (Apr 2025); central bank AI governance survey; data governance as one of four IFC pillars
- [[RBI_1]] through [[RBI_4]] — RBI regulatory instruments; India BFSI AI governance; compare to NFRA (China) data governance approach
- [[SEBI_14]] — India BFSI side

**Concepts:**
- [[Governance_Debt]] — piecemeal AI data governance; global 2026 baseline
- [[Governance_Capacity]] — BCBS 239 compliance gap
- [[Institutional_Coherence]] — cross-authority AI-DPA coordination gap; DRCF model
- [[Accountability]], [[Transparency]]
- [[Regulatory_Parallelism]] — cross-sectoral vs. sector-specific governance tracks

**Institutions:**
- [[_Institutions_MOC]] — International row (BIS/FSI publication)

**Projects:**
- [[02_Projects/P1_SLR_RG]]
- [[02_Projects/P3_BFSI_JEIM]]
- [[fsQCA_Regulatory_Configurations]]

---

_Added: Batch 9 — 2026-06-18 | FSI Insights No. 73 (March 2026) | Most recent BIS corpus document | ⚠V-I8-1 priority: confirm 79% data quality barrier figure and IIF-EY 2025 source_
