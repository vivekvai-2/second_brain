---
type: Framework
status: active
source_type: industry/grey-literature
last_updated: 2026-08-04
tags:
  - type/framework
  - status/active
  - source/grey-literature
  - paper/p1
  - paper/p3
  - paper/p4
  - gate/open
  - engine/phd
  - engine/linkedin
  - content/wiki-entry
  - content/carousel-ready
---

# SAIL 2.0 — Secure AI Lifecycle Framework

**Type:** Framework (practitioner / secondary) **Status:** Active **Last Updated:** 2026-08-04

---

## Core Synthesis

SAIL 2.0 (Pillar Security, June 2026) governs the *agent lifecycle* rather than the software lifecycle it runs alongside. Its central move is definitional: it reframes the AI agent as a **non-human actor** rather than a software component, and argues that the inherited security stack — built on the premise that humans decide and software executes deterministically — fails against a non-deterministic actor that reasons, chains tool calls, and acts at machine speed. The organising thesis is a shift from **access control to action control**: authorising every action, not merely every session.

Within PRIS, SAIL enters as a **secondary/practitioner framework node**, not a regulatory instrument and not an fsQCA case. Its analytical value is that it operationalises — at a granularity the academic AI governance literature rarely reaches — constructs that literature names only abstractly: autonomy tiering, action authorisation, non-human identity, delegated authority failure modes. It is also strong evidence of *practitioner consensus* forming ahead of binding regulation (50,000+ downloads of v1; contributors include CISOs from JPMorgan, Salesforce, ServiceNow, Google Cloud, SAP, Corning), which makes it citable in P1 as an industry-standard artifact illustrating how the regulatory gap is being filled informally pending formal rulemaking.

## Framework Identity

- **Issuing body:** Pillar Security (commercial AI security vendor), with a multi-firm practitioner contributor panel
- **Instrument type:** Voluntary practitioner framework / grey literature
- **Jurisdiction:** None — enterprise-facing, jurisdiction-agnostic
- **Binding status:** Non-binding; no certification, no enforcement, no regulatory recognition
- **Key dates:** SAIL v1 (July 2025) → SAIL 2.0 (June 2026)
- **PRIS classification:** Secondary framework; not an fsQCA case; not IG 2.0 codeable as a primary text

## Structural Overview

SAIL 2.0 is a **7-phase lifecycle** (Plan → Discovery → Build → Test → Deploy → Operate → Govern) crossed against a **3-zone risk topology** (Code & Pipeline / Cloud Agents / Endpoint Agents), producing a **91-row risk catalog**. Each row is mapped to up to five external frameworks: [[ISO_IEC_42001]], [[NIST_AI_RMF]], OWASP Agentic Top 10 (2026), OWASP LLM Top 10 (2025), [[EU_AI_Act]], DASF v3.0 (Databricks), and AIUC-1.

The zone topology is defined by *where risk materialises*, not where the process executes — an analytical device meaningfully distinct from the infrastructure-centric models that dominate enterprise security architecture, and portable beyond SAIL itself.

The cross-mapping table is the framework's single most reusable asset for PRIS. It functions as a **Rosetta Stone** between framework families that do not otherwise cross-reference one another, which is directly useful for comparative regulatory analysis and for the AI Governance Wiki's framework-comparison schema.

## Core Constructs (candidate Concept Notes)

| Construct | Description | PRIS relevance |
|---|---|---|
| **Action control vs. access control** | Access control authorises sessions and identities; action control authorises each discrete action against policy in real time | Central distinction. Maps onto algorithmic accountability and real-time governance debates. Promote to a standalone Concept note if cited more than once |
| **Agentic workforce** | Agents framed as a labour category with access, not a tool category | Rhetorically significant for regulatory classification: is an agent a product, a service, or a worker? |
| **Autonomy tiers** | Supervised / semi-autonomous / fully autonomous; control intensity scales with tier (SAIL 1.11) | Structurally parallel to EU AI Act risk-tiering — useful comparative pairing for fsQCA calibration should agentic regulation enter the case set |
| **Zone-based risk topology** | Code & Pipeline / Cloud Agents / Endpoint Agents | Risk-materialisation logic rather than execution-location logic |
| **Maker-identity inheritance** | Low-code failure mode (SAIL 5.17): the consumer of an agent inherits the builder's access | Directly relevant to [[DPI_Governance]] work on delegated authority in welfare delivery |
| **Confused-deputy agent** | Broadly-scoped agent identity used by a lower-privileged caller to reach systems they are not authorised for (SAIL 5.20) | Portable to IG 2.0 coding of delegation clauses — who is the *Attribute* when a deputy agent acts on delegated authority? |
| **Shadow agents** | Agents provisioned outside security governance; the agentic-era analogue of shadow IT | Feeds [[Governance_Capacity]] and [[Governance_Debt]] |
| **Governance debt** *(implicit, not named in source)* | The gap between agent capability deployed and control/oversight in place — e.g. SAIL 3.18 "Posture Drift" | Strong illustrative evidence for [[Governance_Debt]] even though SAIL never uses the term. Note this as an independent-convergence data point, not a citation of the construct |

## Regulatory Position & Comparative Significance

SAIL occupies a position no PRIS framework currently holds: **operational granularity without any regulatory standing**. Where [[NIST_AI_RMF]] is voluntary-but-institutionally-backed and [[ISO_IEC_42001]] is voluntary-but-certifiable, SAIL is voluntary, vendor-authored, and uncertifiable — yet more prescriptive than either at the control level. That combination is analytically interesting in itself: it is a case of practitioner standard-setting outrunning both regulation and formal standardisation, which is the empirical shape of soft-law formation.

| Framework | Relationship to SAIL |
|---|---|
| [[NIST_AI_RMF]] | Cited as complementary — NIST supplies strategic risk management, SAIL operationalises at lifecycle-phase level |
| [[ISO_IEC_42001]] | Maps to ISO management-system clauses per risk row; positions itself as the operational layer beneath ISO's management system |
| [[EU_AI_Act]] | Article-level mappings (Art. 6, 9, 10, 14, 15, 17, 25, 50, 72, 73) — **all assume high-risk classification** |
| OWASP Agentic Top 10 (2026) / LLM Top 10 (2025) | Vulnerability-identification layer SAIL claims to complement |
| DASF v3.0 (Databricks) | Component-level risk analysis layer |
| AIUC-1 | Newer standard, lightly represented in SAIL. **Flag closed 2026-08-04** — see below |
| [[RBI_Free_AI]] | No mapping (SAIL is jurisdiction-agnostic). The absence is itself a finding for P3/P4 — no practitioner framework maps to Indian sectoral instruments |

## Independent Convergence — Chinese Regulators Reached the Same Pivot (2026-08-04)

SAIL's central move — access control → **action control** — was arrived at independently by Chinese regulators in the same quarter, from a different baseline. [[04_Knowledge_Products/Wiki_Intake/F139_ConcordiaAI_State_of_AI_Safety_China_2026]] documents China's governance framework shifting from **content control** (what models say) to action control, triggered by OpenClaw's proliferation in February 2026 and formalised in CAC agentic-AI guidance in May 2026. TC260's eleven-threat agent taxonomy maps substantially onto SAIL's risk catalogue; both propose agent IDs, least-privilege tool scoping, and human confirmation for high-risk operations. Neither cites the other.

A US commercial vendor and a Chinese state regulator converging on the same governance primitive, from opposite starting points, in the same quarter, is a stronger signal than either document alone. Full framing, caveats, and verification steps in [[Agentic_AI_Governance]]. **China is now the stronger of the two citations** — its instruments are state-issued and one is heading for mandatory status, whereas SAIL remains vendor-authored grey literature.

## AIUC-1 — Open Flag Closed (2026-08-04)

The intake above flagged AIUC-1 as unchecked. [[04_Knowledge_Products/Wiki_Intake/F133_Trout_et_al_AI_Insurance_Stack_2026]] Table 3 characterises it against the three other live AI standards:

| | ISO 42001 | NIST AI RMF | STAR for AI | AIUC-1 |
|---|---|---|---|---|
| **Issuer** | ISO (private) | NIST (public) | Cloud Security Alliance (private) | AIUC (private) |
| **Type** | Auditable + certifiable | Voluntary framework | Auditable + certifiable | Auditable + certifiable |
| **Revision cadence** | Multi-year (~5 yr) | Multi-year | Unknown | Quarterly |
| **Scope** | Broad — all ML, management-system focus | Broad — all ML | Medium — LLM systems, cyber/cloud focus | Narrow — LLM agents in enterprise deployment |
| **Performance-based** | No | No | No | **Yes** — certification requires meeting benchmark scores in quarterly standardised evaluations |
| **Technical depth** | Shallow | Moderate | Deep | Deep |

**Why this matters for SAIL.** SAIL and AIUC-1 occupy the same niche — deep technical prescriptiveness for agentic deployment, fast revision cadence, no regulatory standing — and both position themselves as the operational layer beneath ISO 42001 and NIST AI RMF. They are more usefully treated as **competing practitioner standards** than as complementary layers, which is not how SAIL's own cross-mapping table presents the relationship.

⚠ **Conflict of interest, disclosed.** The lead author of F133 and two co-authors are employed by AIUC, which develops and sells AIUC-1 and underwrites AI insurance. Table 3 rates AIUC-1 as the only performance-based standard of the four. The authors disclose this at fn 29 and state they applied common evaluation dimensions across all four and noted AIUC-1's disadvantages (rigidity, burden, moving-target revision). **Reuse the table with the disclosure attached; do not present it as a neutral comparison.** SAIL carries a structurally identical problem — Pillar Security is a commercial vendor whose framework maps favourably to its own positioning.

The broader point for PRIS: the practitioner-standards layer is now populated by vendor-authored artefacts competing for the same insurability signal, with no accreditation infrastructure adjudicating between them. See [[Assurance_Reuse_Gap]] and [[Regulation_by_Insurance]].

## IG 2.0 Coding Summary

**SAIL is not a regulatory text and should not be coded as one.** It contains no Attribute/Deontic/Aim/Condition/Or-else in the formal institutional-grammar sense.

Its coding value is as a **secondary coding aid**: the risk catalog's "Mitigation" and "Assets Affected" columns supply a controlled vocabulary of agentic AI risk objects and controls, usable when coding primary regulatory texts ([[EU_AI_Act]], [[RBI_Free_AI]], [[DPDP_Act_2023]] Rules) for agentic-specific provisions that binding regulation has not yet caught up to. Treat it as a codebook input, not a coded case.

## fsQCA Calibration

**Not a case.** SAIL is excluded from the fsQCA model — it is neither a jurisdictional instrument nor an institutionally-issued standard, and calibrating RL for a vendor document would be category error. It may enter the fsQCA chapter as *contextual evidence* for the regulatory-lag argument, not as a row in the truth table.

## Key Tensions & Gaps

- **Grey literature, vendor-produced.** Pillar Security is a commercial AI security vendor and the framework functions partly as thought-leadership/GTM content. The breadth of the contributor list reduces single-vendor bias but does not make it peer-reviewed. Triangulate; do not cite as authoritative in an ABDC-A submission.
- **No empirical validation methodology disclosed.** The 91-risk catalog appears to derive from expert elicitation and practitioner consensus, not from incident data or systematic threat-intelligence review. Do not use it as an evidence base for claims about risk *prevalence* — only about risk *articulation*.
- **EU AI Act mappings assume high-risk classification.** Not universally applicable; verify applicability before reusing any mapping.
- **Editorial artifacts.** Overlapping contributor listings between the "SAIL V1" and "SAIL" acknowledgement sections suggest OCR or editorial duplication in the source PDF. Do not over-read structure from the acknowledgements.

## Linked Projects

- [[P1_SLR_RG]] — citable as an industry-standard artifact evidencing informal gap-filling
- [[P3_BFSI_JEIM]] — direct citation candidate; contributor base is heavily BFSI/CISO
- [[P4_Doctrinal_IJLIT]] — regulatory-lag evidence

## Linked Domains

- [[AI_Governance]] (primary)
- [[Cybersecurity_Governance]]
- [[BFSI_Governance]]
- [[DPI_Governance]] — action-control and zone models are portable to agentic intermediaries in Account Aggregator flows

## Linked Concepts

- [[Agentic_AI_Governance]]
- [[Governance_Debt]]
- [[Governance_Capacity]]
- [[Accountability]]
- [[Human_Oversight]]

## Linked Frameworks

- [[NIST_AI_RMF]]
- [[ISO_IEC_42001]]
- [[EU_AI_Act]]
- [[RBI_Free_AI]]

## Linked Knowledge Products

- [[AI_Governance_Wiki]] — the 91-risk catalog and multi-framework mapping table are strong candidates for structured ingestion into the framework-comparison schema
- [[BFSI_AI_Governance_Handbook]] — practitioner-grounding source

## Future Research / Reuse Opportunities

- **Regulatory gap paper.** Map SAIL's zone/phase matrix against EU AI Act risk tiers and RBI FREE-AI provisions to surface agentic-specific provisions — action authorisation, non-human identity governance, maker-identity inheritance — that binding regulation does not address at all. A defensible "regulatory lag" contribution consistent with the [[Regulatory_Parallelism]] and Regulatory Complexity streams.
- **Theoretical angle.** The action-control/access-control distinction could anchor a contribution on real-time algorithmic accountability, positioned against the static ex-ante compliance models dominant in current AI governance literature.
- **Longitudinal case.** Track SAIL v3 and AIUC-1 maturation as an instance of practitioner-standard evolution preceding formal regulation — an institutional-theory angle on regulatory anticipation and soft-law hardening.

## Source

Pillar Security. (2026, June). *SAIL 2.0: Secure AI Lifecycle Framework — A practical guide for building and deploying secure AI applications and agents.* Prior version: SAIL v1 (July 2025).

---

## Log

- 2026-08-04: Intake complete. Classified as secondary/practitioner framework; excluded from fsQCA case set; flagged as IG 2.0 codebook input rather than coded case.
- 2026-08-04: AIUC-1 open flag closed from [[04_Knowledge_Products/Wiki_Intake/F133_Trout_et_al_AI_Insurance_Stack_2026]] Table 3. SAIL and AIUC-1 reclassified as competing rather than complementary practitioner standards. Vendor conflict-of-interest caveat added, applying to both.

---

_Back to [[_Frameworks_MOC]]_
