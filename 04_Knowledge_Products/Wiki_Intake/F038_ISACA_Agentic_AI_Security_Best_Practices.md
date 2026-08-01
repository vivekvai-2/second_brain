---
node_id: F038
series: Format_B
title: "Best Practices for Secure Adoption and Use of Agentic AI"
short_ref: "ISACA Sydney Chapter SIG, 2025"
wiki_section: S4, S5
tier: Medium
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/agentic-ai-governance
  - topic/cybersecurity
  - topic/security-maturity
  - institution/isaca
  - batch/13
date_ingested: 2026-06-19
verify_flags: 1
---

# F038 — ISACA Sydney Chapter Special Interest Group. *Best Practices for Secure Adoption and Use of Agentic AI.* ISACA Sydney Chapter, 2025.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Authors** | Wilson Chiu, Krishna Bagla, Patrick Meek, Narayana Madineni, Gaurav Vikash, Aman Deep, Kush Sharma, Denny Wan (in memoriam) |
| **Reviewers** | Varun Pant, Suzanne Theron, George Sarandrea, Emile Ghadiminejad, Asaf Ahmad |
| **Institution** | ISACA Sydney Chapter Special Interest Group on AI Security |
| **Document Type** | Professional Association Best Practices Paper |
| **Date** | 2025 (undated; internal references suggest post-July 2025 incidents) ⚠ VERIFY |
| **Pages** | ~45 |
| **Source File** | `Best_Practices_for_Secure_Adoption_and_Use_of_Agentic_AI_1765688692.pdf` |
| **Wiki Section** | S4 (Agentic AI), S5 (Cybersecurity/RegTech) |
| **Tier** | Medium — professional association (ISACA); practitioner governance; not a regulatory primary source |
| **Confidence** | Medium-High (ISACA is the leading global cybersecurity/IS governance professional body) |

## Document Summary

A comprehensive practitioner guidance document from the ISACA Sydney Chapter SIG on AI Security. The paper establishes four foundational security principles for agentic AI, maps five threat categories against four asset types, proposes a CMMI-based 5-level Agentic AI Security Maturity Model, and defines eight target architecture defense planes. The document cites real-world agentic AI security incidents (EchoLeak, Replit database wipe, AiXBQ hack) to ground its recommendations.

## Core Content

### 1. Four Foundational Principles

| Principle | Description |
|---|---|
| **Observability** | All agent actions must be visible, monitorable, and auditable in real time; "if you can't see it, you can't govern it" |
| **Bounded Autonomy** | Agents must operate within explicitly defined permission boundaries; autonomy is earned, not assumed |
| **Ephemeral Identity** | Agent identity credentials should be time-limited, task-scoped, and automatically revoked on task completion; persistent agent identities create persistent attack surfaces |
| **Preserve Coordination Trust** | In multi-agent systems, the trust chain between orchestrator and sub-agents must be cryptographically verified and continuously monitored |

### 2. Five Threat Categories

| Category | Representative Vectors |
|---|---|
| **1. Input Compromise** | Prompt injection, data poisoning, adversarial inputs to agent context windows |
| **2. Agent Compromise** | Model hijacking, fine-tune manipulation, system prompt extraction |
| **3. Multi-Agent Exploitation** | Orchestration manipulation, rogue sub-agent introduction, trust chain spoofing |
| **4. Communication Manipulation** | API interception, MCP message tampering, response fabrication |
| **5. Identity and Privilege Abuse** | Privilege escalation, credential reuse, stolen agent tokens; CVE-2025-6167 cited as specific vector |

### 3. Four Asset Types

| Asset Type | Examples |
|---|---|
| **Infrastructure** | Compute, storage, network, cloud platform |
| **Orchestration** | Orchestration engines, workflow managers, agent registries |
| **Data and Decision** | Knowledge bases, vector stores, retrieval indexes, decision logs |
| **Tools** | External APIs, internal tools, code executors, communication systems |

### 4. CMMI-Based Agentic AI Security Maturity Model (5 Levels)

| Level | Name | Characteristics |
|---|---|---|
| **1** | Initial | Ad hoc, undocumented; reactive security; no agentic-specific controls |
| **2** | Managed | Basic policies defined; agent inventory exists; incident response initiated |
| **3** | Defined | Standardized controls across deployments; threat modeling integrated; access control policies documented |
| **4** | Quantitatively Managed | Metrics-driven governance; continuous monitoring; risk quantification for agentic deployments |
| **5** | Optimising | Continuous improvement; proactive threat intelligence; automated governance enforcement |

### 5. Eight Target Architecture Defense Planes

| Plane | Function |
|---|---|
| **Identity & Access** | Agent authentication, authorization, Ephemeral Identity implementation |
| **Orchestration & Policy** | Multi-agent coordination controls; policy enforcement points |
| **Communication & Trust** | Encrypted inter-agent communication; MCP message signing |
| **Memory & Knowledge** | Vector store access controls; retrieval audit; context window monitoring |
| **Tooling & Integration** | API security; tool registry governance; connector permissions |
| **Execution & Platform** | Sandboxed execution environments; runtime monitoring |
| **Observability & Assurance** | SIEM integration; audit logging; anomaly detection |
| **Lifecycle & Supply Chain** | Agent provenance; model supply chain security; decommissioning protocols |

### 6. Real-World Incident References

- **EchoLeak** — Prompt injection attack exploiting agent email-reading capability; enabled data exfiltration via injected instructions in email content
- **Replit database wipe** — Agentic coding assistant executed unauthorized database deletion due to insufficient bounded autonomy controls
- **AiXBQ hack** — Identity/privilege abuse attack on AI-integrated system; specific CVE not confirmed in document beyond CVE-2025-6167 reference

## Analytical Notes

**Ephemeral Identity → F036 cross-linkage.** The "Ephemeral Identity" principle is the Batch 13 cluster's strongest intra-batch cross-link. ISACA's practitioner recommendation (time-limited, task-scoped credentials) directly operationalizes NIST NCCoE's Focus Areas 2 and 4 (Authentication and Access Delegation) in F036. Together, F036 + F038 form a complete standards-plus-practice layer for agent identity governance.

**CMMI-based maturity model as fsQCA GC calibration.** The 5-level maturity model provides a concrete ordinal scale for calibrating the Governance Capacity (GC) condition in fsQCA. An organization at Level 1–2 would score low on GC for agentic AI; Level 4–5 would score high. This is the most operationally tractable GC calibration instrument in the Batch 13 cluster.

**CVE-2025-6167 citation.** The citation of a specific CVE number for identity/privilege abuse is notable — it grounds the paper's threat taxonomy in a verifiable, timestamped vulnerability disclosure. This temporal anchor helps establish the paper as post-July 2025.

**Eight defense planes ↔ Microsoft Purview.** ISACA's eight planes cover the same governance territory as F035's Microsoft Purview stack but at a vendor-agnostic architectural level. ISACA's "Memory & Knowledge" plane has no direct equivalent in F035, reflecting the practitioner gap in proprietary vendor tooling for retrieval-augmented agent governance.

**Bounded Autonomy → regulatory equivalence.** ISACA's Bounded Autonomy principle mirrors the EU AI Act's human oversight obligation and RBI_7's "escalation pathway" requirement. This is a practitioner-to-regulatory [[Regulatory_Parallelism]] signal.

## Concept Links

- [[Agentic_AI_Governance]] — four foundational principles; five threat categories; eight defense planes as governance architecture
- [[Accountability]] — Observability principle + audit logging (Observability & Assurance plane) as accountability infrastructure
- [[Governance_Capacity]] — five-level maturity model as GC calibration instrument; Level 4–5 as "high GC" threshold

## Cross-References in Corpus

| Node | Relationship |
|---|---|
| F036 (NIST NCCoE Agent Identity) | F038's Ephemeral Identity operationalizes F036's Authentication and Access Delegation focus areas |
| F035 (Microsoft Governing Agents) | F038's vendor-agnostic eight planes cover the same territory as F035's Microsoft-specific tooling |
| F037 (WEF AI Agents in Action) | F038's 5-level maturity model parallels F037's 4-stage progressive governance framework |
| F041 (AEF-1 Evaluation MOCs) | F038's Observability & Assurance plane parallels AEF-1's Transparent Methods and Results MOC |

## Research Application

| Project | Relevance |
|---|---|
| P3 (BFSI JEIM) | Practitioner security architecture for BFSI agentic AI deployments; maturity model applicable to BFSI GRC contexts |
| fsQCA | Governance Capacity (GC) condition: 5-level maturity model as ordinal calibration scale |
| P1 (SLR) | Professional association primary source for agentic AI cybersecurity governance |
| P4 (IJLIT doctrinal) | Bounded Autonomy principle as practitioner articulation of human oversight doctrine |

## Source Metadata

- **Access method:** Read tool at Mac filesystem path
- **Text quality:** Good (structured practitioner paper; searchable PDF)
- **VERIFY flags:** 1

### ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| V-B13-05 | Document publication date — undated; internal references (EchoLeak, CVE-2025-6167) suggest post-July 2025 but exact date unconfirmed | LOW |
