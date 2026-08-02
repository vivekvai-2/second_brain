---
type: Standard Concept
tags:
  - type/concept-standard
  - status/active
  - paper/p3
  - paper/p4
  - gate/open
  - engine/consulting
  - engine/teaching
  - engine/linkedin
  - engine/knowledge-product
  - content/carousel-ready
  - content/thought-leadership
---

# Agentic AI Governance

**Type:** Standard Concept  
**Status:** Active — Emerging Consensus (standards not yet settled; NIST/WEF working 2025–26)  
**Last Updated:** 2026-06-14  
**Wiki section:** S4 (Agentic AI Governance)  
**Feeds:** [[AI_Governance_Wiki]] S4 | [[BFSI_AI_Governance_Handbook]] | [[Regulatory_Complexity_Handbook]]

---

## Definition

An AI agent is software with autonomy to act on behalf of users or systems — orchestrating complex workflows, taking decisions, and executing actions without requiring human approval at each step. Agentic AI governance is the set of design choices, accountability structures, audit mechanisms, and runtime controls required to deploy agents with known risks and demonstrable accountability.

The governance challenge is not that agents are intelligent. It is that agents are **fast, chained, and consequential** — three properties that collectively break the assumptions embedded in every existing governance framework designed for human-paced, sequential, document-based decision-making.

---

## Why Agents Change Governance — Five Structural Breaks

### Break 1: Decision Velocity Eliminates the Human Review Window
Traditional governance inserts humans at decision points. Agents eliminate those points. A KYC agent processing 10,000 customer verifications overnight has made 10,000 regulatory decisions before any human reviews the output. Governance must shift from **review before action** to **design before deployment** — the only moment where human oversight is genuinely effective.

*Consulting signal:* If an organisation's AI governance framework primarily consists of approval gates and review committees, it was designed for human-paced tools. It will not catch agent errors until after they have cascaded.

### Break 2: Chained Systems Propagate Errors Without Correction
In a multi-agent workflow (KYC agent → fraud scoring agent → credit decision agent), an error in Agent 1 propagates to Agents 2 and 3 with compounding confidence. No agent in the chain flags an input as erroneous — it simply acts on what it received. The end-state failure (wrong credit denial) is untraceable to a specific decision point without isolated decision logs per agent.

*Consulting signal:* Any organisation deploying chained LLM workflows without agent-level decision isolation is accumulating unauditable liability.

### Break 3: Design Choices Lock In Governance for the System's Lifetime
The governance architecture of an agentic system is determined at the design phase — not at the deployment phase, and not during audits. Choosing between a single orchestrating agent vs. ten parallel specialist agents carries different audit burdens, different failure modes, and different regulator expectations. This choice, typically made by engineers in a sprint planning session, is a governance decision with multi-year implications. It cannot be remedied later without rebuilding the system.

*Teaching application:* Case study prompt — "A CTO chose to build 12 microagents rather than 1 orchestrating agent to accelerate development. Three months later, a customer complaint revealed a cascading error across 7 agents. Who is accountable? What governance artifacts should have existed at design time?"

### Break 4: Shared State Destroys Audit Trail Coherence
When multiple agents share a state object (a customer record, a transaction context, a risk score), it becomes impossible to reconstruct "what did Agent A decide based on?" because Agent B may have modified shared state before Agent A logged its decision. Regulators testing audit trails will ask: "Show me every piece of information your KYC agent relied on to make this specific decision." If the answer requires reconstructing shared state changes across multiple agents, the audit trail has failed — regardless of whether logs exist.

*Regulatory implication (India BFSI):* RBI's IT Governance Master Direction 2023 requires audit trails supporting forensic evidence. Shared state in agentic systems is structurally incompatible with this requirement unless agent-level state snapshots are taken before each decision.

### Break 5: Regulators Now Treat Agents as Regulated Entities, Not Tools
Regulators do not yet have agent-specific rules in most jurisdictions. But they are applying existing frameworks with increasing sophistication. RBI treats any agent performing a regulated function (KYC determination, credit decision, collections instruction) as an **outsourced function** under Material Outsourcing Directions — regardless of whether the agent was built in-house or procured from a vendor. SEBI's 2024–25 Board Memorandum (SEBI_11) explicitly extends AI responsibility to third-party AI tools. NIST is developing agent identity frameworks that treat agents as authenticated principals, not passive software.

*The governance implication:* An agent is not a tool you deploy. It is a decision-maker you are accountable for.

---

## The Runtime Enforcement Gap

Every existing governance framework operates in one of two modes:
- **Pre-deployment:** Policies, risk assessments, DPIAs, approval gates
- **Post-deployment:** Audit logs, incident reports, regulatory inspections

Agentic AI creates a third governance moment — **runtime** — where the decision is being made, at speed, with data the pre-deployment assessment may not have anticipated. Most organisations have no governance infrastructure at the runtime layer. They have policy documents (pre-deployment) and audit logs (post-deployment), but nothing between them.

This is the gap that products like AEGIS OS (runtime decision enforcement, pre-execution validation in <50ms) and PrivacyWeave (runtime data usage evaluation, allow/deny before data moves) are designed to fill. The existence of these products is evidence that the governance gap is commercially visible.

**The governance architecture that works for agents requires all three layers:**

| Layer | Governance Mechanism | When It Operates |
|-------|---------------------|-----------------|
| Pre-deployment | Risk classification, DPIA, design review, agent register | Before build |
| Runtime | Authority binding, admissibility checks, kill switch, purpose enforcement | At decision point |
| Post-deployment | Immutable audit logs, incident detection, regulator reporting | After action |

Most regulated organisations in India currently have only the pre-deployment layer (policies) and a partial post-deployment layer (logs). Runtime enforcement is absent.

---

## Agent System Register — The Minimum Governance Artifact

An agent system register is the foundational governance document for agentic AI. It is not optional for any organisation subject to RBI, SEBI, or DPDP. Without it, there is no way to demonstrate that an organisation knows what agents it is running, who is accountable for them, or what data they access.

**Minimum required fields per agent:**

| Field | Content | Regulatory Driver |
|-------|---------|------------------|
| Agent Identity | Name, version, unique ID | RBI IT Governance §15 (audit trails) |
| Purpose | What decisions does it make? | DPDP DPIA requirement |
| Data Access | What personal/sensitive data? | DPDP §3 (data minimisation) |
| Owner | Named individual with Board-level escalation | RBI IT Governance ITSC; SEBI_11 responsibility assignment |
| Risk Classification | Prohibited / High / Medium / Low | EU AI Act framework; RBI model risk |
| Architecture | Single agent / chained / multi-agent / human-in-loop | Audit trail design determinant |
| Regulatory Status | DPDP / RBI / SEBI / IRDAI applicable? | Compliance evidence |
| Monitoring | What metrics? What triggers escalation? | RBI §27 incident management |
| Incident History | What failed? How resolved? | RBI §27(d) CERT-In + RBI notification |

---

## Five Governance Changes Agents Require

| Governance Dimension | Traditional AI/ML Governance | Agentic AI Governance | Gap |
|---------------------|------------------------------|----------------------|-----|
| Human oversight | Review output before action | Design before deployment; override at runtime | Oversight moves earlier and becomes automated |
| Audit trail | Log what the system did | Log what each agent decided, based on what state | Per-agent decision isolation required |
| Accountability | Owner of the system | Owner of the function the agent performs | Function-based accountability, not system-based |
| Error correction | Detect and fix | Detect before cascade; kill switch in <50ms | Real-time intervention required |
| Regulatory reporting | System-level incident | Agent-level incident; which agent, which decision | Granular incident taxonomy required |

---

## India Regulatory Landscape for Agentic AI

### Current position (June 2026)
No Indian regulator has issued agent-specific governance rules. Governance is applied via four existing hooks:

**RBI (Banking):** Material Outsourcing Directions apply to any agent performing a regulated function — KYC, credit decisions, collections, fraud detection. The hook is the function, not the label "AI agent." Board-approved outsourcing policy, vendor due diligence, continuous monitoring, 6-hour incident notification to RBI, and CERT-In notification all apply. This extends to in-house built agents, not only vendor-provided ones.

**SEBI (Securities):** SEBI_11 (Board Memo 2024–25) proposes mandatory responsibility assignment for AI tools used by MIIs and Intermediaries, covering third-party AI tools explicitly. Audit trails showing decision logic for trading and surveillance AI expected. Pending formal regulation — watch for notification.

**DPDP (All Sectors):** Any agent processing personal data requires DPIA. Purpose limitation applies at runtime — an agent collecting data for KYC cannot repurpose it for model training without explicit consent. Data minimisation means agents should not access more personal data than necessary for the specific decision. Breach notification mandatory and expedited.

**CERT-In (All Sectors):** Cyber incident notification required. Adversarial AI threat taxonomy (CIAD-2025-0013) published March 2025 — covers prompt injection, model stealing, hallucination exploitation, backdoor attacks. Advisory only (not binding) as of June 2026. AIBOM requirement (CERT_4, July 2025) applies to government AI procurement — BFSI entities with government contracts face AIBOM obligations.

### The multi-regulator collision scenario (highest risk)
A BFSI entity deploying a KYC-to-credit-decision agentic chain is simultaneously subject to:
- DPDP (personal data in every agent decision)
- RBI (regulated function performed by each agent)
- SEBI (if the entity is also a registered intermediary)
- CERT-In (cyber incident notification)

A single agent failure in this chain triggers notifications to multiple regulators with different timelines, different formats, and no coordinated response protocol. This is the multi-regulator incident response gap flagged in the AI Governance Wiki S8.3. There is currently no tested playbook for this scenario in Indian BFSI.

---

## Consulting Application Map

### AEGIS OS (🟡 Open — Non-Defence Scope)
AEGIS OS is a runtime decision control layer that implements the **runtime enforcement gap** this concept describes. Its architecture directly operationalises the five governance breaks:

| AEGIS Capability | Governance Break It Addresses |
|-----------------|-------------------------------|
| Pre-execution enforcement in <50ms | Break 1 (decision velocity) — shifts governance to runtime |
| Authority binding (RBAC/ABAC) at decision point | Break 2 (chained propagation) — blocks invalid inputs before cascade |
| Tamper-proof hash-linked audit trail | Break 4 (shared state) — creates per-decision immutable evidence |
| Fail-safe kill switch <50ms | Break 3 (design lock-in) — provides runtime override independent of agent architecture |
| PQC-ready communications | Break 5 (regulatory treatment) — satisfies CERT-In CBOM/QBOM requirement (CERT_4) |

**Advisory framing for AEGIS (commercial/BFSI positioning):**
"AEGIS OS is what the gap between your DPDP policy and your agent's actual behaviour looks like when it is closed. Every Indian bank deploying an agent for KYC or credit decisions has a governance architecture with a missing middle — policy above, logs below, nothing at the moment of decision. AEGIS closes the middle."

**LinkedIn hook (Carousel 1):** "Your KYC agent made 10,000 decisions last night. Your governance framework reviewed zero of them in real time. Here is what runtime AI governance actually looks like."

### PrivacyWeave (🟢 Open)
PrivacyWeave implements the runtime enforcement gap specifically for **data usage** — the DPDP purpose limitation obligation at the moment data moves, not in the policy document.

| PrivacyWeave Capability | Governance Break It Addresses |
|------------------------|-------------------------------|
| Runtime purpose check before data moves | Break 1 (decision velocity) — governance at the moment it matters |
| Allow / partial mask / deny in <100ms | Break 5 (regulatory treatment) — DPDP purpose limitation at runtime |
| Automatic audit log per decision | Break 4 (shared state) — per-access immutable evidence trail |

**Advisory framing for PrivacyWeave (DPDP/India positioning):**
"The DPDP Act requires purpose limitation — data collected for KYC cannot silently become model training data. PrivacyWeave enforces that requirement at the moment the data moves, not in a policy document that no system reads."

**LinkedIn hook (Carousel 2):** "DPDP says your agents can only use data for the purpose you collected it. Who enforces that at 2am when your model retraining pipeline runs? This is the governance primitive that most DPDP compliance frameworks are missing."

### CyberMesh PS-69 / PS-74 (🔴 Conflict Hold — Research Leverage Only)
CyberMesh's architecture surfaces the **distributed trust** problem in agentic systems — how do you govern a system where trust must be re-earned at every hop, not assumed from initial authorisation?

**Research leverage (not consulting):**
The quorum-governed key recovery model (3-of-5, dual-authorisation, logged reconstruction) is an operational implementation of distributed accountability — the governance property that no single actor can make a consequential decision unilaterally. This is directly relevant to the accountability construct in P4 and to the governance design principles in the AI Governance Wiki S1.4 (Decision Stack).

Post-superannuation: CyberMesh's deception-layer architecture (proactive detection through shaped attacker behaviour) is an agentic governance pattern — agents as sensors, not just actors — worth developing as a concept note in `09_Teaching/` for defence governance case studies.

---

## LinkedIn Carousel Architecture (Three Carousels)

### Carousel 1 — "Your Agents Aren't Tools. They're Decision-Makers."
*Engine: Thought leadership + AEGIS framing*

| Slide | Content |
|-------|---------|
| 1 (Hook) | "Your KYC agent made 10,000 decisions last night. Your governance reviewed zero in real time." |
| 2 | What an AI agent actually is — autonomy, chaining, consequence — vs what most people think it is |
| 3 | The 5 governance breaks: velocity, cascade, design lock-in, shared state, regulatory treatment |
| 4 | The runtime gap: pre-deployment policy + post-deployment logs ≠ governance |
| 5 | What runtime governance looks like: authority binding, kill switch, per-decision audit trail |
| 6 | India regulatory hook: RBI Material Outsourcing applies to in-house KYC agents. SEBI_11 is coming. DPDP applies to every decision. |
| 7 (CTA) | "The question is not whether your agents are compliant. The question is whether you can prove it." |

### Carousel 2 — "DPDP and Agents: The Gap Nobody is Talking About"
*Engine: India regulatory + PrivacyWeave framing*

| Slide | Content |
|-------|---------|
| 1 (Hook) | "DPDP says purpose limitation. Your agents don't read your DPDP policy." |
| 2 | What purpose limitation means in practice — and why it fails with agents |
| 3 | The three DPDP obligations agents violate by default: purpose, minimisation, consent |
| 4 | The multi-regulator collision: DPDP + RBI + SEBI + CERT-In on one agent failure |
| 5 | What runtime purpose enforcement looks like vs governance theatre |
| 6 | The audit trail question regulators will ask: "Show me every piece of data your agent used for this specific decision." |
| 7 (CTA) | "DPDP compliance for agents is not a policy document exercise. It is an architecture problem." |

### Carousel 3 — "How to Build an Agent Your Regulator Can Audit"
*Engine: Practitioner checklist + Board visibility*

| Slide | Content |
|-------|---------|
| 1 (Hook) | "A regulator walks in and asks to audit your KYC agent. What do you show them?" |
| 2 | The agent system register: 9 fields every regulated organisation needs |
| 3 | Per-agent decision isolation: why shared state is an audit trail failure |
| 4 | The design-phase governance questions you must answer before building |
| 5 | The 90-day minimum: agent register + risk classification + kill switch + incident playbook |
| 6 | India context: RBI 6-hour notification + CERT-In notification + SEBI audit trail — on one agent failure |
| 7 (CTA) | "Governance-by-design for agents. Not governance-by-audit-after-the-fact." |

---

## Teaching Application

**Core case study:** "The KYC Chain Failure"
- A bank deploys a 3-agent chain (KYC → fraud scoring → credit decision)
- Agent 1 flags a customer as marginal (confidence: 0.61)
- Agent 2 interprets the marginal flag as a fraud signal (no human review point)
- Agent 3 denies credit based on the fraud signal
- The customer complains; the bank cannot reconstruct which agent made which decision
- DPDP audit trail requirement: failed. RBI model risk requirement: failed. SEBI audit trail (if applicable): failed.

**Discussion questions:**
1. At what design decision did this governance failure originate?
2. What governance artifact would have prevented cascade to Agent 3?
3. Who is accountable — the KYC team, the fraud team, the credit team, or the CISO?
4. What does RBI Material Outsourcing require in this scenario?
5. Draft the incident notification sequence: CERT-In, RBI, DPB.

**Frameworks activated:** AI Governance Maturity (S1.2), Accountability Decision Stack (S1.4), India Regulatory Stack (S2), Agent System Register (S4.2), BFSI Use Case Governance (S7.1)

---

## Instances in Corpus

- [[04_Knowledge_Products/Wiki_Intake/Schuett_Three_Lines_Defense_AI_2023]] — direct 3LoD-to-AI-company mapping (first/second/third line roles for AI developers) plus a proposed AI-company org chart; the most direct academic precedent for agent system register / accountability-line design under Break 3 (design lock-in) and Break 5 (regulators treat agents as regulated entities).
- [[04_Knowledge_Products/Wiki_Intake/AFM_Algorithmic_Trading_Governance_2021]] — MAR Art.13/Art.18 governance-and-access-control precedent directly transferable to agent system register "Data Access" and "Regulatory Status" fields for AI-driven trading agents.
- [[04_Knowledge_Products/Wiki_Intake/FCA_Algorithmic_Trading_Compliance_2018]] — four-pillar (governance/oversight, development/testing, risk controls, market conduct) diagnostic, reusable as a pre-deployment layer checklist for agentic trading systems.
- (Batch 6) [[04_Knowledge_Products/Wiki_Intake/AgenticRisks_Enterprise_Wide_Agentic_AI_Risk_Controls_2025]] (F025) — most granular agentic-AI control taxonomy in the corpus to date: 5 categories / 30 risks / 242 controls, with "Governance Failures" (Category D) the single largest category (33% of controls) — directly operationalises Agentic_AI_Governance at control-level granularity.
- (Batch 6) [[04_Knowledge_Products/Wiki_Intake/Eisenberg_Gamboa_Sherman_Unified_Control_Framework_2025]] (F026) — complementary general-enterprise (42-control) layer to F025's agentic-specific (242-control) layer; combined "general + agentic" control-coverage map is a strong P4 deliverable.
- (Batch 6) [[07_Institutions/Corpus/RBI/RBI_5_Operational_Risk_Management_Resilience_NBFC_Guidance_2024]] — RBI's 3LoD/OORF operational-risk architecture (with NBFC-BL line-1/line-2 combination concession) is a direct India-regulatory structural comparator for F021's (Tammenga) AI-specific 3LoD role allocation and F025's Category D governance-ownership controls.
- (Batch 6) [[04_Knowledge_Products/Wiki_Intake/Danielsson_Macrae_Uthemann_AI_Systemic_Risk_2022]] (F030) — "trust creep"/irreversibility argument (2022) and EURISKO reward-hacking example are early/foundational precursors to F025's Category D "Governance Failures" (accountability, explainability, AI-as-moral-agent rejection) — useful intellectual-lineage citation for P1 SLR.
- (Batch 7) [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]] — documents three confirmed Indian judicial AI-hallucination incidents (Karnataka HC trial judge, March 2025; ITAT recalled order, February 2025; Delhi HC ChatGPT-drafted plea, August 2023) alongside the Stanford RegLab 17-34% legal-AI hallucination-rate finding — the corpus's strongest evidentiary basis for human-in-the-loop mandates, directly comparable to NCAIC_1's evaluation gates and CERT_In_1's audit-verification chain.
- (Batch 7) [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] — introduces "AI System Audits" and "AIBOM Auditing" as new audit categories under Section 70B, the first operative (non-proposed) audit mandate in the corpus explicitly targeting AI-system components.
- (Batch 7) [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] — proposed risk-tiering and evaluation-gate architecture for a national AI-governance coordinator; "proposed" counterpart to CERT_In_1's "operative" audit mandate.

- (Batch 13) [[04_Knowledge_Products/Wiki_Intake/F035_Microsoft_Administering_Governing_Agents]] — enterprise operationalization of agentic AI governance: three-tier spectrum (End Users/Makers/Developers), three control types, Microsoft Purview compliance backbone (DLP + sensitivity labels + audit log + eDiscovery + insider risk). Most detailed vendor-level implementation of agentic governance in the corpus; cite as industry evidence with ecosystem-specificity caveat.
- (Batch 13) [[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization]] — first NIST NCCoE-level articulation of agent identity governance as a distinct cybersecurity problem: six focus areas (Identification, Authentication, Authorization, Access Delegation, Logging/Audit, Data Flow Tracking); standards stack (MCP, OAuth 2.0/2.1, OIDC, SPIFFE/SPIRE, SCIM, NGAC); Zero Trust (SP 800-207) and least-privilege as foundational principles; prompt injection as identity governance failure.
- (Batch 13; enriched 2026-07-15) [[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance]] — most comprehensive multi-stakeholder agentic AI governance framework in corpus: seven-dimension classification schema (Function, Role, Predictability, Autonomy, Authority, Use Case, Environment), now illustrated with four worked case studies (robot vacuum, coding co-pilot, autonomous vehicle, personal assistant) plus a BFSI fraud-detection-in-online-banking example; four-stage progressive governance (Classification → Evaluation → Risk Assessment → Governance), now specified precisely as a five-step risk assessment life cycle (Define context → Identify risks → Analyse risks → Evaluate risks → Manage risks) and a nine-mechanism Baseline Governance Table; **five** multi-agent system risks (orchestration drift, semantic misalignment, security and trust gaps, cascading effects, systemic complexity — expanded 2026-07-15 from three originally captured); MCP/A2A/AP2/ACP protocol stack. Regulatory anchors: OECD AI Rec, NIST AI RMF 1.0, ISO/IEC 42001, NIST AI 600-1. Contains a governance-language zero-trust statement ("every agent interaction should be treated as untrusted by default") that pairs with F036's technical SP 800-207 zero-trust architecture.
- (Batch 13) [[04_Knowledge_Products/Wiki_Intake/F038_ISACA_Agentic_AI_Security_Best_Practices]] — practitioner security governance: four foundational principles (Observability, Bounded Autonomy, Ephemeral Identity, Preserve Coordination Trust); five threat categories including CVE-2025-6167 (Identity/Privilege Abuse); CMMI-based 5-level Agentic AI Security Maturity Model; eight target architecture defense planes. Ephemeral Identity principle operationalizes F036's Authentication and Access Delegation focus areas — strongest intra-Batch-13 cross-link.

- (Batch 14 — Autonomy and adaptiveness as the foundational agentic AI governance legal challenge) [[04_Knowledge_Products/Wiki_Intake/F046_UK_LawCommission_AI_and_Law_DiscussionPaper_2025]] — UK Law Commission AI and the Law Discussion Paper (2025), Theme 1 (Autonomy and Adaptiveness): the most legally precise treatment of agentic AI governance in the corpus. AI systems that act beyond their training/instructions, adapt in deployment, and take unanticipated actions challenge agency doctrines (principal-agent; privity of contract) structured around human principals directing each act. Theme 3 (Mens Rea) extends the agentic governance problem to criminal and regulatory law: AI-generated financial market manipulation (s.89 FSA 2012 worked example, directly analogous to SEBI PFUTP) does not trigger mens rea requirements because the AI cannot possess criminal intent. For India BFSI governance: SEBI AI circulars and RBI FREE-AI address AI as a supervised tool; none addresses AI as an autonomous agent whose actions cannot be attributed to an instructing human at the moment of action.
- (Batch 14 — Developer-level agentic AI governance deficit / Existential Safety D/F; Human Uplift Trials absent) [[04_Knowledge_Products/Wiki_Intake/F048_FLI_AI_Safety_Index_Winter_2025]] — Future of Life Institute AI Safety Index Winter 2025 (December 2025): Existential Safety domain — all 8 frontier AI companies score D or F for the second consecutive edition. Two specific agentic-threshold governance gaps: (1) zero companies have conducted Human Uplift Trials (testing whether AI systems provide meaningful assistance to actors attempting mass-casualty events at autonomous operation scale); (2) zero companies have commissioned Independent Reviews of their Safety Evaluation methodologies (whether safety evaluation systems are sufficient to govern increasingly autonomous AI). "Foundational hypocrisy" at the developer level (F048) mirrors "decoupling" at the deployer level (F047) and "adaptiveness" at the legal doctrine level (F046) — the same structural governance failure mechanism operating across the full AI supply chain in Batch 14's Risk/BFSI + Legal sub-cluster: formal commitments without operational safety governance.

- (Batch 15 continuation — BFSI-industry operationalisation of agentic AI risk / minimal footprint + reversibility) [[04_Knowledge_Products/Wiki_Intake/MindForge_MAS_AI_Risk_Management_Executive_Handbook]] (F054) — MindForge C8 (Agentic AI Risk) is the corpus's most operationalised treatment of agentic AI in the BFSI sector. Five specific agentic AI controls: (1) human-in-the-loop for all consequential actions; (2) scope limitation by design ("minimal footprint" principle — agent authorised for minimum necessary actions); (3) reversibility requirement (prefer reversible over irreversible actions); (4) monitoring of multi-step action chains; (5) explicit authorisation boundaries for agent-to-agent interactions. "Minimal footprint" and reversibility are the operational vocabulary that F046's UK Law Commission theoretical agentic-AI governance challenge lacks; MindForge C8 is the first BFSI-sector instrument to convert theory into control specification. India RBI/SEBI have no equivalent agentic AI risk category.
- (Batch 15 continuation — Practitioner-competency taxonomy for agentic AI governance) [[04_Knowledge_Products/Wiki_Intake/IAPP_AIGP_Body_of_Knowledge_v21_2026]] (F055) — Domain IV of AIGP BoK v2.1 (effective Feb 2026) explicitly expands to cover agentic AI governance: autonomous action risk, tool-use governance, multi-agent system oversight are named AIGP competency areas. This reflects the profession's formal recognition of agentic AI as a distinct governance challenge requiring practitioner-competency-level competence. For India: absence of AIGP-equivalent competency ecosystem means agentic AI governance competency is not systematically developed among Indian AI governance practitioners; Domain IV agentic-governance competency deficit is a specific practitioner-capacity gap.

- (Batch 18 — vendor control-catalogue layer beneath F038's architecture) [[04_Knowledge_Products/Wiki_Intake/F070_Databricks_AI_Security_Framework_DASF]] — Databricks AI Security Framework (DASF) v1.0: 12-component AI-system decomposition, 55 technical security risks, 51 numbered mitigation controls (DASF 1–51), each tagged against a 6-way deployment-model matrix (predictive ML/RAG-LLM/fine-tuned LLM/pre-trained LLM/foundational model/external model). Agent/tool-layer is one of twelve components, not the organising principle — materially narrower agentic scope than F036/F038, but the most granular control-numbering instrument in the corpus. Read as the control-implementation layer beneath F038's architectural/maturity-model layer.
- (Batch 18 — AEGIS_OS-relevant runtime enforcement, vendor-practitioner genre) [[04_Knowledge_Products/Wiki_Intake/F071_AWS_AI_for_Security_and_Security_for_AI_2025]] — AWS "AI for Security and Security for AI" (Nov 2025): explicit "excessive agency" prevention best practice (permission boundaries, throttles/alarms on agent workflows to stop automation loops/run-away tasks) and automated-reasoning-as-guardrail (formal verification of LLM outputs against a mathematical policy model, illustrated via an airline-refund worked example). Complements F038/F036 with a formal-verification technique neither covers, and gives Big Tech corroboration of the runtime pre-execution enforcement thesis underlying AEGIS_OS.
- (Batch 18 — senior-leadership governance-question framing, multi-stakeholder genre) [[04_Knowledge_Products/Wiki_Intake/F072_WEF_Oxford_AI_Cybersecurity_Balancing_Risks_Rewards_2025]] — WEF AI Governance Alliance + Oxford GCSCC "Artificial Intelligence and Cybersecurity" (Jan 2025): frames AI cyber risk management as a repeating lifecycle discipline ("shift left, expand right, and repeat") requiring a cross-disciplinary risk function (legal, cyber, compliance, technology, risk, HR, ethics). Derived from structured multi-stakeholder workshops/interviews rather than a single vendor's internal practice — the corpus's clearest instance of consensus-derived (rather than unilaterally-asserted) agentic/AI cyber-risk governance guidance.
- (Batch 18 — threat-intelligence-side corroboration of agentic identity governance) [[04_Knowledge_Products/Wiki_Intake/F073_Google_Cloud_Mandiant_Cybersecurity_Forecast_2026]] — Google Cloud/Mandiant "Cybersecurity Forecast 2026": forecasts "agentic identity management" (AI agents as distinct digital actors with managed identities, just-in-time access, and a formal "chain of delegation") and "Shadow Agent risk" (Shadow AI's 2026 evolution — unauthorised employee-deployed autonomous agents). Explicitly argues banning agents is not viable (drives usage off-network, eliminating visibility) — a sharp capacity-over-prohibition argument. The most direct threat-intelligence-genre articulation yet of the identity/authority-binding problem AEGIS_OS and F036 (NIST NCCoE) address from governance and standards angles respectively.
- (Ad hoc addition, 2026-07-15 — foundational/business-case genre, pre-Batch 19) [[04_Knowledge_Products/Wiki_Intake/F074_McKinsey_What_Is_An_AI_Agent_2025]] — McKinsey "What is an AI agent?" (March 2025): coarser, executive-facing five-type agent taxonomy and a named enterprise case study (Lenovo — up to 15% software-engineering improvement, double-digit customer-service productivity gains) rather than a technical control or identity framework. Its "emergent AI" definition ("capabilities compound... unexpected behaviors and skills... greater than the sum of their parts") is a plain-language companion to F071/F073's more technical "excessive agency"/"Shadow Agent" vocabulary. Primary value is as citable, non-anonymised teaching/consulting material — most other nodes in this cluster are frameworks or threat intelligence, not named case studies.
- (Ad hoc addition, 2026-07-15 — multi-vendor cybersecurity-consortium genre, fifth AEGIS_OS corroboration) [[04_Knowledge_Products/Wiki_Intake/F078_SANS_Critical_AI_Security_Guidelines_v1_2]] — SANS Institute "Draft: Critical AI Security Guidelines v1.2" (24-author multi-vendor consortium): "organizations must enforce focused functionality and apply the principle of least privilege not only to users, but to the agents themselves," operationalised via defined function scope, execution isolation, API/functional-call controls, and feedback loops/escalation — plus an explicit recommendation to enforce access control at the RAG vector-retrieval layer rather than inside the LLM. This is the fifth independent-source-genre corroboration of the AEGIS_OS runtime pre-execution enforcement thesis (after F036 NIST, F038 ISACA, F071 AWS, F073 Google Cloud/Mandiant), now spanning standards bodies, professional associations, Big Tech vendors, threat intelligence, and multi-vendor cybersecurity-training consortia. Document is explicitly draft status (v1.2, ⚠#219) — treat findings as practitioner-consensus-in-progress, not a finalised standard.

See [[Corpus_Index_MOC]] for full node index.

- **(2026-08-02 — newest agentic instrument in the corpus)** [[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]] — IMDA's **Model AI Governance Framework for Agentic AI** (~Jan 2026; ⚠ date not pinned — law-firm summary says January 2026, hosted file carries a 19 May 2026 timestamp). Four pillars: assess and bound risks upfront; **make humans meaningfully accountable**; implement technical controls and processes; enable end-user responsibility. Voluntary and **additive** — layered on Singapore's traditional (2020) and generative (2024) frameworks without replacing either, giving four live voluntary frameworks a deployer must reconcile unaided. Pillar 2's "meaningfully" is a direct instrument-level statement of the nominal-vs-effective oversight distinction that [[Human_Oversight]] treats as its defining boundary condition — the corpus's clearest regulatory acknowledgement that nominal oversight of agentic systems is insufficient.

- **(2026-08-02 — a regulator declines to govern agentic AI as model risk)** [[Model_Risk]] — **SR 26-2** (Fed/OCC/FDIC, 17 Apr 2026), which supersedes SR 11-7, **explicitly carves generative AI and agentic AI out of model risk management scope** as "novel and rapidly evolving," directing institutions to govern them under "broader risk management and governance practices" pending a future Request for Information. Non-generative, non-agentic ML remains in scope. **The boundary is drawn at generative/agentic vs everything else, not at AI vs non-AI.** This is the corpus's strongest evidence that agentic systems are treated as categorically distinct from models by a mature supervisory regime — a considered judgment, not an oversight, and arguably better evidence for the structural-insufficiency thesis than any paper. Consequence: an agentic system outside model validation is also outside the independent-challenge structure validation provides (see [[Human_Oversight]]). Contrast RBI FREE-AI, whose governance scope covers "increasingly autonomous AI systems" — India includes where the US excludes, non-bindingly.


## Connections

**Related concepts:** [[Accountability]] | [[Transparency]] | [[Governance_Debt]] | [[Regulatory_Parallelism]] | [[Institutional_Coherence]] | [[Governance_Capacity]]  
**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_1]] | [[07_Institutions/Corpus/RBI/RBI_2]] | [[07_Institutions/Corpus/SEBI/SEBI_11]] | [[07_Institutions/Corpus/CERT_In/CERT_2]] | [[07_Institutions/Corpus/CERT_In/CERT_4]]  
**Related frameworks:** [[RBI_Free_AI]] | [[SEBI_AI_Circular]] | [[NIST_AI_RMF]] | [[EU_AI_Act]] | [[IndiaAI_Framework]]  
**Related domains:** [[AI_Governance]] | [[BFSI_Governance]] | [[Cybersecurity_Governance]] | [[Privacy_DataProtection]]  
**Related projects:** [[P3_BFSI_JEIM]] | [[P4_Doctrinal_IJLIT]]  
**Related knowledge products:** [[AI_Governance_Wiki]] | [[BFSI_AI_Governance_Handbook]] | [[DPDP_Playbook]] | [[Regulatory_Complexity_Handbook]]  
**Related consulting:** [[AEGIS_OS_Inbound]] | [[PrivacyWeave_Inbound]] | [[CyberMesh_PS69_Inbound]] | [[CyberMesh_PS74_Inbound]]  
**Related content:** [[ADP_Keynote_2026]]  
**Wiki source:** AI Governance Wiki v2.2 S4.1, S4.2, S7.1 (practitioner commentary)  
**Zotero sources:** CERAI AI Agents (C1) | WEF AI Agents in Action (C3) | AWS Agents Security (C4) | Microsoft Administering Agents (C10) | Enterprise-Wide Agentic AI Risk Controls (C8)

---

## Open Questions

- NIST agent identity framework — expected Q2 2026; incorporate when published
- WEF agent auditability standards — expected Q2 2026; incorporate when published  
- SEBI_11 formal notification — pending; watch for amendment to Intermediaries Regulations
- State-level AI governance (Tamil Nadu, Telangana) — Q3 2026; may add agent-specific requirements

---

## Log

- 2026-06-14: Concept note created. S6 session. Sourced from AI Governance Wiki v2.2 S4, consulting inbound analysis (AEGIS, PrivacyWeave, CyberMesh), and corpus nodes written in S5.
