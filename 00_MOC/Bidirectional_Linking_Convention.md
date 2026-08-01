---
type: MOC
tags:
  - type/convention
  - status/active
  - engine/phd
---

# Bidirectional Linking Convention — PRIS Vault

**Status:** Active | **Established:** 2026-06-14 | **Applies to:** All corpus intake batches (Batches 1–3 retrofitted; Batches 4–11 onward apply at creation time)

---

## Why this exists

Corpus nodes (Format A) link **outward** to concepts, projects, institutions, frameworks, and knowledge products via their "Connections" section. Without a corresponding **inward** link, those concept/project pages have no record of which corpus evidence supports them — the vault's value as a compounding research tool depends on this being bidirectional. This convention closes that gap and makes it a standing step, not a one-off cleanup.

---

## The Rule

**Whenever a corpus node is created or edited, and its "Connections" section names a concept, project, institution-MOC table, or knowledge product, the corresponding inward reference must be added in the same session.** Specifically:

### 1. Corpus Index MOC (always)
Add a row to [[Corpus_Index_MOC]] master table: Node | Title | Institution | Wiki Section | Tier | Key Concepts | Key Projects | ⚠VERIFY. Also update the "By Wiki Section" and "By Project" tables.

### 2. Concept files — "Instances in Corpus" section
Every signature concept ([[Regulatory_Parallelism]], [[Governance_Debt]], [[Institutional_Coherence]]) and any standard concept the node cites must have an **"Instances in Corpus"** section (new — added 2026-06-14) listing:
- The corpus node (wikilink)
- One-line statement of what the node contributes as evidence/instance of the concept

This section sits between "Empirical Evidence Base"/"Empirical Application" and "Appears In". Do not duplicate "Appears In" (which lists *papers/projects* the concept appears in) — "Instances in Corpus" lists *primary-source documents* that instantiate the concept.

### 3. Institution MOC — Research Corpus Mapping table
If the node's institution is not yet a row in `_Institutions_MOC.md`'s Research Corpus Mapping table (e.g. International, NITI Aayog), add it, with a pointer to [[Corpus_Index_MOC]] for node-level detail rather than duplicating all nodes inline.

### 4. Concept MOC — Cross-Concept Applications table
If the node produces a *specific finding* (not just a citation) relevant to a concept's cross-paper application (e.g. the MeitY_2 ← RBI_FREE_AI_2025 sutra lineage as Institutional Coherence evidence), add/extend the relevant cell in `_Concepts_MOC.md`'s Cross-Concept Applications table with a short pointer to the corpus node.

### 5. ⚠VERIFY flags
Any new ⚠VERIFY flag raised in a corpus node must also be added to the consolidated tracker in [[Corpus_Index_MOC]].

---

## What this convention does NOT require

- Project state files (P1–P4, fsQCA) do not need a full "Evidence Inventory" rebuild per batch — the [[Corpus_Index_MOC]] "By Project" table is the single source of truth for which corpus nodes are candidate evidence. Project files can reference [[Corpus_Index_MOC]] rather than maintaining their own duplicate list.
- Outbound links from corpus nodes (Connections section) are unchanged — this convention only adds the inward direction.

---

## Retrofit status (Batches 1–3, 2026-06-14)

- ✅ [[Corpus_Index_MOC]] created with all 12 nodes, indexed by Wiki section and project.
- ✅ "Instances in Corpus" sections added to [[Regulatory_Parallelism]], [[Governance_Debt]], [[Institutional_Coherence]], [[Governance_Capacity]].
- ✅ `_Institutions_MOC.md` Research Corpus Mapping extended (International, NITI Aayog rows added; pointer to Corpus_Index_MOC).
- ✅ `_Concepts_MOC.md` Cross-Concept Applications extended with MeitY_2 ↔ RBI_FREE_AI_2025 sutra-lineage finding and International_3 ↔ RBI_FREE_AI_2025 parallelism finding.
- ✅ Consolidated ⚠VERIFY tracker established in [[Corpus_Index_MOC]] (8 flags).

## Going forward (Batches 4–11)

Apply steps 1–5 above at the end of each batch (not per-node, to avoid redundant MOC edits) — i.e., write all nodes in the batch first, then run a single "indexing pass" updating Corpus_Index_MOC, concept Instances-in-Corpus sections, and MOC tables before closing the session. This mirrors the Batch 1–3 retrofit pattern and keeps the indexing pass itself a discrete, checkpointable step.

---

_Back to [[Corpus_Index_MOC]] | [[PRIS_Master_MOC]]_
