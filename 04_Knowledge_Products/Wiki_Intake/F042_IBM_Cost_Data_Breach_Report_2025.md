---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S4
  - section/S5
  - tier/high-medium
  - project/p3
  - project/fsqca
---

# IBM Cost of a Data Breach Report 2025: The AI Oversight Gap

**Node ID:** F042  
**Type:** Wiki Intake Note  
**Wiki Section:** S4 (Agentic AI / Enterprise AI Risk) / S5 (Data, Privacy & Security)  
**Status:** Active  
**Tier:** High-Medium  
**Last Updated:** 2026-06-19  

---

## Source

**Full Citation (APA):** IBM. (2025). *Cost of a data breach report 2025: The AI oversight gap*. IBM Corporation.  
**Document Type:** Annual industry benchmark report (quantitative survey)  
**Issuing Institution:** IBM (sponsor); Ponemon Institute (methodology/fieldwork)  
**Publication Date:** 2025 (exact month not stated in document — ⚠ VERIFY #166)  
**URL / DOI:** ibm.com/security/data-breach (⚠ VERIFY #166 — confirm stable URL)  

---

## Executive Summary

IBM's 2025 Cost of a Data Breach report presents findings from a survey of 600 organisations across 16 countries and 17 industries, examining the financial and operational impact of data breaches with a specific focus on the governance gap in AI oversight. The report identifies a structural disconnect between AI deployment velocity and AI security governance maturity: 63% of sampled organisations lack formal AI governance policies, and 97% of organisations that experienced an AI-related breach lacked adequate AI access controls at time of incident. The 2025 edition introduces "Shadow AI" — unauthorised or ungoverned AI tool usage — as a new cost category, attributing an average USD 670,000 premium per breach to Shadow AI exposure. The intended audience is enterprise security, risk, and technology leadership; the governance problem addressed is the AI security and accountability gap in large-enterprise environments.

---

## Key Frameworks and Findings

### Sample and Scope

| Parameter | Value |
|---|---|
| Organisations surveyed | 600 |
| Countries | 16 |
| Industries | 17 |
| Methodology | ⚠ VERIFY #165 — Ponemon Institute survey; self-reported cost data |
| Reference period | ⚠ VERIFY #165 — confirm breach period covered |

### Financial Benchmarks

| Geography / Category | Average Breach Cost |
|---|---|
| Global average | USD 4.44 million |
| United States | USD 10.22 million |
| India | USD 2.51 million |
| Shadow AI premium | + USD 670,000 |
| Healthcare sector | Highest sector globally (perennial leader) |

### AI Governance Gap Findings

| Finding | Statistic |
|---|---|
| Organisations lacking formal AI governance policies | 63% |
| AI-breach organisations that lacked AI access controls | 97% |
| Organisations with mature AI security posture | Minority (exact % ⚠ VERIFY #165) |

### Shadow AI — New Cost Category (2025)

Shadow AI is defined as AI tools and systems deployed without organisational knowledge, approval, or security review. The 2025 edition is the first iteration of the IBM report to quantify Shadow AI as a distinct breach cost multiplier. Key characteristics:
- Bypasses organisational AI governance frameworks
- Creates unmonitored data flows and access paths
- Compounded by the absence of AI access controls (97% finding above)
- Governance gap: No SEBI/RBI equivalent of a Shadow AI monitoring obligation yet exists in India's financial sector

### Breach Lifecycle and Detection

The report maintains its longitudinal framework examining:
- **Mean time to identify (MTTI)** and **mean time to contain (MTTC)** breach lifecycle metrics
- AI-assisted detection correlates with shorter breach lifecycle and lower costs (IBM finds AI-augmented detection reduces costs materially — ⚠ VERIFY #165 for specific figures)
- Organisations without AI-assisted detection face longer dwell times

### Industry Comparators

Healthcare consistently registers the highest average breach cost globally; Financial Services ranks second or third (⚠ VERIFY #165 for precise 2025 ranking). For India-BFSI context, USD 2.51 million India average understates exposure for systemically important financial entities, which face additional regulatory notification and remediation obligations under RBI CSCRF.

---

## India Relevance and Governance Gap Analysis

The India average of USD 2.51 million is relevant to P3 BFSI JEIM as a cost-of-inaction calibration. However, the India sample size within a 600-organisation global survey is not disclosed (⚠ VERIFY #166 — India sample may be insufficient for statistically independent India estimates; IBM India-specific supplementary data should be sought).

**Key India governance gaps exposed:**

1. **Shadow AI** — RBI CSCRF (2024) and SEBI AI guidelines (2025) do not define or mandate controls for Shadow AI. IBM's USD 670K Shadow AI premium represents a quantifiable unmitigated risk in Indian regulated financial entities.

2. **AI governance policy gap** — 63% global figure for organisations lacking AI governance policies is consistent with India BFSI context, where SEBI's AI guidelines are aspirational rather than prescriptive, and RBI's CSCRF focuses on cybersecurity rather than AI governance holistically.

3. **AI access controls** — 97% of AI-breach organisations lacked adequate AI access controls at breach time. RBI CSCRF Section 4 (Access Management) does not yet address AI-specific access control requirements distinct from general identity and access management.

4. **Accountability gap** — absence of AI-specific breach notification obligations in India. DPDP Act 2023 s.8(6) requires personal data breach notification to DPBI and data principals but does not specify AI-system-origin breach as a distinct notification trigger.

Cross-reference: [[International_11]] (FSB TPRM — third-party AI vendor exit and oversight) and [[F045_PwC_TPRM_Digital_Geopolitical_Era_2025]] (EU DORA third-party incident reporting requirements).

---

## Research Programme Applications

| Project | Application |
|---|---|
| P1 (SLR RG) | AI governance maturity baseline data; Shadow AI as emergent governance concept; cost-of-governance-gap quantification |
| P3 (BFSI JEIM) | Primary — India BFSI breach cost calibration; Shadow AI risk for BFSI entities; AI access control gap; integrates with RBI CSCRF Section 4 gap analysis |
| P4 (Doctrinal IJLIT) | Limited — USD 2.51M India breach cost contextualises regulatory incentive arguments in AI liability doctrine discussion |
| fsQCA | EA condition — breach cost and AI governance policy absence as proxy for External Accountability deficit; OC condition — 63% policy absence figure useful for calibrating Organisational Commitment condition |

---

## Concept Links

- [[Accountability]] — 97% of AI-breach organisations lacked AI access controls; absence of accountability infrastructure (access controls, governance policies) directly produced measurable breach cost outcomes
- [[Transparency]] — Shadow AI premium quantifies the cost of non-transparent AI deployment; 63% policy absence implies opacity in AI governance to boards and regulators
- [[Governance_Capacity]] — 63% without AI governance policies signals systemic governance capacity deficit at the organisational level; IBM finding directly supports Governance_Debt arguments at enterprise level
- [[Governance_Debt]] — Shadow AI as a new vector: organisations deploying AI faster than governance can follow accumulate AI-specific governance debt, now financially quantified at USD 670K per breach
- [[Regulatory_Parallelism]] — India's four regulatory silos (RBI, SEBI, MeitY, IRDAI) have not coordinated a common AI access control or Shadow AI monitoring standard; IBM's global data arrives without an India-specific regulatory response
- [[Agentic_AI_Governance]] — While report predates agentic-AI proliferation concern, Shadow AI concept foreshadows agentic AI deployment outside organisational control perimeters

---

## ⚠ VERIFY BEFORE PUBLISHING

- **V-B14-01 / #165 — Survey self-report bias; Ponemon methodology — MEDIUM.** All cost figures are self-reported by survey respondents. Ponemon Institute methodology uses structured interviews and cost-allocation guidance to mitigate self-report bias, but figures are estimates, not audited financials. Verify: confirm Ponemon methodology description in 2025 edition; note in any citation that figures are survey-based estimates.
- **V-B14-02 / #166 — India sample size; exact publication month — LOW.** The India-specific average (USD 2.51M) is drawn from an undisclosed India subsample within the 600-organisation global survey. Verify: seek IBM India-specific supplementary publication or confirm India sample size before using India figure as independent statistical benchmark. Also confirm exact publication month for APA citation.

---

## Cross-Links to Corpus

- [[F045_PwC_TPRM_Digital_Geopolitical_Era_2025]] — EU DORA third-party incident reporting requirements; TPRM governance framework complements IBM's AI access control findings
- [[F044_Microsoft_AI_Security_Risk_Assessment]] — Microsoft ATML provides the ML attack surface taxonomy that contextualises IBM's breach cost data (what attack types produce what categories of breach exposure)
- [[F048_FLI_AI_Safety_Index_Winter_2025]] — FLI finds no frontier AI company meets EU AI Code of Practice; IBM finds 97% of AI-breach organisations lacked access controls — together, governance gap at company and developer level is corroborated
- [[International_11]] — FSB TPRM; IBM AI access control gap at enterprise level complements FSB's third-party AI vendor governance gap at systemic level
