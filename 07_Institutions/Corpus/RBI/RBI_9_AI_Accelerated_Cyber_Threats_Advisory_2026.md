---
type: corpus-node
node-id: RBI_9
institution: RBI
date: 2026-06
wiki-section: S2
tier: C
ai-explicit: true
status: active-unverified
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - institution/RBI
  - wiki-section/S2
  - tier/C
  - status/primary-source-missing
  - batch/ad-hoc-20260802
  - concept/Evidentiary_Governance
  - concept/Regulatory_Parallelism
  - concept/Governance_Debt
  - concept/Deontic_Bifurcation
  - concept/Agentic_AI_Governance
  - project/P3
  - project/P4
  - jurisdiction/india
---

# RBI_9 — Advisories on AI-Accelerated Cyber Threats and Related Safeguards (AI-ACT&RS)

**Node ID:** RBI_9
**Institution:** Reserve Bank of India (RBI)
**Document type:** Advisory (or advisories — plural in all sources)
**Date:** June 2026 (exact date unconfirmed)
**Jurisdiction:** India — banks and RBI-regulated entities
**Wiki Section:** S2 — India Regulatory
**Tier:** **C — no primary text obtained.** Built from secondary sources only.

> ## ⚠ TIER C — PRIMARY SOURCE NOT OBTAINED
>
> **No copy of the AI-ACT&RS advisory itself has been retrieved.** The advisory does not appear on RBI's public circular index in the sources searched; it appears to have been issued directly to regulated entities rather than published. Everything below derives from:
> 1. **KPMG in India**, "RBI advisory on AI-Accelerated Cyber Threats and Related Safeguards (AI-ACT&RS)", 11 June 2026 — advisory-firm commentary mapping the advisory's control domains.
> 2. **Business Standard**, "RBI asks banks to assess AI risk gaps, draw action plan by June-end", 10 June 2026 — reporting expressly sourced to "people familiar with the matter."
>
> **On-record corroboration exists** and is the strongest element of the evidence base: RBI Deputy Governor **Swaminathan J**, at the post-monetary-policy press conference, stated that RBI "*[has] issued the required advisories*" in relation to Mythos-class cyber threats. The *existence* of the advisory is therefore confirmed on the record by RBI itself; its *contents* are not.
>
> **This node must not be cited in publication-track output for any provision-level claim until the primary text is obtained.** This is the same evidentiary-debt failure mode recorded at [[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025]] and it is being flagged at intake rather than discovered later.

---

## S1. Document Identity

| Field | Detail | Confidence |
|---|---|---|
| Short name | AI-ACT&RS — AI-Accelerated Cyber Threats and Related Safeguards | HIGH (KPMG uses this acronym as its title) |
| Issuing Authority | Reserve Bank of India | HIGH |
| Instrument type | "Advisories" — plural in both KPMG and the Deputy Governor's statement | MEDIUM — whether one instrument or several is unclear |
| Date | June 2026; KPMG commentary dated 11 June 2026; BS report 10 June 2026 | MEDIUM — issuance date not stated in either source |
| Reference number | **Unknown** | — |
| Legal basis | **Unknown** | — |
| Binding status | **Unknown.** Termed "advisory" but paired with a hard compliance deadline and a board-approval requirement | LOW |
| Scope | Banks and other RBI-regulated entities | HIGH |
| Key deadline | **Board-approved gap assessment and time-bound action plan by 30 June 2026** | MEDIUM — reported by BS on anonymous sourcing; not independently confirmed |

---

## S2. Governance Context — the finding that matters

**RBI issued AI-specific cyber guidance in June 2026 and then issued an AI-silent binding cyber framework six weeks later.**

[[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] — the *Cybersecurity, Technology: Risk, Resilience and Assurance Framework Directions, 2026*, issued **31 July 2026**, binding, in force on issuance, 56 pages, 233 paragraphs — contains **zero** AI provisions (verified full-text sweep: *artificial intelligence* 0, *machine learning* 0, *model risk* 0, *generative* 0, *automated decision* 0, bare token `AI` 0).

RBI_9 shows this is not because RBI had nothing to say about AI and cyber. It had said it, in detail, six weeks earlier — in a **non-binding advisory** that was, on the available evidence, not even published.

This converts the intra-regulator parallelism finding recorded at RBI_8 §S5.1 into something sharper and more specific: a **deontic split**. AI content went into the hortatory, unpublished instrument; the binding, published, repealing instrument was kept technology-neutral. That is a textbook [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] pattern operating *within a single regulator across a six-week window*, and it is a stronger claim than the cross-regulator version because it cannot be attributed to inter-agency coordination failure.

⚠ This inference depends on RBI_9's content, which is Tier C. **The finding is robust as to the existence and timing of an AI-specific advisory (on-record, Deputy Governor) but provisional as to its detailed content.**

---

## S3. Reported Content — control domains

Per KPMG's mapping, the advisory has a **two-fold intent**: (i) harden existing technology stacks against AI-accelerated threats, and (ii) put guardrails around how AI, including generative AI, is adopted, integrated and sourced.

KPMG lists the following domains as covered:

| # | Domain (KPMG's terms) | PRIS relevance |
|---|---|---|
| 1 | AI governance | Overlaps RBI_FREE_AI_2025 Seven Sutras |
| 2 | Classification, ownership and lifecycle management | AI asset inventory |
| 3 | Secure development, integration and configuration | — |
| 4 | Access control and data protection | — |
| 5 | AI-specific threat controls | Prompt injection, adversarial |
| 6 | Performance monitoring and output validation | Human oversight |
| 7 | AI change management | — |
| 8 | **Logging, traceability and forensic readiness** | **Direct [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] instance — see S5.1** |
| 9 | Resilience and continuity; **AI agents and privileged access** | [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] |
| 10 | Third-party AI risk management | — |
| 11 | Creation of AI usage policy | — |
| 12 | Audit, testing, training and awareness for AI systems | — |

Per Business Standard, the required exercise obliges REs to "establish a structured cybersecurity framework, undertake AI-led tests against potential threats, and identify existing vulnerabilities."

---

## S4. Key Quotes (from secondary sources — not from the instrument)

**RBI Deputy Governor Swaminathan J, post-monetary-policy press conference (quoted in Business Standard, 10 June 2026):**
> "We have issued the required advisories. We remain fully prepared in terms of handling cyber security threats of this nature as well as conventional threats."

> "This system has been engaging our attention, both at the government level and at the financial sector inter-regulatory forum level. RBI in consultation with the government and other regulators, will take further steps once the contours of participation become clear."

**Union Finance Minister Nirmala Sitharaman, April 2026 (two separate utterances, quoted in Business Standard):**
> "…A new challenge has emerged in the form of Mythos."

> "Not much is known about it yet. The Ministry of Electronics and Information Technology is actively engaging with authorities and governments across the globe, as well as with technology companies, to understand how this will evolve and what kind of preparedness is required in India."

**Kartik Shinde, Partner, Cybersecurity Consulting, EY India (quoted in Business Standard):**
> "For RBI and Sebi… regulated entities, they are required to do a gap assessment against the Mythos-related advisories which include AI adversarial testing, scanning for existing vulnerabilities using AI, among other things."

---

## S5. Analytical Notes

### S5.1 — "Forensic readiness" named by an Indian financial regulator

KPMG lists **"Logging, traceability and forensic readiness"** as a discrete domain of the advisory. If accurate, this is the corpus's first instance of an Indian financial regulator using *forensic readiness* as a named AI-governance control domain — the exact construct at the theoretical core of [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] (Tan 2001; Daubner et al. 2023).

It also completes a striking sequence within RBI's own 2026 output: RBI_9 (June, advisory, non-binding) names AI forensic readiness; [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] (July, binding) defines *digital forensics* by reference to NIST and requires audit trails sufficient for "forensic evidence… including for non-repudiation purposes" — but says nothing about AI.

**RBI has the evidentiary vocabulary and the AI vocabulary. It has not put them in the same binding instrument.** That sentence is, on the current corpus, the sharpest available statement of the intra-regulator parallelism finding.

⚠ Contingent on Tier C content. Confirm against primary text before publication.

### S5.2 — Mythos as a cross-regulator trigger

The same commercial model triggered instruments from two regulators within five weeks: [[07_Institutions/Corpus/SEBI/SEBI_18_AI_Vulnerability_Detection_Advisory_2026]] (5 May 2026, naming "Claude Mythos" in the circular text) and RBI_9 (June 2026). Sitharaman's April 2026 meeting with bank heads preceded both, and MeitY was engaging internationally in parallel.

This is **coordination by common shock rather than by design** — a distinct mechanism from the citation-chain coordination absent everywhere in the corpus, and from the isomorphism recorded at [[07_Institutions/Corpus/International/International_19_IOSCO_AI_Capital_Markets_CR_2025]]. Worth theorising separately: where an external technological event forces simultaneous regulatory response, apparent convergence may reflect a shared exogenous trigger rather than institutional learning. This weakens any naive reading of the seven-week convergence (see [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]]) as evidence of coherence.

### S5.3 — The unpublished-instrument problem

If the advisory was issued to regulated entities without publication, it raises a governance question in its own right: obligations with board-level approval requirements and hard deadlines, not available for public scrutiny, cannot be studied, contested or complied with by non-addressees who are nonetheless affected (vendors, auditors, customers). This is a **transparency deficit at the instrument level**, distinct from the algorithmic transparency questions the corpus usually addresses. Connects to [[05_Concepts/05_Concepts_Standard/Transparency]] and [[05_Concepts/05_Concepts_Standard/Legitimacy]].

⚠ Confirm non-publication before relying on this. Absence from search results is not proof of non-publication.

---

## S6. Concept Linkages

| Concept | Linkage |
|---|---|
| [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] | **Primary linkage.** AI content in a non-binding advisory (June); binding Directions six weeks later (July) are AI-silent. Deontic split within one regulator, one quarter. |
| [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | "Logging, traceability and forensic readiness" as a named control domain (Tier C). |
| [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | Intra-regulator: RBI_9 ↔ RBI_8, no cross-reference either way. |
| [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | Feeds the *intra-regulator parallelism debt* sub-pattern; REs must satisfy a June advisory whose subject matter is absent from the July binding framework that repealed their prior obligations. |
| [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] | "AI agents and privileged access" named as a domain. |
| [[05_Concepts/05_Concepts_Standard/Transparency]] / [[05_Concepts/05_Concepts_Standard/Legitimacy]] | Unpublished-instrument problem (S5.3). |

---

## S7. Project Relevance

| Project | Relevance |
|---|---|
| [[02_Projects/P3_BFSI_JEIM]] | **High** — completes the RBI 2026 sequence and supplies the deontic-split finding. Tier C limits citation until primary obtained. |
| [[02_Projects/P4_Doctrinal_IJLIT]] | **High** — unpublished quasi-binding advisory as a doctrinal problem; deontic bifurcation. |

---

## S8. ⚠ VERIFY Flags

- **⚠ V-RBI9-1 (HIGH — blocking, node-level).** **Primary text not obtained.** Reference number, exact date, legal basis and binding status all unknown. Obtain from RBI or from a regulated entity's compliance function before any provision-level citation. Until then this node is corroborating intelligence, not evidence.
- **⚠ V-RBI9-2 (HIGH).** The 30 June 2026 board-approved gap assessment deadline rests on Business Standard reporting expressly attributed to "people familiar with the matter." **Anonymous sourcing — do not cite as established.**
- **⚠ V-RBI9-3 (MEDIUM).** The twelve control domains at S3 are **KPMG's characterisation** of the advisory, not RBI's own section headings. The "logging, traceability and forensic readiness" formulation — analytically the most valuable item in this node — is therefore an advisory firm's paraphrase. Confirm against primary text before building any argument on it.
- **⚠ V-RBI9-4 (MEDIUM).** Whether AI-ACT&RS is one instrument or several ("advisories", plural, in both KPMG and the Deputy Governor's statement) is unresolved. Node title uses the plural accordingly.
- **⚠ V-RBI9-5 (LOW).** Non-publication is inferred from absence in searched sources (S5.3). Absence of evidence is not evidence of absence — confirm.

---

## Backlinks

**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] | [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] | [[07_Institutions/Corpus/RBI/RBI_7]] | [[07_Institutions/Corpus/RBI/RBI_1]] | [[07_Institutions/Corpus/SEBI/SEBI_18_AI_Vulnerability_Detection_Advisory_2026]] | [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] | [[07_Institutions/Corpus/IRDAI/IRDAI_2_Working_Group_AI_Governance_2026]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] | [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] | [[05_Concepts/05_Concepts_Standard/Transparency]] | [[05_Concepts/05_Concepts_Standard/Legitimacy]]
**Related frameworks:** [[06_Frameworks/RBI_Free_AI]] | [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]]
**Related domains:** [[03_Domains/BFSI_Governance]] | [[03_Domains/Cybersecurity_Governance]] | [[03_Domains/AI_Governance]]
**Related institutions:** [[07_Institutions/RBI]]
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] | [[02_Projects/P4_Doctrinal_IJLIT]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] | [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]]

**Secondary sources used:**
- KPMG in India, *RBI advisory on AI-Accelerated Cyber Threats and Related Safeguards (AI-ACT&RS)*, 11 June 2026
- Kawale, A. & Panda, S., *RBI asks banks to assess AI risk gaps, draw action plan by June-end*, Business Standard, 10 June 2026

---

## Log

- 2026-08-02: Node created at **Tier C — primary source not obtained.** Existence confirmed on-record via RBI Deputy Governor Swaminathan J; contents from KPMG and Business Standard only. Deontic-split finding (RBI_9 non-binding AI advisory June → RBI_8 binding AI-silent Directions July) recorded as the node's primary analytical contribution, flagged as contingent on Tier C content. Five VERIFY flags, two HIGH.
