---
type: Ontology
status: active
last_updated: 2026-06-14
tags:
  - type/ontology
  - status/frozen
  - engine/phd
---

# PRIS Master Ontology — v2.0 (Frozen)

**Personal Regulatory Intelligence System — Reconciled Architecture v2.0**
*Owner: Vivek Vaidyanathan | Status: FROZEN | Supersedes: Master Ontology v1.0 (June 2026), Ontology Overview v1.1 (`PRIS_Ontology_Overview.md`, 2026-06-13), Consolidated Draft v1.2 (13 June 26)*

---

## 0. Why v2.0 Exists

v1.0 froze a target architecture in early June 2026. Corpus-intake work (Batches 1–6) and organic project growth then produced two structural layers and several naming variants that v1.0 did not anticipate. A v1.1 Overview and a v1.2 consolidated draft each tried to describe the resulting state, but neither went through the change-control procedure v1.0 itself required (Decision Journal entry + version increment + MOC propagation).

v2.0 closes that gap. It is the **single authoritative ontology document**. v1.1 and v1.2 are retired (v1.1 archived to `99_Archive/`; v1.2 was never written to the vault). This freeze is logged as **DJ-06** in `12_Decision_Journal/Decision_Journal.md`.

**What changed from v1.0, in summary:**

1. **Corpus Nodes** (`07_Institutions/Corpus/`) and **Wiki Intake Notes** (`04_Knowledge_Products/Wiki_Intake/`) are now permanent, first-class note types — not provisional intake scaffolding.
2. **File naming standardised to `.md`** — the `.md.md` double-extension anomaly has been migrated vault-wide (111 files renamed, wikilinks repaired).
3. **02_Projects** and **05_Concepts** subfolder structure in the ontology now matches the vault as built, rather than the other way round.
4. **P5_AI_Ethics**, **NITI_Aayog**, and **Agentic_AI_Governance** are formally registered as additions to the Active Projects, Institutions, and Standard Concepts tables respectively.

Everything else in v1.0 — the knowledge hierarchy, linking philosophy, system boundaries doctrine, population sequence logic, and minimum viable note schema — remains in force and is restated below for completeness.

---

## 1. Purpose and Doctrine (unchanged from v1.0)

**What PRIS is not:** A second brain. A note collection. A Zotero mirror. An NVivo duplicate.

**What PRIS is:** A Research Intelligence Platform that converts literature, regulations, coding outputs, teaching material, consulting insights, and AI-generated analysis into reusable intellectual assets compounding over a 20-year horizon.

### System Boundaries (clarified)

| System | Authoritative For | Obsidian Role |
|---|---|---|
| **Zotero** | References, papers, books, reports (~1500 entries) | Never replicated |
| **NVivo** | IG 2.0 coding, ADICO, nodes, inter-coder reliability | Never replicated |
| **iCloud PDFs / Policy Dump** | Source PDFs — regulations, standards, policy circulars, advisory reports | Never replicated in full text |
| **Obsidian — Corpus Nodes (07_Institutions/Corpus/)** | Structured *intelligence notes* on individual regulatory instruments (Format A) | Permanent — derived synthesis + ADICO summary + connections, not the source document |
| **Obsidian — Wiki Intake (04_Knowledge_Products/Wiki_Intake/)** | Structured *intelligence notes* on academic/Big4/advisory reports feeding the AI Governance Wiki (Format B) | Permanent — derived synthesis + connections, not the source document |
| **Obsidian — everything else** | Concepts, frameworks, synthesis, projects, knowledge products, strategy | This system |

**Clarification of the "do not replicate" rule:** the rule prohibits storing *primary-source text* (full circulars, full papers) in Obsidian. It does not prohibit *derived intelligence notes about* those sources — that is precisely what Corpus Nodes and Wiki Intake Notes are. This was the implicit reading already in practice; v2.0 makes it explicit.

---

## 2. Knowledge Hierarchy (Inviolable, unchanged)

```
Strategy
    ↓
Projects
    ↓
Knowledge Products
    ↓
Domains
    ↓
Concepts
    ↓
Frameworks
    ↓
Institutions / Corpus Nodes  ← evidence-adjacent intelligence layer
    ↓
Evidence  ← lives in Zotero / NVivo / Policy Dump, not Obsidian
```

Evidence supports corpus nodes and institution notes. These support frameworks and concepts. Concepts support domains. Domains support projects and knowledge products. Projects support strategy. Do not reverse this hierarchy.

---

## 3. Linking Philosophy (unchanged, restated)

- **MOC notes** at `00_MOC/`, each project folder, and each domain folder — index notes that link downward.
- **Flat wikilinks** within folders — notes link to each other as peers using `[[Note Name]]` syntax.
- **No hierarchical `parent::` fields** — navigation is through MOC notes, not metadata chains.
- **Cross-folder links are normal.**
- **Bidirectional linking for corpus nodes** (new in v2.0, formalising the 2026-06-14 `Bidirectional_Linking_Convention.md`): every corpus node's outward "Connections" must have a matching inward reference in `Corpus_Index_MOC`, the cited concept's "Instances in Corpus" section, and the relevant institution/concept MOC table. This is now a standing ontology rule, not a one-off convention.

---

## 4. Complete Folder Hierarchy (as built, v2.0)

```
PRIS/
│
├── 00_MOC/
├── 01_Strategy/
├── 02_Projects/
│   ├── Shared_Anchors/      (foundational literature anchors, peer notes)
│   └── References/          (per-project bibliography lists)
├── 03_Domains/
├── 04_Knowledge_Products/
│   └── Wiki_Intake/          (Format B intake notes — permanent)
├── 05_Concepts/
│   ├── 05_Concepts_Signature/
│   └── 05_Concepts_Standard/
├── 06_Frameworks/
├── 07_Institutions/
│   └── Corpus/                (Format A corpus nodes — permanent)
│       ├── RBI/
│       ├── SEBI/
│       ├── MeitY/
│       ├── NITI_Aayog/
│       ├── CERT_In/
│       ├── IRDAI/
│       ├── TRAI/
│       └── International/
├── 08_Methods/
├── 09_Teaching/
├── 10_Consulting/
├── 11_Content/
├── 12_Decision_Journal/
├── 99_Archive/
└── 99_System_Templates/
```

**File extension:** all notes use `.md` (single extension). The `.md.md` anomaly was fully migrated 2026-06-14 (111 files renamed; all `[[Name.md]]`-style wikilinks repaired to `[[Name]]`).

---

## 5. Folder Specifications — Deltas from v1.0

Only folders with a material change from v1.0 are detailed here. For folders not listed (01_Strategy, 03_Domains, 06_Frameworks, 08_Methods, 09_Teaching, 11_Content, 99_Archive, 99_System_Templates), v1.0's specification continues to apply unchanged.

### 02_Projects — Active Research Projects

**v1.0 specified** `Active/`, `Deferred/`, `Thesis/` subfolders. **As built**, projects sit flat at `02_Projects/` root and the active/deferred distinction is carried in each note's frontmatter (`status: active|deferred`) rather than by folder. v2.0 adopts the as-built convention: **subfolder-based status partitioning is dropped**; status lives in frontmatter and is surfaced via `Projects_MOC.md`.

Two new subfolders are formalised:

| Subfolder | Contents | Rationale |
|---|---|---|
| `Shared_Anchors/` | Peer notes on foundational literature cited across multiple papers (e.g., `DiMaggio_Powell_1983`, `Ragin_2008`, `Fiss_2011`, `EU_AI_Act_Governance`) | Avoids duplicating the same theoretical-source summary inside multiple project state notes |
| `References/` | Per-project bibliography lists (`P2_References`, `P3_References`, `P4_References`, `P5_References`, `fsQCA_References`) | Keeps project state notes free of long reference lists while preserving traceability |

#### Active Papers (updated — five, not four)

| File | Journal | ABDC | Status | Deadline |
|---|---|---|---|---|
| `P2_DPI_JSIS.md` | JSIS Special Issue | A* | Extended abstract submitted; full paper drafting | 30 Sep 2026 |
| `P3_BFSI_JEIM.md` | JEIM | A | Scaffold not executed; activates Q3 2026 | Feb–Mar 2027 |
| `P4_Doctrinal_IJLIT.md` | IJLIT (primary) / ICTL (fallback) | B | Pre-drafting; activates Q4 2026 | Mar–Apr 2027 |
| `P5_AI_Ethics.md` | Book chapter / Ethics outlet | TBD | Scaffold present; socio-technical AI ethics, anchored to `AI_Governance` domain | TBD — **⚠ VERIFY**: target outlet, ABDC rank, and activation window not yet confirmed in project note |
| `fsQCA_Thesis_Chapter.md` | IIM Indore thesis (internal) | N/A | IG coding in progress; thesis-critical | Q2 2027 |

**P5_AI_Ethics — formal registration (v2.0):** P5 was created during the build phase without a corresponding Decision Journal entry. v2.0 formally registers it as the fifth active project. Its target journal/ABDC rank, deadline, and relationship to the P1–P4 + fsQCA sequencing in `01_Strategy/Publication_Pipeline.md` carry an **⚠ VERIFY BEFORE PUBLISHING** flag pending a dedicated review.

#### Deferred Papers

| File | Journal | ABDC | Status | Activation |
|---|---|---|---|---|
| `P1_SLR_RG.md` | Regulation & Governance | A | Decoupled from defence; not active 2026 | Q3 2027 post-defence |

---

### 05_Concepts — Conceptual Layer

**v1.0 specified** `Signature/` and `Standard/`. **As built**, the subfolders are `05_Concepts_Signature/` and `05_Concepts_Standard/` (folder name repeats the parent number/prefix). v2.0 adopts the as-built naming — **no rename required**; the ontology specification is updated to match.

#### Signature Constructs (unchanged)

| File | Appears In | Knowledge Product Potential |
|---|---|---|
| `Regulatory_Parallelism.md` | P3, P4, AI Governance Wiki | Regulatory Complexity Handbook; consulting framework |
| `Governance_Debt.md` | P3, P4, consulting | BFSI AI Governance Handbook; advisory deliverable |
| `Institutional_Coherence.md` | P2, P4, fsQCA | AI Governance Wiki; teaching case |

#### Standard Concepts (updated — five, not four)

| File | Theoretical lineage |
|---|---|
| `Accountability.md` | AI governance; public administration |
| `Legitimacy.md` | Institutional theory; regulatory theory |
| `Transparency.md` | AI governance; information systems |
| `Governance_Capacity.md` | Regulatory governance; institutional theory |
| `Agentic_AI_Governance.md` | AI governance; agency theory / autonomous-systems oversight |

**Agentic_AI_Governance — formal registration (v2.0):** added during corpus intake (cited by RBI_FREE_AI_2025, F025, F026, RBI_5, F030 — see `Corpus_Index_MOC`). Formally registered as a Standard Concept. No DJ entry existed prior to v2.0; see DJ-06.

---

### 07_Institutions — Regulatory Institutions (major addition: Corpus layer)

**v1.0 specified** six flat institution notes (RBI, SEBI, MeitY, CERT_In, UIDAI, TRAI). **As built**, a seventh institution was added, and a `Corpus/` subtree now holds Format A corpus nodes — individual regulatory instruments processed during Policy Dump intake.

| File | Jurisdiction | Relevance |
|---|---|---|
| `RBI.md` | India | P3, P4, BFSI consulting |
| `SEBI.md` | India | P3, P4, BFSI consulting |
| `MEITY.md` | India | P2, P4, AI governance consulting |
| `CERT_IN.md` | India | P3, cybersecurity consulting |
| `UIDAI.md` | India | P2, DPI governance |
| `TRAI.md` | India | AI governance consulting |
| `NITI_Aayog.md` | India | P1, P2 — national AI strategy framing |

**NITI_Aayog — formal registration (v2.0):** added during corpus intake (NITI_3/6/7 corpus nodes; National Strategy for AI #AIforAll). Formally registered as the seventh institution. See DJ-06.

#### `07_Institutions/Corpus/` — Format A Corpus Nodes (permanent layer, new in v2.0)

**Purpose:** One note per regulatory instrument processed from the Policy Dump corpus (`/Users/vivek/Documents/LinkedIn/Policy Dump/`). Each node records: instrument identity (issuer, date, status), structural summary, ADICO/IG2.0 coding summary (pointer to NVivo for full coding), "Connections" to concepts/projects/frameworks/institutions, and any ⚠VERIFY flags.

**Note type:** Corpus Node (Format A)

**Index:** `Corpus_Index_MOC.md` — master table, "By Wiki Section," "By Project," and consolidated ⚠VERIFY tracker.

**Bidirectional linking is mandatory** (see `Bidirectional_Linking_Convention.md`, now part of this ontology per §3 above): every corpus node's outward connections must be mirrored as inward references in `Corpus_Index_MOC`, the cited concept's "Instances in Corpus" section, and the relevant institution MOC row.

Current population (Batches 1–6, per `Corpus_Index_MOC` / `Session_Handoff_Cowork_20260614_Batch6.md`):

| Sub-folder | Nodes |
|---|---|
| `RBI/` | RBI_1–5 (RBI_5 = NBFC Operational Risk, Batch 6) |
| `SEBI/` | SEBI_9–12 |
| `MeitY/` | MeitY_1–3 |
| `NITI_Aayog/` | NITI_3, 6, 7 |
| `CERT_In/` | CERT_1, 2, 4 |
| `IRDAI/` | (folder present, population pending) |
| `International/` | International_1–4, plus `fsQCA_Case_Registry.md` |

**Numbering state (carried forward from Batch 6 handoff):** next IDs — RBI_6, SEBI_13, MeitY_4, NITI_8, International_5; F-series (Wiki Intake) next = F031.

---

### 04_Knowledge_Products/Wiki_Intake — Format B Wiki Intake Notes (permanent layer, new in v2.0)

**Purpose:** One note per academic paper / Big4 or advisory report / industry survey processed from the raw Policy Dump PDF corpus, structured to feed `AI_Governance_Wiki.md`. Distinguished from Corpus Nodes (Format A) by source type: Format B sources are secondary literature (academic, consulting, industry), Format A sources are primary regulatory instruments.

**Note type:** Wiki Intake Note (Format B)

**Index:** `Wiki_Intake_Index.md`, cross-referenced in `Corpus_Index_MOC` ("Batch N — Wiki Intake Notes" tables, F-series IDs).

**Current population:** ~38 notes (Batches 4–6 plus standing process files `PRIS_Cowork_Context.md`, `PRIS_Corpus_Intake_Prompts.md`).

**Rule (unchanged from v1.0 intent, now explicit):** Wiki Intake notes are intermediate — they exist to be absorbed into `AI_Governance_Wiki.md` and into the "Instances in Corpus" / "Cross-Concept Applications" layers. They are not a permanent literature dump; periodic absorption passes into the Wiki and concept files are part of the indexing-pass discipline.

---

## 6. Population Sequence (Build Order) — status update

| Phase | Action | Status as of 2026-06-14 |
|---|---|---|
| **Phase 1** | Create all folders and sub-folders | ✅ Complete (plus `Shared_Anchors/`, `References/`, `Corpus/`, `Wiki_Intake/` — formalised in v2.0) |
| **Phase 2** | Create all MOC shells | ✅ Complete |
| **Phase 3** | `01_Strategy` notes from existing documents | ✅ Complete |
| **Phase 4** | `02_Projects` active notes (P2, P3, P4, fsQCA) | ✅ Complete; **P5 added beyond original scope — ⚠VERIFY** |
| **Phase 5** | `05_Concepts/Signature` notes | ✅ Complete |
| **Phase 6** | `03_Domains` notes | ✅ Complete |
| **Phase 7** | `06_Frameworks` notes (49-framework corpus, fsQCA cases first) | Partial — 6 framework notes populated; Corpus Node layer (Phase 7a, new) substituting for much of the planned framework-corpus breadth |
| **Phase 7a** *(new)* | `07_Institutions/Corpus/` nodes — Policy Dump Batches 1–6 | In progress — 6 of planned 11 batches complete |
| **Phase 8** | `04_Knowledge_Products` notes | Partial — 4 architecture notes + Wiki Intake layer (38 notes) substantially ahead of plan |
| **Phase 9** | `07_Institutions`, `08_Methods` notes | ✅ Complete (7 institutions incl. NITI_Aayog; 4 methods) |
| **Phase 10** | Populate wikilinks across all notes | Ongoing — bidirectional linking convention now standing practice for Corpus Nodes |

**Rule retained from v1.0:** once a layer is structurally adequate, build stops and output production (manuscript drafting, Wiki Intake absorption) resumes. Phase 7a (Corpus Node intake) should not become an indefinite background task — Batches 7–11 are the planned closure of this phase per the Batch 6 handoff.

---

## 7. Note Template — Minimum Viable Structure (unchanged from v1.0)

```markdown
---
type: <NoteType>
status: <active|deferred|draft|archived|superseded>
last_updated: YYYY-MM-DD
tags:
  - type/<note-type>
  - status/<status>
---

# [Note Title]

## Core Synthesis
[2–5 sentences of distilled intelligence — not summary, synthesis]

## Linked Projects
- [[P2_DPI_JSIS]]

## Linked Domains
- [[AI_Governance]]

## Linked Concepts
- [[Regulatory_Parallelism]]

## Linked Frameworks
- [[EU_AI_Act]]

## Future Research / Reuse Opportunities
[Explicit identification of where this note feeds future work]

---
*Back to [[_MOC_relevant_section]]*
```

**Corpus Node (Format A) and Wiki Intake Note (Format B) templates** follow the structures already in use across Batches 1–6 (instrument identity / source identity, structural or argument summary, ADICO/coding summary where applicable, Connections, ⚠VERIFY flags) — these are now formally part of the note-type taxonomy alongside the schema above, but are not restated in full here; see existing populated nodes as the working templates pending a dedicated `99_System_Templates/Corpus_Node_Template.md` and `Wiki_Intake_Template.md` (not yet created — **gap noted for a future session**).

---

## 8. Ontology Change Control

This ontology is frozen as of **2026-06-14** as **v2.0**.

Changes require:

1. A decision log entry in `12_Decision_Journal/Decision_Journal.md` (next: DJ-07).
2. Updates to this file with a version increment.
3. Updates to affected MOC notes (`PRIS_Master_MOC.md`, `_Institutions_MOC.md`, `_Concepts_MOC.md`, `Projects_MOC.md`, as relevant).

**Version:** 2.0
**Supersedes:** v1.0 (frozen June 2026, never committed to vault as a standalone file), v1.1 (`PRIS_Ontology_Overview.md`, archived to `99_Archive/`), v1.2 (consolidated draft, not committed to vault)
**Next review trigger:** Completion of Policy Dump Batches 7–11 (Corpus Node Phase 7a closure), or post-P2 submission (Sep 2026), or post-defence (Q3/Q4 2027) — whichever occurs first.

---

*End of PRIS Master Ontology v2.0*
*For strategic context, see `01_Strategy/VV_Publication_Pipeline_v3.md` and `01_Strategy/VV_Life_Roadmap_V2.md`. For corpus-intake operating procedure, see `04_Knowledge_Products/Wiki_Intake/PRIS_Cowork_Context.md` and `00_MOC/Bidirectional_Linking_Convention.md`.*
