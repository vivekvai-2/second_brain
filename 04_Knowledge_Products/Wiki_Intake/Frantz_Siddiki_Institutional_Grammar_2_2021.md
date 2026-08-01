---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S1
  - section/S7
  - tier/high
  - project/p1
  - project/p2
  - project/p3
  - project/p4
  - project/fsqca
  - method/institutional-grammar
  - batch/16
  - engine/phd
---

# Frantz & Siddiki: Institutional Grammar 2.0 — A Specification for Encoding and Analyzing Institutional Design (2021)

**Node ID:** F056
**Type:** Wiki Intake Note (Format B) — **Methodological Anchor**
**Wiki Section:** S1 (Governance Fundamentals) / S7 (Research Methods)
**Status:** Active
**Tier:** High (Foundational methods reference)
**Last Updated:** 2026-07-14 (Batch 16)

---

## Source

**Full Citation (APA):** Frantz, C. K., & Siddiki, S. (2021). Institutional Grammar 2.0: A specification for encoding and analyzing institutional design. *Public Administration*, *99*(2), 222–247. https://doi.org/10.1111/padm.12719
**Document Type:** Symposium article in peer-reviewed journal (Public Administration, Wiley) — ABDC A (confirmed 2026-07-31, see VERIFY #186 resolution)
**Authors:** Christopher K. Frantz (Department of Computer Science, NTNU, Gjøvik, Norway); Saba Siddiki (Department of Public Administration and International Affairs, Syracuse University, USA)
**Batch:** 16 | **Batch marker:** ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕
**Source corpus:** Policy Dump root — file `Public Administration - 2021 - Frantz - Institutional Grammar 2 0  A specification for encoding and analyzing institutional.pdf`

---

## Summary

Frantz & Siddiki present the formal specification of Institutional Grammar 2.0 (IG 2.0), an updated syntactic framework for encoding and analysing institutional statements — the structured components (Attributes, Deontic, Aim, Conditions, Or-else) that constitute rules governing individual and collective behaviour. The paper positions IG 2.0 as an evolution of Crawford & Ostrom's (1995) original ADICO framework, adding formal syntactic rigor, computational tractability, and expanded operational rules for coding institutional design across policy and administrative domains. The methodological paper anchors the entire PRIS coding pipeline — used throughout P2 (DPI ADICO coding), P3 (BFSI sectoral instrument coding), and P4 (comparative doctrinal analysis) — and provides the empirical grounding for construct claims that rely on ADICO evidence (e.g., [[Deontic_Bifurcation]] deontic ratios; [[Records_Rules_Asymmetry]] attribute-position analysis).

**This is a methodological anchor node — the founding IG 2.0 paper cited across concept files but until now referenced only via [[Institutional_Grammar_IG2]] without a dedicated corpus entry.**

---

## Key Findings and Framework

### IG 2.0 Component Specification

| Component | Function | Coding Notation |
|---|---|---|
| **Attributes (A)** | Actor to whom the rule applies | Actor identifier + role qualifier |
| **Deontic (D)** | Prescriptive modality — obligation, permission, prohibition | SHALL / SHOULD / MAY / MUST NOT |
| **Aim (I)** | Action or outcome the rule prescribes | Verb phrase; distinguishes system-facing vs. citizen-facing |
| **Conditions (C)** | Contextual constraints — when, where, under what circumstances | Temporal / spatial / relational qualifiers |
| **Or-else (O)** | Sanction for non-compliance | Specified consequence + enforcement authority |

### Innovations Over ADICO 1.0

- Explicit hierarchical structure for nested institutional statements
- Formal computational representation (parseable syntax)
- Improved treatment of constitutive vs. regulative statements (Searle-inspired distinction)
- Extended operationalisation guidance for statement typologies (rule / norm / strategy trichotomy)
- Structured elicitation protocols for coder-reliability

### Applications Reported in the Paper

Frantz & Siddiki demonstrate IG 2.0 across three empirical illustrations:
- Watershed governance rules (US context)
- Constitutional-level rules (US and European contexts)
- Automated compliance-checking of policy documents (proof-of-concept computational parsing)

---

## Relevance to Indian Context and PRIS Research

Frantz & Siddiki (2021) is the **methodological cornerstone** of the entire PRIS coding pipeline. Every construct in the PRIS research programme that depends on ADICO-coded evidence — including [[Regulatory_Parallelism]], [[Governance_Debt]], [[Deontic_Bifurcation]], [[Records_Rules_Asymmetry]], and the four-dimension [[Institutional_Coherence]] operationalisation — rests on the syntactic apparatus formalised in this paper.

Load-bearing methodological functions:

- **P2_DPI_JSIS:** All 248 institutional statements (⚠VERIFY count) across 12 DPI documents were coded using this specification
- **P3_BFSI_JEIM:** Sectoral instrument coding (RBI, SEBI, DPDP, CERT-In) follows IG 2.0 rules
- **P4_Doctrinal_IJLIT:** Comparative doctrinal analysis of ADM rules across India-EU-UK-US follows IG 2.0 syntax
- **fsQCA_Thesis_Chapter:** Deontic ratios and rule-density measures used in fsQCA calibration are IG 2.0-derived

## Connections to Research

**[[P1_SLR_RG]]:** Methodology reference for the SLR chapter's coding protocol.

**[[P2_DPI_JSIS]] (primary methodological anchor):** IG 2.0 syntax defines the entire P2 empirical apparatus.

**[[P3_BFSI_JEIM]]:** IG 2.0-based coding of RBI/SEBI/IRDAI/DPDP instruments.

**[[P4_Doctrinal_IJLIT]]:** Comparative doctrinal ADICO coding for cross-jurisdiction analysis.

**[[fsQCA_Thesis_Chapter]]:** IG 2.0 outputs feed fsQCA calibration.

**Concept links (methodological grounding for all):**
- [[Regulatory_Parallelism]] — measured via absence of cross-references in ADICO-coded statements
- [[Governance_Debt]] — measured via unresolved deontic obligations
- [[Institutional_Coherence]] — measured via cross-referencing dimension
- [[Deontic_Bifurcation]] — the SHALL/SHOULD distinction that anchors the construct
- [[Records_Rules_Asymmetry]] — the Attributes-position analysis that anchors the construct
- [[Accountability]] — Or-else component operationalises accountability structure
- [[Institutional_Grammar_IG2]] — this paper IS the reference for the [[Institutional_Grammar_IG2]] method-tag

**Related nodes:**
- [[04_Knowledge_Products/Wiki_Intake/F034_Buscemi_Assessing_High_Risk_AI_2025|F034]] — Buscemi's legal-to-technical verification methodology as a complementary formal specification
- [[Records_Rules_Asymmetry]] — new candidate concept operationalised via IG 2.0 Attributes-position coding

---

## Methodological Notes

**IG 2.0 vs IG 1.0 (ADICO original 1995):** The 2.0 revision adds parseable syntax and explicit computational tractability. PRIS uses IG 2.0 exclusively.

**Coder reliability:** The specification requires ≥90% intercoder agreement for research-grade coding — the standard PRIS aims for (⚠VERIFY against actual P2/P3 intercoder agreement rates).

**Tools:** The Institutional Grammar Research Group at NTNU maintains the reference parser and specification. PRIS coding should verify tool version at time of coding for reproducibility.

---

## VERIFY Flags

**#186 — RESOLVED (2026-07-31, Perplexity Deep Research against full ABDC 2022 Journal Quality List text).** *Public Administration* (Wiley-Blackwell) confirmed **A** — High confidence, resolving the A-vs-A* ambiguity. Symposium-article citation-format question not addressed by this pass — low-priority residual, does not affect the ranking.

---

*Node written: 2026-07-14 | Batch 16 | PRIS v2.3 | Methodological anchor node — foundational to entire coding pipeline*
