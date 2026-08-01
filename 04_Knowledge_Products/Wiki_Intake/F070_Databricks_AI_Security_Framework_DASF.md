---
node_id: F070
series: Format_B
title: "Databricks AI Security Framework (DASF) v1.0"
short_ref: "Databricks, 2024"
wiki_section: S5, S4
tier: Medium
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/ai-security
  - topic/agentic-ai-governance
  - topic/cybersecurity
  - institution/databricks
  - batch/18
date_ingested: 2026-07-15
verify_flags: 2
---

# F070 — Khawaja, O., Pamulapati, A. & Albano, K. *Databricks AI Security Framework (DASF) 1.0.* Databricks, 2024.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Authors** | Omar Khawaja (VP & Field CISO), Arun Pamulapati (Senior Staff Security Field Engineer), Kelly Albano (Product Marketing Manager) — all Databricks |
| **Institution** | Databricks, Inc. |
| **Document Type** | Vendor security framework whitepaper, with named external contributor validation |
| **Date** | 2024 (v1.0; source filename carries a "v4_final" internal revision marker) ⚠ VERIFY |
| **Pages** | Whitepaper, ~50+ (partial read, first 15 pages) |
| **Source File** | `databricks_ai_security_framework_dasf_whitepaper_v4_final_1764622059.pdf` |
| **Wiki Section** | S5 (Cybersecurity/RegTech — primary), S4 (Agentic AI — secondary, via RAG-LLM/multi-component risk coverage) |
| **Tier** | Medium — vendor-authored framework, not independently peer-reviewed or regulatory, but cross-validated by named external practitioners and mapped to recognised standards (NIST AI RMF, MITRE ATLAS) |
| **Confidence** | Medium — vendor self-interest in framing Databricks' own platform as the control point must be discounted; external contributor list (below) adds some independent credibility |

## Document Summary

DASF is a component-and-risk-based AI security framework structured around 12 foundational AI system components (data sources, ingestion, serving/inference, model registry, feature store, orchestration, agent/tool layer, monitoring, etc.), against which it catalogues 55 discrete technical security risks and 51 corresponding mitigation controls (numbered DASF 1–51). Each risk/control pair is tagged for applicability across six AI deployment models: predictive ML, RAG-LLM, fine-tuned LLM, pre-trained/open-weight LLM, foundational model, and externally-hosted/third-party model. The framework explicitly cross-maps to NIST AI RMF, the Biden Administration's EO 14110 (Safe, Secure, and Trustworthy AI), MITRE ATLAS, the OWASP Top 10 for LLM Applications, and Gartner's 2023 Security Leader's Guide to AI.

## Core Content

### 1. Structural Logic

| Layer | Function |
|---|---|
| **12 AI system components** | Decomposes the AI pipeline into discrete security-relevant zones (data, model, serving/inference, orchestration/agent-tooling, monitoring) rather than treating "the model" as a single unit of analysis |
| **55 technical security risks** | Catalogued against components, spanning data poisoning, model theft/extraction, supply-chain (model provenance), prompt injection, insecure tool/agent invocation, inference-endpoint abuse |
| **51 mitigation controls (DASF 1–51)** | Numbered, cross-referenced controls; each tagged for which of the 6 deployment models it applies to |
| **6 deployment-model applicability matrix** | Predictive ML / RAG-LLM / fine-tuned LLM / pre-trained (open-weight) LLM / foundational model / external (third-party API) model — recognises that risk surface differs materially by deployment pattern, a more granular differentiation than most vendor frameworks attempt |

### 2. External Contributor Validation

The whitepaper carries attributed commentary from named security leaders outside Databricks: Hyrum Anderson (CTO, Robust Intelligence), Christopher Sestito and Abigail Maines (CEO/CRO, HiddenLayer), Hasan Yasar (Carnegie Mellon SEI), Ebrima Ceesay (Capital One), Riyaz Poonawala (VP InfoSec, Navy Federal Credit Union), Robert Booker (HITRUST), Grizel Lopez (Barracuda), Diana Kelley (CISO, Protect AI), Brandon Sloane (Meta). This is a materially wider and more BFSI-relevant external validation set (Capital One, Navy Federal Credit Union — both regulated US financial institutions) than typical single-vendor security whitepapers carry, partially offsetting the vendor-interest tier caveat.

### 3. Standards Cross-Mapping

| External Standard | DASF Treatment |
|---|---|
| **NIST AI RMF** | Controls mapped to Govern/Map/Measure/Manage functions |
| **EO 14110** (Biden, Safe/Secure/Trustworthy AI) | Cited as the US federal policy anchor for the framework's risk taxonomy |
| **MITRE ATLAS** | Adversarial-technique mapping for model-level attacks |
| **OWASP Top 10 for LLM Applications** | Direct crosswalk for LLM-specific risk categories (prompt injection, insecure output handling, training data poisoning) |
| **Gartner 2023 Security Leader's Guide to AI** | Cited as market-context validation for the framework's structural approach |

## Analytical Notes

**Component-based decomposition as a Governance_Capacity instrument.** DASF's 12-component/55-risk/51-control structure is a more granular technical-control inventory than most of the corpus's governance-level frameworks (e.g., F038 ISACA's 4-principle/5-threat/8-plane architecture, which operates at the architectural rather than control-catalogue level). DASF is usefully read as the *control-implementation layer* beneath ISACA's *architectural-governance layer* — the two are complementary rather than competing, and a BFSI consulting engagement would plausibly use ISACA's planes to structure the governance narrative and DASF's numbered controls (DASF 1–51) as the underlying control checklist.

**Deployment-model applicability matrix as a Regulatory_Parallelism instrument.** The six-way deployment-model differentiation (predictive ML through externally-hosted models) is analytically useful because it mirrors — independently, from a vendor-security rather than regulatory-doctrine starting point — the same "not all AI is the same risk class" logic that RBI_FREE_AI_2025 and the EU AI Act's risk-tiering apply from a regulatory angle. This is a practitioner-to-regulatory parallel worth noting for the fsQCA calibration work, though it should not be overstated: DASF's tiering is deployment-architecture-driven, not harm/rights-driven, and the two taxonomies are not directly interoperable.

**Vendor self-interest caveat.** As with F035 (Microsoft) and F044 (Microsoft Security Risk Assessment), DASF's framing implicitly favours Databricks-native tooling (Unity Catalog, MLflow, Databricks Model Serving) as the natural home for several of the 51 controls. This should be flagged explicitly in any consulting or teaching reuse — the control *logic* is portable; the specific tooling recommendations are not vendor-neutral.

**Agentic/tool-layer coverage is present but secondary.** DASF's "agent/tool layer" component and associated risks (insecure tool invocation, orchestration-layer compromise) give it a legitimate S4 secondary tag, but the framework predates the more agent-centric treatments in F036 (NIST NCCoE Agent Identity) and F038 (ISACA Agentic AI). DASF's agentic coverage is one component among twelve, not the organising principle — this is a materially different scope than F038, and the two should not be treated as substitutes.

## Concept Links

- [[Agentic_AI_Governance]] — agent/tool-layer component and associated risk/control pairs (secondary emphasis relative to F038/F036)
- [[Governance_Capacity]] — 51-control catalogue as a concrete control-maturity checklist; complements ISACA's (F038) ordinal maturity model with a control-inventory instrument
- [[Regulatory_Parallelism]] — six-way deployment-model risk tiering as an independent (vendor-security-originated) parallel to regulatory risk-tiering logic (RBI FREE-AI, EU AI Act)

## Cross-References in Corpus

| Node | Relationship |
|---|---|
| F038 (ISACA Agentic AI Security Best Practices) | DASF's control-catalogue layer sits beneath ISACA's architectural-governance layer; complementary, not overlapping in altitude |
| F035 (Microsoft Administering/Governing Agents) | Both are Big Tech vendor security frameworks carrying an implicit own-tooling bias; DASF is more granular (component/risk/control triad) than F035's governance-narrative approach |
| F044 (Microsoft AI Security Risk Assessment) | Parallel vendor-security-framework genre; both should carry the same vendor-interest caveat in consulting reuse |
| F036 (NIST NCCoE Agent Identity & Authorization) | DASF's agent/tool-layer risks are a lighter-touch treatment of the same identity/authorization territory NIST NCCoE addresses in depth |

## Research Application

| Project | Relevance |
|---|---|
| P3 (BFSI JEIM) | Control-catalogue instrument for BFSI AI-security advisory; external validation from Capital One and Navy Federal Credit Union gives BFSI-specific credibility |
| fsQCA | Governance Capacity (GC) condition — 51-control inventory as a checklist-style calibration complement to ISACA's (F038) ordinal maturity scale |
| P1 (SLR) | Vendor primary source for the AI-security-framework literature stream, illustrating the control-catalogue genre distinct from academic/regulatory sources |
| Consulting (AEGIS_OS, PrivacyWeave) | Directly reusable as a control-catalogue reference for non-defence AI-security advisory engagements, subject to the vendor-tooling-bias caveat above |

## Source Metadata

- **Access method:** Read tool at Mac filesystem path (bash `pdftotext` fails on this file with a trailer/xref error — consistent with other Policy Dump Future PDFs this session)
- **Text quality:** Good (first 15 pages read; structured vendor whitepaper, searchable PDF)
- **VERIFY flags:** 2

### ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| V-B18-01 | Document is labelled "DASF 1.0" but the source filename carries an internal "v4_final" revision marker — confirm whether a later public DASF version (2.0+) has since superseded this one before citing version-specific control numbers | MEDIUM |
| V-B18-02 | The 55-risk/51-control counts are Databricks' own self-reported framework scope (not independently audited); treat as vendor-asserted figures, not externally validated totals, in any citation | LOW |
