---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S1
  - section/S6
  - tier/high
  - project/p1-primary
  - project/p3
  - project/p4
  - batch/16
  - engine/phd
---

# Costanza-Chock, Raji & Buolamwini: Who Audits the Auditors? Recommendations from a Field Scan of the Algorithmic Auditing Ecosystem (2022)

**Node ID:** F061
**Type:** Wiki Intake Note (Format B)
**Wiki Section:** S1 (Governance Fundamentals) / S6 (Model Risk / Implementation)
**Status:** Active | **Tier:** High
**Last Updated:** 2026-07-14 (Batch 16)

---

## Source

**Full Citation (APA):** Costanza-Chock, S., Raji, I. D., & Buolamwini, J. (2022). Who audits the auditors? Recommendations from a field scan of the algorithmic auditing ecosystem. In *Proceedings of the 2022 ACM Conference on Fairness, Accountability, and Transparency (FAccT '22)* (pp. 1571–1583). https://doi.org/10.1145/3531146.3533213
**Authors:** Sasha Costanza-Chock, Inioluwa Deborah Raji, Joy Buolamwini — all with the Algorithmic Justice League (Cambridge, USA / Berkeley, USA)
**Pages:** 13 | **Type:** ACM FAccT peer-reviewed conference paper
**Batch:** 16 | **Batch marker:** ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕

---

## Summary

Costanza-Chock, Raji & Buolamwini provide the first comprehensive field scan of the algorithmic auditing ecosystem — cataloguing 438 individuals and 189 organisations engaged in AI audit practice, surveying 152 practitioners anonymously, and interviewing 10 industry leaders. The paper identifies that "AI audit" claims are increasingly common but structurally under-defined: without shared standards or regulatory guidance, first-, second-, and third-party audit claims are difficult to verify and may exacerbate rather than mitigate bias/harm. The paper is the foundational empirical grounding for the [[Assurance_Reuse_Gap]] concept — showing that even where audits *exist*, the ecosystem lacks the standards and cross-recognition mechanisms that would let their outputs actually be reusable across governance forums.

---

## Key Findings

### Field-Scan Empirical Structure

| Data Source | Sample Size | Key Insight |
|---|---|---|
| Individual catalogue | N = 438 | Ecosystem is young; most practitioners have <5 years experience |
| Organisation catalogue | N = 189 | Concentrated in North America + UK/EU; sparse in Global South |
| Anonymous survey | N = 152 | Widespread frustration with lack of standards |
| Industry leader interviews | N = 10 | Confirm need for regulatory guidance |

### Central Findings

1. **"AI audit" is under-defined:** First-party (internal), second-party (contracted), and third-party (independent) audits all use the same label but differ radically in independence, rigor, and standards.
2. **No shared standards:** The field lacks equivalents of financial-audit standards (GAAP, GAAS) or medical-device audit standards (ISO 13485).
3. **Audit ≠ accountability:** Auditing without regulatory backing produces the *appearance* of accountability without operational consequence.
4. **Audit ecosystem risks bias amplification:** Poorly-defined audits, particularly first-party ones, can legitimise harmful systems.

### Policy Recommendations

Costanza-Chock, Raji & Buolamwini propose:
- Mandatory third-party audit for high-risk systems (analog to Sarbanes-Oxley for financial statements)
- Public auditor registries with credentialing
- Standardised audit methodologies with cross-jurisdictional recognition
- Auditor legal safe harbours protecting adversarial testing
- Post-audit accountability mechanisms (findings publication + remediation obligations)

---

## Relevance to PRIS Research

**[[P1_SLR_RG]] (primary):** Foundational algorithmic-auditing literature reference. Anchors the SLR's audit-and-assurance chapter.

**[[P3_BFSI_JEIM]]:** Directly grounds the [[Assurance_Reuse_Gap]] construct. India's four-cycle audit stack (DPDP DPIA + SEBI CSCRF + RBI outsourcing + CERT-In cyber audit) exhibits precisely the un-standardised, non-reusable pattern Costanza-Chock et al. document globally.

**[[P4_Doctrinal_IJLIT]]:** Auditor legal safe-harbour recommendation is directly applicable to India's absence of auditor safe harbour + non-recognition-across-regulators framework.

**Concept links:**
- [[Assurance_Reuse_Gap]] — **canonical academic grounding for this concept** (paper predates the PRIS construct but empirically demonstrates it globally)
- [[Governance_Debt]] — audit ecosystem un-standardisation as governance debt
- [[Accountability]] — audit as accountability mechanism; F061 shows the gap where audit exists but accountability doesn't
- [[Institutional_Coherence]] — cross-recognition of audits as coherence mechanism
- [[Governance_Capacity]] — auditor credentialing + safe harbour as capacity building

**Related nodes:**
- [[04_Knowledge_Products/Wiki_Intake/F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations|F041]] — AEF-1 addresses the *evaluation* layer of the same problem F061 addresses at the *audit* layer
- [[04_Knowledge_Products/Wiki_Intake/Hadley_Algorithm_Review_Boards_RAI_2025|F060]] — ARBs (internal) as counterpart to external algorithmic auditors (F061)
- [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] — CERT-In empanelment as India's operative audit-standardisation instance

---

## VERIFY Flags

**#191 — RESOLVED (2026-07-31, WebSearch/ACM Digital Library).** Page range independently confirmed exact match: pp. 1571–1583. Institutional affiliation confirmed per the ACM DL record itself: all three authors listed simply as "Algorithmic Justice League" (no further institutional breakdown on the primary source) — this node's own Authors line already correctly uses this. The more granular individual affiliations (Berkman Klein/Harvard, UC Berkeley, MIT Media Lab) are optional biographical enrichment, not required for citation accuracy. Flag closed.

---

*Node written: 2026-07-14 | Batch 16 | PRIS v2.3*
