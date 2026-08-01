---
type: MOC
status: active
last_updated: 2026-06-19
tags:
  - type/convention
  - status/active
  - engine/phd
---

# PRIS Workflow Discipline Protocol (WDP)

**Authoritative Operational Guide for Preventing Ontology Inflation and Enforcing Compounding Productivity**  
*Owner: Vivek Vaidyanathan & AI Co-working Agents | Status: ACTIVE | Established: 2026-06-19 | Version: 2.0*

---

## 1. The Threat: Ontology Inflation

PRIS is a high-yield research, advisory, and intelligence engine. Its biggest threat is not technical failure, but **ontology inflation**: the uncontrolled proliferation of low-synthesis notes, redundant aliases, and weak pathways. When the cognitive cost of navigating the vault exceeds the value of its insights, PRIS degrades from an intellectual compounder into a digital document dump.

To prevent this, the vault enforces **Ruthless Utility**: every single note must directly support at least one of the **Five Output Pockets**:
1. **Research (R):** Supports an active project (`02_Projects/P1-P5`) or the doctoral thesis.
2. **Consulting (C):** Feeds active or pending advisory inbounds (`10_Consulting/`).
3. **Teaching (T):** Populates a module, case study, or syllabus structure (`09_Teaching/`).
4. **Thought Leadership (TL):** Sources content briefs, LinkedIn carousels, or articles (`11_Content/`).
5. **Knowledge Products (KP):** Directly updates the `AI_Governance_Wiki.md` or handbooks (`04_Knowledge_Products/`).

If a note cannot be mapped to at least one of these pockets, **it must not be created**.

---

## 2. Core Operational Loop

To maintain structural integrity and intellectual compound interest, all sessions (solo and co-working) must strictly adhere to the following workflow-enforced disciplines.

```
       [ Intake / Entry ]
                 ↓
      ┌────────────────────────┐
      │ UPDATE BEFORE CREATE   │ ──► [Search-First Ingestion Matrix]
      └────────────────────────┘
                 ↓
      ┌────────────────────────┐
      │   CONCEPT DISCIPLINE   │ ──► [The Three-Instance Gate]
      └────────────────────────┘
                 ↓
      ┌────────────────────────┐
      │     LINK DISCIPLINE    │ ──► [Two-Way Transit & Contextualisation]
      └────────────────────────┘
                 ↓
      ┌────────────────────────┐
      │  TIERED CLOSE-OUT      │ ──► [L1/L2/L3 Exit Protocols]
      └────────────────────────┘
                 ↓
         [ Compounded Vault ]
```

---

## 3. The "Update Before Create" (UBC) Doctrine

Knowledge base maturity is marked by depth, not file count. The **"Update Before Create" (UBC)** doctrine dictates that agents must never blindly create a new Markdown file when existing files can be enriched. This preserves "link equity" and ensures that new raw data acts as an incremental layer of paint on top of existing knowledge, rather than starting a new canvas every time.

Before executing any file-creation tool, the agent MUST search the vault to determine where the new data fits within the existing structure.

### Search-First Ingestion Decision Tree

| Inbound Data Type           | Vault State                                   | Required Action                                                                                                                  | Target Destination                    |
| :-------------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------ |
| **Concept or Construct**    | Concept exists under similar name/typo        | **Update & Merge:** Do NOT create a duplicate. Update the existing standard or signature concept note and add new citations.     | `05_Concepts/`                        |
| **Concept or Construct**    | Concept is new but has <3 citations in corpus | **Staged Inline:** Do NOT create a standalone note. Stage the concept inline within the most relevant Domain note or parent MOC. | `03_Domains/` or `00_MOC/`            |
| **Regulatory Instrument**   | Node exists as a draft, template, or shell    | **Populate & Extend:** Enrich the existing node with full analytical classification and substantive content.                     | `07_Institutions/Corpus/`             |
| **Regulatory Instrument**   | Document is entirely new to the vault         | **Create New Node:** Generate a new Format A Corpus Node using the correct sequential institutional ID.                          | `07_Institutions/Corpus/[regulator]/` |
| **External Report / Paper** | Document is entirely new to the vault         | **Create Wiki Intake Note:** Generate a Format B Note to capture findings, linking them to S1–S8 of the Wiki.                    | `04_Knowledge_Products/Wiki_Intake/`  |

---

## 4. Link Discipline Workflow (LDW)

**Objective:** Prevent weak, unnavigable, or "blind" links that fragment the knowledge graph.

### LDW-1: The Contextualised Link Mandate
Never insert a bare wikilink (e.g., `- [[Note_Name]]`) in a note's body. Every link must be wrapped in a brief clause explaining the *nature of the relationship* or *analytical relevance*.
*   *Bad:* `This is relevant to [[Regulatory_Parallelism]].`
*   *Good:* `This independent oversight mechanism instantiates [[Regulatory_Parallelism]], as it overlaps directly with SEBI's reporting thresholds without citing them.`

### LDW-2: The Two-Way Transit Rule
Whenever Note A links to Note B, you must transit to Note B and establish the corresponding **inward link** to maintain bidirectional integrity.
*   For **Corpus Nodes (Format A)**: Outbound links in the "Connections" section must be immediately mirrored in the cited Concept's "Instances in Corpus" section, the relevant Institution MOC, and [[Corpus_Index_MOC]].
*   For **Concepts/Frameworks**: When linking a Concept to a Framework, update the Framework's "Linked Concepts" section and the Concept's "Empirical Application" section.

### LDW-3: Index-First Registration
No orphan notes are permitted. A new note must be registered in its parent Map of Content (MOC) or index file *before* the session is closed.
*   Corpus nodes → [[Corpus_Index_MOC]]
*   Wiki intake notes → [[Wiki_Intake_Index]]
*   Concepts → [[_Concepts_MOC]]
*   Frameworks → [[_Frameworks_MOC]]

---

## 5. Concept Discipline Workflow (CDW)

**Objective:** Protect the analytical primacy of PRIS Signature Constructs ([[Regulatory_Parallelism]], [[Governance_Debt]], [[Institutional_Coherence]]) from being diluted by standard or redundant concepts.

### CDW-1: The "Three-Instance" Gate
You are forbidden from creating a new standalone note in `05_Concepts/` unless it meets one of the two **Concept Entry Criteria**:
1.  **Empirical Prevalence:** The concept is observed and explicitly extracted from at least **three distinct primary-source documents (corpus nodes)** in the vault.
2.  **Theoretical Load-bearing:** The concept serves as an explicit theoretical lens or independent/dependent variable in an active research paper (`P1–P5`) or the thesis chapter.

### CDW-2: Inline Staging Protocol
If a concept is valuable but does not yet clear the "Three-Instance" Gate, it must be staged inline.
*   **Where to stage:** In the "Scope and Boundary" or "Core Synthesis" section of the most relevant Domain note (e.g., `03_Domains/AI_Governance.md`) or as an inline tag (e.g., `#concept-candidate/algorithmic-impact-assessment`).
*   **When to elevate:** During periodic indexing passes, scan staged concepts. If a staged concept reaches 3 corpus citations, elevate it to a standard concept note using `99_System_Templates/Concept_Template.md`.

### CDW-3: Signature Centring Rule
Every Standard Concept note (`05_Concepts_Standard/`) must contain an explicit section titled **"Intersection with Signature Constructs"**. This section must define how the standard concept interacts with, feeds, or is governed by:
*   [[Regulatory_Parallelism]]
*   [[Governance_Debt]]
*   [[Institutional_Coherence]]

This maintains a self-reinforcing conceptual hierarchy and prevents standard concepts from becoming isolated, low-synthesis islands.

---

## 6. Tiered Close-Out Discipline Workflow (COW)

**Objective:** Ensure no session ends in an unresolved state, leaving behind raw data, unlinked files, or cognitive friction for the next session.

Close-out requirements scale with the depth of the session. Rather than forcing a heavy, one-size-fits-all administrative burden, PRIS operates a **Tiered Close-out Architecture**.

### Tiered Close-out Architecture

| Close-out Level | Session Trigger | Exit Buffer | Required Deliverables & Operations |
| :--- | :--- | :--- | :--- |
| **Tier 1 (L1) - Micro** | Minor text edits, typo fixes, or simple property updates. | **3 Minutes** | 1. Run YAML frontmatter check.<br>2. Confirm file save and exit. |
| **Tier 2 (L2) - Standard** | Active drafting of sections or ingesting 1–3 new corpus nodes. | **15 Minutes** | 1. Apply the **Two-Way Transit Rule** (LDW-2) for all touched files.<br>2. Register new files in parent MOC or index (LDW-3).<br>3. Generate a standardized session handoff note in `00_MOC/` indicating files written, deferred items, and next available IDs. |
| **Tier 3 (L3) - Deep** | Completing a full PDF batch (e.g., Batch 12), making structural ontology changes, or resolving critical verification flags. | **30 Minutes** | 1. Perform all **L2** checks and operations.<br>2. Execute a full indexing pass: update individual concept files' "Instances in Corpus" sections.<br>3. Update `Decision_Journal.md` if any architectural or boundary decisions were made.<br>4. Update the vault-wide sequential numbering state in the handoff note.<br>5. Append key learnings or instructions to `gemini-scribe/AGENTS.md` to update agent memory. |

---

## 7. The Five-Pocket Utility Audit Checklist

Use this checklist when creating any note to enforce the **Ruthless Utility** doctrine:

| Pocket | Target File / Section | Verification Rule | Checked |
|---|---|---|---|
| 🔴 **Research** | `02_Projects/P[1-5]` or `Thesis_Architecture` | Does this note provide direct empirical evidence or theoretical scaffolding for an active paper? | [ ] |
| 🟡 **Consulting** | `10_Consulting/[Client]_Inbound` | Does this note directly address a technical or regulatory question raised by an active/pending inbound? | [ ] |
| 🟢 **Teaching** | `09_Teaching/[Module]` | Does this note supply a concrete case study, regulatory timeline, or slide-deck content? | [ ] |
| 🔵 **Thought Leadership** | `11_Content/[Brief]` | Does this note contain a highly citable statistic, convergent pattern, or tension suitable for a LinkedIn post? | [ ] |
| 🟣 **Knowledge Product** | `04_Knowledge_Products/AI_Governance_Wiki` | Does this note fill an identified coverage gap in the Wiki or Handbook? | [ ] |

*If all boxes are blank, do not write the note. Keep the source data in Zotero or NVivo.*

---

## 8. Change Control and Integration

This protocol is a living system integrated into:
- `04_Knowledge_Products/Wiki_Intake/PRIS_Cowork_Context.md` (Section 9 & 10)
- `00_MOC/PRIS_Master_MOC.md` (Strategic Layer)
- `00_MOC/Bidirectional_Linking_Convention.md`

Changes to this protocol must be logged as a Decision Journal entry and updated here with a version increment.

**Version:** 2.0  
**Established:** 2026-06-19  
**Change Log:** DJ-08 (WDP rewrite to lighter, robust operating doctrine with UBC and Tiered COW)  

---

*Back to [[PRIS_Master_MOC]] | [[PRIS_Master_Ontology_v2]]*