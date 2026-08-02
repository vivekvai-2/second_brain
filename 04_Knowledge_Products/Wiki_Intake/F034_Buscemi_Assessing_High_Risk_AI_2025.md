---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
---

# Assessing High-Risk AI Systems under the EU AI Act (Buscemi et al., 2025) — Intake Note

**Source:** arXiv (cs.CY / cs.AI); Luxembourg Institute of Science and Technology (LIST) + Research Institutes of Sweden (RISE)
**Year:** 2025 (submitted December 15, 2025; revised April 3, 2026)
**Full title:** *Assessing High-Risk AI Systems under the EU AI Act: From Legal Requirements to Technical Verification*
**File ID:** F034
**Zotero key:** [to be assigned]
**Wiki section(s):** S1/S3/S6
**Confidence:** Medium — arXiv preprint (December 2025 v1, revised v3 April 2026); not yet confirmed in peer-reviewed venue ⚠ VERIFY BEFORE PUBLISHING
**Jurisdiction:** EU (EU AI Act focus); methods applicable globally

---

## Classification

**Document type:** Academic Paper (arXiv preprint, computer science / law intersection)
**Primary audience:** Researcher / Practitioner (AI auditors, compliance teams, conformity assessment bodies, regulators)
**AI explicit:** Yes — specifically addresses EU AI Act high-risk AI system requirements

**Authors:**
- Alessio Buscemi (Luxembourg Institute of Science and Technology, LIST; University of Luxembourg)
- Tom Deckenbrunnen (Luxembourg Institute of Science and Technology, LIST; University of Luxembourg)
- Fahria Kabir (Research Institutes of Sweden, RISE)
- Kateryna Mishchenko (Research Institutes of Sweden, RISE)
- Nishat Mowla (Research Institutes of Sweden, RISE)

**arXiv ID:** 2512.13907

---

## 3–5 Reusable Findings

1. **Legal-to-technical verification gap — the core compliance problem** (feeds S1/S6): The paper's central finding: EU AI Act high-risk requirements are stated in legal/normative language but must be operationalised as *technically verifiable activities*. The authors construct a structured mapping from EU AI Act Articles and Recitals (legal layer) → international standards (ISO/IEC 42001, 23894, NIST AI RMF) → scientific literature (technical verification methods). This gap between legal obligation and technical testability is the PRIS "verification gap" — the same gap that [[Governance_Debt]] manifests as in India's BFSI context: SEBI/RBI have stated AI governance obligations but no standardised technical verification framework to test compliance. F034 is the first paper in the PRIS corpus to operationally bridge this gap.

2. **Eleven macro-categories of trustworthy AI requirements** (feeds S1/S6): The authors identify 11 verification macro-categories derived from the EU Commission's High-Level Expert Group's seven trustworthy AI principles + additional EU AI Act requirements: Transparency and Explainability; Robustness and Reliability; Safety; Privacy and Data Governance; Fairness and Non-discrimination; Accountability; Human Oversight; Security; Accuracy; Record-keeping and Logging; and Post-market Monitoring. These 11 categories provide a structured compliance checklist that maps almost perfectly onto RBI_FREE_AI_2025's Seven Sutras + SEBI_14's disclosure requirements — confirming convergent technical compliance architectures across India and EU, despite different legal instruments.

3. **UNESCO Recommendation + ISO/IEC standards as shared normative baseline** (feeds S1/S3): The paper's regulatory source review explicitly includes UNESCO Recommendation on the Ethics of AI (International_18), EU AI Act, GDPR, and ISO/IEC 42001/23894. The inclusion of UNESCO as a *regulatory source* (not just an ethical reference) in a technical verification framework confirms International_18's status as a functional normative input to compliance methodology. For PRIS: this creates a direct chain — UNESCO Recommendation → EU AI Act verification requirements → technical testing activities — the same chain should apply to India's MeitY AI Guidelines (MeitY_2) but currently terminates at the guideline level without verification framework.

4. **Risk classification challenge — operationalising "high risk"** (feeds S6/S3): The paper identifies a fundamental challenge in EU AI Act compliance: determining whether a system is "high risk" under Annex III involves legal interpretation, not just technical assessment. The authors find that the same AI system may be high-risk in one deployment context and not in another, creating compliance uncertainty for AI developers and deployers. This maps directly to the India BFSI context: SEBI_14 and RBI_7 both impose accountability obligations on AI outputs without a formal risk classification mechanism — the question of which AI system triggers enhanced governance under Indian regulation is unanswered, creating implementation ambiguity identical to the EU Annex III problem.

5. **Conformity assessment methodology** (feeds S6): The paper proposes a structured conformity assessment process covering: (a) system documentation review; (b) technical testing against 11 macro-categories; (c) post-deployment monitoring requirements; (d) traceability chain from requirement to test to evidence. The authors use this to define what a "technical conformity assessment body" (notified body under EU AI Act) must evaluate. For PRIS: this is directly applicable to designing an India-equivalent AI conformity assessment regime — either within RBI's inspection framework or CERT-In's audit function (CERT_In_1).

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The 11 macro-categories (finding 2) provide a ready-made audit checklist adaptable for Indian BFSI AI compliance — directly usable in AEGIS_OS pre-execution governance certification and as a consulting deliverable for CRO/CISO clients asking "how do we assess AI system compliance with RBI/SEBI requirements?"
**Consulting connections:** AEGIS_OS (pre-execution verification of AI systems against the 11 macro-categories — AEGIS_OS operationalises runtime enforcement of categories 1-4; the paper provides the normative basis for categories 5-11); PrivacyWeave (Category 4 Privacy and Data Governance — DPDP Act compliance as the India-specific instantiation)
**Teaching connection:** AI regulatory compliance — doctoral/executive seminar on translating legal AI governance requirements into technical verification; EU AI Act conformity assessment as a case study

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S1, S6
**Concepts:** [[05_Concepts/05_Concepts_Signature/Governance_Debt]], [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Transparency]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Corpus nodes:** [[07_Institutions/Corpus/International/International_18_UNESCO_Recommendation_Ethics_AI_2021]] (UNESCO — cited as normative source), [[04_Knowledge_Products/Wiki_Intake/International_12_HCJP_Legal_AI_BFSI_2025]] (EU AI Act BFSI analysis), [[07_Institutions/Corpus/SEBI/SEBI_14]] (India accountability obligation needing verification framework), [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] (Seven Sutras mapping to 11 macro-categories), [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] (India's operative audit infrastructure)
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes
- [ ] Marked processed

---

## Log

- 2026-06-18: Intake note created. Batch 12. Cowork session. Source: `/Users/vivek/Documents/LinkedIn/Policy Dump Future/ASSESSING_HIGH_RISK_ARTIFICIAL_INTELLIGENCE_1764937709.pdf`. File unreadable via bash (mount deadlock); note written from arXiv abstract page (arxiv.org/abs/2512.13907) and paper HTML versions. ⚠ VERIFY — confirm peer-review venue (v3 revised April 2026; check whether accepted to conference/journal by date of citation). File size in vault (2.6MB) is consistent with full-length academic paper including appendices.
