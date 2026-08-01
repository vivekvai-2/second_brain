---
node_id: F037
series: Format_B
title: "AI Agents in Action: Foundations for Evaluation and Governance"
short_ref: "World Economic Forum + Capgemini, November 2025"
wiki_section: S4, S1
tier: High-Medium
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/agentic-ai-governance
  - topic/ai-governance-frameworks
  - topic/evaluation
  - institution/wef
  - institution/capgemini
  - batch/13
date_ingested: 2026-06-19
last_enriched: 2026-07-15
verify_flags: 3
---

# F037 — World Economic Forum & Capgemini. *AI Agents in Action: Foundations for Evaluation and Governance.* White Paper, November 2025.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Authors / Issuers** | World Economic Forum (WEF) + Capgemini Research Institute |
| **Foreword signatories** | Roshan Gya (CEO, Capgemini Invent); Cathy Li (Head, Centre for AI Excellence; Member of the Executive Committee, World Economic Forum) — added 2026-07-15, previously uncaptured |
| **Contributors** | 40+ named individual contributors across industry, academia, and civil society, listed at document end — notable inclusions: Daniela Rus (MIT), Michael Kearns (University of Pennsylvania), Margaret Mitchell (Hugging Face), Gillian Hadfield (University of Toronto), Animashree Anandkumar (Caltech), Peter Hallinan (AWS), William Bartholomew (Microsoft), Pilar Manchón (Google), Scott Likens (PwC), Kush Varshney (IBM), Jason Ruger (Lenovo), Leonid Zhukov (BCG). Full 40+ list in source document, page 31 — not reproduced verbatim here per this vault's primary-source-preservation convention. Added 2026-07-15; original intake captured zero contributor names.|
| **Document Type** | White Paper (multi-stakeholder; WEF Platform for Shaping the Future of Technology) |
| **Date** | November 2025 (exact day not stated) |
| **Pages** | **34** (corrected 2026-07-15 — original intake estimated "~48"; a second extraction pass traced the source's own Table of Contents exactly: Foreword p.4, Executive Summary p.5, Introduction p.6, Section 1 pp.8–12, Section 2 pp.13–28, Section 3 p.29, Conclusion p.30, Contributors p.31, Endnotes p.34) |
| **Source File** | `AI_Agents_in_Action_Evaluation_and_Governance_1764349644.pdf` |
| **Wiki Section** | S4 (Agentic AI), S1 (Ethics/Principles) |
| **Tier** | High-Medium — WEF multi-stakeholder; Capgemini Research Institute data; not a regulatory primary source |
| **Confidence** | High (WEF official publication; named co-author institution) |

## Document Summary

A WEF–Capgemini white paper establishing three foundational pillars for responsible AI agent adoption: (1) technical foundations (architecture layers and interoperability protocols); (2) functional classification (7-dimension schema for characterizing agents); and (3) evaluation and governance (4-stage progressive governance framework). The paper positions itself as a multi-stakeholder framing document bridging technical specifications and policy frameworks.

## Core Content

### 1. Technical Foundations

**Four technological paradigms AI agents draw on** (added 2026-07-15, missed in original intake): Classical software, Neural networks, Foundation models, Autonomous control. The paper frames modern agents as compositions of these four paradigms rather than as a single new technology category.

**Three architecture layers:**

| Layer | Function |
|---|---|
| **Application** | User-facing interface; task definition and output consumption |
| **Orchestration** | Workflow management; multi-agent coordination; tool routing |
| **Reasoning** | Core LLM/model layer; decision logic; action generation |

**Key interoperability protocols (as of November 2025):**

| Protocol | Source | Date | Purpose |
|---|---|---|---|
| **MCP (Model Context Protocol)** | Anthropic | Late 2024 | Standardized tool-use and resource access for agents |
| **A2A (Agent-to-Agent Protocol)** | Google | April 2025 ⚠ | Direct agent-to-agent communication |
| **AP2 (Agent Payments Protocol)** | Google | September 2025 ⚠ | Agent-initiated payment and commercial transaction capability |
| **ACP (Agent Connect Protocol)** | AGNTCY architecture | Not stated | Fourth named protocol — added 2026-07-15, missing from original intake's three-protocol list |

**Provider and Adopter (definitions added 2026-07-15, missed in original intake):** the source frames agent governance around two roles — **Provider** ("organizations or individuals that supply AI systems, platforms or tools") and **Adopter** ("individuals within an organization who use AI systems, encompassing responsibilities such as procurement and deployment"). This Provider/Adopter distinction structures Section 2 of the source and is the framing this node's Evaluation/Risk/Governance sections below should be read against — evaluation is described as "provider-focused" specifically because of this distinction.

### 2. Functional Classification — 7-Dimension Schema

The paper proposes a 7-dimension schema for classifying AI agents, drawing analogy to **SAE International's *Taxonomy and Definitions for Terms Related to Driving Automation Systems for On-Road Motor Vehicles* (Levels 0 to 5)** — precise citation added 2026-07-15; original intake cited this generically as "SAE J3016 autonomous vehicles levels."

| Dimension | Description |
|---|---|
| **Function** | What type of task does the agent perform? (information retrieval, content generation, action execution, etc.) |
| **Role** | Is the agent an orchestrator, sub-agent, or hybrid? |
| **Predictability** | How deterministic is the agent's output given a defined input? |
| **Autonomy** | To what degree does the agent act without human initiation or oversight? |
| **Authority** | What scope of actions can the agent take (read-only → write → transact → control)? |
| **Use Case** | Domain of deployment (HR, legal, finance, customer service, etc.) |
| **Environment** | Deployment context (sandbox, internal enterprise, public-facing, critical infrastructure) |

**Four worked case studies (added 2026-07-15, entirely missing from original intake)** — the source applies its 7-dimension schema to four concrete examples, useful directly as teaching/consulting illustrations of the classification framework in action:

| Case | Function | Role | Predictability | Autonomy | Authority | Context |
|---|---|---|---|---|---|---|
| **1. Robot vacuum cleaner** | Autonomous indoor navigation | Specialist | Deterministic | Medium | Low | Home vacuuming, moderate environment |
| **2. Coding co-pilot** | Assists human developers with code generation and debugging | Specialist | — | — | — | Development environment |
| **3. Autonomous vehicle** | Performs complete driving tasks without human control | Specialist | Non-deterministic | High | High | Public roads, critical environment |
| **4. Personal assistant** | Manages cross-platform tasks (drafting vs. sending messages dynamically recalibrates autonomy/authority) | Generalist | Non-deterministic | Dynamic | Dynamic | Cross-platform, moderate-to-high environment |

The source also cites a **fraud-detection agent in online banking** as a worked example of adjusting the "Operational context" dimension — directly relevant to P3 (BFSI JEIM); this is the clearest BFSI-specific illustration in the entire document and was not captured in the original intake at all.

### 3. Evaluation and Governance — 4-Stage Framework

| Stage | Focus | Key Mechanisms |
|---|---|---|
| **1. Classification** | Categorize agents using 7-dimension schema | Mandatory registry; deployment scope declaration |
| **2. Evaluation** | Test agent capabilities, limitations, and failure modes | Benchmarks: AgentBench, SWE-bench, HCAST |
| **3. Risk Assessment** | Map risks against deployment context | Risk matrices; scenario testing; adversarial probing |
| **4. Governance** | Apply proportionate oversight based on risk tier | HITL for high-autonomy/authority; HOTL for medium; automated monitoring for low |

**Progressive governance principle:** oversight requirements scale with *autonomy × authority*. An agent with high autonomy and high authority (e.g., transactional execution in financial systems) requires HITL. An agent with low autonomy and read-only authority can operate under automated monitoring.

**Evaluation life-cycle principles (added 2026-07-15, missed in original intake):** Contextualization, Multidimensional assessment, Temporal and behavioural monitoring — these three principles structure how "Evaluation" (Stage 2) should actually be conducted, beyond simply naming benchmarks (AgentBench/SWE-bench/HCAST). A worked example (Case Study 2, coding co-pilot) illustrates evaluation applied to a low-autonomy, high-role-specialisation agent.

**Five-step risk assessment life cycle (added 2026-07-15, missed in original intake):** 1. Define context, 2. Identify risks, 3. Analyse risks, 4. Evaluate risks, 5. Manage risks. This is more precise than the original intake's generic "risk matrices; scenario testing; adversarial probing" characterisation of Stage 3. Worked example: Case Study 3 (autonomous vehicle) — a non-deterministic, high-autonomy, high-authority agent used to illustrate the full five-step cycle.

**Baseline governance mechanisms — Table 2 in source (added 2026-07-15, entirely missing from original intake):** the source specifies nine mechanisms that should apply to *every* agent regardless of autonomy level, not just high-risk ones — Access control, Legal and compliance, Testing and validation, Monitoring and logging, Human oversight, Traceability and identity, Long-term management, Trustworthiness and explainability, Manual redundancy. Key obligations (advisory-strength, source's own language): "At a minimum, every agent should operate under strict access control based on the principle of least privilege"; "Prior to deployment, agents should undergo sandbox or controlled pilot testing using nonproduction data to validate expected behaviour and mitigate unintended effects." Human oversight is specified via two named configurations: **human-in-the-loop (HITL)** and **human-on-the-loop (HOTL)** — Case Study 4 (personal assistant) illustrates dynamic recalibration between these two modes based on action type (drafting vs. sending).

This nine-mechanism baseline table is a genuine gap-filler relative to this corpus's other agentic-AI control catalogues: it is coarser than F070's (Databricks DASF) 51 numbered controls but is explicitly framed as a **universal minimum** applying regardless of risk tier, which neither F070 nor F038 (ISACA) states as explicitly. Cross-reference for [[Agentic_AI_Security_Diagnostic_Template]] §2 — this table is a useful "floor" check to run before applying F070's fuller catalogue.

### 4. Multi-Agent Ecosystem Risks

**Five failure modes** (expanded 2026-07-15 from three in the original intake — two were missing entirely):

| Risk | Description |
|---|---|
| **Orchestration drift** | Orchestrator agent diverges from intended task scope as sub-agent outputs accumulate |
| **Semantic misalignment** | Sub-agents interpret shared context differently, producing conflicting or incoherent joint outputs |
| **Security and trust gaps** | Added 2026-07-15 — missing from original intake |
| **Interconnectedness and cascading effects** | Failure or error in one agent propagates through the pipeline, amplifying impact (originally captured as "Cascading effects" only) |
| **Systemic complexity** | Added 2026-07-15 — missing from original intake |

**Emerging multi-agent ecosystem paradigms (added 2026-07-15, entirely missing from original intake):** Agent-to-agent commerce, Internet of agents, Trust frameworks for inter-agent collaboration, Agent governance and oversight, Embodied agents. Direct quote (p.28): "As organizations begin to deploy multiple agents across departments, systems and networks, a new class of failure modes is emerging..."

### 5. Regulatory References

The paper explicitly references: OECD AI Recommendation (principles-based framing); NIST AI RMF 1.0 (risk management lifecycle); ISO/IEC 42001:2023 (AI management systems); ISO/IEC 23894:2023 (AI risk management); NIST AI 600-1 (generative AI risk).

### 6. Scale Indicator

> "82% of organizations plan to integrate AI agents within 1–3 years." ⚠ VERIFY — attributed to Capgemini Research Institute 2024 survey (endnote 1).

### 7. Key Quotes (added 2026-07-15, entirely missing from original intake)

- On hiring discipline: "Onboarding an AI agent should be treated with the same rigour as onboarding a new employee" — frames the Provider/Adopter governance relationship (§1 above) in HR-onboarding terms; directly reusable in consulting/teaching material aimed at non-technical business leaders (pairs well with F074's Lenovo case study register).
- On zero-trust posture: "Every agent interaction should be treated as untrusted by default." This is the same zero-trust posture NIST NCCoE operationalizes technically via SP 800-207 in [[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization]] — F037 states the *principle* in governance language; F036 states the *mechanism* (continuous verification, no implicit trust based on network location) in identity-architecture language. Worth citing together where a paper needs both the "why" and the "how" of agent zero-trust.
- On least privilege: "At a minimum, every agent should operate under strict access control based on the principle of least privilege" (also captured under Baseline Governance Mechanisms, §3 above).
- On pre-deployment testing: "Prior to deployment, agents should undergo sandbox or controlled pilot testing using nonproduction data to validate expected behaviour and mitigate unintended effects."
- Closing/conclusion framing: "The responsible deployment of agentic systems depends on a baseline of trust, transparency and accountability that remains valid for all digital systems" — ties the entire paper's agent-specific framework back to general digital-governance principles, reinforcing this node's [[Regulatory_Parallelism]] and [[Governance_Capacity]] concept links.

## Analytical Notes

**Progressive governance mirrors EU AI Act risk-based approach.** WEF's autonomy/authority-scaled oversight (Governance Stage 4) is functionally equivalent to the EU AI Act's risk-based tiering (prohibited → high-risk → limited risk → minimal risk) applied specifically to agentic systems. This parallelism across multilateral (WEF), regulatory (EU), and US federal (NIST) frameworks is a strong [[Regulatory_Parallelism]] signal.

**7-dimension schema for fsQCA operationalization.** The autonomy and authority dimensions are the most analytically tractable for fsQCA condition operationalization. "Autonomy" can calibrate the *scope of AI deployment* (SC) condition; "Authority" can calibrate the *enforcement capacity* (EA) condition (higher authority = higher accountability stakes).

**AP2 (Agent Payments Protocol) as governance frontier.** The September 2025 AP2 protocol — enabling agent-initiated commercial transactions — marks the regulatory threshold where agentic AI intersects financial regulation. This has direct implications for P3 (BFSI JEIM) and for SEBI/RBI's forthcoming agentic AI governance obligations.

**Multi-agent cascade risk ↔ Systemic risk.** The "cascading effects" risk echoes the systemic financial stability concerns in FSB TPRM (Batch 10) and IOSCO CR/01/2025 (International_19). The agentic framing extends the systemic risk vector beyond individual model failure to multi-agent pipeline failure.

## Concept Links

- [[Agentic_AI_Governance]] — seven-dimension classification schema; progressive governance framework; multi-agent risk taxonomy
- [[Accountability]] — HITL/HOTL requirements as accountability operationalization
- [[Transparency]] — evaluation benchmarks (Stage 2) and risk assessment (Stage 3) as transparency mechanisms
- [[Governance_Capacity]] — four-stage framework as a governance capacity blueprint; benchmarks (AgentBench, SWE-bench, HCAST) as evaluation capacity indicators
- [[Regulatory_Parallelism]] — progressive governance mirrors EU AI Act risk-based approach; OECD/NIST/ISO stack cited in same document

## Cross-References in Corpus

| Node | Relationship |
|---|---|
| F035 (Microsoft Governing Agents) | F035's three-tier spectrum is an enterprise implementation of F037's 7-dimension classification |
| F036 (NIST NCCoE Agent Identity) | F036's authorization framework maps to F037's Authority dimension |
| F038 (ISACA Agentic AI Security) | F038's 5-level maturity model parallels F037's 4-stage progressive governance framework |
| F041 (AEF-1 Evaluation MOCs) | F037's Evaluation Stage (Stage 2) is operationalized by F041's Minimum Operating Conditions |
| International_19 (IOSCO CR/01/2025) | F037's cascade risk parallels IOSCO's systemic AI risk in capital markets |
| F036 (NIST NCCoE Agent Identity) | Added 2026-07-15 — F037's "untrusted by default" zero-trust principle (§7 Key Quotes) is the governance-language counterpart to F036's SP 800-207 technical zero-trust architecture |
| F070 (Databricks DASF) | Added 2026-07-15 — F037's 9-mechanism Baseline Governance Table (§3) is a coarser universal-minimum floor relative to F070's 51-control catalogue; useful as a pre-check before applying DASF in full |
| F074 (McKinsey "What is an AI agent?") | Added 2026-07-15 — F074's 5-type business taxonomy and 3 architecture patterns are a plain-language executive-communication register; F037's 7-dimension schema and 4-stage framework are the governance-diagnostic register for the same subject matter |

## Research Application

| Project | Relevance |
|---|---|
| P1 (SLR) | Comprehensive governance framework for agentic AI; multi-stakeholder primary with WEF imprimatur |
| P3 (BFSI JEIM) | AP2 protocol and Authority dimension directly relevant to BFSI agentic deployment governance; strengthened 2026-07-15 — the source's own fraud-detection-in-online-banking worked example (§2 above) is a directly citable BFSI illustration of the 7-dimension schema, previously uncaptured |
| fsQCA | SC and EA condition calibration: autonomy and authority dimensions as condition indicators |
| P4 (IJLIT doctrinal) | Multi-agent systemic risk provides doctrinal grounding for cascade liability analysis |

## Source Metadata

- **Access method:** Read tool at Mac filesystem path
- **Text quality:** Good (WEF standard publication PDF)
- **VERIFY flags:** 3

### ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| V-B13-02 | "82% of organizations plan to integrate agents within 1–3 years" — verify against Capgemini Research Institute 2024 survey (endnote 1 in document) before citing as data point | HIGH |
| V-B13-03 | A2A (Agent-to-Agent Protocol) — verify Google release date stated as April 2025 | LOW |
| V-B13-04 | AP2 (Agent Payments Protocol) — verify Google release date stated as September 2025 | LOW |

## Log

- 2026-06-19: Node created (Batch 13), initial intake.
- 2026-07-15: Enriched from a second, independent NotebookLM extraction pass (PROMPT 0b) covering the same source document. This pass was pasted by the user as if a new document; a full-file read confirmed F037 already existed, so no duplicate node was created — existing-node enrichment applied instead, per standing "never recreate existing nodes" rule. Additions: foreword signatories and 40+ contributor list (Bibliographic Record); page-count correction "~48" → precise 34 with TOC-traced reasoning; four technological paradigms; ACP as fourth interoperability protocol; Provider/Adopter role definitions; precise SAE citation; four worked case studies (robot vacuum, coding co-pilot, autonomous vehicle, personal assistant) plus the BFSI fraud-detection-in-online-banking example (new P3 relevance); evaluation life-cycle principles (Contextualization, Multidimensional assessment, Temporal and behavioural monitoring); precise five-step risk assessment life cycle; nine-mechanism Baseline Governance Table with HITL/HOTL detail; multi-agent risks expanded from three to five (added Security and trust gaps, Systemic complexity) plus emerging multi-agent ecosystem paradigms list; five-item Key Quotes section including the zero-trust "untrusted by default" quote cross-referenced to F036's SP 800-207 architecture. Cross-References table extended (F036, F070, F074). Research Application table's P3 row strengthened with the BFSI worked example. No new VERIFY flags required — the three existing flags (V-B13-02/03/04) already cover the only uncertain items surfaced in either extraction pass. `last_enriched: 2026-07-15` added to frontmatter. Indexing pass (Corpus_Index_MOC log note; concept-file "Instances in Corpus" checks) to follow.
