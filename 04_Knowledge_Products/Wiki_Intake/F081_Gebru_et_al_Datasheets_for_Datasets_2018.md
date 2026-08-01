---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - topic/data-documentation
  - topic/data-governance
  - topic/transparency
  - institution/microsoft-research
---

# Datasheets for Datasets — Intake Note

**Source:** Gebru (Black in AI) + Microsoft Research cluster (Wortman Vaughan, Wallach, Daumé III, Crawford) + University of Washington (Morgenstern) + Cornell University (Vecchione) + University of Maryland (Daumé III)
**Year:** 2018 (arXiv draft posted 23 March 2018); later published *Communications of the ACM*, Vol. 64, No. 12, pp. 86–92, December 2021 (DOI 10.1145/3458723 — confirmed via prior Perplexity research pass in this session, resolving the extraction's own noted publication-venue ambiguity)
**Full title:** Datasheets for Datasets
**File ID:** F081
**Zotero key:** [blank]
**Wiki section(s):** S6 (Implementation & Governance Artifacts — primary), S5 (Data, Privacy & Security — secondary, GDPR intersection)
**Confidence:** High (foundational, widely-cited standard; CACM peer-reviewed final venue; DOI 10.1145/3458723)
**Jurisdiction:** Global (technical documentation standard, not jurisdiction-specific; GDPR discussed as an applicability example)

**Note:** Second of two papers deliberately sourced via a Perplexity Deep Research prompt to fill the vault's Domain III (AI Development Governance) documentation-standards gap identified in this session's AIGP BoK (F055) analysis. Companion: [[04_Knowledge_Products/Wiki_Intake/F080_Mitchell_et_al_Model_Cards_for_Model_Reporting_2019]] (Model Cards). Together these two papers are the primary sources behind the "System factsheet/model card, Datasheets" documentation-type taxonomy International_20 (Australia AIIA Tool) cites without naming its origin.

---

## Classification

**Document type:** Academic Paper (arXiv preprint → CACM journal article)
**Primary audience:** Researcher / Practitioner (dataset creators, ML engineers, data-governance/procurement reviewers)
**AI explicit:** Yes

---

## 3–5 Reusable Findings

1. **Seven-stage dataset-lifecycle documentation questionnaire** (feeds S6): Motivation, Composition, Collection Process, Preprocessing/Cleaning/Labeling, Uses, Distribution, Maintenance — the foundational data-documentation counterpart to Model Cards (F080). Together the two papers form a complete model+data documentation pair matching the AIGP BoK Domain III competency area ("data governance for AI: training data quality... data lineage").

2. **GDPR applicability guidance embedded in the Composition stage** (feeds S5): Recommends dataset creators take "a broad interpretation of whether a dataset relates to people" when assessing GDPR relevance — directly relevant to the vault's existing DPDP Act comparator work (MeitY_4) and a concrete practitioner heuristic not previously in the corpus.

3. **Multi-vendor adoption evidence** (feeds S6): By the paper's own account, Microsoft, Google, and IBM had begun piloting datasheets; Google published a follow-up "Data Cards" release alongside the Open Images dataset; IBM proposed "FactSheets"; the Data Nutrition Project and Partnership on AI incorporated the questions into their own documentation guidance — demonstrates this is an adopted practitioner standard across multiple Big Tech vendors already represented in the corpus ([[04_Knowledge_Products/Wiki_Intake/F035_Microsoft_Administering_Governing_Agents]], Google Cloud/Mandiant).

4. **Explicit non-sufficiency caveat** (feeds S1/S6): "Datasheets for datasets do not provide a complete solution to mitigating unwanted societal biases or potential risks or harms" — mirrors Model Cards' (F080) "one transparency tool among many" framing; both foundational documentation papers deliberately avoid overclaiming, a useful calibration precedent for wiki guidance language.

5. **Fully worked example datasheet (Appendix A)** (feeds S6): A complete datasheet for Pang & Lee's movie-review polarity dataset — funding disclosure (five distinct sources), sampling methodology (author caps, star-rating thresholds), and version history (v1.0/v1.1/v2.0, 1,400 → 2,000 instances) — directly usable as a teaching template alongside F080's two worked model cards.

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The seven-stage questionnaire is directly reusable as a data-governance/vendor-data-diligence checklist, completing the model+data documentation pair with F080 for any AI vendor-risk-assessment engagement.
**Consulting connections:** PrivacyWeave (direct — the GDPR/dataset-relates-to-people applicability guidance intersects with purpose-limitation assessment).
**Teaching connection:** The fully worked Pang & Lee example datasheet is strong, ready-to-use classroom material, paired with F080's worked model cards.

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S6, S5
**Concepts:** [[05_Concepts/05_Concepts_Standard/Transparency]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/F080_Mitchell_et_al_Model_Cards_for_Model_Reporting_2019]] (companion documentation-standard pair); [[07_Institutions/Corpus/International/International_20_Australia_DTA_AI_Impact_Assessment_Tool]] (cites datasheets as a documentation type — this node is the primary source that citation was missing); [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (GDPR/DPDP comparator relevance)
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes
- [ ] Marked processed

---

## Source Metadata

- **Access method:** NotebookLM extraction relay, PROMPT 0b
- **Publication-venue ambiguity:** the extraction itself flagged the final publication venue as unclear from the source text alone; this is resolved — the earlier Perplexity Deep Research pass in this session independently confirmed the CACM Dec 2021 final publication (Vol. 64, No. 12, pp. 86–92, DOI 10.1145/3458723). No new VERIFY flag required.

---

## Log

- 2026-07-15: Wiki intake note created. NotebookLM extraction relay, PROMPT 0b. Ad hoc pre-Batch 19 session. Second of two papers sourced via Perplexity Deep Research to fill the S6/Domain III model+data documentation-standards gap identified in this session's AIGP BoK (F055) analysis. Duplicate check run against "Datasheets for Datasets," "Gebru," "Pang and Lee" — no prior match; confirmed new node.
