---
type: Process Document
status: active
last_updated: 2026-08-15
tags:
  - type/process-document
  - status/active
  - engine/phd
---

# Open-Flag Resolution Register & Sourcing Prompts — 2026-08-15 (fourth pass)

**Parent:** [[Thin_Node_Perplexity_Prompts_2026-08-02]] (pass 1) · [[Sector_Gap_Audit_Perplexity_Prompts_2026-08-02]] (pass 2) · [[Missing_Node_and_Tier_Audit_Perplexity_Prompts_2026-08-02]] (pass 3)

**Why a fourth pass.** Passes 1–3 asked *what is missing from the vault*. This pass asks a different question: **what is already written but not yet safe to publish.** The 2026-08-09 session produced five synthesis artefacts and four corrections in a single day; the 2026-08-15 housekeeping session found 64 nodes invisible to the index. Neither problem is a sourcing problem. The binding constraint has moved from **generation** to **closure**.

**Method.** Every open ⚠ flag, decision item and standing task across `Session_Handoff_Current.md`, the Backfill Register in [[Corpus_Index_MOC]], and the notes themselves, triaged onto exactly one of three channels:

| Channel | Meaning | Count |
|---|---|---|
| **P** | External sourcing — needs a document retrieved or a fact checked outside the vault. Prompts in §2. | 11 |
| **V** | Vault-internal — a Cowork/Claude session can execute against existing material. Briefs in §3. | 8 |
| **X** | **Vivek-only** — requires your access, your memory, or your judgment. No agent can do these. §4. | 8 |

**Rule:** a flag is not closed until it is recorded closed **in the node that raised it**, not merely here. See §6.

---

## 1. Triage table — every open item

🔴 = blocks publication-track use · 🟡 = blocks a specific artefact · 🟢 = hygiene

| Flag / item | What is open | Sev | Channel | Gates |
|---|---|---|---|---|
| **⚠#339** | C-02 circulation check — the false *"WDR 2026 never cites India"* claim may have reached P1 draft text, LinkedIn (since 5 Aug), or supervisor correspondence | 🔴 | **X-01** | External credibility |
| **⚠#304** | NABCB / ISO/IEC 42006 contradiction — Parliament_2 (ministerial record, 5 Aug 2026) says an operational AIMS accreditation framework exists; [[06_Frameworks/ISO_IEC_42001]] (sourced via UKAS, 2 Aug) says it does not | 🔴 | **P-01** | ISO_IEC_42001, Parliament_2, CEA_3 |
| **⚠#310** | CEA_3's AI null finding rests on a Devanagari-corrupted bilingual Gazette OCR | 🔴 | **P-02** | CEA_3 headline claim |
| **⚠#351** | [[04_Knowledge_Products/Wiki_Intake/F143_Bradford_Digital_Empires_2023]] written with **no primary text** | 🔴 | **X-07** + **P-10** | Whole node |
| **⚠#329** | F142 (Azimi) states *"NOT FOR CITATION WITHOUT PERMISSION"* twice; no affiliation or contact given | 🔴 | **P-11** → **X-08** | P1, P4, proposals, decks |
| **⚠#320** | Microsoft AI-native security architecture (Signals→Context→Models→Harness→Agents→Actuators) has **no corpus node** — [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] quotes your own carousel | 🟡 | **P-04** | Orchestration_Governance |
| **⚠#322** | [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]]'s NPCI gate instance rests on trade reporting, not a primary instrument | 🟡 | **P-05** | Gate passes without it — drop or source |
| **⚠#324** | OQ-DI-02 — *does any jurisdiction govern decision chains as such?* Unchecked and **load-bearing** on the novelty claim | 🟡 | **P-06** | Decision_Infrastructure abstract |
| **⚠#326** | [[04_Knowledge_Products/Minimum_Evidence_Register_Autonomous_AI]]'s ❌ codings assert corpus-wide absence | 🟡 | **P-07** | Board-facing artefact |
| **⚠#335 / #344** | *Utkarsh 2029* cited in RBI_14 para 2 as the source of a deferred AI-model commitment; not in vault. Lineage (2022 → 2.0 → 2029) inferred, not confirmed | 🟡 | **P-03** | RBI binding-AI roadmap dating |
| **⚠#314** | CERT-In *15 Elemental Cyber Defense Controls for MSMEs* cited by CEA_3 reg 2(1)(a), absent from vault. Also: CERT-In 28 Apr 2022 Directions, flagged blocking in [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] since 2 Aug | 🟡 | **P-08** | Retention_Horizon_Divergence |
| **⚠#343** | Peru Law 31814 + Supreme Decree 115-2025-PCM — mandatory digital-security audits of public-administration AI, structurally close to RBI_14 | 🟢 | **P-09** | Comparative set |
| **⚠#340 / #342** | GRIDMAP is the Data Markets Module (data protection), not AI markets; Bangladesh entry needs a live status check | 🟢 | **P-14** | International_38 |
| **⚠#347** | S/F/X recode is **single-coder**, no reliability statistic | 🟡 | **V-05** / **X-03** | The 5:4:1 split as a *coded* result |
| **⚠#348** | The "opportunity" qualifier in the F code is not independently operationalised (instances 1, 2, 9) | 🟡 | **V-05** | Recode defensibility |
| **⚠#349 / #350** | Instance 7 cross-sector coding assumption; only 10 of 23 P3 pairs recoded | 🟢 | **V-05** | Scope statement |
| **⚠#352 / #353** | Bradford India-treatment inferred from taxonomy structure, not index; *Brussels Effect* (2020) also absent from vault | 🟡 | **P-10** | F143 Findings 3 |
| **⚠#290** | P2_References #7 — Masiero (2020) journal-name cross-contamination with F127 | 🟡 | **X-02** | P2 |
| **P2 #10** | Confirmed citation mix-up — non-existent Seetharaman/Mathew/De' paper conflated with F128 | 🔴 | **X-02** | P2 submission |
| **D1** | `[[NIST_AI_RMF]]` — 44 bare links resolve ambiguously; Obsidian sends all to the Shared Anchor | 🟢 | **X-06** → **V-02** | Graph integrity |
| **D3 / B1** | `Wiki_Intake_Index.md` stale (12 Jun, how-to not index); **24 of 64** backfilled nodes carry no Wiki section / Tier | 🟢 | **V-03 / V-01** | Wiki routing |
| **RRA** | [[05_Concepts/05_Concepts_Signature/Records_Rules_Asymmetry]] downgraded to candidate July 2026. **A UIDAI corpus node now exists** (`UIDAI_1`) and MeitY runs to MeitY_8 — Option A is partly satisfied and nobody noticed | 🟡 | **V-04** | Re-elevation to signature |
| **RBI dup** | [[07_Institutions/Corpus/RBI/RBI_3]] and `RBI_13` are the same instrument. Flagged on both, **not merged** per standing protocol | 🟢 | **X-05** → **V-06** | Corpus integrity |
| **OQ-09** | fsQCA 10-case list lock — **revised deadline 1 Sep 2026, now 17 days out** | 🔴 | **X-04** | fsQCA chapter |
| **Aadhaar** | Aadhaar Authentication Regulations 2016 — flagged missing *"before P2 submission"*, status unconfirmed | 🟡 | **P-12** | P2 |
| **VERIFY state** | Flag numbering is **not authoritative** anywhere. Historical trackers stale; flags scattered across nodes | 🟡 | **V-07** | All flag accounting |
| **Housekeeping** | `_to_delete/` (163 files) staged but not deleted; `MoHFW.md` institution root missing; CERT-In legacy/new naming split; Karnataka_Govt_2 status unknown | 🟢 | **X-05 / V-08 / P-13** | — |

---

## 2. External sourcing — ready-to-paste prompts

> Run in **Perplexity Deep Research** unless noted. Paste the output back into a Cowork session with the flag number; do **not** let the model write the node — the extraction goes into Format A/B here, under the ⚠ protocol.

---

### P-01 🔴 NABCB / ISO/IEC 42006 — resolve the contradiction (⚠#304)

```
Establish, from primary sources only, whether India's National Accreditation Board for
Certification Bodies (NABCB) operates an accreditation programme for certification bodies
auditing AI Management Systems against ISO/IEC 42001, and whether ISO/IEC 42006 has been
published.

Answer these separately and cite a dated, named document for each:
1. Has ISO/IEC 42006 (requirements for bodies auditing and certifying AI management
   systems) been published as a full International Standard? If not, what is its current
   ISO stage code and date? If yes, give publication date and edition.
2. Does NABCB publish a named, dated accreditation scheme document for AIMS / ISO 42001
   certification bodies? Search nabcb.qci.org.in and qcin.org directly. Give the document
   title, reference number and date, or state that none is published.
3. List any NABCB-accredited certification bodies for ISO/IEC 42001 as at August 2026.
4. Does NABCB or any other Indian body act as the accreditation authority for the
   "Technical Criteria Certificate" under the Central Electricity Authority (Cyber Security
   in Power Sector) Regulations, 2026, reg 3(1)(jj)?
5. On 5 August 2026 the Minister of State for Electronics and IT answered Lok Sabha
   Unstarred Question No. 2988 stating that an institutional framework for auditing AI
   exists involving NABCB and ISO/IEC 42006. Quote the relevant passage of that answer
   verbatim from the Lok Sabha website and state whether it asserts an operational scheme
   or a planned one.

Distinguish throughout between: published standard / draft standard / announced intent /
operational accreditation programme. Do not treat a press release or news article as
evidence of an operational scheme. If sources conflict, say so and give both.
```

**On return:** update [[06_Frameworks/ISO_IEC_42001]] and `Parliament_2` together. Do **not** silently prefer one source — the handoff is explicit on this.

---

### P-02 🔴 CEA_3 clean text — re-run the AI null sweep (⚠#310)

```
Locate the authoritative, machine-readable English text of the Central Electricity
Authority (Cyber Security in Power Sector) Regulations, 2026 — notified 31 July 2026,
Gazette No. 484. Prioritise the CEA-hosted PDF at cea.nic.in over the bilingual Gazette
scan. Give direct download URLs for every version you find, and state which is
English-only versus bilingual Hindi/English.

Then confirm, against the English text: do the terms "artificial intelligence", "AI",
"machine learning", "ML", "algorithm", "algorithmic", "automated decision", "model", or
"autonomous" appear anywhere in the 17 regulations, 40 definitions, or 2 Schedules?
Quote every occurrence with its regulation number, or state explicitly that there are none.

Also confirm: which six regulations have no commencement date and are deferred to separate
Authority orders? Have any such orders been issued as at 15 August 2026?
```

**Why first-tier:** the AI-silence finding is CEA_3's headline contribution and the corpus's strongest *deliberate omission with notice* instance. It currently rests on OCR.

---

### P-03 🟡 Utkarsh 2029 (⚠#335, ⚠#344)

```
Locate the Reserve Bank of India's medium-term strategy framework "Utkarsh 2029" as a
primary document. Give the direct rbi.org.in URL, launch date, and the Governor's foreword
date.

Then:
1. Quote paragraph I.10 verbatim. RBI's Draft Guidance on Regulatory Principles for Model
   Risk Management (June 2026) cites it at para 2 as the source of a commitment that
   further AI-model requirements may follow. Confirm or refute that characterisation.
2. Confirm the edition lineage: Utkarsh 2022 (launched July 2019) → Utkarsh 2.0 (2023–25,
   foreword 30 Dec 2022) → Utkarsh 2029. Is Utkarsh 2029 the immediate successor to
   Utkarsh 2.0, or does an intervening edition exist? Cite RBI's own statement of the
   sequence, not an inference.
3. List every reference to artificial intelligence, machine learning, SupTech or RegTech
   in Utkarsh 2029, with paragraph numbers.
```

---

### P-04 🟡 Microsoft AI-native security architecture (⚠#320)

```
Identify the primary Microsoft publication that sets out an AI-native security architecture
organised as a layered stack of Signals, Context, Models, Harness, Agents and Actuators
(or closely equivalent named layers). Likely candidates include Microsoft Security blog
posts, Microsoft Ignite or Build session material, the Microsoft Digital Defense Report,
Security Copilot architecture documentation, or a Microsoft AI Red Team publication,
2024–2026.

Give: exact title, author or team, publication date, canonical microsoft.com URL, and the
verbatim naming of each layer. If Microsoft names the layers differently, give Microsoft's
own terms and note the divergence.

Then state specifically what Microsoft says about governance, approval or authorisation of
the orchestration/harness layer — who approves which workflows an orchestrator may run,
who may change them, and whether orchestration decisions are logged or reconstructable.
Quote directly. If Microsoft does not address these, say so.
```

**Why it matters:** [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] currently cites your own carousel for its central taxonomy. Format B node, not Format A.

---

### P-05 🟡 NPCI as a governed decision-infrastructure operator (⚠#322)

```
Establish, from primary sources, what artificial-intelligence or machine-learning systems
the National Payments Corporation of India (NPCI) operates in production — particularly
federated or network-level fraud scoring across UPI — and what governance instrument, if
any, binds NPCI in respect of them.

Answer separately:
1. NPCI's own primary statements (circulars, annual reports, press releases, procurement
   or tender documents) describing AI/ML fraud detection on UPI. Give document title, date
   and URL. Quote the operative description.
2. Whether any RBI Master Direction, circular or guideline imposes AI-specific obligations
   on NPCI as an operator, as distinct from obligations on banks and PSPs. Name the
   instrument and provision, or state that none exists.
3. NPCI's legal character and regulatory status — Section 8 company; authorised under the
   Payment and Settlement Systems Act 2007; whether designated a critical information
   infrastructure under the IT Act; whether it is a "regulated entity" for the purposes of
   RBI's AI-adjacent instruments.
4. Whether the RBI (Digital Payment Security Controls) Directions 2021 or the RBI
   Cybersecurity Directions 2026 (notified 31 July 2026) apply to NPCI by their own terms.

Do not infer obligations from general sectoral guidance. Either a named instrument reaches
NPCI as operator, or it does not.
```

---

### P-06 🟡 OQ-DI-02 novelty check — the load-bearing one (⚠#324)

```
Determine whether any jurisdiction regulates AI *decision chains* as such — that is, an
instrument whose unit of regulation is the sequence from data through model to workflow to
decision to institutional action, rather than the model, the system, the provider, or the
use case.

Search systematically across: EU (AI Act, DORA, GDPR Art. 22), United States (federal and
state, including Colorado SB 24-205, California SB 53, NYC Local Law 144), United Kingdom,
Canada (AIDA), China, Singapore (MAS FEAT, IMDA), Japan, Korea, Brazil (PL 2338), India,
and sectoral regulators (BIS, IOSCO, FSB, NAIC, EIOPA, IAIS).

For each candidate, state precisely what the regulated unit is in the instrument's own
words, and whether the instrument reaches: (a) automated decision-making as an output;
(b) the workflow or orchestration that produces it; (c) the institutional action taken on
it; (d) the handoff points between these.

The distinction that matters: GDPR Art. 22 regulates a decision's *effect on a person*.
An instrument regulating decision chains would regulate the *architecture* that produces
decisions. Report any instrument that does the latter. If none does, state that
explicitly — that is the finding being tested.

Also search the academic literature (Information Systems, regulation & governance, law &
technology, 2020–2026) for the terms "decision infrastructure", "decision chain
governance", "decision pipeline accountability" as governance constructs, and report prior
art with full citations.
```

**This is the highest-leverage prompt here.** If a jurisdiction does govern decision chains, [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]]'s contribution weakens from *"identifies an ungoverned layer"* to *"documents India's absence"* — a materially different abstract.

---

### P-07 🟡 Minimum Evidence Register — confirm the ❌ codings (⚠#326)

```
For each of the six evidence records below, determine whether ANY binding or draft Indian
regulatory instrument requires it. Search RBI, SEBI, IRDAI, MeitY, CERT-In, NPCI, UIDAI,
BIS and the DPDP Rules 2025.

1. Agent identity — a register or unique identifier for autonomous software agents
2. Model version — retained record of which model version produced an output
3. Delegation approval — recorded authorisation of what an agent may do on whose authority
4. Orchestration workflow — retained record of the workflow an orchestrator executed
5. Permitted actions — an enumerated scope of actions an agent may take
6. Runtime evidence — logs sufficient to reconstruct an automated decision after the fact

Give the instrument, provision number and verbatim text where a requirement exists. Where
none exists, say so explicitly.

Check these two specifically, as they are the most likely to have changed:
- The IRDAI Working Group on AI — has it reported? Report due approximately 18 September
  2026. If a report or exposure draft is out, what does it require on record-keeping?
- SEBI's Cybersecurity and Cyber Resilience Framework (CSCRF) — does it mandate any
  AI-specific artefact class, or is it technology-neutral?

Also state whether any instrument specifies the *evidentiary destination* of a retained
artefact — i.e. whether it must satisfy supervisory inspection or legal admissibility
under Bharatiya Sakshya Adhiniyam s.63.
```

---

### P-08 🟡 CERT-In — two missing instruments (⚠#314)

```
Retrieve two CERT-In documents as primary sources with direct cert-in.org.in URLs:

1. The CERT-In Directions of 28 April 2022 under section 70B(6) of the IT Act 2000
   (No. 20(3)/2022-CERT-In). Give the full text of the log-retention obligation — the
   180-day / 180-days-within-Indian-jurisdiction provision — verbatim, with its clause
   number, plus the six-hour incident-reporting clause. Also state which entities it binds
   and whether it has been amended, superseded or supplemented since April 2022.

2. "15 Elemental Cyber Defense Controls for MSMEs", cited at reg 2(1)(a) of the CEA (Cyber
   Security in Power Sector) Regulations, 2026. Give the exact title, issue date, version,
   URL, and list the fifteen controls. Confirm whether any control addresses AI, machine
   learning or automated decision systems.

For both: state whether the document specifies what retained logs are FOR — supervisory
inspection, incident response, or legal proof.
```

---

### P-09 🟢 Peru — Law 31814 and its implementing decree (⚠#343)

```
Retrieve as primary sources: Peru's Law No. 31814 (promoting the use of artificial
intelligence for economic and social development) and Supreme Decree No. 115-2025-PCM.
Give official El Peruano URLs, promulgation and entry-into-force dates.

Focus on: the mandatory digital-security audit requirement for AI systems used in public
administration — who must audit, how often, against what criteria, who accredits auditors,
and what the audit output must contain. Quote the operative articles.

Then compare structurally against RBI's Draft Guidance on Regulatory Principles for Model
Risk Management (June 2026), specifically its para 46(i) requirement of independent
validation "notwithstanding any validation, certification, or assurance provided by the
third-party provider". Does Peru's regime also refuse assurance reuse, or does it accept
third-party certification?
```

---

### P-10 🟡 Bradford — pending the book itself (⚠#351, #352, #353)

> This does **not** substitute for the primary text (see X-07). It scopes what to read.

```
For Anu Bradford, "Digital Empires: The Global Battle to Regulate Technology" (Oxford
University Press, 2023, ISBN 9780197649268):

1. Give the full table of contents, chapter by chapter with page ranges.
2. Report, from reviews and from any searchable index or excerpt, how substantially the
   book treats India — is India discussed as a distinct regulatory actor, as a battleground
   between the three empires, or largely in passing? Cite reviewers who comment on this.
   Do NOT assert that the book omits India unless a source states so directly.
3. Summarise the principal scholarly criticisms of the three-model taxonomy from peer
   reviews 2023–2026, particularly any arguing the taxonomy fails for large non-Western
   jurisdictions that are simultaneously rule-makers and rule-takers.
4. Distinguish the argument of "Digital Empires" (2023) from "The Brussels Effect" (2020),
   and advise which is the correct anchor for a systematic literature review positioning
   an argument about *intra-jurisdictional* regulatory divergence in India.
5. Locate any response by Bradford, 2024–2026, to arguments that regulatory competition is
   the wrong frame — including any response to World Bank WDR 2026 Box 9.4.
```

---

### P-11 🔴 F142 — locate the author (⚠#329)

```
Identify Behnaz Azimi, author of the July 2026 working paper "How Old Is Your AI
Governance? A Conceptual Investigation into the Temporal Validity of Governance Frameworks
for Continuously Evolving AI Systems". The paper states no affiliation and gives no contact
details, and is marked "NOT FOR CITATION WITHOUT PERMISSION".

Find: institutional affiliation, ORCID, academic or professional email, and where the paper
was posted (arXiv, SSRN, ResearchGate, institutional repository, conference). Give the
canonical version and confirm whether a later version exists WITHOUT the citation
restriction, and whether the reference list is populated in any version — the copy held
carries zero references.
```

**Then X-08:** you write to the author for citation permission. Nothing in P1/P4/proposals/decks until that is in writing.

---

### P-12 🟡 Aadhaar Authentication Regulations 2016 — currency check

```
Retrieve the Aadhaar (Authentication) Regulations, 2016 as a primary source from
uidai.gov.in. Give the gazette reference and date.

Then establish its current status: list every amendment through August 2026, including the
Aadhaar (Authentication and Offline Verification) Regulations 2021 and any 2025–26
amendment, and state whether the 2016 Regulations remain in force, are amended, or are
superseded. Give the currently operative instrument.

Report specifically: obligations on requesting entities regarding authentication records —
what must be retained, for how long, and in what form; any provision on automated or
AI/ML-based authentication (including face authentication); and any audit or inspection
provision. Quote regulation numbers.
```

---

### P-13 🟢 Karnataka — second AI instrument status

```
Determine whether the Government of Karnataka has published an AI policy, framework,
regulation or committee report subsequent to the 2026 instrument already held. Search
karnataka.gov.in, the Department of Electronics IT BT and S&T, and the Karnataka
Responsible AI Committee. Give document titles, dates and URLs, or state that none has
been published as at 15 August 2026.
```

---

### P-14 🟢 WDR 2026 residuals (⚠#340, ⚠#342)

```
Two narrow checks against World Bank sources:
1. GRIDMAP — the World Bank's Global Regulatory Indicators for Digital Markets and
   Platforms. Confirm which modules exist and have been published. The Data Markets Module
   assesses data protection. Is there any published or announced module assessing AI
   markets or AI governance specifically? Give the module names, publication dates and
   economy coverage.
2. Bangladesh — what is the current status of its AI governance instrument as referenced in
   WDR 2026 Spotlight 7? Draft, adopted, or in force, as at August 2026? Give the
   instrument name, issuing body and date.
```

---

## 3. Vault-internal briefs — issue these to a Cowork session

| # | Brief | Prereq |
|---|---|---|
| **V-01** | Classify the **24 backfilled nodes** carrying no `Wiki section` and/or no `Tier classification` (Backfill Register item **B1**) — mostly the 2026-08-02 missing-institutions pass: `Grid_India_1`, `BIS_1`, `DPB_1`, `Sahamati_1`, `UIDAI_1`, `NCIIPC_1`, plus the older un-numbered Wiki Intake notes. Read each node's own content; assign section and tier per §7 of the context packet. **Do not re-source.** | — |
| **V-02** | Execute the `NIST_AI_RMF` disambiguation once **X-06** decides. If option (a): rename `02_Projects/Shared_Anchors/NIST_AI_RMF.md` → `NIST_AI_RMF_2023_Anchor.md`, update the 9 path-qualified links, verify all 44 bare links now resolve to `06_Frameworks/NIST_AI_RMF`, confirm `International_24_NIST_AI_RMF_2023` remains distinct. | X-06 |
| **V-03** | Rebuild `Wiki_Intake_Index.md` (**D3**). It is a how-to dated 12 June listing none of the 161 notes. Either convert to a live index generated from folder contents, or repoint it at the Backfill Register in [[Corpus_Index_MOC]] and retitle it as a protocol document. | — |
| **V-04** | **Re-run the Three-Instance Gate on [[05_Concepts/05_Concepts_Signature/Records_Rules_Asymmetry]].** `UIDAI_1_Circular_8_2025_Data_Vaults_HSM` now exists and MeitY runs to `MeitY_8` — remediation Option A is partly satisfied and was never noticed because neither node was indexed. Test the four constitutive dimensions against UIDAI_1, MeitY_4 (DPDP Rules 2025) and MeitY_8. If the gate passes on real nodes, propose re-elevation to signature; if not, proceed to Option B (ADICO-code MeitY_4). **Note the standing prohibition on fabricated corpus evidence.** | — |
| **V-05** | Recode the **remaining 13 of 23 P3 coordination pairs** against the S/F/X scheme (⚠#350), and operationalise the "opportunity" qualifier as a stated test rather than a judgment (⚠#348). Restate the split over the full base. | — |
| **V-06** | Merge `RBI_3` and `RBI_13` once **X-05** authorises. RBI_3 holds the legal basis; RBI_13 holds the sourcing metadata — the merge needs both. Standing protocol is *report only* until Vivek says otherwise. | X-05 |
| **V-07** | **Rebuild the consolidated VERIFY tracker.** Flag numbering is authoritative nowhere; historical trackers are stale; 906 `VERIFY` mentions across 69 live files. Sweep the vault for `⚠` and `VERIFY #` patterns, build one table of flag / raising node / severity / status, and make it the single source of truth. This is the precondition for ever saying "all flags closed". | — |
| **V-08** | Small hygiene batch: create the missing `07_Institutions/MoHFW.md` institution root (MoHFW_1 exists without one); unify CERT-In legacy (`CERT_1`–`CERT_4`) and new-style (`CERT_In_1`–`CERT_In_3`) naming; add `F143` to the Wiki S3 section. | — |

---

## 4. Vivek-only — nobody else can do these

| # | Action | Why it can't be delegated | When |
|---|---|---|---|
| **X-01** 🔴 | **Run the C-02 circulation check (⚠#339).** Three channels: (a) your P1 draft text — search for any sentence asserting WDR 2026 does not cite India; (b) LinkedIn posts since 5 August 2026; (c) supervisor or committee correspondence. The claim is **false** — India appears ~25+ times and Secretary MeitY sat on the advisory panel. | Only you can see your drafts, posts and correspondence | **Now** |
| **X-02** 🔴 | Fix `02_Projects/References/P2_References.md` entries **#7** (Masiero journal cross-contamination, ⚠#290) and **#10** (confirmed mix-up — correct citation is Seetharaman, P., Mathew, S. K., & De', R. (2024). *Does location matter in IS research? A developing country perspective from India.* Information Systems Journal, 34(6), 1963–1994). Open sub-question: whether #10's Role/Claim text should be rewritten to match F128, or a different DPI-welfare Seetharaman paper located. | File is outside session edit scope by your instruction | Before P2 |
| **X-03** 🔴 | **The five unverifiable metrics.** "248 institutional statements across 12 DPI documents" (P2 ADICO); "23 of 40 coordination pairs" (P3); "0 of 11 rules governing DPI fallback" (P2); fsQCA SR = 0.33 India; "90% intercoder agreement" (P3). No AI session can verify any of these against your NVivo/SmartPLS files. | Your NVivo and coding files | Before any submission |
| **X-04** 🔴 | **OQ-09 — lock the fsQCA 10-case list. Deadline 1 Sep 2026: 17 days.** The only hard external date in the open set. | Research design decision | **By 1 Sep** |
| **X-05** 🟢 | Delete `_to_delete/` (163 files, 1.5 MB — 3 empty scaffolds + 160 fuse artefacts). Now gitignored. Also decide the `RBI_3`/`RBI_13` merge (→ V-06). | This session can move but not delete on your disk | Any time |
| **X-06** 🟢 | Decide `[[NIST_AI_RMF]]` (**D1**): (a) rename the Shared Anchor so bare links land on the Framework node — one move, fixes all 44; (b) path-qualify all 44 individually; (c) accept the current behaviour. | Ontology call, not housekeeping | Before next wiring pass |
| **X-07** 🟡 | **Obtain *Digital Empires*** and re-write F143's Findings 1–5 with page anchors (⚠#351). Until then the node is a flagged placeholder and must not be cited. | You have to get the book | Before P1 positioning |
| **X-08** 🟡 | Write to Behnaz Azimi for citation permission once **P-11** locates them (⚠#329). Nothing from F142 into P1, P4, proposals or decks until permission is in writing. | Your correspondence | Before any F142 use |

---

## 5. Sequencing

**This week — reputational and deadline exposure**

1. **X-01** (C-02 circulation check) — the only item where a known-false claim may already be outside the vault.
2. **X-04** (fsQCA 10-case lock) — 17 days, and the only hard external deadline.
3. **P-02** (CEA_3 clean text) — low effort, removes the sole real risk on the corpus's most valuable recent finding.
4. **P-01** (NABCB/ISO 42006) — a direct contradiction between two vault nodes, both dated within three days of each other.

**Next — unblock the artefacts already written**

5. **P-06** (decision-chain novelty check) — highest leverage; determines what Decision_Infrastructure can claim.
6. **P-04** (Microsoft architecture) and **P-05** (NPCI) — the two remaining S2/S3 follow-throughs.
7. **P-07** (Minimum Evidence Register) — timed against the IRDAI WG-AI report, due ~18 Sep.
8. **V-07** (consolidated VERIFY tracker) — do this before the flag count grows further.

**Then — capacity permitting**

9. **V-04** (Records_Rules_Asymmetry gate) — a construct may be re-elevatable on evidence already sitting in the vault.
10. **P-03**, **P-08**, **P-12** — corpus completion.
11. **V-01**, **V-03**, **V-05**, **V-08**, **X-05**, **X-06** — hygiene.
12. **P-09**, **P-13**, **P-14** — low-priority comparative and status checks.

**Deliberately not scheduled:** any new synthesis construct. The S1–S5 queue closed on 2026-08-09. Adding constructs against an unverified base compounds the closure problem rather than advancing the research.

---

## 6. Closure protocol

A flag is closed only when **all four** hold:

1. The **raising node** carries a dated closure line stating what was found and what changed.
2. Any **downstream note** whose claim depended on the flag is corrected, and the correction is dated.
3. If the flag concerned material that has circulated externally, an entry exists in [[11_Content/Content_Correction_Register]].
4. The consolidated tracker (**V-07**) is updated.

Recording a closure only in this file does not close it. This register is a work queue, not a system of record.

---

## Log

- **2026-08-15:** Created during the vault housekeeping session, as the fourth pass in the Perplexity sourcing-prompt series. Compiles every open ⚠ flag, decision item and standing task across `Session_Handoff_Current.md`, the Backfill Register, and the notes, onto three channels (P / V / X). No flags closed by this document — it is a triage and prompt artefact only. ⚠#347–#353 raised in the same session are included.
