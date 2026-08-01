---
node_id: F035
series: Format_B
title: "Administering and Governing Agents"
short_ref: "Microsoft Corporation, 2025"
wiki_section: S4
tier: Medium
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/agentic-ai-governance
  - topic/enterprise-governance
  - institution/microsoft
  - batch/13
date_ingested: 2026-06-19
---

# F035 — Microsoft Corporation. *Administering and Governing Agents.* Microsoft Whitepaper v1.0, ~2025.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Author / Issuer** | Microsoft Corporation |
| **Document Type** | Industry Whitepaper |
| **Version** | v1.0 |
| **Date** | ~2025 (undated; internal references suggest post-2024 Copilot Studio GA) |
| **Pages** | ~28 |
| **Source File** | `Microsoft_White_Paper_Administering_and_Governing_Agents_1764250855.pdf` |
| **Wiki Section** | S4 (Agentic AI) |
| **Tier** | Medium — industry vendor primary; governance-relevant despite commercial framing |
| **Confidence** | High (Microsoft primary source; product documentation) |

## Document Summary

A Microsoft-published whitepaper setting out the governance architecture for AI agents deployed in enterprise Microsoft 365 and Power Platform environments. The document operationalizes agentic AI governance through a three-tier spectrum (End Users / Makers / Developers), three control types (Identity, Interaction, Agent), and a suite of administrative and compliance tooling across Microsoft 365 Admin Center, Power Platform Admin Center, and Microsoft Purview.

## Core Content

### 1. Three-Tier Governance Spectrum

| Tier | Actor | Typical Role | Governance Focus |
|---|---|---|---|
| End Users | Employees / consumers | Interact with agents in daily work | Usage policies, acceptable use, interaction logging |
| Makers | Business power users / citizen developers | Build agents via Copilot Studio without code | Maker controls, environment management, data connections |
| Developers | Professional IT/dev teams | Build agents via Azure AI Foundry SDK | Code-level controls, API governance, custom connectors |

### 2. Three Control Types

- **Identity controls** — authentication, authorization, and permissioning for agent principals
- **Interaction controls** — governing how agents respond and what actions they can take
- **Agent controls** — lifecycle management, deployment scope, decommissioning

### 3. Administrative Platform Stack

| Platform | Governance Function |
|---|---|
| **Microsoft 365 Admin Center** | Agent deployment approval, tenant-wide agent inventory, user-level access controls |
| **Power Platform Admin Center** | Environment management for Maker-built agents; DLP policies for data connector scope |
| **Microsoft Purview** | Data Loss Prevention (DLP), sensitivity labelling, insider risk management, eDiscovery, audit log |

### 4. Microsoft Purview Governance Layer

The Purview integration represents the compliance backbone of the architecture:
- **DLP policies**: Prevent agents from accessing or transmitting sensitive labelled data
- **Sensitivity labels**: Extend Microsoft Information Protection schema into agent-accessible data
- **Insider risk management**: Detect anomalous agent-assisted data movement
- **eDiscovery**: Ensure agent-generated content is discoverable for legal/regulatory purposes
- **Audit logging**: Provide tamper-resistant audit trail of agent actions for compliance review

### 5. Deployment Governance

A 10-step deployment guide covers: scope definition → environment selection → identity provisioning → data connection review → DLP policy application → maker enablement controls → end-user rollout → monitoring setup → incident response readiness → decommissioning protocol.

### 6. Center of Excellence (CoE) Model

Advocates for a dedicated internal AI governance CoE function responsible for:
- Setting agent governance standards and policy
- Managing the maker/developer tier pipeline
- Overseeing audit and compliance reporting
- Coordinating with CISO/legal on risk thresholds

## Analytical Notes

**Enterprise operationalization of agentic governance.** This document provides the most detailed enterprise-level operationalization of [[Agentic_AI_Governance]] in the Batch 13 cluster. The three-tier spectrum (End User → Maker → Developer) maps directly onto the principal hierarchy framework in F037 (WEF) and the authorization chain in F036 (NIST NCCoE).

**Microsoft Purview as compliance backbone.** The DLP + sensitivity label + audit log stack mirrors what regulatory instruments (RBI_7, SEBI_14) require in terms of [[Transparency]] and [[Accountability]] — but operationalizes them through vendor tooling rather than regulatory mandate. This is a useful "implementation layer" reference when assessing the gap between governance aspiration (regulatory text) and governance capacity (available tooling).

**Tier bias caveat.** The document is a vendor whitepaper. The governance controls described are Microsoft ecosystem-specific and presuppose Microsoft 365/Azure/Power Platform adoption. Not generalizable to multi-vendor or open-source agentic deployments. Cite with this framing explicitly.

**CoE model alignment.** The CoE recommendation echoes the governance structure proposed in F037 (WEF, progressive governance levels) and pre-figures the organizational capacity requirements identified in F041 (AEF-1, Analytic Autonomy).

## Concept Links

- [[Agentic_AI_Governance]] — three-tier governance spectrum; Purview compliance backbone for agent oversight
- [[Accountability]] — audit log + eDiscovery stack provides accountability infrastructure
- [[Transparency]] — sensitivity labelling and DLP as transparency enforcement mechanisms

## Cross-References in Corpus

| Node | Relationship |
|---|---|
| F036 (NIST NCCoE Agent Identity) | F035's identity controls layer is the enterprise implementation of F036's authorization framework |
| F037 (WEF AI Agents in Action) | F035's three-tier spectrum parallels WEF's autonomy/authority-scaled governance |
| F038 (ISACA Agentic AI Security) | F035's DLP/Purview controls map to ISACA's Orchestration & Policy and Communication & Trust defense planes |

## Research Application

| Project | Relevance |
|---|---|
| P3 (BFSI JEIM) | Enterprise agentic governance architecture; illustrates vendor-side implementation of BFSI compliance controls |
| fsQCA | Governance Capacity (GC) condition: vendor tooling availability as a GC sub-indicator |
| P1 (SLR) | Industry evidence for enterprise agentic AI governance; cite as practitioner source with vendor caveat |

## Source Metadata

- **Access method:** Read tool at Mac filesystem path (bash mount not available for Policy Dump Future)
- **Text quality:** Good (searchable PDF; Microsoft standard document production)
- **VERIFY flags:** None
