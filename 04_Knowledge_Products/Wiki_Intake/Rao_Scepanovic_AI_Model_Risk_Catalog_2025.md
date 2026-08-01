---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - engine/phd
  - theme/ai-risk-taxonomy
  - theme/model-cards
  - theme/empirical-ai-governance
---

# Rao, Šćepanović, Jayagopi, Cherubini & Quercia (2025) — The AI Model Risk Catalog: What Developers and Researchers Miss About Real-World AI Harms

**Source:** Pooja S. B. Rao (Univ. Lausanne / IIIT Bangalore), Sanja Šćepanović (Nokia Bell Labs / Univ. Oxford), Dinesh Babu Jayagopi (IIIT Bangalore), Mauro Cherubini (Univ. Lausanne), Daniele Quercia (Nokia Bell Labs / Politecnico di Torino)
**Year:** 2025 (arXiv preprint 21 Aug 2025, arXiv:2508.16672v1 [cs.CY]; AAAI 2025 copyright notice)
**Full title:** "The AI Model Risk Catalog: What Developers and Researchers Miss About Real-World AI Harms"
**File ID:** F024
**Zotero key:** ⚠ VERIFY — not yet assigned
**Wiki section(s):** S6 (Model Risk) / S3 (AI Risk Taxonomies & Classification) / S1 (Governance Fundamentals — risk reporting standards)
**Confidence:** High (AAAI-affiliated, large-scale empirical study; co-authors include IIIT Bangalore — India-affiliated institution — and Nokia Bell Labs)
**Jurisdiction:** Global (HuggingFace model card corpus, no jurisdiction-specific framing; IIIT Bangalore co-authorship gives partial India research-ecosystem relevance)

---

## Classification

Large-scale empirical/computational study (LLM-assisted content analysis of ~460,000 AI model cards from HuggingFace) building the **AI Model Risk Catalog** (2,863 categorized risks from 2,672 model cards) and comparing developer-reported risks against the **MIT AI Risk Repository** (967 researcher-identified risks) and the **AI Incident Database** (869 real-world harms, 4,406 media reports). Not a regulatory/governance-instrument node — Format B Wiki Intake Note, primarily an **empirical risk-taxonomy/classification source** (S3) with direct implications for risk-reporting standards (S1) and model-risk documentation practice (S6).

---

## Reusable Findings

1. **Three-way "risk perception gap" between developers, researchers, and real-world harms (feeds S3/S1):** Developers over-index on technical/capability risks (AI system safety, failures & limitations = 37% of catalog entries; discrimination & toxicity = 44%), researchers over-index on systemic/societal risks (socioeconomic & environmental = 18% of MIT Repository vs. only 4% of real-world incidents), while **malicious use and misinformation — the largest categories of actual recorded harms (22% and 13% respectively)** — are underrepresented in both developer (4%/10%) and researcher (17%/6%) sources. This three-way divergence is a **directly reusable empirical baseline** for arguing that AI governance frameworks built on developer self-disclosure (model cards) or academic taxonomies alone will systematically under-govern fraud/manipulation/social-engineering risks — a finding with direct relevance to RBI/SEBI consumer-protection-oriented AI governance circulars that emphasize fraud and mis-selling.

2. **Documentation-quality decline despite growth (feeds S1/Governance_Debt):** Between the 2022 and 2024 HuggingFace snapshots, the proportion of model cards with *any* completed risk section **fell from 17% to 14%**, and unique (non-duplicated/non-templated) risk content fell to under 1% of all cards. 85% of cards with "risk sections" in 2024 contained no substantive information (mostly unedited templates). This is a strong empirical instance of [[Governance_Debt]]: voluntary disclosure regimes (model cards) do not self-improve with scale — directly relevant to debates on whether India's emerging AI-disclosure expectations (e.g., under DPDP-adjacent guidance or sectoral AI circulars) should rely on voluntary documentation vs. mandated structured risk cards.

3. **"Risk Card" / structured-format proposal as a transferable governance-instrument template (feeds S1/S6):** The paper explicitly calls for a **structured standard for defining and communicating AI risk** (situation + context + likelihood + severity), citing Derczynski et al. (2023) "Risk Cards" and Golpayegani et al. (2024) "AI Cards" (EU AI Act-inspired machine-readable risk documentation) as precedents. This is a **reusable comparator for evaluating RBI FREE-AI / SEBI AI disclosure templates**: do existing/proposed Indian regulatory disclosure formats meet the "situation + context" specificity bar this paper argues is necessary, or do they risk replicating the vague, templated, non-actionable risk language documented in HuggingFace model cards?

4. **Modality-shift risk profile (text → multimodal) as a forward-looking regulatory gap indicator (feeds S3/S6):** Non-text (image/audio/video/multimodal) inputs/outputs, while still a minority (9%/17% of risks respectively), show **disproportionately higher rates of malicious-use (14%) and privacy/security (13%) risk** compared to text-only models, and multimodal input grew from near-zero to 2% of the catalog between 2022 and 2024. This is a reusable "early warning" data point for [[Agentic_AI_Governance]] and any India-BFSI papers (P3) discussing generative/multimodal AI adoption — governance frameworks calibrated to text-based LLMs (most current Indian guidance) may already be lagging the actual risk distribution of deployed models.

5. **Methodological precedent: LLM-as-classifier with majority-voting validation (feeds S7/P1 methods, fsQCA data prep):** The paper validates GPT-4o-based risk extraction/classification against manual annotation (90% agreement on extraction; 83% accuracy / 81% macro-F1 on seven-class classification; majority-vote across 3 runs to reduce variance). This is a **directly reusable methodological precedent** for any LLM-assisted coding step in Vivek's own corpus work (e.g., NVivo-adjacent automated theme classification for the AI Governance SLR or fsQCA condition-coding) — provides a citable benchmark for "what level of LLM-classification accuracy is considered acceptable" in a 2025 AAAI-track paper.

---

## Consulting / Teaching Reuse

- The **three-way Venn-style gap (developers vs. researchers vs. real-world harms)** is a strong visual/talking point for CISO/CRO board briefings: "the people building the model, the people studying AI risk in the abstract, and the actual incidents that occur are all looking at different things — your governance function must explicitly cover the gap, especially fraud/social-engineering."
- The **documentation-decline-despite-scale finding (17%→14%)** is a reusable cautionary data point when advising clients that "self-certification" or "voluntary disclosure" approaches to AI risk reporting tend to degrade, not improve, with adoption scale — supports arguments for mandated structured disclosure (AI Cards / Risk Cards) in India BFSI AI governance consulting.
- The **fraud/social-engineering blind-spot finding** is directly reusable in practitioner content on agentic AI risk (P4) — both developers and academic researchers under-weight the single largest category of real-world AI harm.

---

## Cross-Links

- [[04_Knowledge_Products/Wiki_Intake/Tammenga_AI_3LoD_Banks_2020]] (F021) — Tammenga's "no AI in 3rd line" 2020 finding and this paper's 2025 finding that risk *documentation* itself is deteriorating could be read together as a longitudinal "governance lag" narrative for AI/ML oversight.
- [[04_Knowledge_Products/Wiki_Intake/Kurshan_Shen_Chen_AI_Model_Governance_2020]] (F013) — Kurshan et al.'s "continuous monitoring/reporting module" proposal (Capability 1) is a potential *solution* to the documentation-decline problem this paper diagnoses empirically five years later.
- [[Governance_Debt]] — documentation-quality decline despite scale is a clean empirical instance of governance debt accumulating in a voluntary-disclosure regime.
- [[Institutional_Coherence]] — the three-way divergence (developer/researcher/real-world) as a coherence gap between self-regulatory disclosure, academic risk taxonomies, and lived/regulatory experience of harm.
- [[Agentic_AI_Governance]] — multimodal/agentic risk-profile shift (malicious use, privacy/security rising with multimodality) as an early-warning indicator.
- [[P1_SLR_RG]] — LLM-as-classifier validation methodology (majority voting, accuracy/F1 benchmarks) as a citable precedent for automated coding steps.

---

## ⚠ VERIFY BEFORE PUBLISHING

- Zotero key not yet assigned — add on next Zotero sync.
- Publication status: paper carries an AAAI 2025 copyright notice but is distributed as an arXiv preprint (2508.16672v1, dated 21 Aug 2025); confirm final venue/proceedings citation (AAAI conference track vs. workshop) before using in formal citation lists.
- IIIT Bangalore co-authorship (Pooja S. B. Rao, Dinesh Babu Jayagopi) gives a thin India-research-ecosystem link, but the study itself is not India-specific — do not over-claim India relevance beyond the general applicability of findings.

---

## Processing Status

- [x] PDF read in full (26 pages incl. appendix figures and prompts)
- [x] Classified — Format B, Wiki Intake Note
- [x] Reusable findings extracted (5)
- [x] Cross-links identified
- [ ] Indexing pass (Corpus_Index_MOC, Instances in Corpus) — pending, end of Batch 6

---

## Log

- 2026-06-14: Processed as F024, Batch 6. Selected from raw corpus (AI Model Risk Catalog theme); confirmed not a duplicate of any existing corpus node — first risk-taxonomy/empirical-classification paper in the corpus.

---

_Back to [[Corpus_Index_MOC]] | [[PRIS_Master_MOC]]_
