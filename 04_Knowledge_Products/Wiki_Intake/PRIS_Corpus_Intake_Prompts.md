---
type: Process Document
status: active
last_updated: 2026-07-21
tags:
  - type/process-document
  - status/active
  - engine/phd
---

# PRIS Corpus Intake Prompts — Batch F+
## AI Governance Wiki: Document Scanning, Classification and Vault Node Generation

**Version:** 1.2  
**Created:** 2026-06-14 | **Updated:** 2026-07-15 (added PROMPT 0 — Gemini extraction relay, for iCloud-dataless / host-local-only files that Cowork's sandbox cannot read directly; added PROMPT 0b — NotebookLM extraction relay, same schema, adapted for NotebookLM's multi-source/citation model)  
**For use with:** Cowork (full pipeline) or Claude Project (manual batches); PROMPT 0/0b are for Gemini/NotebookLM specifically  
**Vault MCP:** Active — writes directly to `/Users/vivek/Documents/Second Brain/`  
**Parent:** [[AI_Governance_Wiki]] | [[Wiki_Intake_Index]]

---

## HOW TO USE THESE PROMPTS

Four prompts in this file:

| Prompt | Purpose | When to use | Output |
|--------|---------|-------------|--------|
| **PROMPT 0 — Gemini Extraction Relay** | Read a PDF Cowork's sandbox can't access (iCloud-dataless, image-only, etc.) and produce faithful structured text | Whenever a Policy Dump file shows real `ls` size but 0 bytes on actual read in Cowork | Structured plain-text extraction — paste back into the Cowork/Claude conversation |
| **PROMPT 0b — NotebookLM Extraction Relay** | Same schema as PROMPT 0, adapted for NotebookLM's multi-source notebook + citation model | When documents are already uploaded to a NotebookLM notebook rather than accessed via Gemini directly | Structured plain-text extraction (with native NotebookLM citations preserved) — paste back into the Cowork/Claude conversation |
| **PROMPT 1 — Pilot** | Test 3 documents; calibrate output quality | Before any batch run | 3 corpus nodes + quality check |
| **PROMPT 2 — Classification Sweep** | Classify 10–15 PDFs against wiki schema | Start of each batch session | Classification table |
| **PROMPT 3 — Vault Node Generation** | Convert classification table → vault-ready corpus nodes | After classification is reviewed | `.md` files written to vault |

Run PROMPT 1 first, always, for a genuinely new intake pipeline. If quality is acceptable, proceed to PROMPT 2 → PROMPT 3. Use PROMPT 0 or PROMPT 0b opportunistically, per-file, whenever Cowork reports a file as unreadable or the source is already sitting in a NotebookLM notebook — both produce output in the same schema, so raw extraction quality stays consistent regardless of which tool did the reading.

---

---

# PROMPT 0 — GEMINI EXTRACTION RELAY (for Cowork-unreadable PDFs)

**Use for:** Any Policy Dump Future (or other corpus) PDF that Cowork's sandbox reports as having a real file size (`ls`/`stat`) but returns 0 bytes on actual read — the iCloud-dataless-placeholder signature identified in the Batch 18 session (2026-07-15). Gemini, run from the Mac directly (Gemini app, or gemini.google.com with the file uploaded from Finder), has direct access to the real local file and does not go through Cowork's remote mount, so it can read what Cowork cannot.

**Workflow:** Run this prompt in Gemini once per PDF → copy Gemini's full output → paste it back into the Cowork/Claude conversation with the filename → Claude does the PRIS-specific classification, dedup-check, concept-linking, and vault-node writing from that text (Gemini should not attempt vault formatting itself — it doesn't have the current PRIS context, existing-node list, or concept files loaded).

**Copy everything below the dashed line into Gemini, then attach one PDF:**

---

You are a document extraction assistant. I will give you one PDF. Read the entire document — including running OCR on any pages that are scanned images rather than machine-readable text — and produce a single, complete, faithful structured extraction. Do not summarise for brevity, do not paraphrase to shorten, and do not add your own analysis, opinion, or evaluation of the document's quality. Extract only; a separate system will do the synthesis.

Produce your output in exactly this structure:

## 1. Document Identity
- Full title (exact, as printed on the document)
- Author(s) / contributing organisation(s) — individual names plus stated titles/affiliations
- Publishing institution
- Publication date (exact day/month/year if stated; if only a year is given, or the date is ambiguous/absent, say so explicitly)
- Document type (regulatory instrument, whitepaper, academic paper, standard, government strategy, industry report, threat forecast, etc.)
- Total page count
- Whether the PDF was machine-readable text throughout, or required OCR — and if only some pages needed OCR, say which ones

## 2. Table of Contents / Structure
Reproduce the document's own section/chapter structure, with page numbers if visible in the source.

## 3. Full Structured Content Extraction
Work through the document section by section, following its own structure, and extract:
- Every definition, taxonomy, or named framework/model the document introduces
- Every obligation, requirement, or recommendation — state explicitly whether the source text uses mandatory language ("must," "shall," "is required to") or advisory language ("should," "may," "is encouraged to")
- Every specific figure: percentages, monetary amounts, dates, deadlines, counts, thresholds — quoted exactly as written, with the section or page number it appears on
- Every named person, court case, incident, or worked example cited, with enough detail to be independently checked later
- Any sentence worth preserving verbatim as a quotable line — mark it clearly as a direct quote, with page number if available

Do not skip sections because they look procedural or repetitive — extract too much rather than too little. This is raw material for someone else's synthesis, not a finished summary.

## 4. Uncertain or Ambiguous Items
List anything where: a date is unclear, the document seems to contradict itself, a figure looks like it might be a misprint, an acronym is used but never defined in the document, or you are not fully confident in an OCR reading of a specific number or name. Prefix each with "UNCERTAIN:" and explain why.

## 5. Anything Clearly Out of Scope
If a substantial part of the document is obviously unrelated to AI governance, cybersecurity, financial regulation, or technology policy (e.g., an unrelated facilities-management appendix), just note that briefly rather than extracting it in full.

---

Rules:
- Completeness matters more than brevity — do not compress to save space.
- Do not invent page numbers where none are visible; write "page not numbered" instead.
- If the document is very long, extract as much as fits and end with "CONTINUED — more sections follow" so I can ask you to continue in a follow-up message.
- Plain text / Markdown output only, no HTML.

Now here is the PDF.

---

---

# PROMPT 0b — NOTEBOOKLM EXTRACTION RELAY (same schema, NotebookLM-adapted)

**Use for:** Documents already uploaded as sources in a NotebookLM notebook. Same purpose as PROMPT 0 — produce faithful structured extraction text that Claude/Cowork then classifies and writes into the vault — but adapted for how NotebookLM actually works: a notebook holds multiple sources at once, chat responses are scoped by default to whatever the model judges relevant across all of them, and NotebookLM provides native inline citations back to source passages, which is a genuine advantage over the plain Gemini relay worth preserving rather than discarding.

**Two adaptations versus PROMPT 0:**
1. **Always name the exact source explicitly.** Never ask a generic question in a multi-source notebook — it will blend or summarise across documents instead of extracting one faithfully. Every request below opens with "Using ONLY the source titled '[exact source name as shown in NotebookLM]'."
2. **Keep native citations in the output.** Ask NotebookLM to preserve its inline citation markers — they anchor claims to a specific passage, which is stronger grounding than the plain-text page references Gemini produces.

**Workflow:** One source per request (do not batch several PDFs into one ask — quality and completeness both degrade). Run this prompt once per source in the notebook's chat → copy the full response, including citation markers → paste it back into the Cowork/Claude conversation with the filename → Claude does the PRIS-specific classification, dedup-check, concept-linking, and vault-node writing (same handoff as PROMPT 0 — NotebookLM should not attempt vault formatting itself).

**Copy everything below the dashed line into NotebookLM's chat, with the correct source name substituted:**

---

Using ONLY the source titled "[exact source name as shown in NotebookLM]" — do not draw on any other source in this notebook — read the entire document and produce a single, complete, faithful structured extraction. Do not summarise for brevity, do not paraphrase to shorten, and do not add your own analysis, opinion, or evaluation of the document's quality. Extract only; a separate system will do the synthesis. Keep your native inline citations in the output wherever you make a specific claim.

Produce your output in exactly this structure:

## 1. Document Identity
- Full title (exact, as printed on the document)
- Author(s) / contributing organisation(s) — individual names plus stated titles/affiliations
- Publishing institution
- Publication date (exact day/month/year if stated; if only a year is given, or the date is ambiguous/absent, say so explicitly)
- Document type (regulatory instrument, whitepaper, academic paper, standard, government strategy, industry report, threat forecast, etc.)
- Total page count
- Whether the source appears to have been machine-readable text throughout or required OCR, if you can tell

## 2. Table of Contents / Structure
Reproduce the document's own section/chapter structure, with page numbers if visible in the source.

## 3. Full Structured Content Extraction
Work through the document section by section, following its own structure, and extract:
- Every definition, taxonomy, or named framework/model the document introduces
- Every obligation, requirement, or recommendation — state explicitly whether the source text uses mandatory language ("must," "shall," "is required to") or advisory language ("should," "may," "is encouraged to")
- Every specific figure: percentages, monetary amounts, dates, deadlines, counts, thresholds — quoted exactly as written, with your inline citation preserved
- Every named person, court case, incident, or worked example cited, with enough detail to be independently checked later
- Any sentence worth preserving verbatim as a quotable line — mark it clearly as a direct quote, with its citation

Do not skip sections because they look procedural or repetitive — extract too much rather than too little. This is raw material for someone else's synthesis, not a finished summary.

## 4. Uncertain or Ambiguous Items
List anything where: a date is unclear, the document seems to contradict itself, a figure looks like it might be a misprint, an acronym is used but never defined in the document, or you are not fully confident in a reading of a specific number or name. Prefix each with "UNCERTAIN:" and explain why.

## 5. Anything Clearly Out of Scope
If a substantial part of the document is obviously unrelated to AI governance, cybersecurity, financial regulation, or technology policy (e.g., an unrelated facilities-management appendix), just note that briefly rather than extracting it in full.

---

Rules:
- Completeness matters more than brevity — do not compress to save space.
- Do not invent page numbers where none are visible; write "page not numbered" instead.
- If the document is very long, extract as much as fits and end with "CONTINUED — more sections follow" so I can ask you to continue in a follow-up message, still scoped to this same source only.
- Plain text / Markdown output only, no HTML.
- Do not incorporate content from any other source in this notebook, even if it seems related.

---

---

# PROMPT 1 — PILOT RUN (3 Documents)

**Use for:** First run only. Pick one regulatory instrument, one Big Tech/Big 4 whitepaper, one academic paper. Review output before running the full corpus.

**Copy everything below the dashed line into Cowork or Claude:**

---

You are operating as a corpus intake agent for PRIS (Personal Regulatory Intelligence System), a long-term research intelligence platform supporting doctoral research, consulting, and teaching in AI governance.

## YOUR TASK

Read the three PDFs I will provide. For each document, produce a corpus node in Obsidian Markdown format ready to be written to the vault. Do not summarise. Do not produce a literature review. Extract only intelligence that compounds in value across research, consulting, and teaching.

## VAULT CONTEXT

The vault is an Obsidian knowledge base at `/Users/vivek/Documents/Second Brain/`. It contains:
- `07_Institutions/Corpus/` — regulatory and policy source documents (subfolders: CERT_In/, RBI/, SEBI/, NITI_Aayog/, IRDAI/, MeitY/, TRAI/, International/)
- `04_Knowledge_Products/Wiki_Intake/` — intake notes for Big 4, Big Tech, and advisory reports
- `05_Concepts/05_Concepts_Standard/` — standard concept notes
- `05_Concepts/05_Concepts_Signature/` — signature constructs (Regulatory_Parallelism, Governance_Debt, Institutional_Coherence)

**Existing corpus nodes already written (do not duplicate):**
- CERT_In/: CERT_1.md, CERT_2.md, CERT_4.md
- RBI/: RBI_1.md, RBI_2.md
- SEBI/: SEBI_9.md, SEBI_10.md, SEBI_11.md
- NITI_Aayog/: NITI_3.md, NITI_6.md

## CLASSIFICATION RULES

Apply this sequence to each document before writing a node:

**Step 1 — Out-of-scope check:**
Ask: Does this document address AI governance, data governance, cybersecurity for AI, AI regulation, or AI use cases in regulated sectors? If not, output: `[FILENAME] — OUT OF SCOPE: [reason]` and stop.

**Step 2 — Document type:**
- If it is a **regulatory instrument** (circular, direction, act, gazette notification, advisory from RBI/SEBI/CERT-In/MeitY/IRDAI/NITI Aayog or international equivalent): write a **Corpus Node** → save to `07_Institutions/Corpus/[regulator_folder]/`
- If it is a **Big 4 / Big Tech / advisory firm / industry body report**: write a **Wiki Intake Note** → save to `04_Knowledge_Products/Wiki_Intake/`
- If it is an **academic paper**: write a **Wiki Intake Note** → save to `04_Knowledge_Products/Wiki_Intake/`
- If it is a **framework or standard** (NIST, ISO, OECD, IEEE): write a **Corpus Node** → save to `07_Institutions/Corpus/International/`

**Step 3 — Metadata classification (fill all fields):**
- Jurisdiction: India / EU / US / Global / APAC / Singapore / Australia / Japan / UK / Multi-Jurisdictional
- Regulator/Source: DPB / RBI / SEBI / IRDAI / CERT-In / DPIIT / MeitY / TRAI / EU AI Office / NIST / FTC / OECD / MAS / Big4 / BigTech / Academia / Other
- Primary Wiki Section: S1 Governance Fundamentals / S2 India Regulatory / S3 International / S4 Agentic AI / S5 Data Privacy Security / S6 Implementation / S7 Use Cases / S8 Reference
- Status: Settled / Consensus / Emerging / Debate
- Confidence: High (primary regulation/official guidance) / Medium (framework/standards body) / Low (commentary/academic)
- AI explicit: Yes / No / Partial

**Step 4 — Vault folder assignment:**
| Document type | Folder |
|--------------|--------|
| RBI circular/direction | `07_Institutions/Corpus/RBI/` |
| SEBI circular/direction | `07_Institutions/Corpus/SEBI/` |
| CERT-In advisory/guideline | `07_Institutions/Corpus/CERT_In/` |
| MeitY / IndiaAI / DPDP | `07_Institutions/Corpus/MeitY/` |
| IRDAI | `07_Institutions/Corpus/IRDAI/` |
| NITI Aayog | `07_Institutions/Corpus/NITI_Aayog/` |
| TRAI | `07_Institutions/Corpus/TRAI/` |
| EU / US / NIST / OECD / international frameworks | `07_Institutions/Corpus/International/` |
| Big 4 / Big Tech / advisory / academic | `04_Knowledge_Products/Wiki_Intake/` |

## OUTPUT FORMAT — CORPUS NODE (regulatory/framework documents)

Use this exact format:

```markdown
# [SHORT_ID] — [Full Document Title]

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/[folder]/[SHORT_ID].md`
**Institution:** [[07_Institutions/[InstitutionFile]]]
**Issuing body:** [Full name]
**Document date:** [Date or year]
**Pages:** [Number if determinable]
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]] [add others as relevant]

---

## Instrument Identity

**Full title:** [exact title]
**Type:** [Master Direction / Circular / Advisory / Act / Framework / Standard]
**Target entities:** [who it binds or addresses]
**Legal basis:** [authority under which issued, if stated]
**Companion documents:** [related instruments if any]

---

## Analytical Classification

**Wiki section:** [S1–S8]
**Jurisdiction:** [from metadata]
**Confidence:** [High/Medium/Low]
**AI explicit:** [Yes/No/Partial]
**P3 corpus role:** [In canonical corpus / Screening corpus / Post-corpus / Not applicable]
**AI Governance Wiki relevance:** [HIGH/MEDIUM/LOW — one sentence why]
**Tier classification:** [Tier A = explicit AI regulation / Tier B = technology-neutral with AI application / Tier C = AI-adjacent]

---

## Substantive Content

[Structured synthesis — NOT a summary. Extract only:
- Definitions and taxonomies that will be reused
- Mandatory obligations with deontic strength (must/shall/should/may)
- Specific thresholds, timelines, penalties
- Governance structures (boards, committees, roles)
- Key provisions by section/chapter
Use headers, tables, and bullet lists. Minimum 300 words. No encyclopedic narrative.]

---

## Analytical Significance for PRIS Research

### For [most relevant project — P3/P4/fsQCA/AI Governance Wiki]
[2–4 specific sentences on how this document contributes to the named project. Be precise — what argument does it support, what gap does it fill, what evidence does it provide?]

### Regulatory Parallelism / Coordination Pattern [only if relevant]
[Does this document overlap, complement, contradict, or duplicate obligations in other vault documents? Which ones? What is the pattern?]

---

## Connections

**Related corpus nodes:** [wikilinks to existing nodes]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] [add others]
**Related frameworks:** [wikilinks]
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] [add others]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** [In canonical corpus with X RUs / Screening corpus / Not applicable]
- **Wiki intake status:** [Pending / Complete]

---

## Log

- [YYYY-MM-DD]: Corpus node created. Batch F pilot run.
```

## OUTPUT FORMAT — WIKI INTAKE NOTE (Big 4 / Big Tech / advisory / academic)

Use this exact format:

```markdown
---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
---

# [Document Short Title] — Intake Note

**Source:** [Organisation — e.g. McKinsey, Deloitte, WEF, CERAI, IBM]
**Year:** [Year]
**Full title:** [Exact document title]
**Zotero key:** [leave blank — to be added manually]
**Wiki section(s):** [S1/S2/S3/S4/S5/S6/S7]
**Confidence:** [High/Medium/Low]
**Jurisdiction:** [Global/India/EU/US/etc]

---

## Classification

**Document type:** [Industry Report / Academic Paper / Framework / White Paper / Case Study]
**Primary audience:** [Board / CRO / CISO / GC / Practitioner / Academic]
**AI explicit:** [Yes/No/Partial]

---

## 3–5 Reusable Findings

[Each finding must be:
- A specific, citable claim — not a general observation
- Directly usable in a wiki section, concept note, or consulting/teaching context
- Expressed in one to three sentences
- Labelled with the wiki section it feeds]

1. **[Finding title]** (feeds S[X]): [Specific claim. What does the document actually say? Quote the key phrase in quotation marks if under 15 words, or paraphrase precisely.]

2. **[Finding title]** (feeds S[X]): [Specific claim.]

3. **[Finding title]** (feeds S[X]): [Specific claim.]

[Add 4th and 5th only if genuinely distinct and reusable]

---

## Consulting/Teaching Reuse

**Highest-value reuse opportunity:** [One sentence: what can be extracted from this document that is directly usable in an engagement or classroom in the next 6 months?]

**Relevant inbound connections:** [AEGIS_OS / PrivacyWeave / CyberMesh / other — or None]

---

## Cross-Links

**Related wiki sections:** [[AI_Governance_Wiki]] S[X]
**Related concepts:** [wikilinks]
**Related corpus nodes:** [wikilinks to existing vault nodes]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] [add others]

---

## Processing Status

- [ ] PDF in Zotero
- [ ] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to relevant concept notes
- [ ] Marked processed

---

## Log

- [YYYY-MM-DD]: Intake note created. Batch F pilot run.
```

## QUALITY CHECK INSTRUCTIONS

After producing the three nodes, output a one-paragraph quality note for each:
- Did you find enough substantive content to write a useful node, or was the document too thin?
- Are there any claims you were uncertain about — thresholds, dates, penalties — that need verification?
- Did this document significantly overlap with an existing vault node? (If so, name which one.)
- What is the single most reusable finding for consulting or teaching?

---

**Now read the three PDFs and produce the three nodes.**

---

---

# PROMPT 2 — CLASSIFICATION SWEEP (10–15 Documents)

**Use for:** Batch classification of a folder or document set before vault node generation. Run this first; review the table; then run Prompt 3.

**Copy everything below the dashed line into Cowork or Claude:**

---

You are a corpus classification agent for PRIS (Personal Regulatory Intelligence System). Your task is to classify a batch of documents against the AI Governance Wiki classification schema, producing a structured table that will guide vault node generation in the next step.

## WHAT TO PRODUCE

A classification table — one row per document. No node generation yet. No synthesis yet. Classification only.

## CLASSIFICATION SCHEMA

For each document, determine:

| Field | Options |
|-------|---------|
| File ID | Assign sequentially: F001, F002, F003... (continuing from existing A001–E033) |
| Short title | 3–6 word descriptive label |
| Source / Issuer | Organisation name |
| Document type | Regulatory Instrument / Framework-Standard / Industry Report / Academic Paper / White Paper / Government Strategy / Advisory |
| Jurisdiction | India / EU / US / Global / APAC / Singapore / Australia / Japan / UK / Multi |
| Primary wiki section | S1 / S2 / S3 / S4 / S5 / S6 / S7 / S8 |
| AI explicit | Yes / No / Partial |
| Confidence | High / Medium / Low |
| Vault destination | `07_Institutions/Corpus/[subfolder]/` or `04_Knowledge_Products/Wiki_Intake/` |
| Node type | Corpus Node / Wiki Intake Note |
| In-scope | Yes / No |
| Out-of-scope reason | [if No — one phrase] |
| Priority | 🔴 Critical / 🟡 High / 🟢 Normal |
| Estimated reuse | Research / Consulting / Teaching / LinkedIn / Multiple |

## PRIORITY RULES

Mark 🔴 Critical if the document:
- Is a primary regulatory instrument from RBI, SEBI, IRDAI, CERT-In, MeitY, DPB, or DPDP
- Is explicitly cited in the AI Governance Wiki v2.2 as a source (Batch A–E file IDs)
- Directly addresses agentic AI governance (feeds `Agentic_AI_Governance.md` concept node)
- Contains BFSI-specific AI governance content (feeds P3 or BFSI AI Governance Handbook)

Mark 🟡 High if the document:
- Is a major international framework (NIST, OECD, EU AI Act, UNESCO)
- Is a Big 4 / Big Tech report on Indian AI governance or BFSI AI
- Addresses DPDP, data localisation, or privacy governance for AI

Mark 🟢 Normal for everything else in scope.

## OUT-OF-SCOPE CRITERIA

Mark out-of-scope if the document primarily addresses:
- Military doctrine, weapons systems, or defence procurement (not governance framing)
- Quantum cryptography without AI governance intersection
- Pure product management or project management methodology
- General cybersecurity without AI-specific content
- Social media regulation without AI component

## OUTPUT FORMAT

Produce the classification table in Markdown. Then, below the table, add:

**Batch summary:**
- Total documents: [N]
- In scope: [N]
- Out of scope: [N] — list filenames
- 🔴 Critical priority: [N] — list short titles
- 🟡 High priority: [N] — list short titles
- Documents that overlap with existing vault nodes: [list — note which existing node]
- Recommended processing order for next session: [ranked list of top 10 by priority]

---

**Now classify the documents I am providing.**

---

---

# PROMPT 3 — VAULT NODE GENERATION (from classification table)

**Use for:** Converting a completed classification table (from Prompt 2) into vault-ready corpus nodes and intake notes. Run after reviewing the Prompt 2 table.

**Copy everything below the dashed line into Cowork or Claude:**

---

You are a vault node generation agent for PRIS (Personal Regulatory Intelligence System). You have a completed classification table from a prior session. Your task is to generate vault-ready Obsidian Markdown nodes for a specified subset of documents, then write them directly to the vault using the filesystem MCP tool.

## VAULT WRITE INSTRUCTIONS

The filesystem MCP is active. Write each completed node directly to its target path. Do not output nodes as chat text — write them to disk. After writing each file, confirm: `✓ Written: [filepath]`.

Target paths by document type:
- RBI instruments → `/Users/vivek/Documents/Second Brain/07_Institutions/Corpus/RBI/[ID].md`
- SEBI instruments → `/Users/vivek/Documents/Second Brain/07_Institutions/Corpus/SEBI/[ID].md`
- CERT-In instruments → `/Users/vivek/Documents/Second Brain/07_Institutions/Corpus/CERT_In/[ID].md`
- MeitY / DPDP / IndiaAI → `/Users/vivek/Documents/Second Brain/07_Institutions/Corpus/MeitY/[ID].md`
- IRDAI → `/Users/vivek/Documents/Second Brain/07_Institutions/Corpus/IRDAI/[ID].md`
- NITI Aayog → `/Users/vivek/Documents/Second Brain/07_Institutions/Corpus/NITI_Aayog/[ID].md`
- International frameworks (NIST, OECD, EU AI Act, UNESCO) → `/Users/vivek/Documents/Second Brain/07_Institutions/Corpus/International/[ID].md`
- Big 4 / Big Tech / advisory / academic → `/Users/vivek/Documents/Second Brain/04_Knowledge_Products/Wiki_Intake/[ShortTitle].md`

## DOCUMENTS TO PROCESS THIS SESSION

[INSTRUCTION: Paste the subset of rows from the Prompt 2 classification table that you want processed in this session. Process 🔴 Critical documents first. Limit to 8–10 documents per session to maintain synthesis quality.]

## EXISTING VAULT NODES (do not duplicate)

The following corpus nodes already exist. When generating new nodes, link to these where relevant but do not recreate them:

**CERT_In:** CERT_1.md (CIAD-2023-0015 LLM Security) | CERT_2.md (CIAD-2025-0013 GenAI Best Practices) | CERT_4.md (SBOM/AIBOM/HBOM/QBOM/CBOM v2.0)  
**RBI:** RBI_1.md (IT Governance Master Direction 2023) | RBI_2.md (IT Outsourcing Master Direction 2023)  
**SEBI:** SEBI_9.md (AI/ML Reporting MIIs Jan 2019) | SEBI_10.md (AI/ML Reporting Mutual Funds May 2019) | SEBI_11.md (AI Responsibility Board Memo 2024–25)  
**NITI_Aayog:** NITI_3.md (Responsible AI Part 2 Aug 2021) | NITI_6.md (Enforcement Mechanisms Draft Jan 2021)

## EXISTING CONCEPT NODES (link to these where relevant)

**Signature:** Regulatory_Parallelism | Governance_Debt | Institutional_Coherence  
**Standard:** Accountability | Transparency | Governance_Capacity | Legitimacy | Agentic_AI_Governance

## ACTIVE CONSULTING CONNECTIONS (flag if a document feeds these)

- AEGIS_OS_Inbound — runtime enforcement, pre-execution governance, PQC, audit trails
- PrivacyWeave_Inbound — runtime data usage control, DPDP purpose limitation, audit trail
- CyberMesh_PS69_Inbound — distributed trust, zero-trust, incident response (🔴 HOLD — research only)
- CyberMesh_PS74_Inbound — cyber deception, AI/ML detection, policy-governed response (🔴 HOLD — research only)

## CORPUS NODE FORMAT

For each regulatory instrument or international framework, write this exact structure:

```markdown
# [FILE_ID] — [Full Document Title]

**Type:** Corpus Node
**Vault path:** `[target path]`
**Institution:** [[07_Institutions/[InstitutionFile]]]
**Issuing body:** [Full institutional name]
**Document date:** [Date]
**Pages:** [N]
**Domain:** [[03_Domains/AI_Governance]] [add others]

---

## Instrument Identity

**Full title:** [exact]
**Type:** [instrument type]
**Target entities:** [who it binds]
**Legal basis:** [authority]
**Companion documents:** [related instruments]

---

## Analytical Classification

**Wiki section:** [S1–S8]
**Jurisdiction:** [jurisdiction]
**Confidence:** [High/Medium/Low]
**AI explicit:** [Yes/No/Partial]
**P3 corpus role:** [canonical / screening / post-corpus / not applicable]
**AI Governance Wiki relevance:** [HIGH/MEDIUM/LOW — one sentence]
**Tier classification:** [Tier A / Tier B / Tier C]

---

## Substantive Content

[Structured synthesis. Headers and tables. Mandatory provisions clearly distinguished from recommendations. Specific thresholds, timelines, penalties extracted. No narrative padding. Minimum 300 words.]

---

## Analytical Significance for PRIS Research

### [Most relevant project]
[2–4 precise sentences. What argument does this support? What evidence does it provide?]

### Coordination / Parallelism Pattern [if applicable]
[Does this overlap with or contradict an existing vault node? Name it. What is the pattern type: Convergence / Parallelism / Contradiction / Unidirectional / Unpaired?]

### Consulting Connection [if applicable]
[Does this feed AEGIS, PrivacyWeave, or CyberMesh advisory framing? One sentence.]

---

## Connections

**Related corpus nodes:** [wikilinks]
**Related concepts:** [wikilinks]
**Related frameworks:** [wikilinks]
**Related projects:** [wikilinks]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** [wikilinks if applicable]

---

## Coding Status

- **P3 NVivo:** [status]
- **Wiki intake:** [Pending / Complete]

---

## Log

- [YYYY-MM-DD]: Corpus node created. Batch [F/G/H]. [Session ID].
```

## WIKI INTAKE NOTE FORMAT

For each Big 4 / Big Tech / advisory / academic document:

```markdown
---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
---

# [Short Title] — Intake Note

**Source:** [Organisation]
**Year:** [Year]
**Full title:** [Exact title]
**File ID:** [F001 etc from classification table]
**Zotero key:** [leave blank]
**Wiki section(s):** [S1–S8]
**Confidence:** [High/Medium/Low]
**Jurisdiction:** [jurisdiction]

---

## Classification

**Document type:** [type]
**Primary audience:** [audience]
**AI explicit:** [Yes/No/Partial]

---

## 3–5 Reusable Findings

[Numbered. Each: specific, citable, one to three sentences. Label which wiki section each feeds. Paraphrase — no verbatim reproduction.]

1. **[Finding label]** (feeds S[X]): [Claim.]
2. **[Finding label]** (feeds S[X]): [Claim.]
3. **[Finding label]** (feeds S[X]): [Claim.]

---

## Consulting/Teaching Reuse

**Highest-value reuse:** [One sentence.]
**Consulting connections:** [AEGIS / PrivacyWeave / CyberMesh / None]
**Teaching connection:** [Case study / Framework / Example — or None]

---

## Cross-Links

**Wiki sections:** [[AI_Governance_Wiki]] S[X]
**Concepts:** [wikilinks]
**Corpus nodes:** [wikilinks to existing nodes]
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Processing Status

- [ ] PDF in Zotero
- [ ] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes
- [ ] Marked processed

---

## Log

- [YYYY-MM-DD]: Intake note created. Batch [F/G/H]. [Session ID].
```

## SESSION COMPLETION CHECKLIST

After writing all nodes for this session, output:

```
SESSION SUMMARY — Batch [F/G/H]
================================
Files written to vault: [N]
  - Corpus nodes: [N] → [list filenames]
  - Wiki intake notes: [N] → [list filenames]

New connections to existing vault nodes:
  - [New node] → [existing node]: [relationship type]

Concept notes that should be updated or created based on this batch:
  - [concept]: [why — what this batch adds]

Documents flagged for manual review:
  - [filename]: [reason — uncertain claim / needs legal verification / possible duplication]

Recommended priority for next batch:
  1. [document]
  2. [document]
  3. [document]

Session handoff note updated in: 00_MOC/Session_Handoffs/Session_Handoff_Current.md (single rolling file — overwrite, do not create a new dated file; see DJ-11 in Decision_Journal.md)
```

---

**Now process the documents listed in the classification table subset above. Write each file directly to the vault. Confirm each write.**

---

---

## USAGE NOTES FOR VIVEK

### Session sizing
- Pilot (Prompt 1): 3 documents per run. Always run first.
- Classification sweep (Prompt 2): 10–15 documents per run.
- Node generation (Prompt 3): 8–10 documents per run. Quality degrades above 10.
- Full corpus of ~80 documents = approximately 8–10 Prompt 3 sessions.

### Folder-first batching (recommended order)
Process one folder at a time from the Finder corpus. Suggested sequence:

| Session | Folder | Estimated docs | Priority |
|---------|--------|---------------|----------|
| F-01 | Regulations/ | 8–12 | 🔴 — primary regulatory instruments |
| F-02 | AI Agents/ | 8–10 | 🔴 — feeds Agentic_AI_Governance concept node |
| F-03 | Frameworks/ | 6–8 | 🟡 — NIST, OECD, ISO, EU |
| F-04 | Cybersecurity/ | 6–8 | 🟡 — feeds CERT-In and cybersecurity domain |
| F-05 | Third Party Advisory/ | 8–10 | 🟡 — Big 4 / Big Tech whitepapers |
| F-06 | Papers/ | 8–10 | 🟢 — academic literature |
| F-07 | Country Documents/ | 6–8 | 🟢 — Japan, Singapore, Australia comparators |
| F-08 | Academia Reports/ | 6–8 | 🟢 — secondary academic |
| F-09 | Threat Outlook/ | 4–6 | 🟢 — cybersecurity threat intelligence |
| F-10 | Big Tech/ | 4–6 | 🟢 — Google, Microsoft, OpenAI papers |

### What to verify manually before accepting any node
Three categories of claim require human verification before a node is committed to the vault:
1. **Penalty figures** (rupee amounts, percentage of turnover) — verify against primary instrument text
2. **Notification timelines** (hours/days) — verify against primary instrument text; do not rely on secondary sources
3. **Scope statements** ("applies to all banks" vs "applies to scheduled commercial banks only") — check exact target entity definition

These are the categories where the wiki v2.0 had to retire three claims from v1.0 (the 6-hour DPDP breach SLA, the INR 50 crore penalty figure, the blanket data localisation mandate). Verify before vault-writing.

### When to run Prompt 2 vs skip straight to Prompt 3
Run Prompt 2 (classification sweep) when:
- Processing a mixed folder (multiple document types, multiple jurisdictions)
- You have more than 8 documents to process
- You are unsure whether documents are in or out of scope

Skip Prompt 2 and go straight to Prompt 3 when:
- All documents in the batch are the same type (e.g., all RBI circulars)
- You know exactly which vault folder they belong to
- The batch is 5 or fewer documents

---

_Back to [[Wiki_Intake_Index]] | [[AI_Governance_Wiki]]_

## Log

- 2026-06-14: Prompt file created. S6 session. Three prompts: Pilot, Classification Sweep, Node Generation.
