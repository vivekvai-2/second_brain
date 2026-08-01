---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - topic/ai-fairness
  - topic/llm-bias
  - topic/agentic-ai-governance
  - institution/cerai-iitm
---

# Where Should I Study? Biased Language Models Decide! — Intake Note

**Source:** Centre for Responsible AI (CeRAI), Wadhwani School of Data Science and AI, IIT Madras
**Year:** 2025 (exact date not stated; citations run through 2025)
**Full title:** Where Should I Study? Biased Language Models Decide! Evaluating Fairness in LMs for Academic Recommendations
**File ID:** F076
**Zotero key:** [blank]
**Wiki section(s):** S1 (Governance Fundamentals — bias/fairness evidence), S7 (Use Cases & Decision Stages — education AI; explicitly generalised to job and healthcare recommendation)
**Confidence:** High (peer-reviewed-style academic methodology paper; named authors and institutional affiliation; reproducible quantitative methodology with disclosed hyperparameters and compute)
**Jurisdiction:** Global (cross-national LLM evaluation; India-based research institution)

**Note:** This is very likely the previously iCloud-dataless `LLM CERAI.pdf` flagged in `Corpus_Index_MOC.md` as a high-value blocked file explicitly named to fill the wiki's stated **S4 institutional-coverage gap** ("All Batch C documents (CERAI, WEF, AWS, Microsoft, IBM)"). Content-wise the paper is an AI-fairness/bias measurement study rather than an agentic-governance framework, so it is indexed here primarily under S1/S7 — but it satisfies the CERAI-source coverage gap and should be treated as closing that line item.

---

## Classification

**Document type:** Academic Paper (empirical methodology + evaluation study)
**Primary audience:** Researcher / Practitioner (AI fairness auditors, LLM deployers in recommendation-system contexts)
**AI explicit:** Yes

---

## 3–5 Reusable Findings

1. **Systemic geographic/institutional bias in LLM academic recommendations** (feeds S1): Across three open-source LLMs (LLaMA-3.1-8B, Gemma-7B, Mistral-7B) and over 25,000 recommendations generated from 360 synthetic user profiles (40 nationalities × 3 economic classes × 3 genders), 52–80% of recommendations favoured institutions in the US and UK — direct quantitative evidence of geographic concentration bias in LLM-mediated decision-support outputs.

2. **Portable dual-metric fairness-audit framework (DRS/GRS)** (feeds S1, S6-adjacent): The paper introduces a Demographic Representation Score (weighted composite of socio-economic accessibility, institutional-reputation alignment, and academic-program alignment) and a Geographic Representation Score (geometric mean of normalised representation and reputational coverage). Both are explicitly designed as reusable, CI/CD-integrable fairness baselines — the authors recommend comparing new model versions against these scores before deployment.

3. **Economic-class and gender disparities within individual models** (feeds S1): Mistral's reputation-alignment score for low-economic-class profiles dropped 41% relative to baseline; LLaMA's composite fairness score for high-class profiles was 1.14× that of low-class profiles; Gemma's academic-alignment score for transgender user profiles collapsed to 0.35 — concrete, model-specific bias magnitudes usable as illustrative figures in practitioner briefings.

4. **Prompt-engineering is an insufficient governance control** (feeds S6): The paper's RQ3 test found that user-side prompt engineering (e.g., injecting regional-accessibility context) shifted recommendation distributions but did not eliminate systemic representational bias — evidence against treating prompt-level mitigation as a sufficient AI governance control for fairness-critical LLM deployments.

5. **Framework explicitly generalised to job and healthcare recommendation systems** (feeds S7): Appendix C adapts DRS/GRS to job-recommendation systems (commute/salary-band accessibility, employer-rating reputation, skill-Jaccard academic alignment) and healthcare-provider selection (travel time/insurance-network accessibility, patient-satisfaction reputation, specialty alignment) — directly extends this paper's bias-measurement methodology into the employment- and healthcare-discrimination harm vectors already documented in [[04_Knowledge_Products/Wiki_Intake/F039_ICAAD_KWM_AI_Harm_Human_Rights]]'s rights-harm mapping.

---

## Consulting / Teaching Reuse

**Highest-value reuse:** DRS/GRS as a portable, reproducible bias-audit metric pair directly usable in an AI-fairness-audit engagement scoping any LLM-based recommendation or decisioning system (HR screening, credit/insurance decisioning by the paper's own extension logic).
**Consulting connections:** None of the three named inbounds (AEGIS_OS, PrivacyWeave, CyberMesh) map directly; closest future fit is a BFSI/HR-tech AI-fairness-audit engagement.
**Teaching connection:** Strong case-study candidate — a concrete, quantified, reproducible LLM bias study suitable for an AI governance/ethics classroom module.

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S1, S7 (also closes the CERAI institutional-coverage line item under S4)
**Concepts:** [[05_Concepts/05_Concepts_Standard/Accountability]] (deployment-testing obligation implied by "compare against fairness baselines before deployment"), [[05_Concepts/05_Concepts_Standard/Transparency]] (disclosed methodology as a transparency model)
**Corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/F039_ICAAD_KWM_AI_Harm_Human_Rights]] (employment/healthcare rights-harm mapping — direct extension target per Appendix C)
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes
- [ ] Marked processed

---

## ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| #214 | Exact publication date not stated in source; citations run through 2025 implying a 2025 publication — verify via arXiv/IIT Madras CeRAI publication listing before using a precise date in formal citation | LOW |
| #215 | Contradictory total-generation counts: Section 4.4 states 21,600 total responses; Appendix A.2 states 32,400 (360 profiles × 3 prompts × 3 models × 10 runs — arithmetic supports 32,400). Likely a misprint or the 21,600 figure represents a subset — verify against the published/final version before citing a specific generation-count figure | MEDIUM |

---

## Log

- 2026-07-15: Wiki intake note created. NotebookLM extraction relay, PROMPT 0b. Ad hoc pre-Batch 19 session. Duplicate check run against "Where Should I Study," "Krithi Shailya," "Demographic Representation Score," "CeRAI" — no prior node match (only unrelated generic mentions of "CeRAI" elsewhere in the vault); confirmed new node. Likely resolves the previously iCloud-dataless `LLM CERAI.pdf` flagged as a high-value blocked file in `Corpus_Index_MOC.md`.
