---
type: Framework
tags:
  - type/framework
  - status/active
  - paper/p2-primary
  - paper/p4
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - engine/knowledge-product
  - content/wiki-entry
  - content/carousel-ready
---

# DEPA — Data Empowerment and Protection Architecture

**Type:** Framework **Status:** Active **Last Updated:** 2026-08-02 (created — closes the vault's largest missing-node gap, 72 referencing notes)

---

## Core Synthesis

DEPA is the consent-layer architecture of India Stack: a design in which an individual authorises data flow between a provider and a user of that data through a licensed, **data-blind** intermediary — the Consent Manager — which brokers permission without ever seeing the payload. Within PRIS its analytical significance is not the design but the **enactment pathway**. DEPA was published by NITI Aayog in August 2020 as a "Draft for Discussion," was never superseded by a final version, and was never enacted as an instrument of any kind. It nonetheless became operative across two sectors and was subsequently written into statutory law — the DPDP Rules 2025 Consent Manager provisions are DEPA's architecture in statutory form. This is the inverse of the pattern already documented for [[DPDP_Act_2023]] (enacted but not operative). DEPA is **operative but never enacted**, and the pairing of the two gives PRIS a two-sided account of the gap between formal instrument status and governance reality in India.

## Framework Identity

- **Issuing body:** NITI Aayog, jointly with RBI, SEBI, IRDAI, PFRDA and the Ministry of Finance
- **Instrument type:** Policy framework / architectural design document — **explicitly labelled "Draft for Discussion"**
- **Binding status:** **Non-binding, and never finalised.** No NITI Aayog final version or v2.0 exists
- **Jurisdiction:** India; sectoral operationalisation via financial-sector and health-sector regulators
- **Key dates:**
  - **August 2020** — DEPA published as Draft for Discussion. Public comment window closed either 1 October 2020 (per the Executive Summary) or 30 November 2020 (per a secondary source) — ⚠ the two primary/near-primary figures conflict; do not cite a closing date without resolving this
  - **2 September 2016** — RBI NBFC-AA Master Directions issued, *predating* DEPA by four years: the regulatory instrument came before the architecture document that describes it
  - **8 November 2019** — ReBIT AA API Specification v1.1; **9 August 2023** — v2.0.0
  - **5 June 2026** — RBI recognises Sahamati as Self-Regulatory Organisation for the AA ecosystem
  - **DPDP Rules 2025, Rule 4** — Consent Manager registration; commences one year after Gazette publication, **registration not yet open**

## Structural Overview

Four roles: the individual (data principal); the **Financial Information Provider (FIP)** holding the data; the **Financial Information User (FIU)** seeking it; and the **Account Aggregator (AA)** — an RBI-licensed NBFC that brokers consent and is contractually and technically barred from reading the data it moves. The ReBIT API specification defines six functional flows: account discovery/linking, consent flow, consent handle management, FI data flow, notification flow, and monitoring flow.

The architecture has been instantiated three times, under three different governance regimes:

| Sector | Consent Manager instance | Governing instrument | Status |
|---|---|---|---|
| **Finance** | Account Aggregator (NBFC-AA) | RBI Master Directions 2016, as amended through 6 Sep 2024 | **Statutory, operative** |
| **Health** | Health Information Exchange & Consent Manager (HIE-CM), linked to every ABHA Address | NHA Health Data Management Policy; HIP/HIU Guidelines under ABDM | Government policy, operative |
| **Cross-sector** | Consent Manager under DPDP | DPDP Rules 2025 Rule 4 + First Schedule | **Statutory, not yet operative** |
| **Telecom** | — | — | **Announced 2020, never built** ⚠ confirmed absence |

## Regulatory Position & Comparative Significance

**The central finding, and a new pattern for the vault: operationalisation without enactment.** DEPA's normative content reached binding force by three separate routes, none of which involved adopting DEPA itself — RBI licensing (2016, predating the document), NHA policy (2021), and MeitY statutory rules (2025). The architecture propagated; the instrument never did. This is not simply soft law hardening over time: the soft-law document was never even finalised, and the earliest binding instrument preceded it.

For [[Institutional_Coherence]] this is a strong positive case — five regulators co-authored a common architecture and three of them implemented it compatibly, which is the clearest instance of successful cross-regulator coordination anywhere in the PRIS corpus. It should be read against [[Regulatory_Parallelism]] as the counter-example: Indian regulators demonstrably *can* converge on shared architecture. They did it for consent and did not do it for AI. That contrast is a [[Governance_Capacity]] finding, not a capability gap, and it materially strengthens the parallelism argument by removing the "they lack the machinery" rebuttal.

**Chiasmus worth stating explicitly in P2 and P4.** The AA consent-manager regime is *operative but not statutorily enacted as such* (it runs on 2016 NBFC licensing plus a draft architecture). The DPDP consent-manager regime is *statutorily enacted but not operative* (Rule 4 registration has not opened). India therefore has two consent-manager regimes at once, each missing the half the other has.

## Contestability Architecture — the corpus's most developed redress chain

The AA ecosystem operates a **four-tier** grievance mechanism, per the Sahamati Participation Terms:

1. Automated grievance ascertainment against Participant records, with compensation determination (Cl. 14.1)
2. Participant's Grievance Redressal Officer / Internal Ombudsman (Cl. 14.2)
3. The applicable **statutory** regulator ombudsman — RBI Integrated Ombudsman Scheme 2021, SEBI SCORES, IRDAI Grievance Redressal Cell, or PFRDA Grievance Redressal Cell
4. Sahamati-empanelled **ODR** institution for mediation, failing which arbitration by an independent sole arbitrator

Tiers 1, 2 and 4 are self-regulatory; only tier 3 is statutory, and tier 4 activates only where the statutory route "is not available, accessible or resolution by which is unsatisfactory."

**This is the sharpest contrast available to [[Contestability_Redress]].** India has built a functioning four-tier redress architecture for *data-sharing* disputes while providing no contestability right whatever over *automated decisions* — DPDP 2023 contains no ADM provision and there is no Indian equivalent of GDPR Art. 22(3). The capacity to design layered redress plainly exists. It has not been extended to algorithmic decisions. That is [[Governance_Debt]] with the excuse removed.

## Key Tensions & Gaps

- **No final DEPA text.** Every downstream instrument cites a document its own authors labelled a draft. Any citation must say so.
- **NPCI: ~~confirmed gap~~ deontic placement.** 🔴 **CORRECTED 2026-08-15 — see [[07_Institutions/Corpus/NPCI/NPCI_1_AI_ML_Payments_Operations_2025_2026]] and ⚠#361.** "Federated AI fraud detection" is **not supported by any NPCI primary source**; no NPCI document describes federated learning, and the AI/ML passage in NPCI's fraud Best Practices addresses **member banks**, not EFRM. **Restated:** NPCI's EFRM issues ecosystem-level fraud alerts member banks are directed to prioritise. And it is **not** a governance absence — `RBI/DPSS/2024-25/123` binds NPCI as a Large Non-Bank PSO from 1 Apr 2025 and carries **no AI provision**: Deontic-Placement Debt, not gap.
- *(original, retained)* ~~**NPCI: confirmed gap.** UPI runs AI-based fraud detection — a federated AI fraud-detection pilot generating comparative risk scores across partner banks, plus NPCI's own claims of "proven AI models" and continuous monitoring — with **no published governance instrument of any kind**. Evidence is secondary reporting (Economic Times BFSI, 3 Apr 2025) and NPCI promotional material. India's highest-volume payment rail governs its AI by press release. Strong [[Governance_Debt]] instance at the infrastructure layer.
- **Telecom extension: confirmed absent.** The 2020 draft stated the framework would extend to health *and telecom* and claimed telecom piloting was already underway. No DoT, TRAI or NITI instrument operationalising a telecom consent manager was located. Corroborates [[Telecom_AI_Governance]]'s "institutional vision exceeding institutional reach" finding from an independent direction.
- **No cross-sectoral consent layer exists as an operative instrument.** The National Health Stack's "Consent layer" framing is architectural, not regulatory.
- **Sahamati's SRO status is new and under-analysed.** Recognition on 5 June 2026 converts a voluntary industry alliance into an RBI-recognised standard-setter with delegated authority over operational and technical standards, dispute resolution and interoperability. A novel institutional form in Indian data governance, and one with no AI-sector counterpart.

## fsQCA Calibration

DEPA is a candidate additional case, but enter it with care. On **Regulatory Logic (RL)** the framework document itself scores at or near full non-membership — non-binding, never finalised, no or-else. On **State Institutionalisation (SI)** the same architecture scores high, because it is instantiated in a licensed intermediary regime with statutory ombudsman integration. A case whose RL and SI diverge this sharply is analytically useful precisely because it breaks the assumption that the two travel together — but it will also sit awkwardly in a truth table built on that assumption. Flag for TAC discussion before including in the 10-case set. If the calibration unit is taken as *the AA regime* rather than *the DEPA document*, both scores rise and the divergence disappears — which is itself a case-definition decision that must be made explicitly and defended.

## Linked Projects

[[P2_DPI_JSIS]]

[[P4_Doctrinal_IJLIT]]

[[fsQCA_Thesis_Chapter]]

## Linked Domains

[[DPI_Governance]]

[[Privacy_DataProtection]]

[[BFSI_Governance]]

[[Healthcare_Governance]]

[[Telecom_AI_Governance]]

## Linked Concepts

[[Contestability_Redress]]

[[Governance_Capacity]]

[[Institutional_Coherence]]

[[Regulatory_Parallelism]]

[[Governance_Debt]]

[[Accountability]]

[[Transparency]]

## Linked Frameworks

[[DPDP_Act_2023]]

## Linked Institutions

[[RBI]]

[[MEITY]]

[[NITI_Aayog]]

[[SEBI]]

[[IRDAI]]

[[Sahamati]]

[[NPCI]]

## Linked Corpus Nodes

[[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]]

[[07_Institutions/Corpus/RBI/RBI_12_ReBIT_AA_API_Specifications_2023]]

[[07_Institutions/Corpus/Sahamati/Sahamati_1_SRO_Recognition_and_Grievance_Architecture_2026]]

[[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]]

[[07_Institutions/Corpus/RBI/RBI_10_Storage_Payment_System_Data_2018]]

## Future Research / Reuse Opportunities

- **"Operationalisation without enactment"** is a publishable pattern and, paired with DPDP's "enacted but not operative," gives P4 a two-sided typology of instrument-status/reality divergence. Strongest new theoretical material from this intake.
- The four-tier AA redress chain versus zero ADM contestability is the cleanest single slide in the whole corpus for practitioner audiences, and unblocks [[DPDP_Playbook]] Ch. 4 (Consent Architecture and DEPA Alignment) and Ch. 7 (Cross-Border).
- Sahamati's SRO recognition is a live consulting angle: an RBI-recognised SRO exists for data sharing and none exists for AI. Feeds [[VV_Advisory_BD_Authority_Index]].
- The five-regulator co-authorship of DEPA is the strongest available counter-evidence to a "regulators cannot coordinate" reading of [[Regulatory_Parallelism]] — it should be written into that note as a boundary condition, not left as an unexamined tension.

---

_Back to [[_Frameworks_MOC]]_
