---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - source/practitioner-deck
  - content/wiki-entry
  - gate/open
  - section/S5
  - section/S6
  - topic/agentic-ai-threats
  - topic/vulnerability-management
  - topic/cybersecurity
  - paper/p3
  - paper/p4
---

# Preventing AI-Assisted/Led Cyber Attacks: A Field Guide to Reducing Exposure and Building Cyber Resilience in the Age of Agentic AI Threats (Joshi, 2026) — Intake Note

**Source:** Col. Deepak Joshi (Retd.), CISO Lead & Principal — ISC2 Chapter keynote / CISO webinar briefing
**Year:** 2026
**File ID:** F140
**Zotero key:** [leave blank — to be added manually]
**Wiki section(s):** S5 (Data, Privacy & Security — threat landscape), S6 (Implementation & Governance Artifacts)
**Confidence:** Medium — practitioner keynote deck synthesising named regulatory instruments (verifiable independently) with the author's own operating-model and metrics framework (not independently verifiable)
**Jurisdiction:** India-primary (CERT-In, RBI, SEBI, IRDAI), with a global-framework baseline (EU AI Act, NIST AI RMF, ISO/IEC 42001, OWASP LLM Top 10, MITRE ATLAS)

---

## Classification

**Document type:** Conference/webinar keynote deck (24 slides), practitioner-authored, not peer-reviewed or regulator-issued
**Primary audience:** CISOs, board members, security leadership ("board-ready narrative" is explicit session framing)
**AI explicit:** Yes — entire deck is organised around AI-accelerated/AI-led cyber threats
**PRIS role:** Secondary synthesis of four Indian regulatory instruments already in the corpus, plus an independently reusable practitioner operating model (12 defensive principles, phased implementation roadmap, AI Exposure Management scope definition)

---

## Value and limits of this document

This deck's principal value to PRIS is **consolidation, not new primary content**: it names and dates four Indian regulator AI-cyber instruments already present in the vault, in one place, with a synthesis claim about their convergence. Its secondary value is a genuinely independent practitioner framework — an "AI Exposure Management" operating model that extends CVE-based vulnerability management to non-CVE AI risk surfaces (models, training/inference data, prompts, APIs/vector databases, autonomous agents).

It should **not** be cited for provision-level regulatory detail — where it summarises a named instrument, go to the corpus node it maps to, not this deck.

---

## Regulatory Instruments Named — Cross-Reference to Existing Corpus Nodes

| Named in deck | Vault node | Match confidence |
|---|---|---|
| "CERT-In Blueprint (V1.0, 25.05.2026)" — 38-page implementation blueprint for AI-driven cyber risk | [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] | High — version and date match |
| "AI-Accelerated Cyber Threats advisory," RBI, issued June 2026, mandating gap assessments | [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]] | High — name and month match; note RBI_9 is itself Tier C (primary text not obtained) in the vault, so this deck is a second secondary source on the same underlying advisory, not independent corroboration of its contents |
| "Advisory on Emerging Advanced Artificial Intelligence (AI) Tools for Vulnerability Detection," SEBI, issued May 2026 | [[07_Institutions/Corpus/SEBI/SEBI_18_AI_Vulnerability_Detection_Advisory_2026]] | High — title and month match |
| IRDAI Working Group on AI Governance (WG-AI), Office Order dated 17 June 2026, chaired by Prof. Sandeep K. Shukla (IIIT Hyderabad) | [[07_Institutions/Corpus/IRDAI/IRDAI_2_Working_Group_AI_Governance_2026]] | High — date and chair name match |

**Reusable finding:** independent confirmation (from a practitioner source outside the vault's own Perplexity/NotebookLM intake pipeline) that these four instruments cluster within a roughly six-week window (April–June 2026), consistent with the "coordination by common shock" reading already recorded at RBI_9 §S5.2 (the Mythos-class threat as a shared exogenous trigger). This deck independently supports that reading without having been built to make that argument — a useful corroboration from a differently-motivated source.

---

## Reusable Findings

1. **AI Exposure Management scope (feeds S6).** The deck defines a five-part non-CVE AI attack surface — models/fine-tunes, training/inference datasets, prompts/system instructions, APIs/vector databases, autonomous agents/tool access — and argues traditional CVE-based vulnerability management structurally misses all five. Directly reusable as a scoping checklist independent of the deck's regulatory claims.

2. **Convergence claim across four Indian regulators (feeds S2/S5).** The deck's own synthesis: "One Program, Not Three Reports — A single AI-aware VM program satisfies all three [CERT-In/RBI/SEBI] regulators — and travels internationally," framed against a stated "Unified Regulatory Direction" claim that India's approach mirrors NIST AI RMF, ISO/IEC 42001 and the EU AI Act. This is a compliance-efficiency argument for [[05_Concepts/05_Concepts_Signature/Governance_Debt]] — a practitioner asserting that duplication *can* be resolved operationally even where the underlying instruments are not formally coordinated. Treat as an industry claim to be weighed against, not a substitute for, the vault's own parallelism findings (e.g. RBI_8/RBI_9's intra-regulator split).

3. **CERT-In risk-based remediation clock (feeds S5).** Reported indicative timelines: known-exploited/internet-facing vulnerabilities ≤ 12 hours; critical externally-exposed ≤ 1 day; critical internal (high-value) ≤ 3 days; high-severity ≤ 5 days. Consistent in register with CERT-In's six-hour incident-reporting clock already recorded elsewhere in the corpus (RBI_8 §S4, para 182) but is a distinct, patch-timeline obligation, not the same clock. ⚠ Verify against CERT_In_3 primary text before citing these specific hour/day figures.

4. **"RBI Model Risk Governance Architecture" slides — provenance uncertain.** Slides 11–15 present a detailed RBI model-risk framework (three-lines-of-defense execution, risk-tiering, 10-year model-inventory retention, explainability/bias/drift controls, prompt-injection safeguards, kill-switch requirements) cited to "RBI Guidance DOR.ORG.REC.XXXX/2026-27." The circular number is a literal unfilled placeholder ("XXXX") in the source deck. **Do not treat this content as a confirmed instrument** — see VERIFY flag below.

5. **Board-facing metrics reframe (feeds S1/S6).** Proposes MTTR-on-critical-exposures, unresolved-critical-findings-on-customer-facing-platforms, a composite "AI Risk Score," and exposure-window duration as board-relevant metrics, explicitly rejecting raw CVSS/vulnerability counts as insufficient for board reporting. Reusable as a board-reporting template independent of its regulatory sourcing.

---

## Citation Hygiene

| Flag | Issue | Handling |
|---|---|---|
| **Unfilled placeholder citation** | The "RBI Model Risk Governance Architecture" content (slides 11–15) is attributed to "RBI Guidance DOR.ORG.REC.XXXX/2026-27" — an unfilled template circular number | Treat this content as **unconfirmed / possibly illustrative or drafted-ahead-of-issuance** material, not a verified RBI instrument, until a real circular number is located. Do not cite the specific control requirements (10-year inventory rule, RMCB approval SLAs, etc.) as binding RBI text without independent confirmation |
| **Secondary-on-secondary** | RBI_9 content in this deck is itself downstream of KPMG/Business Standard reporting already flagged Tier C in the vault | Do not use this deck to upgrade RBI_9's tier — it adds no new primary-source confirmation |
| **No named organisational affiliation for figures cited** | "5 perfect phishing emails in 5 minutes by AI vs 16 hours by humans" and similar statistics are presented without a named study or source | Treat as illustrative/anecdotal, not citable empirical findings |

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The AI Exposure Management scope definition (models/data/prompts/APIs/agents) and the phased 0–7/8–30/31–60-day implementation roadmap are both directly usable as a client-facing maturity-assessment starting template for AEGIS_OS or PrivacyWeave engagements without further sourcing work.
**Consulting connections:** AEGIS_OS (runtime enforcement — AI Exposure Management scope overlaps directly with AEGIS_OS's authority-binding and kill-switch positioning)
**Teaching connection:** Usable as a case-study slide set for an IIM-K "AI Risk Stack" session on board-level metrics reframing (finding 5 above)

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S5, S6
**Concepts:** [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] | [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]
**Corpus nodes:** [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] | [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]] | [[07_Institutions/Corpus/SEBI/SEBI_18_AI_Vulnerability_Detection_Advisory_2026]] | [[07_Institutions/Corpus/IRDAI/IRDAI_2_Working_Group_AI_Governance_2026]]
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] | [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]]
**Projects:** [[02_Projects/P3_BFSI_JEIM]] (indirect — corroborates the intra/cross-regulator clustering finding), [[02_Projects/P4_Doctrinal_IJLIT]]

---

## VERIFY Flags

**#306 (MEDIUM) — RBI Model Risk Governance Architecture provenance.** Slides 11–15 cite "RBI Guidance DOR.ORG.REC.XXXX/2026-27" with a literal placeholder circular number. Locate the actual instrument (if one exists) before citing any of the specific controls described (10-year model-inventory retention, RMCB approval SLAs, explainability/bias thresholds) as confirmed RBI text. Until resolved, treat as unconfirmed.

**#307 (LOW) — CERT-In remediation-clock figures.** The ≤12h/≤1d/≤3d/≤5d risk-based patch timeline is attributed to "CERT-In Blueprint V1.0, 25.05.2026." Cross-check against the primary text of [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] before citing the specific hour/day figures in publication-track output.

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [x] Linked to concept notes
- [ ] Marked processed

---

## Log

- 2026-08-09: Intake note created via Cowork corpus intake session (Desktop-folder ad hoc batch). Pre-flight duplicate check found no existing node for this deck or author. Four named regulatory instruments cross-referenced to existing corpus nodes with high confidence. One unfilled-placeholder citation identified and flagged (#306). Not yet added to `Corpus_Index_MOC.md` batch table.
