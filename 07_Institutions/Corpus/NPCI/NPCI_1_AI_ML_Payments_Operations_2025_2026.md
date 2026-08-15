---
type: Corpus Node
status: active
last_updated: 2026-08-15
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/npci
  - paper/p3
  - paper/p4
---

# NPCI_1 — AI/ML in Retail Payments Operations (2025–2026)

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/NPCI/NPCI_1_AI_ML_Payments_Operations_2025_2026.md`
**Institution:** [[07_Institutions/NPCI]]
**Issuing body:** National Payments Corporation of India
**Document date:** Composite — three primary NPCI documents, June 2025 to February 2026
**Domain:** [[03_Domains/BFSI_Governance]] | [[03_Domains/DPI_Governance]]

---

## Instrument Identity

**This is not a regulatory instrument.** It is an operator-conduct node built from NPCI's own primary documents, on the pattern of [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]] — created to close ⚠#322 on [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]], which required either a primary source for the NPCI instance or its removal.

| # | Document | Date | URL |
|---|---|---|---|
| **A** | *Effective Controls to Mitigate Frauds and Other Losses Due to Emerging Modus Operandi* (Best Practices & Operational Recommendations), NPCI Risk Management Division | undated | `npci.org.in/PDF/npci/risk-management/Best-Practices.pdf` |
| **B** | *NPCI Advances India's Sovereign AI Infrastructure for Digital Payments With NVIDIA* | 18 Feb 2026 | `npci.org.in/uploads/NPCI_Advances_India_s_Sovereign_AI_Infrastructure_for_Digital_Payments_With_NVIDIA_7305ed3754.pdf` |
| **C** | *Expression of Interest for Identifying Switching Infrastructure Solution for NVIDIA GPUs*, Ref. NPCI/EOI/2025-26/IT/02 | 25 Jun 2025 | `npci.org.in/PDF/npci/tenders-notices/2025/Expression-of-Interest-for-identifying-Switching-Infrastructure-Solution-for-NVIDIA-GPUs.pdf` |

---

## 🔴 The correction this node exists to make

[[05_Concepts/05_Concepts_Signature/Governance_Debt]] §Infrastructure-layer (2026-08-02) records that **"NPCI runs federated AI fraud scoring across UPI."** That claim propagated into Decision_Infrastructure's Three-Instance Gate as instance 2.

**Primary sourcing does not support it as stated.** What the primary documents support is narrower, and the narrower version is still sufficient for the construct:

| Claim as recorded | Primary-source position |
|---|---|
| NPCI runs **federated** AI fraud scoring | ❌ **Not evidenced.** No NPCI document uses "federated" or describes federated learning across member banks. |
| NPCI runs network-level fraud **scoring** | ⚠ **Partly.** Document A establishes NPCI's **Enterprise Fraud Risk Management (EFRM)** system produces **ecosystem-level alerts** which member banks are directed to act on — network-level fraud intelligence, functionally cross-institutional. Whether it emits a *score* is not stated. |
| That system is **AI/ML-based** | ❌ **Not evidenced — this is the load-bearing gap.** See ⚠#361. |
| NPCI operates production AI on UPI | ⚠ **One identified deployment, and it is not fraud.** Document B's only named live/pilot system is the **UPI Help Assistant**, a **grievance-resolution** assistant on the FiMI small language model. |

---

## What the primary documents actually establish

### A — EFRM and ecosystem-level alerting

Document A directs member banks:

> *"It is important to build Artificial Intelligence/Machine Learning (AI/ML) capabilities in fraud monitoring, identification of mule accounts etc when dealing with huge volumes of transaction where typical rule-based approach will be ineffective. Effectively use NPCI's EFRM system to complement any existing fraud monitoring system used by the bank... Alerts from NPCI to be acted on priority as these are sent basis specific intelligence built at an ecosystem level."*

**Read carefully, the AI/ML sentence is addressed to banks, not to EFRM.** The document tells banks to build AI/ML capability *and, separately,* to use NPCI's EFRM and prioritise NPCI's ecosystem-level alerts. It does not state that EFRM is itself AI/ML-driven. ⚠#361.

**What it does establish, and this is the part the construct needs:** a central operator generates cross-institutional fraud intelligence that member banks are instructed to act on with priority. **The decision input crosses the institutional boundary.** Whether it was produced by a model or a rule engine does not change the accountability structure — which is precisely the construct's point.

### B — Announced, largely prospective AI programme (18 Feb 2026)

> *"NPCI will use NVIDIA Nemotron ... in its model development journey to create a payments-native AI foundation model aligned with India's regulatory and data sovereignty requirements."*

Trajectory described as *"evolv[ing] from use-case–specific agents to a foundational, scalable AI layer for the payment ecosystem"*; Mixture-of-Experts architecture for *"high-volume, low-latency payment environments."* **The release does not claim the sovereign model currently performs fraud scoring, mule-account graph clustering, or transaction blocking** — those are framed as capabilities the programme is expected to support *"over time."*

The one system named as live or piloted:

> *"NPCI recently introduced the UPI Help Assistant as a pilot initiative, supported by FiMI (Financial Model for India) fine-tuned and pre-trained Small Language Model (SLM) developed specifically for the payment ecosystem... The assistant supports grievance resolution for UPI users by enabling more timely and consistent responses at scale."*

**Note where this lands:** an AI system operating on **grievance resolution** — i.e. on [[05_Concepts/05_Concepts_Standard/Contestability_Redress]], the very channel through which a person would contest an automated outcome. An AI mediating the redress path is a distinct governance question from AI producing the original decision, and no Indian instrument addresses it. ⚠#362.

### C — Procurement evidence (25 Jun 2025)

Switching infrastructure for **NVIDIA H200 HGX GPU servers**, leaf–spine fabric, 32 nodes per site, 400 Gbps NIC uplinks, 800G line-rate ports, RoCEv2, lossless transport. Rationale: *"High-performance switches are essential for GPU(Model H200) servers used in AI workloads."* Dated, concrete, and eight months ahead of Document B — capability build preceding announcement.

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S4 (DPI Governance)
**Jurisdiction:** India
**Confidence:** **High on the regulatory-perimeter finding; Medium on the AI-deployment finding** (announced programme, one named pilot)
**AI explicit:** Yes — NPCI's own documents
**Tier classification:** **Tier C** — operator conduct, not a regulatory instrument. Analytically load-bearing for the operator-layer argument.

---

## 🔷 The regulatory perimeter — the strongest finding in this node

| Question | Position | Basis |
|---|---|---|
| Is NPCI a "Regulated Entity" for RBI's AI-adjacent instruments? | **No.** RBI_14 (Model Risk), RBI_9 and RBI_FREE_AI address REs — banks, NBFCs, AIFIs, CICs — under the Banking Regulation Act 1949 / RBI Act 1934 | Instrument applicability clauses |
| What is NPCI? | **Section 8 company**; **authorised non-bank Payment System Operator** under ss. 4 and 7, Payment and Settlement Systems Act 2007 | PSS Act; NPCI financials |
| Do the RBI (Digital Payment Security Controls) Directions, 2021 apply? | **No.** Scope is Scheduled Commercial Banks, Small Finance Banks, Payments Banks and credit-card-issuing NBFCs — participant endpoints and customer channels, **not the central switch operator** | Directions, para 2 |
| Does any RBI instrument reach NPCI as operator? | **Yes — one, and it is not about AI.** *Master Directions on Cyber Resilience and Digital Payment Security Controls for non-bank PSOs* (`RBI/DPSS/2024-25/123`), under s.10(2) r/w s.18 PSS Act. NPCI falls in the **Large Non-Bank PSO** tier, compliance from **1 April 2025**: baseline cyber resilience, 24×7 SOC, network anomaly alerting, third-party vendor risk | The Master Directions |
| Any AI-specific obligation on NPCI? | **None.** No explainability, model validation, bias testing, model inventory, or AI audit obligation binds NPCI as operator | Sweep of RBI AI-adjacent instruments |
| Other designation | **Critical Information Infrastructure / Protected System**, s.70 IT Act 2000, via MeitY/NCIIPC | — |

**The finding.** India's retail-payments switch — an operator that generates cross-institutional fraud intelligence member banks are told to prioritise, and is building a payments-native AI foundation model — sits inside a **binding cyber-resilience perimeter** and **entirely outside every AI-governance perimeter**. This is not regulatory absence through oversight. RBI reached NPCI deliberately in 2024 for cyber resilience, and its 2026 AI instruments reach past it to the REs on either side.

**This is [[05_Concepts/05_Concepts_Signature/Governance_Debt]]'s Deontic-Placement Debt in its cleanest form:** the same regulator, the same statutory power, the same entity — obligations imposed for cyber, withheld for AI.

**Governance disclosure.** NPCI's CTO states the focus is *"enabling the broader ecosystem to innovate responsibly through robust governance frameworks and secure, future-ready infrastructure."* Document B **publishes no such framework** — no model-approval committee, no human-review gate, no validation threshold, no audit or logging procedure, no allocation of accountability for model outputs. A governance *commitment* is evidenced; a governance *instrument* is not. Structurally identical to the ISO 42001 finding recorded the same day at [[06_Frameworks/ISO_IEC_42001]] — capability without the binding layer.

---

## ⚠ VERIFY

| Flag | Sev | Issue |
|---|---|---|
| **⚠#361** | **MEDIUM** | **EFRM is not evidenced as AI/ML-based.** Document A's AI/ML sentence addresses banks; the EFRM sentence is separate. Do not describe EFRM as an AI system without a source that says so. Retrieve NPCI's EFRM product documentation or circulars directly. **The construct does not need this to be true** — see the correction table — but the vault stated it, and it must not be restated. |
| **⚠#362** | LOW-MED | The UPI Help Assistant / grievance-resolution finding is this session's reading of Document B, not NPCI's framing. The redress-channel-AI point is analytically new and unverified against any second source. |
| **⚠#363** | MEDIUM | Document A is **undated**. Its currency is unestablished. Date it before citing the EFRM passage in publication-track output. |
| **⚠#364** | LOW | `RBI/DPSS/2024-25/123` applicability to NPCI as a "Large Non-Bank PSO" is taken from secondary analyses of the Master Directions, not from a tiering list naming NPCI. Confirm against the Directions' own applicability schedule. |
| **⚠#365** | LOW | Document B is a press release. Announced programmes are not deployments. Nothing in it should be cited as evidence of production AI beyond the UPI Help Assistant pilot. |

---

## Instances / Feeds Into

- [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] — closes ⚠#322; Three-Instance Gate instance 2 now primary-sourced, **restated and narrowed**
- [[05_Concepts/05_Concepts_Signature/Governance_Debt]] — Deontic-Placement Debt; infrastructure-layer sub-pattern corrected
- [[05_Concepts/05_Concepts_Standard/Contestability_Redress]] — AI mediating the redress channel (⚠#362)
- [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — RBI reaches NPCI for cyber and not for AI; a within-regulator, within-entity variant
- [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]] — the power-sector analogue; same structure, different sector
- [[07_Institutions/Corpus/Sahamati/Sahamati_1_SRO_Recognition_and_Grievance_Architecture_2026]] — the third operator-layer node

## Log

- **2026-08-15:** Node created from Perplexity pass P-05 to close ⚠#322. **The pass ran in two rounds that contradicted each other** — round 1 asserted the NVIDIA release evidenced "real-time anomaly detection, graph-based mule account clustering across the UPI switch"; round 2 retracted this, finding the release prospective and the UPI Help Assistant the only named live/pilot system. **Round 2 is the reading adopted here**, being the one that quotes the release rather than characterising it. The divergence is itself instructive: the vault's pre-existing claim matched round 1, which is the round that did not hold up. **New corpus-node candidate identified:** `RBI/DPSS/2024-25/123` (Cyber Resilience and Digital Payment Security Controls for non-bank PSOs, 2024) is the only instrument reaching NPCI as operator and is **not in the vault**.
