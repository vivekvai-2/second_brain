---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S3
  - section/S1
  - tier/high
  - project/p1
  - project/p3
  - project/fsqca
---

# Future of Life Institute: AI Safety Index — Winter 2025 (December 2025)

**Node ID:** F048  
**Type:** Wiki Intake Note  
**Wiki Section:** S3 (International Comparators) / S1 (Governance Fundamentals)  
**Status:** Active  
**Tier:** High  
**Last Updated:** 2026-06-19  

---

## Source

**Full Citation (APA):** Future of Life Institute. (2025, December). *AI safety index: Winter 2025*. Future of Life Institute.  
**Document Type:** Annual index / governance evaluation report (third edition)  
**Issuing Institution:** Future of Life Institute (FLI) — independent nonprofit; Cambridge, MA  
**Expert Review Panel:** Stuart Russell (UC Berkeley), David Krueger (University of Montreal), Dylan Hadfield-Menell (MIT), Sharon Li (University of Wisconsin-Madison), Jessica Newman (UC Berkeley), Sneha Revanur (Encode Justice), Tegan Maharaj (HEC Montréal), Yi Zeng (Chinese Academy of Sciences)  
**Publication Date:** December 2025  
**Evidence cutoff:** November 8, 2025 (does not reflect Gemini 3 Pro, Grok 4.1, GPT-5.1, Claude Opus 4.5)  
**URL / DOI:** aisafetyindex.ai (⚠ VERIFY for canonical URL)  

---

## Executive Summary

The Future of Life Institute's Winter 2025 AI Safety Index is the third edition of an annual comparative evaluation of frontier AI companies across six governance domains and 35 indicators, conducted by an independent expert panel. Eight companies are assessed: Anthropic, OpenAI, Google DeepMind, xAI, Z.ai, Meta, DeepSeek, and Alibaba Cloud. No company scores above C+ overall; the Existential Safety domain yields D or F grades for all eight companies for the second consecutive edition, indicating a structural and persistent governance gap between frontier AI capability deployment and existential safety governance. The index introduces "foundational hypocrisy" as a characterisation of companies that publicly acknowledge the possibility of transformative or catastrophic AI risk while simultaneously accelerating capability development without commensurate safety infrastructure. Chinese companies (DeepSeek, Alibaba Cloud) are noted for stronger baseline accountability in some indicator categories due to binding domestic regulatory obligations (mandatory watermarking under GB45438-2025; incident reporting requirements). All companies fall below the standards of the EU AI Code of Practice. India is not included in the index; the index provides quantitative calibration anchors for fsQCA's Evaluative Authority (EA) condition.

---

## Key Frameworks and Findings

### Assessment Architecture

| Parameter | Value |
|---|---|
| Companies assessed | 8 |
| Governance domains | 6 |
| Indicators | 35 (32 from Summer 2025 + 3 new Information Sharing indicators) |
| Previous evaluation series replaced | UK AI Safety Institute and Cisco evaluations (replaced by CAIS Safety Index for this edition) |
| Evidence collection method | Desk research + company survey (5/8 companies responded — Meta, DeepSeek, Alibaba Cloud did not submit) |
| Expert grading | Individual expert grades averaged; individual grades kept confidential |
| Evidence cutoff | November 8, 2025 |

### Flagship Models Evaluated

Anthropic: Claude-Sonnet-4.5 | OpenAI: GPT-5 | Google DeepMind: Gemini-2.5-Pro | xAI: Grok-4 | Z.ai: not specified | Meta: not specified (Llama series) | DeepSeek: R1 | Alibaba Cloud: Qwen3-Max

### Overall Grades

| Company | Overall Grade | Numeric Score (⚠ VERIFY #176) |
|---|---|---|
| **Anthropic** | C+ | 2.67 |
| **OpenAI** | C+ | 2.31 |
| **Google DeepMind** | C | 2.08 |
| **xAI** | D | 1.17 |
| **Z.ai** | D | 1.12 |
| **Meta** | D | 1.10 |
| **DeepSeek** | D | 1.02 |
| **Alibaba Cloud** | D- | 0.98 |

*Grading scale: A = 4.0; B = 3.0; C = 2.0; D = 1.0; F = 0. C+ = 2.33–2.66 range approximation.*

### Six Governance Domains

| Domain | Description | Key Finding |
|---|---|---|
| **Risk Assessment** | Pre-deployment risk evaluation; red-teaming; capability evaluations | Anthropic leads; most companies conduct some evaluations but methodology transparency varies |
| **Current Harms** | Misuse prevention; content safety; bias and discrimination | Higher scores than Existential Safety; OpenAI and Anthropic relatively stronger |
| **Safety Frameworks** | Responsible scaling policies; deployment thresholds; capability pause commitments | Anthropic RSO model cited as best practice; most companies lack binding commitments |
| **Existential Safety** | AGI development plans; catastrophic risk controls; human oversight mechanisms | **All companies: D or F** (second consecutive edition); no Human Uplift Trials by any company; no Independent Reviews of Safety Evaluations by any company |
| **Governance and Accountability** | Board accountability; external audit; transparency to regulators | Chinese companies score higher on some indicators due to binding domestic regulations |
| **Information Sharing** | Threat intelligence sharing; incident disclosure; research transparency | New domain (3 new indicators in Winter 2025); low scores across all companies; no company has robust non-contingent disclosure |

### Key Findings

#### Finding 1 — Existential Safety: Structural and Persistent Deficit
All eight companies score D or F in Existential Safety in both Summer 2025 and Winter 2025 editions. The FLI characterises this as indicating that frontier AI companies are:
- Developing increasingly capable AI systems (GPT-5, Claude Sonnet 4.5, Gemini 2.5 Pro)
- Without credible, independently verified plans for controlling catastrophic outcomes from those systems
- While publicly acknowledging (in some cases) that such outcomes are possible

This is the "foundational hypocrisy" characterisation: the gap between stated safety commitments and operational safety infrastructure.

#### Finding 2 — No Human Uplift Trials; No Independent Safety Evaluation Reviews
Across all 8 companies: zero have conducted Human Uplift Trials (testing whether AI systems provide meaningful uplift to bad actors attempting to cause mass casualties); zero have commissioned independent reviews of their safety evaluation methodologies. These are the two most severe individual indicator gaps in the index.

#### Finding 3 — Chinese Companies — Binding Regulation as Accountability Baseline
DeepSeek and Alibaba Cloud score above their overall D/D- grades on specific governance and accountability indicators due to:
- **GB45438-2025:** Chinese national watermarking standard — mandatory content watermarking on AI-generated material
- **Deep Synthesis Regulations:** Mandatory incident reporting for AI-generated content harms
- **Interim Measures for Generative AI:** Registration, security assessment, and content requirements

FLI notes this creates a paradox: Chinese companies with D/D- overall scores may have stronger *baseline accountability* (mandatory, enforceable obligations) than Western companies with C/C+ overall scores but voluntary or aspirational governance commitments. The FLI does not endorse Chinese AI governance overall; the observation is specific to the accountability infrastructure dimension.

#### Finding 4 — EU AI Code of Practice — All Companies Below Standard
The EU AI Code of Practice (applying to GPAI providers from August 2025) sets transparency, model documentation, incident reporting, and copyright compliance requirements. All eight companies fall below EU CoP standards in at least one material area, with Western companies additionally not meeting GPAI obligations in full.

#### Finding 5 — Anthropic's Default-On User Training Data Concern
Despite leading in all six domains, Anthropic's shift toward default-on user data contribution to training (opt-out rather than opt-in) is noted by the index as a governance concern — reversing a prior more privacy-protective stance.

### Domain Score Matrix (Appendix A — Abridged)

| Company | Risk Assessment | Current Harms | Safety Frameworks | Existential Safety | Governance & Accountability | Information Sharing |
|---|---|---|---|---|---|---|
| Anthropic | Highest | Highest | Highest | D (highest D) | High | Moderate |
| OpenAI | High | High | Moderate | D | Moderate | Moderate |
| Google DeepMind | Moderate-High | Moderate | Moderate | D | Moderate | Low |
| xAI | Low | Low | Low | D | Low | Very Low |
| Z.ai | Low | Low | Low | F | Low | Very Low |
| Meta | Low | Moderate | Low | D | Low (but binding obligations) | Very Low |
| DeepSeek | Very Low | Low | Very Low | F | Moderate (binding regulations) | Very Low |
| Alibaba Cloud | Very Low | Very Low | Very Low | F | Moderate (binding regulations) | Very Low |

*Note: Values above are directional summaries from document. Full numeric grades per domain are in the document's Appendix A grading sheets. ⚠ VERIFY #177 — confirm against Appendix A scores before using specific domain figures in research outputs.*

---

## India Relevance and Governance Gap Analysis

**India is not included in the FLI AI Safety Index.** The index assesses companies, not jurisdictions. However, the index is directly relevant to India across three vectors:

### 1. India's Exposure to All 8 Companies
All eight assessed companies either operate in India, provide AI services to Indian enterprises, or have Indian entities as significant users:
- Anthropic, OpenAI, Google, Meta: Active in Indian developer/enterprise market
- DeepSeek, Alibaba Cloud (via Alibaba Cloud India): Growing Indian market presence

India's regulatory framework (RBI CSCRF, SEBI AI guidelines, DPDP Act) does not require Indian entities using these frontier AI systems to apply any governance standard equivalent to the EU AI Code of Practice. The governance gap India faces is compounded by the finding that even the most advanced Western companies score only C+.

### 2. Chinese Regulatory Baseline as India Comparator
FLI's commendation of Chinese binding regulations (GB45438-2025 watermarking, Interim Measures) as creating stronger baseline accountability than voluntary Western frameworks is directly relevant to India's regulatory design choice. India could adopt:
- Mandatory AI content watermarking (analogous to GB45438-2025) in the forthcoming DPDP Rules
- Mandatory incident reporting for AI-caused harms to DPBI under DPDP Act s.8(6) extension
- SEBI mandatory AI audit trail requirements (analogous to Deep Synthesis incident reporting)

None of these are currently mandated. India's emerging AI governance (draft NITI AI governance framework; possible AI Act consultation) has the opportunity to incorporate binding accountability obligations; the FLI index empirically demonstrates that voluntary commitments produce C+/D grades even in the most sophisticated companies.

### 3. fsQCA Calibration — EA Condition
The FLI index's six-domain quantitative grades provide a calibration anchor for the Evaluative Authority (EA) condition in fsQCA:
- **Existential Safety:** All D/F → EA on existential risk = minimal across all companies
- **Governance & Accountability:** D–C+ range → EA on organisational accountability varies
- **Information Sharing:** Universally low → EA on transparency is systemically weak
- For fsQCA, FLI scores can be mapped to EA condition calibration across the 4 jurisdictions in the fsQCA sample (India, EU, US, China) as follows: US companies C+/C → EA=0.6–0.7; Chinese companies D/D- with binding regulations → EA=0.3–0.4 (overall grade) but EA=0.5+ on specific binding indicators; India → EA unmeasured but inferred low
- (2026-07-15) "Chinese companies... with binding regulations" is now primary-sourced: [[07_Institutions/Corpus/International/International_21_China_CAC_GenAI_Interim_Measures_2023]] (CAC Interim Measures for GenAI, effective Aug 2023) is the base-layer binding instrument behind this grade — see that node's "no self-contained fine" finding, which supports the graded (0.3–0.5) rather than binary EA coding used above.

### 4. "Foundational Hypocrisy" and India's Regulatory Permissiveness
India's AI governance posture (NITI's "responsible AI" principles + sectoral guidelines) mirrors the voluntary governance pattern that FLI characterises as foundational hypocrisy. India's formal governance commitments outpace its enforcement infrastructure and its evaluative capacity — the same gap the FLI documents at the company level.

---

## Research Programme Applications

| Project | Application |
|---|---|
| P1 (SLR RG) | **Primary** — FLI index methodology (35 indicators, 6 domains, independent expert grading) is a landmark governance evaluation methodology contribution; "foundational hypocrisy" as a conceptual framing; Chinese binding-regulation finding challenges voluntary-vs-mandatory governance dichotomy; cross-jurisdictional accountability calibration |
| P3 (BFSI JEIM) | Frontier AI company governance grades are relevant to BFSI risk assessment of AI vendor selection; Anthropic/OpenAI C+ grades mean even "responsible" AI vendors operate without credible existential safety infrastructure |
| P4 (Doctrinal IJLIT) | Limited — FLI's finding that all companies fall below EU AI CoP standards supports P4 argument for mandatory AI governance obligations rather than voluntary frameworks |
| fsQCA | **Primary** — EA condition calibration across 8 companies and 4 jurisdictions; Governance & Accountability and Information Sharing domain scores provide OC/CC condition anchors; "foundational hypocrisy" framing supports the causal logic of fsQCA conditions (formal commitment without operational implementation does not produce trustworthy AI outcome) |

---

## Concept Links

- [[Accountability]] — Governance & Accountability domain directly maps; zero Human Uplift Trials and zero Independent Safety Evaluation Reviews are the most acute accountability gaps; FLI's methodology of grading companies on 35 indicators is itself an accountability infrastructure tool
- [[Transparency]] — Information Sharing domain (new in Winter 2025); universally low scores indicate systemic non-transparency; Anthropic's default-on training data shift is a transparency regression; "foundational hypocrisy" is a transparency failure at the governance commitment level
- [[Governance_Capacity]] — Existential Safety domain (all D/F) measures the governance capacity gap at the most consequential level; the absence of Human Uplift Trials indicates that even leading companies lack the technical governance infrastructure to evaluate their own existential risk exposure
- [[Governance_Debt]] — "Foundational hypocrisy" is governance debt at the company level: capability advances creating safety obligations that governance infrastructure has not caught up with; second consecutive Existential Safety D/F edition indicates the debt is accumulating, not being retired
- [[Legitimacy]] — Chinese binding regulation vs. Western voluntary commitment finding challenges the conventional framing: legitimacy-seeking voluntary governance (C+) may produce weaker accountability than enforced baseline compliance (D overall, but D with binding mandates). The legitimacy value of voluntary governance is questioned empirically
- [[Regulatory_Parallelism]] — EU AI CoP + national voluntary frameworks + company RSO policies + FLI index = parallel, uncoordinated governance accountability instruments; the index itself notes the replacement of UK AISI/Cisco evaluations with CAIS Safety Index as an instance of evaluative framework discontinuity
- [[Agentic_AI_Governance]] — Existential Safety domain encompasses the AGI control problem; flagship models evaluated (GPT-5, Claude Sonnet 4.5, Gemini 2.5 Pro) are the foundation for agentic AI systems; the governance gap at the model level propagates into agentic AI governance gaps at the deployment level

---

## ⚠ VERIFY BEFORE PUBLISHING

- **V-B14-13 / #176 — Overall grades and numeric scores — LOW.** All grades and scores (e.g., Anthropic C+ / 2.67; OpenAI C+ / 2.31) are the index's own documented outputs from Appendix A grading sheets. These are the document's core deliverable. Verify: confirm against full Appendix A grading tables before citing specific domain-level scores; note evidence cutoff of November 8, 2025, when using in publications after early 2026.
- **V-B14-14 / #177 — Non-responding companies confirmed — LOW.** FLI states that Meta, DeepSeek, and Alibaba Cloud did not submit the company survey instrument; only 5 of 8 companies responded. This means those companies' scores rely solely on desk research (publicly available information), not on company-provided data. Consequence for citation: Meta, DeepSeek, and Alibaba Cloud scores should be cited as desk-research-based estimates, not company-confirmed assessments.

---

## Cross-Links to Corpus

- [[F043_MIT_AI_Risk_Mitigation_Taxonomy_2025]] — FLI cites the MIT/FutureTech taxonomy (Slattery et al. 2024/2025) as a foundational reference; both documents converge on the model alignment gap as the most critical and least-addressed governance risk
- [[F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations]] — AEF-1 minimum operating conditions for AI evaluations defines the institutional infrastructure required for credible safety evaluations; FLI's finding that zero companies have Independent Reviews of Safety Evaluations confirms the AEF-1 institutional gap at the company level
- [[F046_UK_LawCommission_AI_and_Law_DiscussionPaper_2025]] — F046 opacity theme (Anthropic: "nobody really knows how they work internally") is consistent with FLI's Existential Safety D grades; the legal opacity problem and the safety governance deficit are manifestations of the same fundamental challenge
- [[F047_BAIR_Berkeley_Responsible_GenAI_Playbook_2025]] — BAIR's 9%/0.8% organisational RAI maturity at deployer level is consistent with FLI's C+/D grades at developer level; governance deficit is pervasive across both developer and deployer tiers
- [[F042_IBM_Cost_Data_Breach_Report_2025]] — IBM's 97% lacking AI access controls (deployer level) and FLI's Governance & Accountability D grades (developer level) together establish a full-stack AI governance deficit from model development through to enterprise deployment
- [[International_19_IOSCO_AI_Capital_Markets_CR_2025]] — EU AI Act; FLI's finding that all companies fall below EU AI Code of Practice standards calibrates the regulatory effectiveness of the EU's mandatory governance architecture relative to voluntary company governance
