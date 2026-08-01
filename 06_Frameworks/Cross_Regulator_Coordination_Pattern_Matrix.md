---
type: Framework
tags:
  - type/framework
  - status/active
  - project/p3
  - engine/phd
  - jurisdiction/india
---

# Cross-Regulator Coordination Pattern Matrix

**Type:** Framework **Status:** First-pass matrix populated 2026-07-31 (Synthesis 3) from six citing corpus nodes **Last Updated:** 2026-07-31

---

## Core Synthesis

India's BFSI-adjacent AI/IT governance is produced by at least four regulators (RBI, SEBI, CERT-In, MeitY) operating on materially different clocks, different explicitness levels, and — with one late exception (MeitY_4's own cross-references) — with almost no formal coordination mechanism between them. The dominant pattern across the six corpus nodes populating this matrix is **not conflict** but **silent parallel evolution**: each regulator builds its own AI-adjacent governance layer, occasionally converging in substance (identical taxonomies, overlapping vendor-accountability logic) without ever formally cross-referencing the other regulator's instrument. Where coordination *is* visible, it is almost always **unidirectional and structural** rather than negotiated — one regulator's reporting chain terminates in another regulator's inbox (RBI→CERT-In incident reporting) rather than the two regulators jointly designing a rule. This matrix is the empirical substrate for [[Regulatory_Parallelism]] at the BFSI-instrument level (as distinct from the principles-level parallelism logged separately for NITI vs. RBI/MeitY).

---

## Framework Identity

**Populated from:** [[07_Institutions/Corpus/RBI/RBI_1]], [[07_Institutions/Corpus/RBI/RBI_2]], [[07_Institutions/Corpus/CERT_In/CERT_4]], [[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]], [[07_Institutions/Corpus/SEBI/SEBI_11]] — the six nodes that forward-referenced this framework as a stub. A seventh node, [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]], was found during population to already carry its own "Coordination / Parallelism Pattern" section citing SEBI_9, SEBI_10, and RBI_6_AIFI_Outsourcing_Directions_2025 — folded in below as a fourth regulator (MeitY) rather than re-deriving fresh analysis for it.

**Regulators covered:** RBI, SEBI, CERT-In, MeitY (data-protection dimension only, via DPDP Rules)
**Time span:** January 2019 (SEBI_9) – 2024/25 (SEBI_11, MeitY_4)
**Instrument types:** Master Directions (RBI), Regulatory Circulars (SEBI), Technical Guidelines (CERT-In), Statutory Rules (MeitY)

---

## Structural Overview — The Matrix

| Regulator Pair | Coordination Mechanism | Evidence | Pattern Type |
|---|---|---|---|
| **RBI ↔ SEBI** | None found | RBI_1 (Nov 2023, IT Governance Master Direction) is technology-neutral with **0 AI-specific requirements** — issued four years *after* SEBI_9 (Jan 2019) and SEBI_10 (May 2019) established explicit AI/ML reporting regimes for functionally comparable entities (MIIs, Mutual Funds vs. banks). Neither RBI_1 nor RBI_2 cites either SEBI circular. | **Parallelism** (null-vs-explicit) — the corpus's clearest cross-regulator instance; RBI's silence is not neutral, it is a governance-architecture divergence documented explicitly in RBI_1's own Analytical Significance section. |
| **RBI ↔ CERT-In** | **Formal, mandatory** — the one genuine coordination mechanism in this matrix | RBI_1 §27(d): "REs shall pro-actively notify CERT-In and RBI regarding incidents, as per regulatory requirements." Combined with RBI_2 §17(h)'s three-level reporting chain (service provider → RE → RBI within 6 hours → RBI/CERT-In), this creates a **dual-channel incident-reporting requirement** for the same cyber event. | **Manifestation (M1)** — not parallelism but genuine structural coordination, though asymmetric: CERT-In receives reports, it does not co-design RBI's IT governance framework. |
| **SEBI ↔ CERT-In** | None found | CERT_4 (July 2025, AIBOM technical standard) requires AI system component inventories from government/public-sector AI procurers. SEBI's AI/ML reporting regime (SEBI_9/10, 2019) requires functionally equivalent AI-system inventories from securities-market entities. **No cross-reference either direction** despite functional equivalence at the AI-transparency layer. | **Parallelism** (functional equivalence, zero cross-citation) — CERT_4's own Analytical Significance section flags this explicitly as "Unidirectional or Unpaired." |
| **RBI ↔ CERT-In (AIBOM)** | None found | CERT_4's AIBOM mandate (government/public-sector AI procurement) has no RBI equivalent for BFSI AI procurement; RBI_2's vendor-due-diligence framework (§13–14) does not reference AIBOM/SBOM standards despite substantial functional overlap (both govern third-party AI/IT component disclosure). | **Gap** — no BFSI-specific AIBOM requirement exists; CERT-In's general-purpose standard and RBI's BFSI-specific vendor framework run in parallel, unlinked. |
| **Intra-SEBI (SEBI_9 ↔ SEBI_10)** | **Deliberate, internal** | Identical six-category AI/ML taxonomy (Annexure A/B) issued four months apart for MIIs vs. Mutual Funds — the corpus's clearest *convergence* (not parallelism) instance, coded as Cluster C09 in SEBI_9/SEBI_10's own coordination-pattern sections. | **Convergence** — intentional definitional consistency within a single regulator, the mirror image of the cross-regulator parallelism above. |
| **SEBI (2019) → SEBI (2024)** | Internal regulatory evolution, not cross-regulator | SEBI_11 (2024–25) shifts SEBI's own AI governance logic from *inventory* (SEBI_9/10, "know what AI exists") to *accountability* (SEBI_11, "assign responsibility for AI tools, including third-party-procured ones") — a five-year internal maturation with no RBI equivalent proposed as of 2024–25. | **Unidirectional advancement** — SEBI_11 itself flags (in its own Coordination Pattern Observation table) that "RBI has no parallel initiative as of 2024–25." |
| **SEBI ↔ RBI (vendor accountability)** | None found | SEBI_11 explicitly extends AI responsibility to third-party-procured AI tools; RBI_2 governs IT/AI vendor outsourcing generically (§13–17) but has no AI-specific responsibility-assignment analogue. | **Emerging parallelism** — SEBI_11's own text names this gap directly. |
| **RBI ↔ MeitY (algorithmic/data governance)** | None found (per MeitY_4's own coordination section) | MeitY_4 (DPDP Rules, 2025) cites [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] as a "cloud/algorithmic governance parallel" — same substantive territory (outsourced algorithmic/cloud processing of personal data), issued in the same window (2025), no formal cross-reference between the two instruments. | **Parallelism** — folded in from MeitY_4's pre-existing analysis; consistent with the RBI↔SEBI pattern above (RBI as the "silent" party in cross-regulator pairs). |
| **SEBI ↔ MeitY (AI/ML + data governance)** | None found | MeitY_4 separately cites SEBI_9 and SEBI_10 (AI/ML reporting parallels) and SEBI_11 (AI accountability assignment parallel) in its own Coordination/Parallelism Pattern section — DPDP Rules' data-fiduciary obligations and SEBI's AI/ML governance regime cover overlapping ground (AI systems that process personal financial data) without formal linkage. | **Parallelism** — third instance of the same silent-parallel-evolution pattern, this time between a general-purpose data-protection regulator (MeitY) and a sectoral securities regulator (SEBI). |

---

## Key Tensions & Gaps

The matrix shows a consistent asymmetry: **RBI is the "silent" party in every cross-regulator pairing** where it appears (vs. SEBI, vs. CERT-In-adjacent AIBOM territory, vs. MeitY) — it issues technology-neutral instruments and does not cross-reference sector peers who have gone AI-explicit, even when the underlying entities and risks substantially overlap. The sole exception is the RBI↔CERT-In incident-reporting channel, which is **mandated by regulation** (§27d), not voluntarily coordinated — meaning India's only confirmed formal cross-regulator coordination mechanism for AI/IT-adjacent governance in this matrix is a downstream *reporting obligation*, not an upstream *rule-design* collaboration. No joint circular, MOU, or formally negotiated cross-regulator AI standard appears anywhere across the six populating nodes plus MeitY_4.

---

## Linked Corpus Nodes

[[07_Institutions/Corpus/RBI/RBI_1]] | [[07_Institutions/Corpus/RBI/RBI_2]] | [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] | [[07_Institutions/Corpus/CERT_In/CERT_4]] | [[07_Institutions/Corpus/SEBI/SEBI_9]] | [[07_Institutions/Corpus/SEBI/SEBI_10]] | [[07_Institutions/Corpus/SEBI/SEBI_11]] | [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]]

## Linked Domains

[[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]]

## Linked Concepts

[[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]]

## Linked Frameworks

[[06_Frameworks/Manifestation_Evidence_Layer]] (RBI↔CERT-In M1 evidence)

## Linked Projects

[[02_Projects/P3_BFSI_JEIM]] (primary) | [[02_Projects/P4_Doctrinal_IJLIT]]

---

## Future Research

1. This matrix was built entirely from six (now seven, with MeitY_4) corpus nodes that happened to forward-reference it — not from a systematic sweep of all RBI/SEBI/CERT-In/MeitY/IRDAI instruments. A dedicated pass reading RBI_6, IRDAI_1, and SEBI_8 directly (rather than via secondary citation in other nodes) would likely surface additional pairs and could revise the "RBI is always silent" finding if RBI_6 shows different behaviour.
2. The RBI↔CERT-In §27(d) mandatory reporting chain is the strongest quantifiable M1 evidence in the corpus — worth checking whether an equivalent mandatory-reporting-to-CERT-In clause exists in any SEBI or IRDAI instrument (would upgrade this from a two-regulator to an N-regulator coordination hub finding, with CERT-In as the common node).
3. Candidate fsQCA condition: "presence/absence of AI-specific reporting obligation" as a configurational variable, using this matrix's regulator-pair rows as cases — RBI (0), SEBI (1, then upgraded to accountability), CERT-In (1, general-purpose not sector-specific), MeitY (0, data-fiduciary framing rather than AI-system framing).

---

## Log

- 2026-07-31: Created as a stub during link-hygiene audit (six broken/missing forward-references from CERT_4, RBI_1, RBI_2, SEBI_9, SEBI_10, SEBI_11).
- 2026-07-31 (Synthesis 3, same session): Populated as first-pass matrix. Built entirely from the six citing nodes' own "Coordination Pattern" sections (no fresh research) plus MeitY_4's pre-existing Coordination/Parallelism Pattern section, discovered while cross-checking RBI references. No fabricated cells — every matrix row traces to a specific corpus-node citation.
