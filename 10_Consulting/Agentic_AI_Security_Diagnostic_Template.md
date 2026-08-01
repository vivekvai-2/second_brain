---
type: Consulting Template
tags:
  - type/consulting-template
  - status/active
  - engine/consulting
  - engine/knowledge-product
  - content/checklist
  - topic/agentic-ai-governance
---

# Agentic AI Security & Control Maturity Diagnostic — Template

**Type:** Consulting Deliverable Template
**Status:** Active
**Created:** 2026-07-15
**Use for:** Paid diagnostic engagements assessing a client's agentic AI deployments (piloted or production) against architectural maturity, control-implementation completeness, and identity/authority-binding readiness. Sibling instrument to [[Governance_Diagnostic_Report_Template]] — that template scores regulatory-overlap exposure; this one scores technical-governance readiness for autonomous/agentic systems specifically.
**Anchors on:** [[Agentic_AI_Governance]], [[Governance_Capacity]], [[Accountability]]

---

## Purpose

Most clients adopting agentic AI (LLM-orchestrated agents, tool-calling systems, multi-agent workflows) have no structured way to answer three questions: how mature is our agentic AI security posture, which specific controls are and are not implemented, and are our agents individually identifiable and authority-bound at runtime. This diagnostic answers all three using scoring instruments already validated against the corpus rather than invented per engagement — do not re-derive the diagnostic logic; instantiate it against the client's specific agent inventory.

This is also, not incidentally, the diagnostic that precedes an AEGIS_OS-style runtime-enforcement engagement: Section 4 below is designed to surface exactly the gaps a pre-execution enforcement layer closes.

---

## 1. Agentic AI System Inventory

List every agentic AI system the client operates or is piloting. Classify each against the seven-dimension schema from [[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance|F037]] (WEF/Capgemini).

| Agent / System | Business Function | Autonomy Level | Authority Scope | Data / Tool Access | Deployment Status (Pilot / Production) |
|---|---|---|---|---|---|
| | | | | | |

**Output:** a one-page agentic AI footprint — in most engagements, the first time the client has seen every autonomous system they operate listed in one place, including "shadow agent" deployments nobody centrally approved.

---

## 2. Control-Catalogue Coverage Assessment

Score the client's agentic AI systems against the 12-component / 51-control structure in [[04_Knowledge_Products/Wiki_Intake/F070_Databricks_AI_Security_Framework_DASF|F070]] (Databricks DASF). Do not reproduce all 51 controls verbatim in the client deliverable — pull the specific controls relevant to the client's deployment-model mix (predictive ML / RAG-LLM / fine-tuned LLM / pre-trained LLM / foundational model / external model) from the source node.

| DASF Component | Control Area | Implemented? (Y/N/Partial) | Evidence | Deployment Model(s) Affected |
|---|---|---|---|---|
| Data sources / ingestion | | | | |
| Serving / inference | | | | |
| Model registry / feature store | | | | |
| Orchestration | | | | |
| Agent / tool layer | | | | |
| Monitoring | | | | |

**Note:** flag explicitly, per [[Corpus_Index_MOC]] VERIFY #199–200, that DASF's control counts are the vendor's own self-reported scope — treat as a checklist instrument, not an audited-compliance certification, when presenting findings to the client.

---

## 3. Maturity Scoring (CMMI 5-Level)

Score the client against the four foundational principles from [[04_Knowledge_Products/Wiki_Intake/F038_ISACA_Agentic_AI_Security_Best_Practices|F038]] (ISACA), Level 1 (Initial: ad hoc, no agentic-specific controls) through Level 5 (Optimising: continuous improvement, automated governance enforcement).

| Foundational Principle | Current Level (1–5) | Evidence | Target Level | Gap |
|---|---|---|---|---|
| Observability (agent actions visible, monitorable, auditable in real time) | | | | |
| Bounded Autonomy | | | | |
| Ephemeral Identity | | | | |
| Preserve Coordination Trust | | | | |

**Benchmark note:** most Indian BFSI entities are estimated (per corpus finding, Batch 13) to sit at Level 1–2 on this scale — use as a sector baseline, not a client-specific assumption.

---

## 4. Identity & Authority-Binding Readiness

This section is the direct diagnostic precursor to an AEGIS_OS-style runtime enforcement conversation. It converges three independent evidentiary genres — federal standards ([[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization|F036]], NIST NCCoE), vendor best-practice ([[04_Knowledge_Products/Wiki_Intake/F071_AWS_AI_for_Security_and_Security_for_AI_2025|F071]], AWS), and threat intelligence ([[04_Knowledge_Products/Wiki_Intake/F073_Google_Cloud_Mandiant_Cybersecurity_Forecast_2026|F073]], Google Cloud/Mandiant) — that independently reach the same architectural conclusion: agents need distinct, individually accountable identities with dynamic, just-in-time, delegation-chain-bound authorization.

| Dimension | Client Practice | Gap | Runtime-Enforcement Opportunity |
|---|---|---|---|
| Identification — is each agent a distinct identity, or does it inherit a shared service-account/human identity? (F036) | | | |
| Authentication & Authorization — is agent access scoped and time-bound, or standing/broad? (F036) | | | |
| Access Delegation / Chain of Delegation — can the client trace which human or agent authorised a given downstream action? (F036, F073) | | | |
| Excessive-Agency Controls — are there permission boundaries, throttles, or alarms preventing automation loops / run-away tasks? (F071) | | | |
| Logging / Audit — is every agent action logged with sufficient granularity for post-incident reconstruction? (F036) | | | |
| Shadow Agent Exposure — can employees deploy agents outside a governed pipeline, and is this monitored rather than merely prohibited? (F073) | | | |

**Classification rule:** any dimension scored "Gap = standing/broad authority with no delegation trail" is a direct, immediately quotable case for pre-execution runtime enforcement — this is the sentence-level bridge from diagnostic finding to AEGIS_OS engagement pitch.

---

## 5. Recommendations (Three Levels)

Mirror the recommendation architecture in [[Governance_Diagnostic_Report_Template]] §5 — credibility comes from distinguishing what the client cannot fix from what they can.

### Ecosystem level (context only — not actionable by client)
- Note any standards-maturity gaps the client is exposed to but cannot remedy (e.g. NGAC/SPIFFE-SPIRE for AI agents remain early-adoption per F036 — the client cannot single-handedly mature an immature standard).

### Enterprise level (actionable — this is the paid deliverable's core value)
1. Control-catalogue closure opportunities — which specific DASF controls (Section 2) close the largest number of Section 4 gaps simultaneously.
2. Maturity-uplift sequencing — which CMMI principle (Section 3) to invest in first for the fastest Section-4 gap closure.
3. Runtime enforcement opportunities — where a technical pre-execution control (cf. AEGIS_OS pattern in [[Inbound_Pipeline_Index]]) converts a standing-authority gap into an enforced, auditable authorization boundary.

### Board level
- A one-slide summary translating Sections 3–4 into a board-legible risk statement — reuse [[Board_AI_Risk_Oversight_Checklist]] as the board-facing companion instrument, and format for direct reuse in [[Executive_Board_Briefing_Deck_Template]].

---

## Engagement Notes

- **Typical scope:** single client entity, agentic AI systems only (not general AI/ML estate — see [[Governance_Diagnostic_Report_Template]] for the broader regulatory-overlap diagnostic), 3–5 week window.
- **Pricing anchor:** fixed-fee diagnostic — the four-section scoring structure is what makes fixed-fee pricing defensible against a client's own uncosted "just tell us what to do" ask.
- **Upsell path:** diagnostic → [[Workshop_Masterclass_Curriculum_Template]] (agentic AI security workshop variant) → AEGIS_OS or equivalent runtime-enforcement pilot conversation.
- **Confidentiality:** client-specific instances of Sections 1–4 stay in the client deliverable only. Do not log client names in vault concept "Instances in Corpus" sections — those are reserved for published/public regulatory corpus evidence.
- **Scope discipline:** per [[AEGIS_OS_Inbound]]'s gate, keep all client conversations framed around commercial/enterprise/BFSI agentic AI use cases. Defer any defence-adjacent agentic AI scenario to post-superannuation.

---

## Linked Vault Nodes

**Signature/Standard Concepts:** [[Agentic_AI_Governance]], [[Governance_Capacity]], [[Accountability]]

**Source Corpus Nodes:** [[04_Knowledge_Products/Wiki_Intake/F038_ISACA_Agentic_AI_Security_Best_Practices|F038]], [[04_Knowledge_Products/Wiki_Intake/F070_Databricks_AI_Security_Framework_DASF|F070]], [[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization|F036]], [[04_Knowledge_Products/Wiki_Intake/F073_Google_Cloud_Mandiant_Cybersecurity_Forecast_2026|F073]], [[04_Knowledge_Products/Wiki_Intake/F071_AWS_AI_for_Security_and_Security_for_AI_2025|F071]], [[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance|F037]]

**Knowledge Products:** [[AI_Governance_Wiki]], [[BFSI_AI_Governance_Handbook]]

**Domains:** [[AI_Governance]], [[Cybersecurity_Governance]], [[BFSI_Governance]]

**Consulting:** [[Consulting_Deliverable_Templates_Index]], [[AEGIS_OS_Inbound]], [[Inbound_Pipeline_Index]], [[Board_AI_Risk_Oversight_Checklist]]

---

_Back to [[Consulting_Deliverable_Templates_Index]]_
