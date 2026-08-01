---
node_id: F129
series: Format_B
title: "From Shore to Core: Building Secure and Resilient Subsea Networks"
short_ref: "Pandey & Kumar (Koan Advisory / USI), 2025"
wiki_section: S5, S2
tier: Medium-High
status: active
tags:
  - type/wiki-intake
  - series/format-b
  - topic/critical-infrastructure
  - topic/cybersecurity
  - topic/data-sovereignty
  - topic/india-regulatory
  - institution/koan-advisory
  - institution/usi-india
  - batch/ad-hoc
date_ingested: 2026-07-20
verify_flags: 5
---

# F129 — Pandey, V., & Kumar, S. (Koan Advisory Group / USI). *From Shore to Core: Building Secure and Resilient Subsea Networks.* United Service Institution of India & Koan Advisory Group, October 2025.

## Bibliographic Record

| Field | Detail |
|---|---|
| **Authors** | Vedika Pandey, Samrridhi Kumar |
| **Institution** | Koan Advisory Group (lead author org); published jointly with United Service Institution of India (USI) |
| **Document Type** | Industry / Outcome Report (roundtable proceedings + policy analysis) |
| **Date** | October 2025 |
| **Pages** | 14 (printed pagination; endnotes terminate on p. 14; participant list on unnumbered final page) |
| **Source File** | `Subsea_Cable_Report_1764590527.pdf` |
| **Wiki Section** | S5 (Data, Privacy & Security); S2 (India Regulatory Framework) |
| **Tier** | Medium-High — USI is India's oldest strategic studies institution; Koan Advisory is credible policy-advisory firm; grey literature but domain-specific and roundtable-backed (25 named participants) |
| **Confidence** | Medium-High (primary-source roundtable outcome; figures require independent verification — see VERIFY flags) |

## Document Summary

A post-roundtable policy report examining India's subsea cable infrastructure vulnerabilities and governance gaps. Covers six thematic areas: redundancy/concentration risk, repair infrastructure, socio-political (fishing community) challenges, coordination/policy direction, cybersecurity/data exfiltration, and geopolitics. Proposes a National Subsea Cable Policy and sovereign repair capacity as the two headline recommendations. Jointly convened by USI and Koan Advisory; 25 named participants spanning government, military, telecom, and academia.

## Core Content

### 1. India's Subsea Infrastructure — Key Data Points

| Data Point | Detail |
|---|---|
| Global subsea traffic share | >95% of international data traffic carried by subsea cables ⚠VERIFY #294 |
| Global annual cable cuts | ~150–200 worldwide per year ⚠VERIFY #295 |
| Cause split | 70% accidental (fishing/anchoring); 30% deliberate or environmental |
| India cable landing stations | Only 5 geographic locations |
| Mumbai concentration | 15 of India's 17 cables land within a 6 km patch at Versova ⚠VERIFY #296 |
| Comparator (Australia) | 8+ landing locations despite avg. monthly consumption of only 40 GB |
| India internet traffic share | ~20% of global internet traffic ⚠VERIFY #297 |
| India tele-density | ~85% (vs. global average of ~111%) |
| Subsea transmission speed | Up to 320 terabits per second |
| Cable cut downtime cost | ~USD 5,600 per minute ⚠VERIFY #298 |
| Sovereign repair vessel cost | ~USD 100 million per vessel |

### 2. Six-Point Resilience Framework

| # | Measure | Core Policy Ask |
|---|---|---|
| 1 | National Subsea Cable Policy | Unified framework covering repair, security, and governance |
| 2 | Domestic Repair & Maintenance Capacity | Sovereign repair vessel; empanelled list of private vessels |
| 3 | Cable Landing Station Security | Classify as Critical Information Infrastructure under IT Act 2000 |
| 4 | Marine Spatial Planning & Resource Coordination | Interministerial coordination framework |
| 5 | Technological Resilience & Threat Detection | Local caching, in-country cloud storage, quantum-resistant encryption |
| 6 | Regional & International Collaboration | QUAD-led multilateral cooperation; "Trusted sources initiative" |

### 3. Regulatory/Legal Frameworks Cited

| Instrument | Relevance |
|---|---|
| **Information Technology Act, 2000** | Landing stations recommended for classification as "Protected Systems" / Critical Information Infrastructure (CII) |
| **Telecommunications (Critical Telecommunication Infrastructure) Rules, 2024** | Existing CII designation framework for telecom; subsea cable coverage is the gap |
| **Australian Telecommunications Act** | Comparator: criminal penalties for damaging activities in cable protection zones |
| **Australia's Critical Infrastructure Resilience Strategy** | Referenced as best-practice model for repair pre-approval mechanisms |
| **"Clean network initiatives"** (US and allies) | Supply-chain security framing for cable infrastructure |
| **"Trusted sources initiative"** (India) | India's domestic equivalent; relevance to subsea cable procurement |

### 4. Key Recommendations (Condensed)

**Governance / institutional:**
- Designate nodal government authority (likely under Ministry of Communications) for repair coordination
- Whole-of-government coordination model: MoD/MHA (security) + MoEFCC (coastal/environmental clearances) + State govts/MoPSW/DoF (fishing/maritime)
- Remove requirement for DoT official physical presence on repair vessels (or pre-designate officials available at short notice)

**Infrastructure / capacity:**
- Develop sovereign repair vessel (~USD 100M); alternatively, explore retrofitting Indian Navy deep-sea vessels launched 2022
- Create pre-approved empanelled list of repair vessels; Free Ports with bonded storage to waive customs duties on repair equipment

**Socio-political:**
- Establish Cable-Protection Zones (CPZs) through multi-stakeholder consultation (not mandatory in isolation)
- Establish formal industry-fishermen liaison (cf. Oregon Fishermen's Cable Committee, US)

**Technology:**
- Increase local caching and in-country cloud storage to reduce dependence on subsea links
- Quantum-resistant encryption for data-in-transit on subsea routes ("harvest now, decrypt later" threat)

### 5. Incidents and Worked Examples

| Incident / Example | Significance |
|---|---|
| Baltic Sea + Red Sea (recent, pre-Oct 2025) | Multiple cable faults → temporary EU–Asia–Middle East internet disruption |
| Taiwan Strait (Jan 2025) | Disruptions in one month exceeded prior two years combined |
| Cyclone Vardah 2016 (Bay of Bengal) | Eastern India connectivity loss; precedent for natural-disaster cable vulnerability |
| GIFT City, Gujarat | BFSI hub cited as at risk from Mumbai-concentration vulnerability |
| Kochi–Lakshadweep + Chennai–Andaman cables | Positive example of India extending connectivity to island territories |
| SE Asia + Indian Ocean Cable Maintenance Agreement | Regional private consortium model (vessel: Cable Retriever) — low-cost alternative to sovereign vessel |
| Indonesian Telekom Indonesia | Another low-cost consortium option cited |

## Analytical Notes

**Mumbai concentration as systemic governance debt.** The 15/17 cables in a 6 km Versova patch is a textbook [[Governance_Debt]] pattern: infrastructure concentration that has accumulated without regulatory intervention. The report's comparison to Australia (8+ landing locations, lower traffic) makes the gap precise and policy-actionable.

**CII classification gap is a Regulatory_Parallelism instance.** Submarine cable landing stations are neither unambiguously covered by the IT Act 2000's "Protected Systems" provisions nor explicitly within the Telecom CII Rules 2024's scope. The report's recommendation to close this gap maps onto [[Regulatory_Parallelism]] — the same physical asset sits in a jurisdictional seam between telecom regulation and cybersecurity law.

**Sovereign capacity as Governance_Capacity indicator.** The recommendation for a sovereign repair vessel and empanelled alternatives is a direct [[Governance_Capacity]] deficit signal — India currently depends on private consortia and foreign vessels for repair of nationally-critical infrastructure.

**QUAD geopolitics framing.** The Wavelength Forum (New Delhi, July 2025) and QUAD's multistakeholder subsea cable discussions position this as a live governance event, not purely historical. Directly reinforces the broader [[Governance_Capacity]] narrative about India's international positioning.

**P4 relevance — IT Act 2000 CII classification.** The specific recommendation to apply "Protected Systems" status to cable landing stations is doctrinal material for P4: it identifies a gap between the letter of existing cyber law and the operational reality of critical infrastructure. The 2024 Telecom CII Rules represent a partial legislative response; the report's critique establishes that the response is incomplete.

## Concept Links

- [[Governance_Debt]] — Mumbai concentration risk; absence of sovereign repair capacity; CPZ non-implementation
- [[Governance_Capacity]] — sovereign repair vessel proposal; nodal authority; QUAD engagement
- [[Regulatory_Parallelism]] — landing stations straddling IT Act / Telecom CII Rules jurisdictional boundary
- [[Accountability]] — nodal authority for repair coordination; DoT oversight mechanism
- [[Legitimacy]] — mandatory stakeholder consultation for CPZs; fishermen liaison model

## Cross-References in Corpus

| Node | Relationship |
|---|---|
| F036 (NIST NCCoE Agent Identity) | Data Flow Tracking (Focus Area 6) — subsea cables are the physical substrate for the data flows F036 proposes to trace and control |
| F073 (Google Cloud Mandiant Cybersecurity Forecast 2026) | Threat-landscape context for the "harvest now, decrypt later" attack type cited in this report |
| F044 (Microsoft AI Security Risk Assessment) | Broader cybersecurity risk-management framing within which cable infrastructure resilience sits |
| F042 (IBM Cost of a Data Breach 2025) | Cost-of-disruption framing — USD 5,600/minute cable-cut figure is analogous in genre to IBM's per-breach cost data |

## Research Application

| Project | Relevance |
|---|---|
| P3 (BFSI JEIM) | GIFT City vulnerability cited explicitly; data sovereignty implications for BFSI data pipelines dependent on subsea links |
| P4 (IJLIT doctrinal) | IT Act 2000 CII classification gap; Telecom CII Rules 2024 as partial legislative response; doctrinal material on critical infrastructure law |
| P1 (SLR) | Peripheral — AI content limited to data exfiltration / "harvest now, decrypt later" framing; not core AI governance literature |
| Consulting | Critical infrastructure resilience as a cyber risk practice area; GIFT City + BFSI sector data points directly applicable |

## Source Metadata

- **Access method:** NotebookLM extraction relay (document previously blocked as iCloud-dataless at `Subsea_Cable_Report_1764590527.pdf`; NotebookLM ingestion pipeline resolves the access barrier)
- **Text quality:** Machine-readable throughout (no OCR required per extraction note)
- **Participants:** 25 named roundtable participants (military, telecom, government, academia) — participant list on unnumbered final page

### ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| #294 | "95 percent of international data traffic" carried by subsea cables — widely repeated figure but source not cited in document; verify current estimate | MEDIUM |
| #295 | "150–200 cable cuts worldwide" per year — cited figure, no primary source given | LOW |
| #296 | "15 of India's 17 cables landing in a 6 km patch at Versova, Mumbai" — infrastructure figure likely to change; verify against latest DoT/industry data before citing | HIGH |
| #297 | India accounts for "nearly 20 per cent of global internet traffic" — this figure is unusually high; likely conflates user-base share with traffic share; verify against ITU/Ookla/Cloudflare data before citing | HIGH |
| #298 | "USD 5,600 per minute" unplanned downtime cost from cable cuts — specific cost figure; primary source not identified in document | MEDIUM |
