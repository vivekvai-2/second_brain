---
type: Session Handoff
status: archived
last_updated: 2026-07-21
tags:
  - type/session-handoff
  - status/archived
  - engine/phd
---

# Session Handoff — NotebookLM Ingestion Pipeline, 2026-07-15

**Scope:** This is a pipeline handoff, not a batch handoff. It documents how to process documents the user runs through NotebookLM (extraction relay, PROMPT 0b) and pastes into a PRIS session — a workflow added *after* `Session_Handoff_Cowork_20260614.md` (which covers the Batch 1–3 PDF-direct pipeline and the Batch 4–11 plan). Read that file first for vault structure/numbering baseline; read this file for the NotebookLM-specific ingestion steps.

---

## What PROMPT 0b is

`04_Knowledge_Products/Wiki_Intake/PRIS_Corpus_Intake_Prompts.md` (v1.2) contains PROMPT 0b — a NotebookLM-scoped variant of the original PROMPT 0 (Gemini Extraction Relay). The user runs a single source through NotebookLM with an instruction to extract, using ONLY that named source, a 5-part structured output: Document Identity, TOC/Structure, Full Structured Content Extraction, Uncertain/Ambiguous Items, Out of Scope. NotebookLM's native inline citations are preserved. The user pastes this output directly into the session.

## Pipeline — follow in this order, every time

1. **Duplicate check before writing anything.** Search the vault by title, author/institution, and subject before assuming the pasted document is new. Check: `Corpus_Index_MOC.md` (by-node and by-institution tables), the relevant `07_Institutions/Corpus/[regulator]/` folder or `04_Knowledge_Products/Wiki_Intake/` for F-series files, and `_Institutions_MOC.md`. This step caught two false "new documents" this session (PwC TPRM was already F045; WEF/Capgemini was already F037) — treat every paste as a suspected duplicate until proven otherwise, not the reverse.
2. **If genuinely new:** classify Format A (Corpus Node — regulatory/institutional instrument) vs Format B (Wiki Intake Note — Big4/BigTech/academic), assign the next sequential number, write the full node per Section 7 of `PRIS_Cowork_Context.md`. Include a `## Log` entry recording the NotebookLM relay source and the duplicate-check result.
3. **If a duplicate is found:** read the existing node in full. Diff the new extraction against it — do not rewrite wholesale. Add only the delta, with inline `(added 2026-07-15, missed in original intake)`-style annotations so the provenance of each addition is traceable. Never recreate the node. Close the loop with a `## Log` entry describing what was added and why no new VERIFY numbers were needed (or which were).
4. **Indexing pass (mandatory, every document, no exceptions):**
   - `Corpus_Index_MOC.md` — update the by-section/by-project table row if new; add a dated log note if an enrichment; update the VERIFY flags table (new numbers) or note that existing flags already cover the uncertain items; update the vault numbering-state footer line.
   - Concept files' "Instances in Corpus" sections — add a new bullet for new nodes; for enrichments, only edit an existing bullet if the new content actually changes or strengthens the claim being made (e.g., a count changing from "three risks" to "five risks" must be corrected; a claim that remains accurate as originally written should be left alone rather than edited for the sake of it).
   - `_Institutions_MOC.md` / `_Concepts_MOC.md` — update if a new institution or concept linkage was introduced.
5. **Never skip step 1.** The cost of a missed duplicate (a second node needing a later merge) is higher than the cost of a dedup search that comes back empty.

---

## Documents processed via this pipeline this session

| Source | Outcome | Node | Notes |
|---|---|---|---|
| PwC Netherlands — *Navigating Third Party Risk Management in the Digital and Geopolitical Era* | Enrichment | F045 | Added full 7-author citation, Data Act/Product Liability Directive rows, Five Board Questions, Aggregation Risk definition, 5 case studies, 5 quotes. Closed a pre-existing [[Governance_Capacity]] backlink gap dating to 2026-06-19. |
| McKinsey Explainers — *What is an AI agent?* (March 2025) | New node | F074 | Confirmed not previously in vault (re-checked explicitly on user instruction). Five agent types, 4-step operational loop, $4.4T/Lenovo business-impact figures (⚠ #211, unverified McKinsey-asserted), 3 tech-architecture patterns. Flagged as foundational/business-case register, distinct from the technical agentic-AI security cluster (F036–F038, F070–F073). |
| WEF + Capgemini — *AI Agents in Action: Foundations for Evaluation and Governance* (Nov 2025) | Enrichment | F037 | Page count corrected ~48 → 34 (TOC-traced); 4 worked case studies + BFSI fraud-detection example (strengthens P3 relevance); precise 5-step risk assessment cycle; 9-mechanism Baseline Governance Table; multi-agent risks expanded 3→5; 5 key quotes incl. zero-trust cross-ref to F036. No new VERIFY numbers — existing V-B13-02/03/04 already covered the uncertain items. |

All three used the enrichment-not-recreation path except F074.

---

## Vault numbering state as of 2026-07-15 (ad hoc, pre-Batch 19)

- F-series → **F074** (next = **F075**)
- VERIFY → **#211** (next = **#212**)
- International / CERT-In / RBI / SEBI / MeitY / NITI series → unchanged from the 2026-06-14 handoff
- Batch marker unchanged at 16 ⊕s — this was ad hoc single-document processing, not a formal Batch 19 run. Batch 19 still opens at 17 ⊕s whenever it formally starts.

---

## Model selection guidance — can Haiku run this pipeline?

Split by step, not as a single yes/no:

**Suitable for Haiku:** mechanical, low-judgment sub-tasks — formatting a NotebookLM paste into the PROMPT 0b schema shape if it arrives slightly malformed; ticking Processing Status checkboxes; frontmatter field formatting; assigning the next sequential number once a classification decision has already been made by something else.

**Not recommended for Haiku — keep on Sonnet or Opus:** the two steps that actually carry risk in this pipeline are (1) the duplicate check and (2) deciding what in a new extraction changes an existing analytical claim versus what's cosmetic. Both failed silently would be expensive: a missed duplicate creates a second node needing a later merge (exactly the failure this session's step-1 discipline was built to catch — twice); an under-powered diff either misses genuine content gaps (leaving the node incomplete) or over-edits a concept file's "Instances in Corpus" bullet where the original claim was already accurate. The Format A/B classification call, the Analytical Notes synthesis, and the judgment about which concept-file bullets actually need editing are the parts of this pipeline doing real interpretive work, and that's where a lighter model is most likely to produce plausible-looking but wrong output — the kind of error that's hardest to catch on a skim, given the ABDC-A/academic-rigor bar this vault is held to.

**Net recommendation:** run the classify → enrich-or-create → index steps on Sonnet (or Opus for anything that will feed the P1–P4 publication pipeline directly). Haiku is fine as a cost-saver for the mechanical formatting/checklist steps only, if you want to split the pipeline that way — but it isn't a safe drop-in for the whole thing.

---

## Next session starting point

Continue accepting NotebookLM pastes one at a time through this pipeline. No batch is currently open — Batch 19 (formal, 8–10 documents from the remaining Policy Dump corpus) is still the next scheduled unit of work per the 2026-06-14 handoff, whenever the user is ready to move off ad hoc single-document processing.
