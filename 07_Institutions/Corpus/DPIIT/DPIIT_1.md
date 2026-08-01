---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/dpiit
---

# DPIIT_1 — Working Paper on Generative AI and Copyright (Part 1): One Nation One License One Payment

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/DPIIT/DPIIT_1.md`
**Institution:** [[07_Institutions/DPIIT]]
**Issuing body:** Department for Promotion of Industry and Internal Trade (DPIIT), Ministry of Commerce and Industry, Government of India
**Document date:** December 8, 2025 (notification date); Working Paper December 2025
**Notification reference:** P-24029/34/2025-IPR-VII
**Pages:** ~115 pages (including 5 annexures; Annexure I = Nasscom Dissent Note)
**Domain:** [[03_Domains/AI_Governance]]

---

## Instrument Identity

**Full title:** Working Paper on Generative AI and Copyright — Part 1: ONE NATION ONE LICENSE ONE PAYMENT — Balancing AI Innovation and Copyright
**Type:** Government Consultation Paper / White Paper (Working Paper — not yet binding; soliciting stakeholder feedback)
**Target entities:** AI developers, AI deployers, copyright holders, collecting societies, technology companies, creative industries, and Government bodies (incl. MEITY, MIB, NASSCOM, creative sector bodies)
**Legal basis:** Copyright Act, 1957 (as amended); DPIIT mandate under Ministry of Commerce & Industry for IPR policy; Committee formed April 28, 2025 under Chairmanship of [⚠ VERIFY: committee chair name not captured in extraction]
**Companion documents:** None in current vault — candidate for linkage to [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (DPDP Act, personal data interface for AI training datasets) and any future NCAIC coordination node

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S3 (International Regulatory Context — comparative IP/AI framework) / S4 (Agentic AI Governance — training data provenance)
**Jurisdiction:** India
**Confidence:** High — primary DPIIT government document; officially notified; MEITY-endorsed recommendation
**AI explicit:** Yes — the entire paper addresses GenAI training data copyright
**Tier classification:** Tier A — Explicit AI regulation (proposed): the Hybrid Model, if enacted, would create binding AI training data licensing obligations
**AI Governance Wiki relevance:** HIGH — First Indian government document proposing a mandatory licensing framework specifically for GenAI training data; major policy development with direct implications for AI developer compliance costs and for India's competitive position in global GenAI development

---

## Substantive Content

### Context and Committee Background

DPIIT constituted an expert committee on April 28, 2025 to examine the intersection of generative AI and copyright. The Working Paper is the output of this committee's deliberations. It represents India's first government-level consultative framework for GenAI and copyright.

**MEITY endorsement:** The paper records that MEITY (Ministry of Electronics and Information Technology) endorsed the committee's **Hybrid Model** recommendation. This is significant — it indicates intra-Government alignment between DPIIT (IP policy) and MEITY (digital/technology policy) on the GenAI training data approach.

### Options Considered and Rejected

The committee evaluated and rejected three alternatives:

| Option | Basis | Rejection Reason |
|---|---|---|
| **TDM (Text and Data Mining) Exception** | EU approach (Directive 2019/790, Art. 4) | Majority rejected; Nasscom dissented *in favour* |
| **Voluntary Licensing** | Market-based negotiation | Rejected as insufficient — power asymmetry between large AI developers and individual rightsholders |
| **Extended Collective Licensing (ECL)** | Nordic model | Rejected as inadequate for India's scale and sector diversity |

**Nasscom dissent (Annexure I):** Nasscom formally dissented, supporting the TDM exception model. The dissent note is included as Annexure I to the Working Paper, preserving the minority view.

### Recommended Model: Hybrid Model

The committee's recommended approach combines two mechanisms:

**Mechanism 1 — Mandatory Blanket License**
- AI developers may use any **lawfully accessed** copyrighted content for GenAI training **without prior permission** from rights holders
- The mandatory nature means opt-out by individual rights holders is not possible
- Applies to content accessible through lawful means (purchased, licensed, publicly available)
- Retroactive application: includes content used in models **already deployed** at time of enactment

**Mechanism 2 — Statutory Remuneration Right + CRCAT**
- Rights holders receive a **statutory remuneration right** (not a blocking right; cannot prevent training use, but can receive payment)
- Payment collected and distributed by **CRCAT** (Copyright Royalties Collective for AI Training) — a non-profit designated by the Central Government to act as the collecting society for AI training royalties
- **Revenue-based flat rate:** Royalty calculated as a **percentage of the AI developer's gross global revenue** (exact % to be determined by a Government-appointed committee; ⚠ VERIFY: specific % range not stated in extraction)
- **Trigger:** Royalty obligation arises upon commercialisation of the AI model, not upon training
- Pre-commercial / research-stage training is not subject to royalty obligation ⚠ VERIFY: confirm pre-commercial carve-out scope precisely

**CRCAT Architecture:**
- Non-profit body
- Designated by Central Government (not self-constituted)
- Responsible for: collecting royalties from AI developers, distributing to rights holders, administering the blanket license scheme
- Governance model not yet fully specified in Working Paper ⚠ VERIFY: confirm CRCAT governance structure details when final legislation emerges

### Retroactivity

The Hybrid Model explicitly addresses the retroactivity question: AI developers who have already trained and deployed models on copyrighted content would be covered by the statutory remuneration obligation upon enactment. This is a significant policy position distinguishing India's approach from jurisdictions where pre-enactment training is considered outside regulatory scope.

### Scope of "Lawfully Accessed" Content

The paper uses "lawfully accessed" rather than "lawfully obtained" — this is a broader standard. Content that is freely accessible on the open internet (even if not explicitly licensed for AI training) would qualify under the lawful-access framing, subject to ⚠ VERIFY against final wording.

### Key Absences in Working Paper

The Working Paper (Part 1) does **not** address:
- GenAI **output** copyright (who owns AI-generated content) — deferred to Part 2
- Copyright in **synthetic training data** — deferred
- Cross-border AI training (content from overseas rightsholders) — ⚠ VERIFY: unclear whether CRCAT will have international reciprocity arrangements

---

## Analytical Significance for PRIS Research

### For P4 — Doctrinal / Comparative AI Governance (IJLIT)

DPIIT_1 is the **primary India data point for comparative AI training data copyright governance**. The Hybrid Model occupies a distinct position in the global comparative landscape:

| Jurisdiction | Approach | Mechanism |
|---|---|---|
| EU | TDM Exception (Directive 2019/790, Art. 4) + opt-out | Rights holder opt-out; no royalty |
| Japan | Non-enjoyment TDM exception | Broad exception; no royalty |
| UK | Ongoing consultation; no settled position | — |
| US | Fair use doctrine; case-by-case litigation | Courts, not regulation |
| **India (proposed)** | **Hybrid Model** | **Mandatory blanket license + CRCAT statutory royalty** |

India's Hybrid Model is the **most rights-holder-compensatory approach** of any major jurisdiction, while simultaneously enabling AI training without prior permission — a policy synthesis that will be significant for P4's comparative doctrinal analysis.

### For P1 — SLR (Regulation & Governance)

DPIIT_1 fills the India-copyright-AI gap in the global AI governance SLR. While most governance literature focuses on risk, accountability, and deployment, training data regulation is an emerging frontier. India's position as a proponent of mandatory licensing (vs the EU's TDM exception and the US's fair-use approach) is a distinctive configuration for the fsQCA truth table.

### For fsQCA — Regulatory Configurations

Adds a new dimension to India's AI governance configuration: beyond the RBI/SEBI/MeitY regulatory parallelism pattern, India now has a DPIIT-led IP layer that interacts with but is structurally separate from the financial/data/cyber regulatory stack. This demonstrates India's AI governance is not merely parallelistic within BFSI but is also **multi-ministry and multi-sector** in character.

### Consulting Connection

Relevant to **PrivacyWeave** (DPDP purpose enforcement): AI training data usage intersects with DPDP Act personal data protections — if training datasets include personal data, the Hybrid Model's mandatory blanket license does not override DPDP consent requirements. This creates a compliance intersection that PrivacyWeave's runtime enforcement layer would need to address.

---

## Connections

**Related corpus nodes:**
- [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] — DPDP Act interface: personal data in AI training datasets remains subject to DPDP Rules regardless of CRCAT licensing
- [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] — NCAIC proposed as national coordinator; DPIIT_1 sits outside NCAIC's proposed remit (IP is Commerce Ministry, not MEITY/NCAIC)

**Related concepts:**
- [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — DPIIT operating independently of MEITY's AI governance framework despite MEITY endorsing the Hybrid Model; IP governance remains in Commerce Ministry silo separate from MeitY's AI policy work
- [[05_Concepts/05_Concepts_Standard/Accountability]] — Statutory remuneration right as an accountability mechanism for AI developers re: rights holder compensation
- [[05_Concepts/05_Concepts_Standard/Transparency]] — CRCAT administration and distribution methodology will require transparency requirements (not yet specified)
- [[05_Concepts/05_Concepts_Standard/Legitimacy]] — Procedural legitimacy: committee consultation process, Nasscom dissent formally preserved

**Related projects:**
- [[02_Projects/P4_Doctrinal_IJLIT]] — Primary: comparative IP/AI doctrinal analysis
- [[02_Projects/P1_SLR_RG]] — AI governance landscape (India copyright layer)
- [[02_Projects/fsQCA_Thesis_Chapter]] — India configuration: multi-ministry, multi-layer AI governance

**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

**Related consulting:** PrivacyWeave (DPDP / AI training data intersection)

---

## ⚠ VERIFY BEFORE PUBLISHING

1. **Committee Chair name** — not captured in extraction; verify from notification P-24029/34/2025-IPR-VII
2. **Royalty rate (% of gross global revenue)** — specific percentage range stated in Working Paper not captured; verify before citing as a specific figure
3. **Pre-commercial carve-out scope** — confirm exact wording of exemption for pre-commercialisation training
4. **CRCAT governance structure** — non-profit but exact governance model (board composition, dispute resolution) not confirmed from extraction
5. **Cross-border / international reciprocity for CRCAT** — unclear from available content whether international rights holders are covered

---

## Coding Status

- **P3 NVivo:** Not applicable (copyright/IP governance, not BFSI AI governance)
- **P4 NVivo:** Canonical corpus — IP/AI comparative doctrinal analysis
- **Wiki intake status:** Pending

---

## Log

- 2026-06-18: Corpus node created. New institution folder DPIIT created. Batch 4 (Policy Dump intake). Cowork session.
