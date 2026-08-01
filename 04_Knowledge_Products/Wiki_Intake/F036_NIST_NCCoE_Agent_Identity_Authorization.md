---
node_id: F036
series: Format_B
title: "Software and AI Agent Identity and Authorization"
short_ref: "Booth, Fisher, Galluzzo, Roberts (NIST NCCoE), 2026"
wiki_section: S4, S5
tier: High
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/agentic-ai-governance
  - topic/cybersecurity
  - topic/identity-authorization
  - institution/nist
  - batch/13
date_ingested: 2026-06-19
verify_flags: 1
---

# F036 — Booth, D., Fisher, M., Galluzzo, A., & Roberts, J. (NIST NCCoE). *Draft Concept Paper: Software and AI Agent Identity and Authorization.* National Cybersecurity Center of Excellence, February 2026.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Authors** | Donna Booth, Marc Fisher, Anthony Galluzzo, Jason Roberts |
| **Institution** | National Institute of Standards and Technology — National Cybersecurity Center of Excellence (NIST NCCoE) |
| **Document Type** | Draft Concept Paper (public comment period; not yet a NIST SP) |
| **Date** | February 2026 |
| **Pages** | ~32 |
| **Source File** | `Software_AI_Agent_Identity_and_Authorization_1772214243.pdf` |
| **Wiki Section** | S4 (Agentic AI), S5 (Cybersecurity/RegTech) |
| **Tier** | High — US federal primary source; NIST NCCoE is the applied implementation arm of NIST |
| **Confidence** | High (official NCCoE draft; February 2026) |

## Document Summary

An NCCoE draft concept paper proposing a comprehensive framework for software and AI agent identity and authorization governance. The paper identifies six focus areas (Identification, Authentication, Authorization, Access Delegation, Logging/Audit, Data Flow Tracking) and maps them against an existing standards stack (MCP, OAuth 2.0/2.1, OIDC, SPIFFE/SPIRE, SCIM, NGAC). Published for public comment in February 2026; the paper represents the first NIST-level attempt to frame agent identity governance as a distinct cybersecurity problem domain.

## Core Content

### 1. Six Focus Areas

| Focus Area | Core Governance Question |
|---|---|
| **1. Identification** | How is an agent uniquely identified across its lifecycle? |
| **2. Authentication** | How does a system verify that an agent is who/what it claims to be? |
| **3. Authorization** | What resources and actions is an authenticated agent permitted to access? |
| **4. Access Delegation** | How does an agent acquire and scope permissions delegated by a human principal? |
| **5. Logging and Audit** | How are agent actions recorded for accountability and forensic review? |
| **6. Data Flow Tracking** | How are data movements within and across agent systems traced and controlled? |

### 2. Standards Stack Referenced

| Standard | Role in Agent Identity Framework |
|---|---|
| **MCP (Model Context Protocol)** | Emerging protocol for agent-to-tool and agent-to-resource interaction; Anthropic-originated |
| **OAuth 2.0 / 2.1** | Delegated authorization for agent actions on behalf of human principals |
| **OIDC (OpenID Connect)** | Identity layer over OAuth for agent authentication |
| **SPIFFE / SPIRE** | Workload identity framework for software agents in cloud/microservices environments |
| **SCIM (System for Cross-domain Identity Management)** | Agent identity provisioning/deprovisioning at scale |
| **NGAC (Next Generation Access Control)** | Attribute-based and policy-based access control for fine-grained agent permissions |

### 3. Key NIST SP Anchors

- **SP 800-207 (Zero Trust Architecture)** — governing principle: agents should be treated as untrusted by default; least-privilege enforced per request
- **SP 800-63-4 (Digital Identity Guidelines)** — identity assurance levels applicable to agent principals

### 4. Key Threat: Prompt Injection

The paper specifically identifies **prompt injection** as the primary threat vector exploiting the gap between agent identity and authorization boundaries. An injected prompt can cause an agent to act outside its authorized scope, bypassing the authentication/authorization layer. This framing positions prompt injection as an identity governance failure, not merely a model robustness issue.

### 5. Core Governance Principle: Least Privilege

Consistent with SP 800-207 (Zero Trust), the paper adopts **least privilege** as the foundational authorization principle for agent systems: agents should receive the minimum permissions necessary to complete a defined task, and those permissions should be scoped temporally (time-bounded) and contextually (task-bounded).

### 6. Three Enterprise Use Cases

1. **Agentic coding assistant** — developer-facing agent with file system and repository access
2. **Customer service agent** — consumer-facing agent with CRM and knowledge base access
3. **Multi-agent pipeline** — orchestrator agent delegating tasks to sub-agents across enterprise systems

## Analytical Notes

**First NIST-level frame for agent identity as a distinct problem.** Prior NIST AI governance documents (AI RMF 1.0, AI 600-1) address AI systems generally; this paper is the first NCCoE-level articulation of *agent-specific* identity governance. This is analytically significant for the [[Governance_Capacity]] condition in fsQCA — it marks the emergence of technical standards capacity for agentic AI governance at the US federal level.

**Prompt injection as identity governance failure.** The paper's reframing of prompt injection (from a safety/alignment issue to an identity/authorization boundary failure) is the most novel analytical move. This has direct implications for [[Accountability]] — if an agent acts outside its authorization scope due to injection, who is the accountable principal?

**Cross-link to F038 (ISACA Ephemeral Identity).** F036's authorization and access delegation framework (Focus Areas 3–4) is the standards-level articulation of the "Ephemeral Identity" principle in F038. The two documents represent theory-standard and practice-checklist layers of the same governance requirement.

**Standards stack maturity gap.** Several standards cited (NGAC, SPIFFE/SPIRE for AI agents) remain in early adoption stages. The paper acknowledges this; the proposed NCCoE project would include reference implementations. This gap is itself evidence of [[Governance_Debt]].

## Concept Links

- [[Agentic_AI_Governance]] — six focus areas define the identity governance architecture for agentic systems
- [[Accountability]] — logging/audit (Focus Area 5) and data flow tracking (Focus Area 6) as accountability infrastructure
- [[Transparency]] — agent identification and data flow tracking as transparency mechanisms
- [[Governance_Capacity]] — NIST NCCoE operationalizing technical standards for agent identity; marks US federal capacity development

## Cross-References in Corpus

| Node | Relationship |
|---|---|
| F035 (Microsoft Governing Agents) | F035's identity controls are the enterprise product implementation of F036's standards framework |
| F037 (WEF AI Agents in Action) | F036's authorization framework parallels WEF's authority dimension in 7-dimension classification |
| F038 (ISACA Agentic AI Security) | F038's Ephemeral Identity principle operationalizes F036's Focus Areas 2–4 at practitioner level |
| F041 (AEF-1 Evaluation MOCs) | F036's logging/audit requirements (Focus Area 5) parallel AEF-1's transparency and record requirements |

## Research Application

| Project | Relevance |
|---|---|
| P3 (BFSI JEIM) | Agent authorization and audit trail requirements for regulated BFSI agentic deployments |
| fsQCA | Governance Capacity (GC): US federal standards development for agent identity as a GC indicator |
| P1 (SLR) | Primary source for agentic AI cybersecurity governance; US federal primary |
| P4 (IJLIT doctrinal) | Authorization delegation + prompt injection framing; accountability gap in multi-agent systems |

## Source Metadata

- **Access method:** Read tool at Mac filesystem path
- **Text quality:** Good (standard NCCoE draft PDF format)
- **VERIFY flags:** 1

### ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| V-B13-01 | Whether this concept paper progressed to a full NCCoE project and/or NIST SP after the February 2026 public comment period | MEDIUM |
