---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - source/practitioner-explainer
  - content/wiki-entry
  - gate/open
  - section/S6
  - section/S8
  - topic/iso-42001
  - topic/aims
  - topic/certification
  - paper/p3
  - paper/p4
---

# ISO 42001 Cheat Sheet — A Founder's Guide (Kırış Can / techletter.co, 2026) — Intake Note

**Source:** Nesibe Kırış Can (techletter.co), based on the *ISO 42001 Starter Guide* (HUX AI, 2025), co-authored with Burçin Kızılcıklı, Ege Uğur Amasya, Hayriye Anıl, İdil Kula, Onur Pişirir
**Year:** 2026 (v1.0)
**File ID:** F141
**Zotero key:** [leave blank — to be added manually]
**Wiki section(s):** S6 (Implementation & Governance Artifacts), S8 (Reference & Glossary)
**Confidence:** Medium — well-structured practitioner explainer with a disclosed primary-standard citation (ISO/IEC 42001:2023) and named companion standards, but not a peer-reviewed or regulator-issued source; explicitly labelled "Informational content, not legal or compliance advice"
**Jurisdiction:** Global, with a named comparator table (NIST AI RMF/US, EU AI Act/EU, ISO 42001/Global) and a Singapore-specific pointer (IMDA agentic AI framework)

---

## Classification

**Document type:** Practitioner explainer / "founder's guide" (7-page structured cheat sheet), CC BY-NC 4.0
**Primary audience:** Founders, executives, GCs — people making the certify/don't-certify decision, not implementers
**AI explicit:** Yes — entire document is the ISO/IEC 42001 AIMS standard
**PRIS role:** A well-organised operational companion to the vault's existing, more analytically pointed [[06_Frameworks/ISO_IEC_42001]] framework node. This intake note supplies structural/operational detail (clause map, Annex A/C contents, founder decisions, failure modes, checklist) that the framework node does not carry at this granularity; it does **not** carry the framework node's core finding (no jurisdiction grants ISO 42001 a compliance presumption) and should not be cited in place of it.

---

## Reusable Findings

1. **Seven founder decisions, one per clause (feeds S6).** A compact decision framework mapping each of Clauses 4–10 to a specific leadership call: scope boundary (Cl. 4), non-delegable accountability (Cl. 5), written acceptance of residual risk (Cl. 6), competence budget (Cl. 7), kill-switch/rollback readiness before launch (Cl. 8), auditor independence from builders (Cl. 9), and treating repeated failures as governance failures, not technical ones (Cl. 10). Directly reusable as a board briefing structure — more actionable than the standard's own clause numbering for a non-specialist audience.

2. **Annex A/C structure — 9 control families, 38 controls, named risk sources (feeds S6/S8).** Annex A: policies, internal organization, resources/governance, impact assessment, AI system lifecycle (split into management guidance A.6.1 and lifecycle A.6.2), data operations, information for interested parties, use of AI systems, third parties — 9 families, 10 objective groups, 38 controls total. Annex C risk sources named explicitly: environmental complexity, lack of transparency/explainability, level of automation, ML-specific risks (data quality/poisoning), hardware issues, technology readiness, life-cycle issues. Reusable as a gap-analysis checklist independent of certification intent.

3. **Where implementations fail — six named failure modes (feeds S6).** Certification treated as a project with an end date rather than an ongoing management system; policies without named owners/deadlines; auditors reporting to the people they audit (independence collapse); residual risk never formally documented/accepted; vendor AI bought with no vendor risk assessment ("their risk becomes yours, silently"); generic risk registers naming no specific system. Directly usable as a client-facing red-flag checklist for AEGIS_OS/PrivacyWeave engagement scoping.

4. **Four-standard comparison table, reused from Trout et al. (feeds S6).** ISO 42001, NIST AI RMF, STAR for AI, and AIUC-1 compared on issuing body, revision cadence, scope and performance-basis; the cheat sheet notes only AIUC-1 is performance-based (certification conditioned on benchmark scores, quarterly revision). This is the same comparison already captured with a conflict-of-interest caveat at [[04_Knowledge_Products/Wiki_Intake/F133_Trout_et_al_AI_Insurance_Stack_2026]] — treat as independent corroboration of the table's contents, not as a second neutral source, since this cheat sheet does not appear to have independently verified AIUC-1's positioning.

5. **Singapore IMDA agentic AI framework flagged as the sector's first (feeds S3).** "Jan 2026: Singapore's IMDA published the Model AI Governance Framework for Agentic AI, the first governance framework dedicated to AI agents," framed as answering the autonomy/oversight question the management-system standards leave open (L1 Human-Led → L4 Autonomous graduated-autonomy scale). Already covered in the vault at [[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]] and [[06_Frameworks/Singapore_AI_Governance]] — this document supplies independent corroboration of the "first dedicated agentic AI framework" characterisation, useful as a citable third-party confirmation of that claim's novelty framing.

---

## The India Angle — Contradiction Flagged, Not Resolved

This document does not itself discuss India, but its Annex A/C detail sharpens a live, unresolved contradiction already surfaced this session: [[06_Frameworks/ISO_IEC_42001]] records a confirmed gap ("no NABCB accreditation programme located" as of 2026-08-02), while [[07_Institutions/Corpus/Parliament/Parliament_2_Unstarred_Question_2988_Institutional_Framework_Auditing_AI_2026]] (5 August 2026) has the Government stating NABCB accreditation against ISO/IEC 42006:2025 is operational. This cheat sheet's clean statement of what a *functioning* accreditation-of-certifiers layer looks like (Clause 9 auditor independence; ISO/IEC 42006 as the scheme-specific competence standard) is useful as a checklist for verifying which of the two claims is accurate once NABCB's own documentation is located — see VERIFY #304 on the Parliament_2 node.

---

## Citation Hygiene

| Flag | Issue | Handling |
|---|---|---|
| **Non-independent authorship network** | Author group overlaps with HUX AI's own *ISO 42001 Starter Guide*; this is a condensed, re-published derivative, not an independently sourced second opinion | Cite as a single source lineage (HUX AI / Nesibe Kırış Can), not as corroborating evidence separate from the Starter Guide it is based on |
| **Worked case study is explicitly fictional** | The X Corporation AI-HR-screening example (§06) is labelled "A FICTIONAL CASE, A REAL PATTERN" | Do not cite the case study's figures (78% fairness alert, 82→91% post-retraining) as empirical findings — illustrative only |
| **No legal/compliance status claim** | Document footer: "Informational content, not legal or compliance advice" | Do not use for anything requiring authoritative legal sourcing; defer to [[06_Frameworks/ISO_IEC_42001]] and primary ISO/IEC text for anything publication-track |

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The seven-founder-decisions framework (finding 1) and the six failure-mode checklist (finding 3) are both immediately usable, with attribution, as slides or handouts in an AEGIS_OS/PrivacyWeave scoping conversation or an IIM-K governance session — they translate ISO/IEC 42001's clause structure into decision-maker language more directly than the standard itself or the vault's own framework node.
**Consulting connections:** AEGIS_OS, PrivacyWeave (both scoped around exactly the governance-not-engineering distinction this cheat sheet argues)
**Teaching connection:** Usable alongside F140 (Joshi ISC2 deck) for a combined "governance vs engineering" teaching module

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S6, S8
**Concepts:** [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | [[05_Concepts/05_Concepts_Standard/Accountability]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]]
**Frameworks:** [[06_Frameworks/ISO_IEC_42001]] (primary framework node — this note is a supporting operational companion, not a replacement) | [[06_Frameworks/Singapore_AI_Governance]] | [[06_Frameworks/NIST_AI_RMF]] | [[06_Frameworks/EU_AI_Act]]
**Corpus nodes:** [[07_Institutions/Corpus/BIS/BIS_1_LITD30_and_IS_ISO_IEC_42001_Adoption]] | [[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]] | [[07_Institutions/Corpus/Parliament/Parliament_2_Unstarred_Question_2988_Institutional_Framework_Auditing_AI_2026]] (contradiction cross-link)
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] | [[04_Knowledge_Products/Wiki_Intake/F133_Trout_et_al_AI_Insurance_Stack_2026]] (shared four-standard comparison table)
**Projects:** [[02_Projects/P3_BFSI_JEIM]], [[02_Projects/P4_Doctrinal_IJLIT]]

---

## VERIFY Flags

**#308 (LOW).** The four-standard comparison table (finding 4) is reused verbatim in structure from AIUC/Trout et al.'s Table 3 without disclosing AIUC's conflict of interest (see [[04_Knowledge_Products/Wiki_Intake/F133_Trout_et_al_AI_Insurance_Stack_2026]]'s Citation Hygiene table). If reusing this table downstream, carry F133's conflict-of-interest caveat forward regardless of which document is cited as the proximate source.

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [x] Linked to concept notes
- [ ] Marked processed

---

## Log

- 2026-08-09: Intake note created via Cowork corpus intake session (Desktop-folder ad hoc batch). Pre-flight duplicate check against [[06_Frameworks/ISO_IEC_42001]] and existing Wiki Intake notes found no prior node for this specific document; treated as a supporting companion to the existing framework node rather than a duplicate given materially different content (operational/clause-level detail vs the framework node's compliance-recognition finding). Surfaced and cross-linked to the NABCB/ISO 42006 contradiction between [[06_Frameworks/ISO_IEC_42001]] and the same-session [[07_Institutions/Corpus/Parliament/Parliament_2_Unstarred_Question_2988_Institutional_Framework_Auditing_AI_2026]] node. One new VERIFY flag (#308, LOW).
