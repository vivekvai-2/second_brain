# **PRIS — Ontology & Workflow Architecture Guide**

**Type:** System Architecture MOC  
**Status:** Active  
**Last Updated:** 2026-06-13  
**Version:** Ontology v1.1  
**Target Audience:** LLM Agents & System Architects  

---

## **1. Core System Philosophy & Purpose**

**PRIS (Personal Regulatory Intelligence System)** is a Research Intelligence Platform designed to convert academic literature, regulatory analysis, coding outputs, consulting insights, and AI-generated analysis into reusable intellectual assets that compound over a twenty-year horizon. 

### **The PRIS Creed**
*   **Not a Second Brain:** PRIS is not a passive note collection. It is an active production engine.
*   **Asset Compounding:** Every note must serve as a building block for multiple outputs (Papers, Handbooks, Consulting Frameworks, Presentations).
*   **Structural Rigour:** High-density, structured, and deeply linked notes are preferred over fragmented, stream-of-consciousness writing.
*   **System Boundaries:** Source-level literature lives in Zotero; raw coding structures live in NVivo; PDFs live in iCloud. PRIS is the synthesising and authoring layer.

---

## **2. Knowledge Hierarchy (Ontology)**

The PRIS knowledge architecture operates on a strict top-down and bottom-up relational hierarchy:

```text
       [ Strategy ]          <-- Long-horizon roadmaps, publication pipelines
            ↓
       [ Projects ]          <-- Active/thesis papers, state tracking, references
            ↓
  [ Knowledge Products ]     <-- Reusable intellectual assets, handbooks, wikis
            ↓
       [ Domains ]           <-- Domain-level synthesis & subject matter areas
            ↓
       [ Concepts ]          <-- Signature constructs (original) & Standard constructs
            ↓
      [ Frameworks ]         <-- Analytical policy and legal frameworks
            ↓
     [ Institutions ]        <-- Regulatory bodies and governance actors
            ↓
       [ Methods ]           <-- Applied research methods (e.g., fsQCA, IG 2.0)
            ↓
       [ Evidence ]          <-- Authority source documents (Zotero/iCloud)
```

---

## **3. Folder-by-Folder Structural Mapping**

As of June 2026, the vault contains exactly **96 files** organized across 15 functional folders.

### **00_MOC (Map of Content)**
*   **Path:** `00_MOC/`
*   **Note Count:** 10 files
*   **Purpose:** The central navigation and index layer. Contains MOCs for each structural branch of the hierarchy.
*   **Key Notes:** 
    *   [[PRIS_Master_MOC]] — The master entry point for the entire vault.
    *   [[Research_Dashboard]] — High-level view of research programs and schedules.
    *   `_Concepts_MOC.md.md`, `_Frameworks_MOC.md.md`, `_Institutions_MOC.md.md`, `_Methods_MOC.md.md` — Relational indices.

### **01_Strategy**
*   **Path:** `01_Strategy/`
*   **Note Count:** 2 files
*   **Purpose:** Long-term direction, career transitions, and portfolio management.
*   **Key Notes:**
    *   [[VV_Publication_Pipeline_v3]] — Portfolio management of all active/future papers.
    *   `VV_Life _Roadmap_V2.md` — Career, academic, and professional milestones (Army exit, PhD defence).

### **02_Projects**
*   **Path:** `02_Projects/`
*   **Note Count:** 24 files (7 at root, 12 in `Shared_Anchors/`, 5 in `References/`)
*   **Purpose:** Active paper drafting, thesis chapters, and academic literature anchors.
*   **Key Notes:**
    *   [[P2_DPI_JSIS]] — State file, gap analysis, and action plan for the Digital Public Infrastructure paper targeted at JSIS.
    *   [[P3_BFSI_JEIM]] — State file for the BFSI AI Governance paper.
    *   `02_Projects/Shared_Anchors/` — Summaries of foundational literature (e.g., `Kallinikos_Aaltonen_Marton_2013.md.md`, `Seidel_Frick_vomBrocke_2025.md.md`).
    *   `02_Projects/References/` — Comprehensive bibliography lists for specific projects.

### **03_Domains**
*   **Path:** `03_Domains/`
*   **Note Count:** 5 files
*   **Purpose:** High-level synthesis of specific subject-matter areas.
*   **Key Notes:**
    *   [[AI_Governance]] — Synthesis of the AI regulatory landscape.
    *   [[DPI_Governance]] — Synthesis of Digital Public Infrastructure governance.
    *   [[BFSI_Governance]], [[Privacy_DataProtection]], [[Cybersecurity_Governance]].

### **04_Knowledge_Products**
*   **Path:** `04_Knowledge_Products/`
*   **Note Count:** 13 files (4 at root, 9 in `Wiki_Intake/`)
*   **Purpose:** Reusable intellectual assets designed for public or commercial distribution.
*   **Key Notes:**
    *   [[AI_Governance_Wiki]] — Compiled knowledge base of AI governance parameters.
    *   [[DPDP_Playbook]] — Practical compliance handbook for the Digital Personal Data Protection Act.
    *   [[BFSI_AI_Governance_Handbook]] — Playbook for financial institutions.
    *   `04_Knowledge_Products/Wiki_Intake/` — Raw summaries and indices of external corporate/regulatory reports (EY, PwC, Deloitte, NASSCOM) serving as intake feeds.

### **05_Concepts**
*   **Path:** `05_Concepts/`
*   **Note Count:** 7 files (4 in `05_Concepts_Standard/`, 3 in `05_Concepts_Signature/`)
*   **Purpose:** Theoretical building blocks. Signature concepts are original constructs; Standard concepts are established scholarly constructs.
*   **Key Notes:**
    *   [[Governance_Debt]] (Signature) — Accumulated compliance duplication burden transferred to regulated enterprises.
    *   [[Regulatory_Parallelism]] (Signature) — Uncoordinated overlapping mandates from independent regulators.
    *   [[Institutional_Coherence]] (Signature) — The alignment of regulatory logic across domains.
    *   `05_Concepts_Standard/` — [[Accountability]], [[Legitimacy]], [[Transparency]], [[Governance_Capacity]].

### **06_Frameworks**
*   **Path:** `06_Frameworks/`
*   **Note Count:** 7 files
*   **Purpose:** Deep-dive analyses of specific regulatory, policy, or legal frameworks.
*   **Key Notes:**
    *   [[RBI_Free_AI]] — Analysis of the RBI's framework for AI in BFSI.
    *   [[EU_AI_Act]], [[NIST_AI_RMF]], [[OECD_AI_Principles]], [[SEBI_AI_Circular]], [[IndiaAI_Framework]].

### **07_Institutions**
*   **Path:** `07_Institutions/`
*   **Note Count:** 7 files (6 at root, 1 in `Corpus/International/`)
*   **Purpose:** Intelligence profiles of regulatory and policy actors.
*   **Key Notes:**
    *   [[RBI]] (Reserve Bank of India), [[SEBI]] (Securities and Exchange Board of India), [[MEITY]] (Ministry of Electronics and Information Technology).
    *   `07_Institutions/Corpus/International/fsQCA_Case_Registry.md.md` — Empirical case tracking.

### **08_Methods**
*   **Path:** `08_Methods/`
*   **Note Count:** 4 files
*   **Purpose:** Applied research methodologies and coding protocols.
*   **Key Notes:**
    *   [[Institutional_Grammar_IG2]] — Rules, norms, and strategies coding (ADICO syntax).
    *   [[fsQCA]] — Fuzzy-set Qualitative Comparative Analysis.
    *   [[SLR_Protocol]] — Systematic Literature Review protocol.

### **09_Teaching**
*   **Path:** `09_Teaching/`
*   **Note Count:** 0 files (Placeholder for future course development)

### **10_Consulting**
*   **Path:** `10_Consulting/`
*   **Note Count:** 7 files
*   **Purpose:** Client engagements, proposals, and inbound pipeline management.
*   **Key Notes:**
    *   [[Inbound_Pipeline_Index]] — Master tracker of consulting opportunities.
    *   `CyberMesh_PS74_Inbound.md.md`, `AEGIS_OS_Inbound.md.md` — Specific client proposals.

### **11_Content**
*   **Path:** `11_Content/`
*   **Note Count:** 1 file
*   **Purpose:** Derivative short-form communication, keynotes, and presentation drafts.
*   **Key Notes:**
    *   `ADP_Keynote_2026.md.md` — Keynote speech outline.

### **12_Decision Journal**
*   **Path:** `12_Decision Journal/` (Note: space in folder name, but referenced as `12_Decision_Journal` in metadata)
*   **Note Count:** 1 file
*   **Purpose:** Log of high-consequence strategic decisions and learning records.
*   **Key Notes:**
    *   [[Decision_Journal]] — Tracks design freezes, target journal shifts, and major pivots.

### **99_Archive**
*   **Path:** `99_Archive/`
*   **Note Count:** 0 files (Placeholder for retired notes)

### **99_System_Templates**
*   **Path:** `99_System_Templates/`
*   **Note Count:** 5 files
*   **Purpose:** System-standard templates enforcing structural uniformity.
*   **Key Notes:**
    *   `Method_Template.md.md`, `Framework_Template.md.md`, `Concept_Template.md.md`, `Domain_Template.md.md`, `Project Template.md.md`.

---

## **4. File Naming & Extension Anomaly**

> ⚠️ **CRITICAL LLM NOTE:** A significant portion of the files in this vault use a double extension anomaly: **`.md.md`** (e.g., `P2_DPI_JSIS.md.md`, `Governance_Debt.md.md`). 
> *   When searching, reading, or writing files, you must check if the file uses `.md.md` or `.md`.
> *   When creating new files, check the folder's existing files to match their extension style (most standard folders use `.md.md` while `04_Knowledge_Products` root and `01_Strategy` use `.md`).
> *   Obsidian WikiLinks should be written as standard links: e.g., `[[Governance_Debt]]` or `[[P2_DPI_JSIS]]` without the extension, which Obsidian resolves automatically.

---

## **5. Note Metadata Schema (Frontmatter)**

PRIS notes use structured YAML frontmatter to enable automated querying, indexing, and dashboard updates.

### **Example: Project Note Frontmatter**
```yaml
---
type: Project
tags:
  - type/project
  - status/drafting
  - phase/q3-2026
  - paper/p2-primary
  - paper/fsqca
  - gate/open
  - engine/phd
---
```

### **Example: Concept Note Frontmatter**
```yaml
---
type: Signature Concept  # or "Standard Concept"
tags:
  - type/concept-signature
  - status/active
  - paper/p3-primary
  - engine/phd
  - engine/consulting
---
```

---

## **6. Relational Causal Loops (Upstream / Downstream)**

The power of PRIS lies in its relational logic. Notes are designed to "feed" each other across the hierarchy:

1.  **Frameworks & Institutions** (e.g., [[RBI_Free_AI]] + [[RBI]]) are coded using **Methods** (e.g., [[Institutional_Grammar_IG2]]).
2.  This coding reveals structural anomalies, which are conceptualised into **Concepts** (e.g., [[Regulatory_Parallelism]] and [[Governance_Debt]]).
3.  These concepts are synthesized into **Domains** (e.g., [[BFSI_Governance]]).
4.  Domains and Concepts are packaged into commercial **Knowledge Products** (e.g., [[BFSI_AI_Governance_Handbook]]) and academic **Projects** (e.g., [[P3_BFSI_JEIM]]).
5.  **Consulting** engagements (e.g., `CyberMesh_PS74_Inbound.md.md`) identify real-world pain points that are fed back into the **Concepts** and **Knowledge Products** layers, creating a continuous intellectual compounding loop.

---

## **7. Workflow Blueprints for LLM Agents**

When an LLM is asked to perform tasks in this vault, it must follow these standardized workflow blueprints:

### **Workflow A: Ingesting a New Regulatory Report / Policy Circular**
1.  **Create Wiki Intake Note:** Create a note in `04_Knowledge_Products/Wiki_Intake/` named `Source_Name_Year.md.md`.
2.  **Extract Key Elements:** Map the source's main claims, affected sectors, and regulatory mandates.
3.  **Link Upstream/Downstream:** 
    *   Link to the issuing [[Institutions]] (e.g., [[RBI]]).
    *   Link to the relevant [[Frameworks]] (or create a new framework note in `06_Frameworks/` if it's a major regulatory shift).
    *   Link to relevant [[Domains]] (e.g., [[BFSI_Governance]]).
4.  **Identify Concept Connections:** Does this source show evidence of [[Regulatory_Parallelism]] or generate [[Governance_Debt]]? Link them.

### **Workflow B: Generating or Refining a Concept Note**
1.  **Use Concept Template:** Copy the structure of `99_System_Templates/Concept_Template.md.md`.
2.  **Define the Core Construct:** Write a precise, scholarly Definition and describe the underlying Mechanism.
3.  **Provide Empirical Evidence:** Cite specific coded data, papers, or regulatory clauses where this construct is observed.
4.  **Theoretical Positioning:** Position the concept against existing literature (e.g., Enterprise Information Management, Institutional Layering).
5.  **Map Upstream/Downstream Causes & Effects:** Clearly state what causes this concept (Upstream) and what it feeds into (Downstream).

### **Workflow C: Academic Drafting & Paper Progression (The DDP Protocol)**
The **Drafting Discipline Protocol (DDP)** is binding for all paper drafting:
*   **Rule 1: Lock the Narrative Spine first.** Before writing or modifying any section of a paper, the standard narrative spine template must be fully populated and locked in Section 6 of the paper's state file (e.g., `P2_DPI_JSIS.md.md`).
*   **Rule 2: Contribution claim placement.** The core contribution claim of the paper must appear in Section 1 (Introduction) before the first 500 words.
*   **Rule 3: Avoid fragmentation.** Maintain 5–6 substantive sections. No small, fragmented sub-sections. Each section must be at least 600 words.
*   **Rule 4: Flow and Transitions.** Every section must end with a forward-referencing transition to the next section.
*   **Rule 5: Run Cadence Elimination.** Run the `ai-cadence-elimination` skill on the entire manuscript to remove AI writing tells (such as "in conclusion", "not only... but also", "delve", "testament").

---

## **8. Master Index of Active Research Projects**

| Paper ID | Target Outlet | Core Focus | Supporting Concepts | Sibling State File |
|---|---|---|---|---|
| **P1** | Systematic Lit Review | SLR of AI Governance & Institutional Grammar | [[SLR_Protocol]] | [[P1_SLR_RG]] |
| **P2** | *JSIS* Special Issue | DPI Governance & Rules-Records Asymmetry | [[DPI_Governance]] | [[P2_DPI_JSIS]] |
| **P3** | *JEIM* | BFSI AI Governance & Governance Debt | [[Regulatory_Parallelism]], [[Governance_Debt]] | [[P3_BFSI_JEIM]] |
| **P4** | *IJLIT* | Doctrinal analysis of AI Circulars | [[Institutional_Coherence]] | [[P4_Doctrinal_IJLIT]] |
| **P5** | Book Chapter / Ethics | Socio-technical AI Ethics | [[AI_Governance]] | [[P5_AI_Ethics]] |

---

_This guide serves as the authoritative system overview for all automated agents operating within the PRIS Vault. Maintain these boundaries, respect the naming conventions, and enforce the relational linkages with absolute discipline._
