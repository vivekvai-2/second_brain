---
type: corpus-node
node-id: International_11
institution: International
date: 2023-12
wiki-section: S6
tier: A
ai-explicit: false
tags:
  - type/corpus-node
  - institution/International
  - wiki-section/S6
  - tier/A
  - batch/10
  - concept/Governance_Debt
  - concept/Institutional_Coherence
  - concept/Regulatory_Parallelism
  - concept/Governance_Capacity
  - project/P3
  - project/P4
---

# International_11 — FSB: Enhancing Third-Party Risk Management and Oversight: A Toolkit for Financial Institutions and Financial Authorities (December 2023)

**Node ID:** International_11  
**Institution:** Financial Stability Board (FSB)  
**Document type:** FSB Toolkit — cross-jurisdictional implementation guidance for financial authorities and financial institutions  
**Date:** 4 December 2023  
**Jurisdiction:** Global  
**Wiki Section:** S6 — Implementation & Operational Risk / Third-Party Governance  
**Tier:** A (FSB authorship; December 2023; foundational global standard directly adopted/referenced by RBI, SEBI CSCRF, and IRDAI; pre-dates AI-specific guidance but materially governs AI vendor relationships)  
**Source PDF:** FSB Enhancing Third-Party Risk Management and Oversight.pdf (Additional Policies/)

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | Enhancing Third-Party Risk Management and Oversight: A Toolkit for Financial Institutions and Financial Authorities |
| Publisher | Financial Stability Board (FSB) |
| Date | 4 December 2023 |
| Pages | 58 |
| Scope | Global financial authorities + financial institutions + service providers |
| Primary purpose | Harmonise TPRM regulatory approaches across jurisdictions; reduce compliance cost fragmentation |
| India adoption | Directly reflected in: RBI_2 (IT Outsourcing Directions 2023), RBI_6 (AIFI Outsourcing 2025), SEBI CSCRF (SEBI_15), IRDAI_1 |
| AI relevance | GenAI/LLM providers are "third-party service providers" under FSB TPRM — all AI vendor relationships in financial services fall within scope |

---

## S2. Governance Context

International_11 is the foundational global standard for third-party risk management (TPRM) in financial services. Although not AI-specific, it is the upstream document that governs how Indian and global financial regulators approach AI vendor relationships. The FSB TPRM Toolkit's direct descendants in the PRIS corpus include RBI_2 (IT Outsourcing Master Direction 2023), RBI_6 (AIFI Outsourcing 2025), and elements of SEBI CSCRF (SEBI_15). Understanding International_11's framework is prerequisite to understanding those Indian regulatory instruments.

The Toolkit's critical innovation is the shift from **outsourcing** (narrow, legacy concept) to **holistic third-party risk management** — a broader concept that captures cloud providers, data service providers, AI/ML model vendors, and sub-contractors within the same governance framework. This shift has direct implications for how Indian BFSI firms should classify GenAI providers (OpenAI, Google, Anthropic, domestic equivalents) — they are third-party service providers under FSB TPRM, not merely technology vendors with a lighter-touch governance regime.

---

## S3. Toolkit Architecture (Four Chapters)

| Chapter | Focus | Key Content |
|---|---|---|
| Chapter 1 | Common terms and definitions | Harmonised TPRM glossary — "critical services," "service provider," "sub-contractor," "concentration risk" |
| Chapter 2 | Scope and general approaches | Critical services focus; holistic TPRM vs. narrow outsourcing; regulatory interoperability; proportionality |
| Chapter 3 | Financial institutions' TPRM tools | Eight implementation tools (see below) |
| Chapter 4 | Financial authorities' oversight | Supervisory approach; authority-to-authority incident reporting; systemic dependency mapping |

### Chapter 3 — Eight TPRM Implementation Tools

| Tool | Description | AI Application |
|---|---|---|
| 3.1 | Identification and criticality assessment of services | Classify GenAI/LLM providers against critical-service threshold |
| 3.2 | Onboarding and ongoing monitoring | Due diligence framework for AI model vendors before and during engagement |
| 3.3 | Incident reporting (TPSP → FI) | AI vendor must notify FI of model failures, data breaches, service disruptions |
| 3.4 | Register of third-party service relationships | Live register including all AI vendor relationships, criticality, contractual terms |
| 3.5 | Sub-contractor supply chain risk | Foundation model supply chains (US model → EU cloud → India bank) |
| 3.6 | Business continuity | Tested continuity plan if AI provider fails or is unavailable |
| 3.7 | Exit strategies | Tested exit strategy before engaging critical AI vendors — common gap in 2023–25 AI contracts |
| 3.8 | Concentration risk | Single AI provider serving multiple FIs = systemic concentration; monitor at sector level |

---

## S4. Key Provisions

> "Financial institutions rely on third-party service providers for a range of services, some of which support their critical operations. These dependencies have grown in recent years as part of the digitalisation of the financial services sector and can bring multiple benefits to financial institutions including flexibility, innovation and improved operational resilience. However, if not properly managed, disruption to critical services or service providers could pose risks to financial institutions and, in some cases, financial stability." — FSB TPRM Toolkit, Executive Summary

> "The primary emphasis is on critical services given the potential impact of their disruption on financial institutions' critical operations and financial stability. It also looks holistically at third-party risk management, which is wider than the historical narrower focus on outsourcing, in light of changing industry practices and recent regulatory and supervisory approaches to operational resilience." — FSB TPRM Toolkit, Chapter 2

> "The FSB has developed a toolkit for financial authorities and financial institutions as well as service providers for their third-party risk management and oversight. The toolkit also aims to reduce fragmentation in regulatory and supervisory approaches across jurisdictions and different areas of the financial services sector, thereby helping mitigate compliance costs for both financial institutions and third-party service providers, and facilitate coordination among relevant stakeholders." — FSB TPRM Toolkit, Executive Summary

---

## S5. Concept Linkages

| Concept | Evidence from International_11 |
|---|---|
| [[Regulatory_Parallelism]] | FSB Toolkit provides the upstream template from which RBI_2, RBI_6, and SEBI CSCRF all derive — but India's three regulatory instruments implement it with different scope, thresholds, and coverage, creating intra-India TPRM fragmentation despite a common FSB parent |
| [[Governance_Debt]] | AI vendor exit-strategy requirement (Tool 3.7) is routinely absent from Indian BFSI AI contracts signed 2023–25 — a systemic governance gap relative to the international standard |
| [[Governance_Capacity]] | Tool 3.2 (ongoing monitoring of AI vendors) requires FIs to maintain technical capacity to assess AI model changes, version updates, and performance drift — a capability not yet systematically embedded in most Indian BFSI firms |
| [[Institutional_Coherence]] | FSB Toolkit is explicitly designed to reduce regulatory fragmentation across jurisdictions (Chapter 2) — the fact that RBI and SEBI have implemented it differently (different scope for "critical services," different reporting timelines) signals [[Regulatory_Parallelism]] within India despite the common global standard |

---

## S6. Project Relevance

| Project | Relevance |
|---|---|
| P3 (BFSI — JEIM) | International_11 is the foundational document for any P3 analysis of AI vendor governance; every Indian BFSI regulatory instrument on outsourcing derives from or must be benchmarked against this Toolkit |
| P4 (Doctrinal — IJLIT) | The shift from "outsourcing" to "holistic TPRM" is a doctrinal development with direct implications for Indian IT Act, Companies Act, and RBI/SEBI regulatory instrument classification — is a GenAI provider an "outsourced service provider" or a new category? |
| P1 (SLR — RG/GIQ) | TPRM frameworks as a governance instrument type — International_11 is the canonical international reference point for how regulators institutionalise third-party risk governance at system level |

---

## S7. ⚠ VERIFY Flags

| Flag | Claim | Action |
|---|---|---|
| ⚠V-FSB1 | Confirm RBI_2 (IT Outsourcing Master Direction 2023) explicitly cites or adopts FSB TPRM Toolkit — verify in RBI_2 node | Cross-check RBI_2.md text for FSB citation |
| ⚠V-FSB2 | Confirm whether FSB has updated TPRM Toolkit post-2023 to explicitly address AI/GenAI vendors | Web search: "FSB TPRM AI update 2024 2025" |
| ⚠V-FSB3 | "Exit strategies" (Tool 3.7) — verify whether any Indian BFSI regulator has issued explicit AI vendor exit-strategy guidance (RBI/SEBI/IRDAI) | Check corpus and web |

---

## Backlinks

← [[07_Institutions/Corpus/RBI/RBI_2]] (IT Outsourcing Master Direction — India implementation)  
← [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] (AIFI Outsourcing — India implementation)  
← [[99_Archive/SEBI_15_pre_population_2026_07_14/SEBI_15_TEMPLATE_original]] (SEBI CSCRF — India implementation)  
← [[07_Institutions/Corpus/International/International_9]] (BIS FSI No. 63 — cites TPRM concentration risk)  
← [[07_Institutions/Corpus/International/International_10]] (BoE FSiF — AI service provider concentration risk)  
← [[05_Concepts/05_Concepts_Signature/Governance_Debt]]  
← [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]
