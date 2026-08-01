---
node_id: F073
series: Format_B
title: "Cybersecurity Forecast 2026"
short_ref: "Google Cloud / Mandiant, 2025"
wiki_section: S5, S4
tier: Medium
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/cybersecurity
  - topic/threat-landscape
  - topic/agentic-ai-governance
  - institution/google-cloud
  - institution/mandiant
  - batch/18
date_ingested: 2026-07-15
verify_flags: 3
---

# F073 — Google Cloud Threat Intelligence Group, Mandiant Consulting & Google Cloud Office of the CISO. *Cybersecurity Forecast 2026.* Google Cloud, 2025.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Contributors** | Sandra Joyce (VP, Google Threat Intelligence); Charles Carmakal (CTO, Mandiant Consulting); Jon Ramsey (VP & GM, Google Cloud Security); plus researchers/analysts/responders across Google Threat Intelligence Group, Mandiant Consulting, Google Security Operations, and Google Cloud's Office of the CISO |
| **Institution** | Google Cloud (Google Threat Intelligence Group, Mandiant Consulting, Google Security Operations, Office of the CISO) |
| **Document Type** | Vendor threat-intelligence forecast report (annual series) |
| **Date** | 2025 (forecasting calendar year 2026); exact release date not stated in extracted pages ⚠ VERIFY |
| **Pages** | 15 |
| **Source File** | `Google_Cloud_Security_Cybersecurity_Forecast_2026_1764121839.pdf` |
| **Wiki Section** | S5 (Data, Privacy & Security — primary; directly addresses the AI Governance Wiki's stated S5 gap "threat landscapes; adversarial AI"), S4 (Agentic AI Governance — agentic identity management, Shadow Agent risk) |
| **Tier** | Medium — vendor threat-intelligence forecast, not peer-reviewed or regulatory, but grounded in named frontline incident-response (Mandiant) and threat-intelligence leadership rather than marketing content |
| **Confidence** | Medium — forward-looking/predictive framing explicitly acknowledged by the authors themselves |

## Document Summary

Google Cloud's annual threat forecast for 2026, organised around three themes: adversary and defender use of artificial intelligence, cybercrime as the most disruptive global threat category, and continued nation-state operations (Russia, China, Iran, North Korea). The AI section is the most PRIS-relevant: it forecasts a shift of threat-actor AI use from exception to norm, articulates "Shadow Agent" risk as the 2026 evolution of "Shadow AI," and frames "agentic identity management" as a coming security paradigm shift. The report explicitly disclaims "crystal ball" predictions in favour of extrapolation from observed 2025 evidence and frontline (Mandiant incident-response) data.

## Core Content

### 1. AI Threat-Landscape Forecast (2026)

| Forecast | Substance |
|---|---|
| **Adversaries fully embrace AI** | Threat-actor AI use transitions from exception to norm; extends to social engineering, information operations, malware development, and increasingly to agentic-system-automated attack chains |
| **Prompt injection manipulates AI** | Anticipated significant rise in prompt-injection attacks through 2026, driven by growing enterprise AI integration and low-cost/high-reward attack economics; shift from proof-of-concept to large-scale data exfiltration/sabotage |
| **AI-enabled social engineering** | Named threat actor (ShinyHunters/UNC6240) forecast to escalate AI-driven voice cloning ("vishing") for executive/IT-staff impersonation; AI-scaled reconnaissance and phishing-message crafting |

### 2. Defender-Side AI Forecast

| Forecast | Substance |
|---|---|
| **AI Agent Paradigm Shift** | Traditional security deployments not designed for AI-agent operation; requires new frameworks to map AI ecosystems and assess introduced vulnerabilities |
| **Agentic identity management** | Identity concept expands to treat AI agents as distinct digital actors with managed identities; adaptive, AI-driven continuous risk evaluation; just-in-time access; robust "chain of delegation" — explicit move beyond conventional human-authentication/service-account models |
| **Supercharged security analysts / "Agentic SOC"** | Analysts shift from manual alert correlation to directing AI agents; AI-generated case summaries, decoded obfuscated commands, MITRE ATT&CK mapping; analyst role shifts to strategic validation of AI-recommended SOAR containment actions |

### 3. Shadow Agent Risk

Forecasts escalation of "Shadow AI" into a "Shadow Agent" problem as employees independently deploy autonomous agents for work tasks regardless of corporate approval, creating invisible/uncontrolled data pipelines and compliance-violation risk. Explicitly rejects banning agents as a viable strategy (drives usage off-network, eliminating visibility) in favour of secure-by-design AI governance that safely routes and monitors agent traffic while preserving auditability.

## Analytical Notes

**"Agentic identity management" and "chain of delegation" as direct AEGIS_OS runtime-enforcement corroboration.** This is the most explicit corpus articulation to date of AI agents as distinct identity-bearing actors requiring dynamic, context-aware, just-in-time access control with a formal delegation chain — precisely the runtime authority-binding and pre-execution enforcement thesis underlying AEGIS_OS. This is threat-intelligence-side (rather than governance-framework-side) corroboration, adding a third genre of evidence (alongside regulatory and vendor-governance-framework sources) for the same architectural conclusion.

**Shadow Agent risk as Governance_Capacity gap evidence.** The explicit statement that "banning agents is not a viable option" because it "drives usage off the corporate network, eliminating visibility" is a sharp articulation of the governance-capacity problem: prohibition without capacity-building is self-defeating. This corroborates from a threat-intelligence angle what governance-framework sources (e.g., F072 WEF/Oxford's "shadow AI" inventory point) argue from a risk-management angle.

**Forecast/predictive framing requires explicit citation caveat.** Unlike regulatory instruments or empirical academic papers elsewhere in the corpus, this document's claims are explicitly forward-looking assessments ("we anticipate," "we expect") rather than observed fact, even though grounded in 2025 frontline data. Any citation should preserve this predictive framing rather than presenting 2026 forecasts as established fact.

## Concept Links

- [[Agentic_AI_Governance]] — agentic identity management, chain of delegation, Shadow Agent risk, Agentic SOC
- [[Governance_Capacity]] — "banning agents is not viable" as an explicit capacity-over-prohibition argument
- [[Accountability]] — agentic identity as a distinct, individually accountable digital actor requiring its own access-control lifecycle

## Cross-References in Corpus

| Node | Relationship |
|---|---|
| F072 (WEF/Oxford AI Cybersecurity) | F072's "shadow AI" inventory best-practice is corroborated and extended by F073's "Shadow Agent" forecast — governance-framework and threat-intelligence sources converging on the same risk category |
| F071 (AWS AI for Security and Security for AI) | F071's "excessive agency" prevention (permission boundaries, throttles) is the AWS-side technical-control counterpart to F073's "agentic identity management" — same problem (agent authorization), governance-whitepaper vs. threat-forecast genres |
| F036 (NIST NCCoE Agent Identity Authorization) | F073's "agentic identity management" forecast is a threat-intelligence-side corroboration of the identity/authorization problem NIST NCCoE addresses as a standards-development exercise |
| F038 (ISACA Agentic AI Security Best Practices) | Complementary agentic-risk genre; F073 adds frontline threat-actor-behaviour evidence that F038's architectural framework does not carry |

## Research Application

| Project | Relevance |
|---|---|
| P3 (BFSI JEIM) | Threat-intelligence-side evidence for the agentic-identity/authority-binding governance gap, complementing regulatory and vendor-framework sources already in the corpus |
| Consulting (AEGIS_OS) | Directly reusable: "agentic identity management," "chain of delegation," and "Shadow Agent risk" are close-to-verbatim framing for AEGIS_OS's runtime pre-execution enforcement pitch to prospective clients |
| P1 (SLR) | Fills the explicitly identified AI Governance Wiki S5 gap ("threat landscapes; adversarial AI") with a named, current (2025/2026-cycle) Big Tech threat-intelligence source |
| Teaching | "Shadow AI → Shadow Agent" progression is a compact, dated (2025→2026) illustration of how agentic AI changes an existing governance risk category rather than creating an entirely new one |

## Source Metadata

- **Access method:** `pdftotext` (searchable PDF; clean extraction)
- **Text quality:** High for the AI section (pages 3–6, fully read); Cybercrime and Nation States sections (pages 7–13) read via table of contents only, not full text
- **VERIFY flags:** 3

### ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| 207 | Exact publication/release date not stated in the extracted pages (title page carries a stylised "GO EMBAR[GO]" watermark suggesting an embargo date exists) — confirm official release date via Google Cloud/Mandiant blog before citing as a dated 2025 publication | MEDIUM |
| 208 | Named threat actor attributions (ShinyHunters/UNC6240, UNC5221) are current as of the document's writing — threat-intelligence attributions are frequently revised/merged; verify current attribution status before citing in any external-facing work | MEDIUM |
| 209 | All AI-threat claims in this document are explicitly forecasts/anticipations ("we anticipate," "we expect"), not confirmed incidents — any downstream citation must preserve this predictive framing and not present 2026 forecasts as observed fact | LOW |
