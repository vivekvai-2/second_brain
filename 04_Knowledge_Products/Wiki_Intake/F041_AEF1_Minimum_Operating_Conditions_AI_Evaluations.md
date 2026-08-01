---
node_id: F041
series: Format_B
title: "AEF-1: Minimum Operating Conditions for Independent Third Party AI Evaluations"
short_ref: "Stosz et al. (Transluce, METR, GovAI, et al.), December 2025"
wiki_section: S1, S3
tier: High-Medium
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/ai-governance-frameworks
  - topic/ai-evaluation
  - topic/accountability
  - institution/transluce
  - institution/metr
  - institution/govai
  - institution/princeton
  - institution/stanford
  - batch/13
date_ingested: 2026-06-19
verify_flags: 1
---

# F041 — Stosz, C., et al. *AEF-1: Minimum Operating Conditions for Independent Third Party AI Evaluations.* Version 1, December 4, 2025.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Authors (24)** | Conrad Stosz, Karson Elmgren (Transluce); Charles Foster, Michael Chen, Elizabeth Barnes, Christopher Painter, Luca Righetti (METR/GovAI); George Balston, Sean McGregor, Grace Werner (AVERI); Seth Donoughe, Samira Nedungadi, Jasper Götting (SecureBio); Sayash Kapoor, Arvind Narayanan (Princeton); Sarah Schwettmann, Rishi Bommasani, Rob Reich (Stanford/Transluce); Aidan Homewood (GovAI); Divya Siddharth, Faisal Lalani (Collective Intelligence Project); Jaime Sevilla (Epoch AI); Jacob Steinhardt (UC Berkeley/Transluce) |
| **Issuing Organizations** | Transluce, METR (Model Evaluation & Threat Research), AI Verification and Evaluation Research Institute (AVERI), SecureBio, Princeton University, MIT, Stanford HAIS, GovAI (Centre for the Governance of AI), Collective Intelligence Project, Epoch AI, UC Berkeley |
| **Document Type** | Voluntary standard + evaluation checklist |
| **Version** | Version 1 |
| **Date** | December 4, 2025 |
| **URL** | https://aievaluatorforum.org/initiatives/minimum-operating-conditions |
| **Pages** | ~35 |
| **Source File** | `Minimum_operating_conditions_for_AI_evaluations__1765178960.pdf` |
| **Wiki Section** | S1 (Ethics/Principles), S3 (International Comparators) |
| **Tier** | High-Medium — multi-institutional academic + policy consortium; directly cited in EU AI Act CoP and California SB 53 |
| **Confidence** | High (versioned V1; December 4, 2025; named institutional affiliations; regulatory citations verified) |

## Document Summary

AEF-1 is the first versioned voluntary standard establishing Minimum Operating Conditions (MOCs) for independent third-party AI evaluations. Published by a 24-author, multi-institutional consortium spanning leading AI governance research organizations (Transluce, METR, GovAI, Princeton, Stanford, UC Berkeley, Epoch AI), the document defines five MOCs organized around three operational dimensions (Independence, Access, Transparency). AEF-1 is explicitly referenced in the EU AI Act Code of Practice (Safety & Security Chapter, Measure 7.3(1)(g)) and California SB 53 (§22757.12(c)(2)(C)), giving it direct regulatory adjacency despite its voluntary status.

## Core Content

### 0. Scope — Four Appropriate-Use Contexts (added 2026-07-16, second-pass extraction)

AEF-1's own Scope section (§2) names four contexts in which the standard is intended to apply, not documented in this node's original 2026-06-19 intake:

1. Establish that a system provider has adequately addressed risks of acute public concern.
2. Satisfy regulatory mandates for independent third-party evaluations or audits.
3. Serve as a significant basis for critical internal governance decisions concerning public interest or well-being.
4. Guide high-risk AI procurement decisions.

The Scope section also contains an explicit **limitation disclaimer** worth citing directly: "The standard does not cover all aspects of third-party AI evaluation. In particular, it does not address the many critical methodological considerations for conducting scientifically valid AI evaluations, nor does it exhaustively cover evaluators' various responsibilities towards system providers..." — AEF-1 is a *process/independence* standard, not a methodological-validity standard; useful to note when citing it so as not to overclaim what compliance with it demonstrates.

### 1. Three Operational Dimensions

| Dimension | Core Principle |
|---|---|
| **Independence** | Evaluators must be free from organizational, financial, and editorial control by AI providers |
| **Access** | Evaluators must have sufficient technical, informational, computational, and temporal access to conduct meaningful evaluation |
| **Transparency** | Evaluation methods and results must be disclosed without provider interference or contingent conditions |

### 2. Five Minimum Operating Conditions (MOCs)

#### MOC 1: Sufficient Access and Resources

| Component | Requirement |
|---|---|
| **Technical access** | Query access; scaffolding permissions; safeguard exemptions for evaluation purposes; intermediate model states; finetuning access; weight access (where relevant); access to tools and user data representative of deployment context |
| **Information sharing** | Provider must share training data characteristics, safety testing history, and known limitations |
| **Computational resources** | Adequate compute provided or funded for evaluation scope |
| **Time** | **Minimum 20 business days** for substantially novel systems; cited in EU CoP Appendix 3.4 |
| **Legal safe harbor** | Evaluators must be protected from legal liability arising from evaluation activities (NDA provisions, liability waivers) |

#### MOC 2: Minimized Conflicts of Interest

| Requirement | Detail |
|---|---|
| No contingent compensation | Payment must not be conditioned on evaluation outcomes (positive or negative) |
| No organizational/financial control | Provider may not have organizational or financial control over the evaluation entity |
| Published CoI policy | Evaluator must publicly maintain a conflict of interest policy |
| CoI disclosure (5 categories) | Financial interests; personal relationships; research collaboration history; prior employment; advisory relationships |
| Staff recusals | Individual staff with conflicts must be recused from relevant evaluation components |
| Agreement disclosure | Terms of evaluation agreements must be disclosed (redacted for confidential business information) |

#### MOC 3: Analytic Autonomy

| Requirement | Detail |
|---|---|
| Scoping flexibility | Evaluators may identify and pursue relevant evaluation questions beyond the initial scope |
| Evaluation method autonomy | Evaluators choose their own metrics, methodologies, and rubrics without provider prescription |
| Direct system access | Evaluators should have direct API/system access, not solely provider-mediated access |
| **Editorial control (7 elements)** | Evaluators control: (1) what findings to report; (2) how to characterize findings; (3) confidence levels; (4) comparison to other systems; (5) recommendations; (6) timing of publication; (7) response to provider comments |

#### MOC 4: Transparent Methods and Results

| Requirement | Detail |
|---|---|
| Methodological transparency | Full disclosure of evaluation methodology, metrics, and limitations |
| Upfront disclosure rights | Provider must commit to disclosure terms before evaluation begins |
| **Non-contingent release** | Evaluation results may not be withheld contingent on provider approval of findings |
| No misrepresentation | Evaluators may not misrepresent findings at provider request |
| Timely disclosure | Results must be published within a defined period after evaluation completion |
| **No provider redaction authority over concerning findings** | Provider may not redact findings related to safety, capability, or risk concerns |
| Redaction disclaimer | If any redaction occurs (for legitimate confidentiality), this must be disclosed in the published report |

#### MOC 5: Protection of Sensitive Information

| Requirement | Detail |
|---|---|
| Publication permission | Evaluators obtain necessary permissions for responsible publication |
| Evaluation integrity | No gaming (providers may not manipulate system to perform differently during evaluation); no pre-release leaking of evaluation content |
| Confidentiality protection | Genuinely sensitive provider information is protected within agreed boundaries |
| **Responsible disclosure policy** | Evaluators commit to a responsible disclosure framework; **60-day disclosure window** for public-facing vulnerabilities before mandatory publication |

### 3. Regulatory Anchors

| Instrument | Provision | AEF-1 Connection |
|---|---|---|
| **EU AI Act Code of Practice** | Safety & Security Chapter, Measure 7.3(1)(g) | AEF-1 cited as benchmark for third-party evaluation standards |
| **California SB 53** | §22757.12(c)(2)(C) | AEF-1 explicitly cited as evaluation standard for covered AI systems |
| **EU CoP Appendix 3.4** | Minimum evaluation time | 20-business-day minimum cited in Appendix 3.4 |

### 4. Key Specific Precedent

> METR's evaluation of GPT-5 took 3 weeks — just over the 20-business-day minimum threshold specified in MOC 1.

### 5. Referenced Evaluation Bodies and Documents

- Bengio International AI Safety Report (January 2025)
- Frontier Model Forum Third-Party Assessments paper (April 2025)
- NTIA AI Accountability Policy Report (March 2024)
- AISI UK (AI Safety Institute) early evaluation lessons
- Anthropic Claude Sonnet 4.5 System Card (September 2025) — cited as compliance example
- Gemini 2.5 Pro Model Card (June 2025) — cited as compliance example

### 6. Appendix B — Formal Terminology (added 2026-07-16, second-pass extraction)

AEF-1's Appendix B supplies precise, citable definitions not previously captured in this node:

| Term | Definition |
|---|---|
| **Conflict of interest** | "A situation that creates a risk that evaluator, its employees, or other agents working on its behalf to carry out an evaluation of a particular system could be influenced by an incentive to not provide as rigorous and accurate an evaluation as possible." |
| **Evaluator** | "An organization that conducts assessments of an AI system provider's systems or processes." |
| **System provider** | "An organization which develops or operates AI models or systems." |
| **System vulnerability** | "A weakness in a system that could be exploited by a malicious actor to harm the confidentiality, integrity, or availability of the system and its data, or which could be used to bypass safeguards intended to constrain the system's behavior to prevent misuse." |
| **Information hazard** | "Information about the misuse of AI systems or the general pursuit of harmful acts that, if disclosed, would foreseeably cause more harm than benefit, such as specific details of how to produce dangerous chemical, biological, radiological, or nuclear (CBRN) materials or child sexual abuse material (CSAM)." |
| **Third-party** | "A separate organization that is not under the control of the system provider." |

The **information hazard** definition's explicit CBRN/CSAM framing is notable given SecureBio's co-authorship (a biosecurity-focused organisation) — it signals AEF-1's responsible-disclosure provisions (MOC 5.4, 60-day window) were drafted with catastrophic-risk information hazards specifically in mind, not merely conventional cybersecurity vulnerabilities.

## Analytical Notes

**First standardized checklist for third-party evaluation independence.** AEF-1 is the inaugural attempt to codify what "independent" means for AI evaluation — defining independence through three enforceable operational dimensions (Independence, Access, Transparency) rather than vague aspirational language. This fills a concrete [[Governance_Capacity]] gap: prior governance frameworks (NIST AI RMF, EU AI Act, Singapore MAS) mandated evaluation but did not specify the operational conditions for independence.

**Anti-"evaluation capture" provisions.** The most novel provisions are editorial control (MOC 3, 7 elements) and the anti-redaction requirements (MOC 4). These prevent "evaluation capture" — the phenomenon where providers influence evaluation conclusions through funding control, access restriction, or editorial veto. The analogy to credit rating agency independence rules (SEC Rule 17g-5, PCAOB ET101 on auditor independence) is explicit in the document. This framing has direct implications for how BFSI regulators should structure AI evaluation mandates.

**fsQCA GC calibration.** AEF-1 provides the most concrete benchmark for calibrating the Governance Capacity (GC) condition for fsQCA:
- **High GC**: Jurisdictions with MOC-compliant third-party evaluation requirements (EU CoP, California SB 53)
- **Medium GC**: Jurisdictions mandating evaluation without independence standards
- **Low GC**: Jurisdictions without third-party evaluation requirements

The 20-business-day minimum is a particularly tractable concrete indicator.

**Regulatory Parallelism signal.** EU AI Act CoP and California SB 53 independently converge on third-party evaluation requirements within the same period (late 2025). AEF-1 both reflects and accelerates this convergence — the voluntary standard was adopted into two regulatory instruments within months of publication.

**Cross-link to F037 (WEF Evaluation Stage).** F037's Governance Framework Stage 2 (Evaluation) is the high-level policy prescription; AEF-1 is its operational specification. Together they represent the complete policy-to-practice layer for AI evaluation governance.

**India gap.** Neither MeitY's responsible AI framework nor any Indian BFSI regulator (RBI, SEBI, IRDAI) has published independent AI evaluation standards as of this session. AEF-1 provides the benchmark against which this gap can be measured for P4 (IJLIT) and P3 (BFSI JEIM).

## Concept Links

- [[Accountability]] — editorial control + anti-redaction requirements prevent evaluation capture; responsible disclosure policy as accountability mechanism
- [[Transparency]] — MOC 4 (Transparent Methods and Results) as the operational definition of evaluation transparency
- [[Governance_Capacity]] — 20-business-day minimum, CoI framework, and editorial control requirements as concrete GC indicators; AEF-1 as GC calibration benchmark
- [[Regulatory_Parallelism]] — EU AI Act CoP + California SB 53 independently converge on third-party evaluation requirements; voluntary standard captured into two regulatory instruments

## Cross-References in Corpus

| Node | Relationship |
|---|---|
| F037 (WEF AI Agents in Action) | F037's Evaluation Stage (Stage 2) is the high-level prescription; AEF-1 is its operational specification |
| F036 (NIST NCCoE Agent Identity) | F036's Logging/Audit focus area (Focus Area 5) parallels AEF-1's Transparent Methods requirements |
| F038 (ISACA Agentic AI Security) | F038's Observability & Assurance defense plane parallels AEF-1's MOC 4 transparency requirements |
| F039 (ICAAD+KWM AI Harm & Human Rights) | F039's FRIA obligation (EU AI Act Art. 27) and F041's evaluation independence both operate as ex ante accountability mechanisms |
| F040 (ELI ADM Principles) | F040's Principle 5 (Traceability) is the doctrinal precursor to AEF-1's transparency and logging requirements |

## Research Application

| Project | Relevance |
|---|---|
| P1 (SLR) | Primary source: first versioned third-party AI evaluation standard; high relevance for governance capacity analysis |
| fsQCA | Governance Capacity (GC) condition calibration: AEF-1 MOCs as concrete GC indicators; 20-day minimum as a measurable threshold |
| P3 (BFSI JEIM) | Independent AI evaluation as BFSI governance requirement; anti-capture provisions relevant to BFSI regulatory models |
| P4 (IJLIT doctrinal) | Evaluation governance as accountability mechanism; India gap against AEF-1 benchmarks |

## Source Metadata

- **Access method:** Read tool at Mac filesystem path
- **Text quality:** High (multi-institutional academic document; clean PDF; versioned release)
- **VERIFY flags:** 1 (see below; document is explicitly versioned V1, December 4, 2025; all regulatory citations are independently checkable)

**#293 — RESOLVED (2026-07-31, editorial judgment).** Page count is presentational metadata, not a citation-content element — it does not appear in the APA reference and doesn't affect citation accuracy. All substantive bibliographic details (authors, date, title, URL) match exactly across both extractions, confirming same document. No further action needed.

## Log

- 2026-07-16: Second NotebookLM extraction of this same document (PROMPT 0b relay) matched this existing F041 node exactly (same 24 authors, same title, same December 4, 2025 date, same institutional consortium). Per the standing "never recreate, enrich in place" rule, no new F-number assigned. Enriched with: the Scope section's four appropriate-use contexts and explicit methodological-limitation disclaimer (§0 above), and Appendix B's six formal terminology definitions (§6 above), neither captured in the original 2026-06-19 intake. One new VERIFY flag added (#293, page-count discrepancy — LOW). No changes to existing concept links, cross-references, or analytical notes — all remain valid and unaffected by this enrichment.
