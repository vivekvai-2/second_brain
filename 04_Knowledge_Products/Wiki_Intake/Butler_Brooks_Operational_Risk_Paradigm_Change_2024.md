---
file_id: F049
title: "Time for a Paradigm Change: Problems with the Financial Industry's Approach to Operational Risk"
authors: Butler, T., & Brooks, R.
year: 2024
outlet: "Risk Analysis"
outlet_rank: "Not ABDC-ranked (confirmed against full ABDC 2022 Journal Quality List text via Perplexity Deep Research, 2026-07-31 — #178 resolved)"
doi: "10.1111/risa.14240"
document_type: Academic Paper
format: B
wiki_sections: [S1, S6]
tags: [3LoD, operational-risk, risk-accounting, governance-failure, organizational-learning, AI-enabled-risk, enterprise-data-fabric, Model-I-II, Kabuki-theatre, Credit-Suisse, BCBS]
corpus_cluster: Cluster_2
priority: A
project_relevance: [P3, P4]
date_added: 2026-06-24
batch: B15
batch_marker: ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕
---

# F049 — Butler & Brooks (2024): "Time for a Paradigm Change"
*Operational Risk, 3LoD Failure, and Risk Accounting*

> **Wiki Intake Note — Format B**
> Butler, T., & Brooks, R. (2024). Time for a paradigm change: Problems with the financial industry's approach to operational risk. *Risk Analysis, 44*, 1285–1304. https://doi.org/10.1111/risa.14240

---

## 1. Core Argument

The financial industry's approach to operational risk management (ORM) is fundamentally broken: it is backward-looking, siloed, ceremonially compliant, and structurally unable to prevent the large-scale operational failures it purports to govern. The Three Lines of Defence (3LoD) model — the dominant governance architecture for operational risk — has failed because it privileges formal structure over substantive risk culture. The authors propose a paradigm shift to **Risk Accounting** using standardised, quantitative **Risk Units (RU)** implemented through AI-enabled enterprise data architectures.

The paper situates this failure in organisational learning theory (Argyris & Schön, 1978): banks operate on **Model I** logic (single-loop learning, defensive, competitive, non-transparent) rather than the **Model II** logic (double-loop learning, collaborative, error-embracing) that genuine risk governance requires. The gap between *espoused theory* (what banks say their risk frameworks do) and *theory-in-use* (actual risk behaviour) is the primary driver of persistent operational risk losses.

---

## 2. Evidence Base

| Metric | Value | Source |
|--------|-------|--------|
| Gross operational losses, 30 G-SIBs, 10-year period | €522.6 billion | ORX (2022) |
| Gross operational losses, 34 largest US banks | $281 billion | Curti et al. (2022) |
| European banks not modelling op-risk capital allocation | ~80% | Woodall (2020), Risk.net — independently corroborated 2026-07-31, see VERIFY #179 resolution below |
| Credit Suisse operational risk events (Feb 2020–Jun 2022) | 8 major events | Paper's case analysis |
| Credit Suisse: total cost to UBS merger | ~$17 billion | Paper's case analysis |
| Rise in operational risk events, 2022 | +26.4% YoY | ORX (2022) |

The Credit Suisse collapse (culminating in the 2023 UBS-forced merger) is the paper's flagship case study. The authors document 8 discrete operational risk events over 28 months that eroded approximately $17bn in value, each attributable to Model I governance culture — not idiosyncratic bad actors.

---

## 3. The 3LoD Critique: "Kabuki Theatre"

Butler & Brooks deploy the "Kabuki theatre" metaphor — borrowed directly from banking practitioners — to characterise how 3LoD produces *ceremonial* compliance rather than *substantive* risk control:

> "Tick-box efforts are valued over efficacy."

Key structural failures identified:

1. **Accountability displacement**: First-line business managers are structurally dis-incentivised from owning risk; the second line (Risk function) takes ownership, creating moral hazard.
2. **Data fragmentation**: Risk data exists across incompatible siloed systems; no enterprise-wide risk aggregation; BCBS 239 compliance (risk data aggregation) remains aspirational for most banks.
3. **Backward-looking capital modelling**: Operational risk capital under Basel is modelled on historical loss data (AMA / SMA methods), not forward-looking risk states.
4. **Cultural entrenchment**: Schein's (1984) three-layer culture model — artifacts, espoused values, underlying assumptions — shows op-risk frameworks are artifacts only; underlying assumptions remain Model I.
5. **Regulatory epistemic gap**: Bank of England "Dear CEO" letters (2021, 2022) confirm the regulator itself documents the espoused-theory vs theory-in-use gap at industry level.

This critique extends and operationalises the Davies & Zhivitskaya (→[[04_Knowledge_Products/Wiki_Intake/Davies_Zhivitskaya_3LoD_2018]]) finding that 3LoD governance is structurally ambiguous at the board level, down into the operational execution layer.

---

## 4. The Risk Accounting Proposal

**Risk Accounting** (Hughes, 2021, 2023) reframes operational risk as a quantifiable resource, analogous to financial accounting:

### 4.1 Risk Unit (RU) Metrics

| Metric | Formula | Variables |
|--------|---------|-----------|
| **Inherent Risk (IR)** | IR = EUF × VBW | EUF: Event Uncertainty Factor (0–20 scale); VBW: Value Being Warehoused (0–163.6 scale) |
| **Residual Risk (RR)** | RR = (IR / 100) × (100 − RMI) | RMI: Risk Mitigation Index (0–100) |
| **Risk Unit** | Standardised non-financial measure | Enables cross-firm, cross-period comparability |

The EUF and VBW scales are proprietary (Hughes/Risk Accounting Standards Board) — the paper describes the architecture but cites published Risk Accounting standards for calibration detail.

### 4.2 AI-Enabled Enterprise Data Fabric

Implementation requires an integrated technology architecture:

- **Enterprise Data Fabric**: Integrates structured and unstructured risk data across the enterprise in near-real-time
- **ML components**: Predictive risk modelling, anomaly detection in risk event data
- **NLP components**: Automated extraction from loss event descriptions, control attestations, audit findings
- **Ontological layer**: Common risk taxonomy enabling cross-silo data harmonisation
- **Risk Accounting Calculation Engine (RACE)**: Automated RU computation from aggregated inputs

This architecture directly addresses BCBS 239 data aggregation requirements and is positioned as the technical enabler for genuine (not ceremonial) 3LoD execution.

---

## 5. Theoretical Scaffolding

| Theory | Authors | Application in Paper |
|--------|---------|---------------------|
| Organisational learning (Model I / II) | Argyris & Schön (1978) | Single-loop vs double-loop learning in risk culture; espoused theory vs theory-in-use |
| Organisational culture (3 layers) | Schein (1984) | Artifacts / espoused values / underlying assumptions as diagnostic frame for 3LoD failure |
| Institutional theory (isomorphism) | DiMaggio & Powell (1983) | Implied — ceremonial compliance driven by normative / coercive isomorphism from regulators |
| Paradigm theory | Kuhn (1970) | Framing device: 3LoD is an incommensurable paradigm requiring replacement, not reform |

---

## 6. PRIS Concept Connections

### [[Governance_Debt]]
This paper provides the **seventh documented variant** of [[Governance_Debt]] in the Batch 15 corpus: **espoused-theory vs theory-in-use divergence as governance debt mechanism**. The gap is not merely cultural slack — it is a structural, institutionally-reproduced condition documented by regulators themselves (Bank of England "Dear CEO" letters). The 3LoD framework creates governance debt by: (a) displacing accountability from first line, (b) producing data siloes that prevent early warning, (c) requiring backward-looking capital modelling that cannot price forward risk. Unlike prior GD variants that locate debt at regulatory/policy levels (→[[04_Knowledge_Products/Wiki_Intake/F042_IBM_Cost_Data_Breach_Report_2025]], [[04_Knowledge_Products/Wiki_Intake/F047_BAIR_Berkeley_Responsible_GenAI_Playbook_2025]], [[04_Knowledge_Products/Wiki_Intake/F048_FLI_AI_Safety_Index_Winter_2025]]), Butler & Brooks locate it at the enterprise governance execution layer.

### [[Governance_Capacity]]
The ~80% of European banks not modelling their op-risk capital allocation (independently corroborated via EBA data, #179 resolved) constitutes the most direct empirical evidence of **deep governance incapacity** in the operational risk layer encountered in the Batch 1–15 corpus. Governance capacity failure here is not about missing frameworks (the frameworks exist) but about institutionally-entrenched inability to execute them substantively.

### [[Accountability]]
The paper's core structural diagnosis is an accountability failure: 3LoD moves accountability *away* from those closest to risk (first line) toward a bureaucratic second-line function that cannot possess the operational knowledge needed to govern effectively. This maps directly onto the accountability deficit documented in →[[04_Knowledge_Products/Wiki_Intake/Davies_Zhivitskaya_3LoD_2018]] (Davies & Zhivitskaya) and the board-level accountability gap in →[[04_Knowledge_Products/Wiki_Intake/Schuett_Three_Lines_Defense_AI_2023]] (Schuett).

### [[Transparency]]
Risk Accounting as proposed is fundamentally a transparency mechanism: standardised RUs enable cross-firm comparability, external scrutiny, and regulator-accessible forward-looking risk data. This mirrors the transparency design logic in the EU AI Act's conformity assessment regime (→[[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance]]) and MAS FEAT (→International_8).

### [[Regulatory_Parallelism]]
Indirect relevance only. The paper is single-institution focused; it does not address multi-regulator fragmentation. However, the AI-enabled Enterprise Data Fabric architecture has structural implications for [[Regulatory_Parallelism]]: a firm that has genuinely integrated risk data across the enterprise is better positioned to produce coherent, consistent regulatory reporting to multiple overlapping regulators simultaneously. This is a **second-order RP mitigation mechanism** worth flagging for the fsQCA paper.

---

## 7. Research Project Applications

### P3 — BFSI AI Governance Regulatory Parallelism (JEIM)
- F049's 3LoD critique deepens the governance infrastructure argument: the governance frameworks through which AI risk is supposed to be managed are themselves institutionally compromised. If 3LoD fails for conventional operational risk, it is *a fortiori* under-resourced for AI risk (where event uncertainty is higher, data aggregation harder, and accountability more diffuse). This builds the P3 argument that BFSI AI governance requires *new* governance architectures, not merely AI-adaptation of existing frameworks.
- AI-enabled Enterprise Data Fabric: directly relevant to P3's technical governance architecture argument.

### P4 — BFSI AI Governance Doctrinal (IJLIT)
- The "Dear CEO" regulatory letters as evidence of a documented, regulator-acknowledged espoused-vs-actual gap is useful legal/doctrinal evidence: regulators are not merely aspirational in their frameworks — they actively acknowledge that operational compliance diverges from substantive governance. This weakens doctrinal arguments that current frameworks are adequate.

### fsQCA (Thesis Chapter)
- The ceremonial compliance variable: Butler & Brooks offer a measurable proxy (op-risk event frequency + loss magnitude vs capital adequacy) for distinguishing genuine from ceremonial governance configurations. Potentially usable as a condition calibration anchor for the governance-quality dimension in fsQCA.

---

## 8. Consulting Relevance

| Inbound | Relevance |
|---------|-----------|
| **AEGIS_OS** | High — Risk Accounting / RACE architecture is a pre-execution governance enforcement model; the Enterprise Data Fabric design maps directly onto AEGIS's proposed AI model registry + monitoring architecture. The RU metric could inform AEGIS's AI risk scoring approach. |
| PrivacyWeave | Low — operational risk focus, not privacy/data-governance |
| CyberMesh | Medium — BCBS 239 data aggregation architecture overlaps with CyberMesh's enterprise risk data integration challenges |

---

## 9. AI Governance Wiki Classification

| Field | Classification |
|-------|---------------|
| **Primary Wiki Section** | S6 — Implementation & Governance Artifacts (3LoD design, risk framework architecture) |
| **Secondary Wiki Section** | S1 — Governance Fundamentals (cultural change, paradigm shift, governance theory) |
| **Instrument Type** | Academic Paper — Conceptual/Prescriptive + Empirical (case evidence) |
| **Jurisdiction** | Global (Basel/G-SIB focus; CS case in Switzerland/EU) |
| **Regulator/Author** | University College Cork (Butler) / Accenture (Brooks) |
| **AI Governance Maturity** | Framework critique + prescriptive architecture |

---

## 10. Key Quotations

> "The 3LoD model is not unlike Kabuki theatre — there are formal roles, structured performances, and an audience that knows the rituals — but the real risk decisions are made offstage." *(paraphrase of practitioner voice cited in paper)*

> "…tick-box efforts are valued over efficacy." *(p. 1291)*

> "The banking industry's response to operational risk is essentially backward-looking: it uses historical loss data to model capital requirements, while leaving the first line to manage risk through increasingly elaborate but fundamentally ceremonial control frameworks." *(paraphrase, pp. 1288–1290)*

---

## 11. VERIFY Flags

- **#178 — RESOLVED (2026-07-31, Perplexity Deep Research against full ABDC 2022 Journal Quality List text).** *Risk Analysis* (SRA/Wiley) does **not** appear anywhere on the official ABDC 2022 list — confirmed not ABDC-ranked, High confidence. Consistent with this node's own prior evidence-base note that it "failed the 50% business-element test." Cite as a non-ABDC-ranked risk-management journal, not as an ABDC-tier academic outlet.
- **#179 — RESOLVED (2026-07-31, Perplexity Deep Research).** Independently corroborated, High confidence: a Risk.net article (Louie Woodall, December 2020) states "less than 20% of European banks use models to calculate their operational risk capital requirements," based on EU-wide EBA transparency-exercise data covering 135 named banks across the EU/EEA/UK, of which only 23 used advanced modelling approaches — mathematically equivalent to "~80% not modelling." Critically, the underlying figure traces to **official EBA transparency-exercise data**, not merely Woodall's own analysis, making it independently verifiable via EBA source data even though the Risk.net article itself remains paywalled. Safe to cite without the "verify independently" qualifier.
- **#180 — RESOLVED (2026-07-31, editorial convention).** Standard academic practice cites the printed volume/issue year, not the earlier copyright year — this node's own Citation section already correctly uses **2024** (matching *Risk Analysis*, 44, 1285–1304). No change needed — flag closed as already-compliant.

---

## 12. Citation

Butler, T., & Brooks, R. (2024). Time for a paradigm change: Problems with the financial industry's approach to operational risk. *Risk Analysis, 44*, 1285–1304. https://doi.org/10.1111/risa.14240

**Linked nodes**: [[04_Knowledge_Products/Wiki_Intake/Davies_Zhivitskaya_3LoD_2018]] [[04_Knowledge_Products/Wiki_Intake/Schuett_Three_Lines_Defense_AI_2023]] F009 (unlinked — no vault note found under this ID; likely dead reference from early corpus planning, see link audit 2026-07-31) [[04_Knowledge_Products/Wiki_Intake/Bantleon_et_al_3LoD_Coordination_2020]] F013 (unlinked — same as F009) [[04_Knowledge_Products/Wiki_Intake/F042_IBM_Cost_Data_Breach_Report_2025]] [[04_Knowledge_Products/Wiki_Intake/F047_BAIR_Berkeley_Responsible_GenAI_Playbook_2025]] [[04_Knowledge_Products/Wiki_Intake/F048_FLI_AI_Safety_Index_Winter_2025]] [[Governance_Debt]] [[Governance_Capacity]] [[Accountability]] [[Transparency]] [[Regulatory_Parallelism]] [[Institutional_Coherence]]

---
*Batch 15 — PRIS Corpus Intake | Processed: 2026-06-24*
