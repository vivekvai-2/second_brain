---
type: Framework
tags:
  - type/framework
  - status/active
  - paper/p3-primary
  - paper/p4-primary
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/linkedin
  - engine/consulting
  - content/carousel-ready
  - content/wiki-entry
  - content/checklist
---

# SEBI AI Circular

**Type:** Framework **Status:** Active **Last Updated:** 2026-06-12

---

## Core Synthesis

The SEBI AI governance instruments — anchored by the 2019 AI/ML Reporting Circular and extended by the February 2025 accountability amendments (Regulation 16C) — constitute the capital markets regulator's evolving AI governance architecture for Indian securities intermediaries. Within PRIS, SEBI's AI instruments are the second member of the P3 coordination pair that generates the Regulatory Parallelism finding: they govern AI deployment in the same regulated entities as RBI FREE-AI (major banks operating as SEBI intermediaries) with zero cross-reference to RBI's parallel obligations. The analytical significance of the SEBI AI Circular within PRIS is therefore inseparable from its relationship to RBI FREE-AI: it is the other pole of the parallelism construct, and its architectural characteristics — earlier, less taxonomically developed, but rapidly evolving — define the second coordinate in the coordination-pair matrix.

## Framework Identity

- **Issuing body:** Securities and Exchange Board of India (SEBI)
- **Instrument type:** Regulatory circular / gazette notification — binding within SEBI's jurisdictional mandate (securities intermediaries, stock exchanges, depositories, portfolio managers, investment advisors)
- **Jurisdiction:** India — capital markets, securities trading infrastructure, investment advisory services under SEBI regulation
- **Binding status:** Binding within SEBI's jurisdiction; non-compliance subject to SEBI enforcement action
- **Key dates:**
    - January 2019: SEBI AI/ML Reporting Circular — first SEBI AI governance instrument; taxonomy; mandatory quarterly reporting for algorithmic trading AI _(verify gazette reference via Perplexity)_
    - February 2025: Regulation 16C — sole accountability amendment: intermediaries bear full liability for AI/ML output, including third-party AI tools
    - February 2025: Retail Algo Trading Circular — OAuth API governance, broker empanelment requirements
    - October 2025: SEBI Cybersecurity Framework — 24/7 SOC requirement, quarterly board cyber reviews, Zero Trust architecture
    - 2025: AI-ML Reporting Framework harmonised across NSE, BSE, MCX, NCDEX

## Structural Overview

SEBI's AI governance architecture has evolved in two phases, producing a layered instrument set rather than a single coherent framework.

**Phase 1 (2019 baseline):** The 2019 circular established the foundational vocabulary — AI/ML system classification, quarterly reporting obligations, and algorithmic trading governance. Its structural logic was **disclosure and reporting**: intermediaries must categorise, document, and periodically report AI/ML systems to SEBI. This is a transparency-first architecture, not a risk-management architecture.

**Phase 2 (2025 evolution):** Three 2025 instruments substantially extend the baseline. Regulation 16C introduces a **sole accountability** principle: intermediaries are solely responsible for AI/ML outputs, including outputs from third-party tools they deploy. This is a significant liability architecture — it closes the vendor-accountability gap by assigning all consequences to the regulated intermediary, but it creates a downstream vendor-risk management obligation that is not itself specified. The Retail Algo Trading Circular adds **access governance** (OAuth requirements, empanelment of algorithmic providers) — a structural control layer for AI delivery mechanisms. The Cybersecurity Framework adds **operational resilience** requirements with direct AI-system implications (SOC monitoring of algorithmic systems, board-level cyber review).

The structural logic of SEBI's architecture as of mid-2026 is **accountability without coordination**: each instrument adds an accountability or reporting obligation, but none references RBI's parallel requirements for AI systems that operate across both regulatory domains (a bank's AI-driven portfolio recommendation system is simultaneously a SEBI-regulated advisory function and an RBI-regulated financial services function).

## Regulatory Position & Comparative Significance

Within the PRIS framework set, the SEBI AI Circular occupies the capital-markets-sectoral-binding position — the direct pair to RBI FREE-AI in the Indian BFSI coordination analysis. Against FREE-AI, the SEBI instruments are earlier in origin (2019 vs 2025), less architecturally developed (no equivalent risk taxonomy), but more explicit on liability attribution (sole accountability under Regulation 16C). Against IndiaAI, SEBI's instruments are binding where IndiaAI is advisory — but they are also sector-constrained where IndiaAI aspires to cross-sectoral coherence. The SEBI AI Circular's significance within PRIS is therefore primarily relational: it is the instrument whose parallelism with FREE-AI defines the empirical core of P3 and P4.

## IG 2.0 Coding Summary

Full ADICO-level coding is in NVivo. At the construct level, SEBI's AI instruments are expected to generate moderate **Deontic** density — the 2019 circular uses reporting-obligation language (shall report, must classify) while Regulation 16C uses accountability-assignment language (solely responsible, shall not disclaim). **Attribute** specification is clearer in the 2025 instruments — "intermediary" is the defined Attribute holder with unambiguous accountability. **Or-else** components are implicit (SEBI enforcement authority, listing requirements, exchange sanctions). **Condition** specification is present through the reporting taxonomy (AI system type, trading algorithm category) but is less developed than FREE-AI's eight-category risk taxonomy. The overall ADICO profile is expected to position SEBI's instruments below FREE-AI on RL (less taxonomically detailed, less explicit on supervisory expectations) but comparably strong on the accountability/Deontic dimension.

## fsQCA Calibration

This framework is a candidate case in the 10-case fsQCA model. Case-level calibration is pending NVivo IG 2.0 coding (Q3 2026). Anchors: 0.00 / 0.33 / 0.67 / 1.00.

|Condition|Score|Status|
|---|---|---|
|EA — Ethical Alignment|⏳|Pending Q3 2026|
|SR — Stakeholder Role Clarity|⏳|Pending Q3 2026|
|RL — Regulatory Logic|⏳|Pending Q3 2026|
|SI — Stakeholder Inclusion|⏳|Pending Q3 2026|

_Prior (to be confirmed against coded data, not a result):_ Expected moderate-high RL (binding, accountability-focused, but less risk-taxonomy depth than FREE-AI), moderate SR (sole-accountability attribution is clear but internal governance role specification is less detailed than FREE-AI's six-pillar architecture), low EA (ethical AI principles not explicitly articulated in SEBI instruments — conduct/liability framing dominates), low SI (no institutionalised stakeholder participation). If confirmed, the SEBI profile will position it below FREE-AI on RL and SR but above non-binding international instruments — a distinct middle position in the truth table.*

## Coordination Pair Classification

The SEBI AI Circular is a **P3 corpus member** — one of 18 binding instruments in the RBI/SEBI/CERT-In corpus (2012–2024). Its coordination-pair relationship with RBI FREE-AI is the empirical centre of the Regulatory Parallelism construct.

**Key empirical finding (from P3 corpus, not repeated here in full — see [[P3_BFSI_JEIM]]):**

- SEBI instruments participate in multiple coordination pairs with RBI FREE-AI covering functionally equivalent AI governance domains: model risk governance, algorithmic surveillance, third-party AI accountability, data governance
- Across all identified coordination pairs, **zero cross-references** from SEBI instruments to RBI instruments are documented (and zero in the reverse direction)
- Three SEBI→CERT-In references exist in the corpus, confirming that cross-referencing is institutionally possible for SEBI — making the zero RBI-SEBI cross-references a structural choice or institutional logic gap rather than a technical oversight
- Classification: Parallelism — the dominant coordination pattern (23 of 40 pairs classified as parallelism)

## Key Tensions & Gaps

The sole-accountability principle in Regulation 16C is architecturally significant but creates an unresolved vendor-risk governance gap: intermediaries are fully liable for third-party AI outputs but SEBI has not specified how vendor due diligence, audit rights, or contractual protections must be structured to operationalise this liability. This gap — identified in the HNLU CCLS analysis referenced in the AI Governance Wiki — is expected to be addressed through a vendor-accountability consultation in 2026. A second tension is the cross-domain entity problem: major Indian banks are simultaneously RBI-regulated entities (subject to FREE-AI) and SEBI-regulated intermediaries (subject to Regulation 16C) operating the same AI-enabled systems under two non-coordinated frameworks. This is not a gap SEBI can resolve unilaterally — it requires the cross-regulator coordination mechanism that P4 proposes.

## Linked Projects

- [[P3_BFSI_JEIM]]
- [[P4_Doctrinal_IJLIT]]
- [[fsQCA_Thesis_Chapter]]

## Linked Domains

- [[AI_Governance]]
- [[BFSI_Governance]]

## Linked Concepts

- [[Regulatory_Parallelism]]
- [[Governance_Debt]]
- [[Institutional_Coherence]]
- [[Accountability]]
- [[Transparency]]

## Linked Frameworks

- [[RBI_Free_AI]]
- [[IndiaAI_Framework]]
- [[EU_AI_Act]]

## Linked Institutions

- [[SEBI]]
- [[RBI]]
- [[CERT_IN]]

## Linked Methods

- [[Institutional_Grammar_IG2]]
- [[fsQCA]]

## Future Research / Reuse Opportunities

In the fsQCA truth table, the SEBI AI Circular's calibration profile will be compared directly to RBI FREE-AI — the two Indian sectoral cases. If they calibrate differently on RL or SR despite governing the same domain, this would be a novel empirical finding: structural heterogeneity between parallel sectoral instruments as a measurable property, not merely an assertion. For P4, the sole-accountability principle under Regulation 16C is a specific doctrinal provision requiring analysis in the fragmentation diagnosis section (intermediaries face contradictory accountability signals from two non-coordinating regulators). For the BFSI AI Governance Handbook, SEBI's quarterly reporting requirements and Regulation 16C liability architecture are practitioner-facing compliance obligations that require direct coverage. Perplexity monitoring targets: vendor-accountability consultation outcome (2026), any SEBI clarification on Regulation 16C implementation, and the harmonised AI-ML reporting framework across exchanges.

---

_Back to [[_Frameworks_MOC]]_