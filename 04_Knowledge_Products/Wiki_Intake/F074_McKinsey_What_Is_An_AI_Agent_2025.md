---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S4
  - tier/medium
  - project/agentic-ai
  - engine/consulting
  - content/carousel-ready
---

# McKinsey Explainers: What Is an AI Agent? (2025)

**Node ID:** F074
**Type:** Wiki Intake Note
**Wiki Section:** S4 (Agentic AI) primary / S7 (Use Cases) secondary
**Status:** Active
**Tier:** Medium
**Last Updated:** 2026-07-15

---

## Source

**Full Citation (APA):** Hämäläinen, L., Amar, J., Bawcom, A., Hu, A., Yao, L., von Bismarck, N., Roberts, R., Tavakoli, A., Harreis, H., Giovine, C., Kaplan, J., Rowshankish, K., Yee, L., Chui, M., Lerner, L., Thomas, R., & Chung, V. (2025, March). *What is an AI agent?* McKinsey & Company (McKinsey Explainers). [⚠ VERIFY #210 — exact publication day not stated; only "March 2025" confirmed]
**Authors:** 16 named McKinsey partners/senior partners/fellows across multiple offices (Seattle, Miami, Boston, Düsseldorf, London, New York, Bay Area, Washington DC, Mumbai, Hong Kong), plus two named external contributors — Arthur Hu (CTO, Lenovo Solutions and Services Group) and Linda Yao (COO and Head of Strategy, Lenovo) — cited within the piece as a case-study source, not co-authors in the traditional sense.
**Document Type:** Industry Report / Explainer (McKinsey Explainers series)
**Issuing Institution:** McKinsey & Company
**Publication Date:** March 2025 (day not stated)
**Pages:** Not paginated (web explainer format)
**URL/DOI:** Not captured this pass — ⚠ VERIFY #210

**Routing note:** Practitioner/advisory explainer, not primary regulation or peer-reviewed research. Format B (Wiki Intake Note) applies.

---

## Executive Summary

A foundational, definitional-level explainer on AI agents from McKinsey, structured as a Q&A across ten questions. It defines AI agents, taxonomizes five agent types by capability/role, describes a four-step operational loop (plan → allocate/execute → iterate → act), distinguishes agent-LLM relationships, quantifies business impact ($4.4 trillion long-term enterprise value potential; specific Lenovo deployment figures), surveys three tech-architecture enablement patterns, and closes with adoption-hurdle and implementation guidance. Lower technical/governance depth than this corpus's existing agentic-AI security cluster (F036 NIST identity, F037 WEF/Capgemini evaluation, F038 ISACA maturity, F070–F073 Batch 18 security/threat cluster) — this document's value is as a **foundational definitional and business-case anchor**, not a control framework. Most useful for teaching/consulting narrative material (the Lenovo case study is a concrete, named, citable enterprise deployment) rather than technical governance synthesis.

---

## Classification

**Document type:** Industry Explainer
**Primary audience:** Business/enterprise leaders (not technical practitioners, not regulators)
**AI explicit:** Yes — entirely about AI agents

---

## Key Content

### Definition

"An AI agent is a software component that has the agency to act on behalf of a user or a system to perform tasks. Users can organize agents into systems that can orchestrate complex workflows, coordinate activities among multiple agents, apply logic to thorny problems, and evaluate answers to user queries." Named examples: Microsoft Copilot, Amazon Q, Google's Project Astra.

### Five Agent Types (taxonomy)

| Type | Description |
|---|---|
| Individual augmentation ("copilot" agents) | Augments user productivity — Microsoft 365 Copilot, ChatGPT |
| Workflow automation platforms | Orchestrator/executor for single/multistep tasks — Microsoft Copilot Studio, Salesforce Agentforce |
| Gen AI-native agents for domain solutions | Purpose-built for a specific domain — e.g., AI-driven customer service |
| AI-native enterprises and operating models | Woven through the interaction layer, processes, and business model |
| AI virtual workers | Function as employees/team members within the existing operating model |

This is a coarser, business-facing taxonomy than F037's (WEF/Capgemini) autonomy × authority dimensional framework or F036's (NIST) identity-focused classification — useful as an executive-communication register rather than a governance-diagnostic one.

### Four-Step Operational Loop

1. User assigns a task; agent system autonomously plans how to achieve it.
2. Agent system plans, allocates, and executes — a manager agent assigns specialised subagents.
3. Agent system iteratively improves output, requesting user feedback as needed.
4. Agent executes the action.

### Agent–LLM Relationship

Worked example: a self-driving car runs a mixture of agents, some using an LLM (destination understanding) and some using specialised non-LLM models (safe-turn execution) — illustrates that "AI agent" does not imply "LLM-based agent" uniformly; agent systems may mix model types by task.

### Business Impact Figures

- USD 4.4 trillion — potential long-term annual value from enterprise gen AI use cases.
- 14% per hour — issue-resolution increase for orgs using gen-AI customer service agents.
- 9% — reduction in time spent handling issues, same context.
- Lenovo case study: up to 15% improvement in software engineering; "double-digit" productivity gains in customer-service call handling time. Named sources: Arthur Hu (CTO, Lenovo Solutions and Services Group), Linda Yao (COO/Head of Strategy, Lenovo).

### Emergent AI (defined term)

"When agents' capabilities compound in reaction to their environments when they work together. They can develop unexpected behaviors and skills that are not explicitly programmed, equaling greater than the sum of their parts." — directly relevant to [[Agentic_AI_Governance]]'s treatment of unanticipated multi-agent risk, and a softer, business-narrative-register companion to the more technical "excessive agency"/"shadow agent" language used in F071 (AWS) and F073 (Google/Mandiant).

### Three Tech-Architecture Enablement Patterns

| Pattern | Description |
|---|---|
| Super platforms | Next-gen third-party business applications (e.g., CRM) with built-in gen AI agents |
| AI wrappers | Enterprise services communicate with third-party APIs without exposing proprietary data |
| Custom AI agents | Employees fine-tune a pretrained LLM or use RAG with proprietary data |

Worked examples: a CRM super platform auto-generating and communicating sales reports; a bank building a wrapper around an internal credit-risk model to query a vendor LLM without sharing data; an employee building a custom RAG agent from call-centre transcripts/policies.

This three-pattern taxonomy is a useful, business-facing complement to the deployment-model schema already used in [[Agentic_AI_Security_Diagnostic_Template]] §2 (predictive ML / RAG-LLM / fine-tuned LLM / pre-trained LLM / foundational model / external model, per F070 DASF) — the "AI wrapper" pattern in particular maps closely to the "external model" deployment category and is a good plain-language explanation of why that category carries distinct data-exposure risk.

### Adoption Hurdles and Governance-Adjacent Recommendations

- "People must trust AI enough to hand over tasks. Companies' ethical decisions must be rooted in the values unique to each organization and the values of a society that places humans at the center of the AI ecosystem."
- Worked example: a bank addressed trust issues by building an architecture that checks for errors/hallucinations before answers reach a customer — a plain-language business-narrative version of the "human-in-the-loop"/verification-layer control pattern already documented more technically in F070/F071.
- "Companies that are pursuing an AI agent program should carefully implement the proper controls for security, operations, and data" — advisory-strength language, no specific control catalogue (contrast with F070 DASF's 51 named controls).

### Implementation Guidance (three leader focus areas)

1. Scrutinise long-timeline, high-headcount tech proposals for where gen AI could reduce cost/time.
2. Focus on the largest, most complex (expensive, multi-year, technical-debt) problems first.
3. Get ahead of talent, technology, and operating-model implications before scaling.

---

## Consulting/Teaching Reuse

**Highest-value reuse opportunity:** The Lenovo case study (named CTO/COO, specific % figures, both software-engineering and customer-service deployment) is one of the more citable concrete enterprise-deployment examples in the corpus — most other agentic-AI corpus documents (F036–F038, F070–F073) are frameworks/standards/threat-intelligence rather than named case studies. Directly usable as illustrative material in a workshop, briefing deck, or LinkedIn carousel without needing anonymisation, since the client (Lenovo) and the named executives are already public in the source.

**Relevant inbound connections:** None directly (AEGIS_OS/PrivacyWeave/CyberMesh are runtime-enforcement/governance plays; this document is pre-governance business-case material) — but the "three tech-architecture patterns" taxonomy could feed a future workshop module explaining *why* agentic AI needs governance to a non-technical audience, ahead of introducing the technical diagnostic in [[Agentic_AI_Security_Diagnostic_Template]].

---

## Cross-Links

**Related wiki sections:** [[AI_Governance_Wiki]] S4, S7

**Related concepts:** [[Agentic_AI_Governance]], [[Governance_Capacity]]

**Related corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization]] (identity-focused vs. this document's business-case focus), [[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance]] (finer-grained autonomy/authority taxonomy vs. this document's five-type business taxonomy), [[04_Knowledge_Products/Wiki_Intake/F070_Databricks_AI_Security_Framework_DASF]] (deployment-model schema this document's "wrapper" pattern maps to)

**Consulting:** [[Agentic_AI_Security_Diagnostic_Template]] §1 (Agentic AI System Inventory) — this document's five-type taxonomy and three architecture patterns are useful plain-language framing to walk a client through before applying the more technical inventory schema

**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted (via NotebookLM extraction relay, PROMPT 0b)
- [x] Wiki sections updated
- [x] Linked to relevant concept notes
- [x] Marked processed

---

## ⚠ VERIFY BEFORE PUBLISHING

- **#210 — Publication date — LOW.** Only "March 2025" is stated; exact day not captured. Verify via McKinsey's website before using a precise date in a formal citation.
- **#211 — Business-impact figures — MEDIUM.** The $4.4 trillion long-term value figure, the 14%/9% customer-service figures, and Lenovo's specific percentages (15% engineering improvement, "double-digit" productivity gains) are McKinsey's own reported figures with no independent methodology disclosed in this explainer — treat as McKinsey-asserted, not independently verified, if citing externally.

---

## Log

- 2026-07-15: Node created via NotebookLM extraction relay (PROMPT 0b). No duplicate found in corpus (checked McKinsey-as-source, Lenovo, and title match — all clean; existing McKinsey mentions elsewhere in the corpus are incidental statistic citations within other nodes, e.g. F047, International_9).

---

_Back to [[Wiki_Intake_Index]] | [[AI_Governance_Wiki]]_
