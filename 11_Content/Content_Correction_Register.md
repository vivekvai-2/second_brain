---
type: Content Register
status: active
last_updated: 2026-08-09
tags:
  - type/content-register
  - status/active
  - engine/linkedin
  - engine/consulting
---

# Content Correction Register — published and draft practitioner material

**Purpose.** Practitioner content (LinkedIn carousels, keynote decks, webinar slides) is drafted fast and often precedes the vault node that later verifies it. When the vault subsequently corrects a claim, the correction lands in the concept file and **the content artefact keeps circulating uncorrected**. This register is the reverse index: it lists claims that appeared in content, were later found wrong, and must not be republished.

**Rule.** Before reusing, reposting, or adapting any listed artefact — including into a deck, article, or client-facing material — check this register first.

---

## 🔴 C-01 — "NIST Digital Forensics Artifact Catalog" does not exist

| Field | Detail |
|---|---|
| **Artefact** | LinkedIn carousel, 9 slides, "NIST perfected the process. AI governance has yet to define the evidence." Drafted ~2026-08-01. File on Desktop: `AI Governance Evidence  2.pdf` |
| **The error** | Slide 1 presents **"NIST DIGITAL FORENSICS ARTIFACT CATALOG"** as the carousel's central visual anchor and organising authority. **No such NIST publication exists.** |
| **When found** | 2026-08-02, during the intake that produced [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]]. Recorded in that note's Provenance and Correction Record section. |
| **Status** | ✅ Corrected in the vault. ❌ **Not corrected in the carousel**, which still carries the attribution as of 2026-08-09. |
| **Risk** | External publication risk. The claim attributes a named publication to a standards body that never issued it, on the slide that frames the entire argument. A reader from the forensics or standards community would catch it immediately, and it is the kind of error that costs credibility disproportionately in a governance-authority positioning. |

### What NIST actually publishes in this space

| Programme | What it is |
|---|---|
| **CFTT** — Computer Forensics Tool Testing | Forensic *tool* reliability testing |
| **CFReDS** — Computer Forensic Reference Data Sets | Reference test datasets |
| **SP 800-86** (2006, unsuperseded) | A four-phase forensic *process* guide: collection, examination, analysis, reporting |

The community-maintained **ForensicArtifacts / Artifact Definitions** repository is the nearest thing to an artefact catalogue and has **no institutional relationship to NIST**.

### The argument survives — only the attribution fails

The forensics-to-AI-oversight structural analogy does not depend on the NIST attribution. Slides 2–9 (the same-question mapping, artefacts-vs-documents, the AI evidence layer, the lifecycle spread, the four-regulator evidence-question table, the four-audience table, and the policy → controls → evidence → assurance → trust ladder) are unaffected and remain sound.

### Verified replacement anchor — use this instead

[[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] **Definition 14** imports a digital-forensics definition into **binding Indian banking regulation**, expressly attributed to *NIST Cloud Computing Forensic Science Challenges*:

> "'Digital Forensics' — The process used to acquire, preserve, analyse, and report on evidence using scientific methods that are demonstrably reliable, accurate, and repeatable. (Source: adapted from NIST Cloud Computing Forensic Science Challenges)"

This is stronger than the original claim in every respect that matters for the carousel's purpose: it is an actual instrument, actually citing NIST, actually binding, actually Indian, and dated 31 July 2026 — which also makes it current rather than generic.

⚠ Confirm the underlying source is **NISTIR 8006** before using the lineage in publication-track output. RBI names the report title without a NISTIR number and says "adapted from," not "reproduced" (⚠ V-RBI8-2).

**Suggested slide-1 reframe:** rather than a NIST catalogue that does not exist, lead with the real and more interesting fact — that India's newest banking cyber regulation reaches into NIST's forensic-science vocabulary to define what evidence means, while India's AI-specific instruments define nothing of the kind. That is the carousel's actual thesis, and it now has a citable instrument behind it.

---

## 🔴 C-02 — "WDR 2026 never once cites India" is false

**Where it originated:** [[07_Institutions/Corpus/International/International_38_World_Bank_WDR2026_AI_Governance]], created 2026-08-05 from secondary extraction only. The node presented the claim as *"the strongest single contribution of this node"* and **explicitly recommended three uses**: a P1 SLR positioning sentence, a rationale for the vault's independent India corpus, and LinkedIn practitioner content under the "AI Governance & Cyber Risk" brand.

**Why it is wrong.** The primary text, obtained 2026-08-09, cites India roughly twenty-five times. Telangana's AI weather forecasting appears in the **Foreword**, the Overview *and* Chapter 5. Sarvam AI is the report's flagship "advance" exemplar. UPI is the recurring DPI model, invoked in the Foreword as the answer to the sovereignty problem. Also cited: BHASHINI, the IndiaAI Mission, iGOT Karmayogi, TGDeX, Kisan e-Mitra, Odisha's Ama Krushi, Tamil Nadu's diabetic-retinopathy screening, Wadhwani AI's Cough Against TB, a Maharashtra HTA of Qure.ai's qXR, the 20-year data-centre tax holiday, Microsoft's $17.5bn India commitment, and the **largest single country sample in the Enterprise Survey on AI Adoption at 1,355 firms**. **S. Krishnan, Secretary of MeitY, sat on the high-level advisory panel.** The **Reserve Bank Innovation Hub** is among consulted organisations.

**Failure mode this exemplifies.** A secondary-extraction pass reported an absence. An absence claim about a document is only as good as the coverage of the extraction — and the extraction covered Chapter 9 and Spotlight 7, roughly 15% of the report. **Absence findings must not be asserted from partial extraction.** That is a general rule worth carrying, not a one-off.

### The corrected claim — use this instead

> **WDR 2026 treats India as an AI-deployment and digital-public-infrastructure exemplar, and never as an AI regulatory-governance case.** India is absent from Box 9.1's horizontal-law comparator set, from Chapter 9's existing-law case studies (Senegal, Kenya, Chile, Colombia, Philippines, Singapore), from Spotlight 7's coordination cases (Singapore, Egypt, Bangladesh), and from Box 9.4. The sharpest instance: the RBI participated institutionally through RBIH, yet [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] — a textbook case of the report's own "extend existing instruments" logic — goes uncited, as do the DPDP Act and the SEBI AI circular.

This version is **stronger** than the false one, because it identifies a structural pattern in how the development-policy literature positions India rather than making a coverage claim that collapses on inspection.

### Action required

| Channel | Check | Status |
|---|---|---|
| P1 SLR draft text | Search for "never", "omits India", "does not cite India" in any positioning or gap paragraph | ⚠ **Vivek to confirm** — not verifiable from the vault |
| LinkedIn / practitioner content since 2026-08-05 | Any post citing WDR 2026 on India's absence | ⚠ **Vivek to confirm** |
| Supervisor or committee correspondence | Same | ⚠ **Vivek to confirm** |
| Vault | Corrected in place at International_38 with the original struck, not deleted | ✅ Done 2026-08-09 |

If the claim has circulated, the correction is easy and reflects well: the sharper finding replaces the looser one, and the report is publicly available for anyone to check.

---

## Watch items — claims in content that are correct but fragile

| # | Artefact | Claim | Caveat to carry |
|---|---|---|---|
| **W-01** | NIST evidence carousel, slide 6 | The DPDP / RBI / CERT-In / Bharatiya Sakshya Adhiniyam four-regulator evidence-question table | Sound, and now upgraded — see [[06_Frameworks/Evidentiary_Destination_Matrix]], which supplies the researched version with s.63 conditions actually crosswalked. Reuse the matrix, not the improvised table. |
| **W-02** | Microsoft architecture carousel | "Six engineering layers, six unanswered questions"; the six-record minimum evidence register | Sound and now vault-backed — see [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] and [[04_Knowledge_Products/Minimum_Evidence_Register_Autonomous_AI]]. Note the register's six records currently map to **almost nothing** in binding Indian law; state that as the finding rather than implying the records are required. |
| **W-03** | Decision Infrastructure Series, Release 0.1 | "Institutional risk emerges not in the model, but where the model becomes action" | Sound and now gated — see [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]]. The Power-sector leg is now evidenced by a binding 2026 instrument ([[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]]); avoid the earlier framing that CEA's instruments merely "predate" ML. |
| **W-04** | Any carousel citing RBI_9 (AI-ACT&RS) | The advisory's content, including "logging, traceability and forensic readiness" | **Tier C — primary text not obtained.** Existence is confirmed on the record by RBI's Deputy Governor; contents derive from KPMG and Business Standard only. Do not present provision-level detail as RBI's own wording. |

---

## How to use this register

1. **Before republishing** any practitioner artefact, search this file for its name.
2. **When the vault corrects a claim** that originated in content, add a row here in the same session — the correction is not complete until the content side is flagged.
3. **When a content claim is later vindicated** by a corpus node, move it to Watch items with the supporting node named, rather than deleting it.

---

## Log

- 2026-08-09 (later, WDR2026 primary-text pass): **C-02 added** — the "WDR 2026 never once cites India" claim, which originated in International_38 on 2026-08-05 and was explicitly recommended for P1 SLR positioning and LinkedIn use. Falsified by the primary text (~25+ India citations, including three in the Foreword and Overview). Replaced with the deployment-versus-governance asymmetry, which is both true and sharper. **General rule extracted and worth carrying beyond this instance: absence claims about a document must not be asserted from partial extraction.** Three channels need a check that only Vivek can run — P1 draft text, LinkedIn since 5 August, and supervisor correspondence.
- 2026-08-09: Register created. Opened with C-01, the NIST Digital Forensics Artifact Catalog attribution — corrected in [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] on 2026-08-02 but never corrected in the carousel, which continued to circulate. Four watch items recorded. Created as part of the H1–H4 / S1–S5 sequence run this session.

---

_Back to [[00_MOC/PRIS_Master_MOC]]_


---

## C-03 — "NABCB has no ISO 42001 accreditation scheme" (raised and corrected 2026-08-15)

| | |
|---|---|
| **The error** | [[06_Frameworks/ISO_IEC_42001]] recorded as a **"❌ confirmed gap"** (2026-08-02) that no NABCB accreditation programme, scheme document or auditor-competence guidance for ISO/IEC 42001 existed, and that **ISO/IEC 42006 was "not published — work item in development (confirmed by UKAS)."** |
| **The truth** | **ISO/IEC 42006:2025 was published in July 2025**, thirteen months before the finding was written. **NABCB 220** (*Accreditation Criteria for AIMS*, April 2026) is a dated, named, published scheme document aligned to it. **Three certification bodies are accredited** — AI 001 TUV India (from 11 Feb 2025), AI 002 TUV SUD South Asia, AI 003 Maverick Quality Advisory — and certificates have been issued to real clients (Mphasis, Oct 2025). |
| **Probable cause** | NABCB's public scheme-listing webpage still captions the entry **"ISO/IEC DIS 42006"** — correct in Feb 2025 when NABCB accredited AI 001 against the draft, stale after the April 2026 transition. A single stale webpage caption was read as an absence. |
| **Severity** | 🔴 **High.** Three downstream artefacts were built on it: (1) an fsQCA recalibration recommendation that would have scored India at **full non-membership on a condition where it is a member** — mis-specifying the Indian case in the thesis chapter; (2) a **consulting/policy recommendation addressed to NABCB by name** to build a scheme it had already published — a credibility failure in front of the named recipient; (3) the framing of India's position as capacity lag rather than completed-investment-without-recognition. |
| **Circulation channels to check (Vivek)** | Any LinkedIn post, carousel or comment since 2 August 2026 asserting India lacks an AI-certification accreditation scheme · the "certification without recognition" paper draft · P1/P4 draft text · BIS LITD 30 correspondence or engagement material · any client or inbound-opportunity deck referencing the NABCB gap |
| **Replacement claim (stronger)** | India has built the **entire assurance chain** — standard adopted, lead auditors trained, accreditation criteria published, certification bodies accredited, certificates issued — and **no Indian regulator attaches any consequence to its output.** Recorded at ISO_IEC_42001 as a candidate new sequencing variant, *assurance before demand*. The policy ask inverts: it is regulatory **recognition**, addressed to RBI/SEBI/IRDAI/MeitY, not scheme creation addressed to NABCB. |
| **Status** | Vault corrected 2026-08-15 (ISO_IEC_42001 Framework Identity + India tables, fsQCA section, reuse section; Parliament_2 vindicated). **External circulation check outstanding — Vivek.** |

**The general rule this yields, and it is the second of its kind:** *a stale index page, listing page or catalogue caption is not evidence of absence.* C-02 established that partial extraction cannot support an absence claim. C-03 establishes that a secondary listing cannot either — the register and the dated scheme document are the evidence, not the page that links to them.


---

## C-04 — "NPCI runs federated AI fraud scoring across UPI" (raised and corrected 2026-08-15)

| | |
|---|---|
| **The error** | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] §Infrastructure-layer (2026-08-02) asserted that NPCI runs **federated AI fraud detection generating cross-institutional customer risk scores** across UPI, with **no published governance instrument of any kind**, sourced to *"secondary reporting (Economic Times BFSI, 3 Apr 2025) and NPCI promotional material."* |
| **The truth** | **No NPCI primary source describes federated learning.** The AI/ML passage in NPCI's fraud Best Practices document is addressed to **member banks**, not to NPCI's EFRM system, and EFRM is nowhere evidenced as AI/ML-based (⚠#361). The only NPCI AI system named as live or piloted is the **UPI Help Assistant**, a grievance-resolution SLM. And it is **not** a governance absence: `RBI/DPSS/2024-25/123` binds NPCI as a **Large Non-Bank PSO from 1 April 2025** — it simply contains no AI provision. See [[07_Institutions/Corpus/NPCI/NPCI_1_AI_ML_Payments_Operations_2025_2026]]. |
| **Severity** | 🟡 **Medium externally, 🔴 high internally.** The structural argument survives intact and is stronger restated. But the claim was stated as fact in a **Three-Instance Gate** — the vault's own evidentiary threshold — and the gate passed on it. |
| **Propagation — the part worth recording** | The claim was written **once**, on 2026-08-02, from secondary reporting. In **thirteen days** it appeared in **nine notes**: `Governance_Debt` (origin), `Decision_Infrastructure` (×3 — prose, gate table, instances), `DPI_Governance`, `DEPA`, `Contestability_Redress`, `_Institutions_MOC`, `NPCI` (institution root), `Power_Grid_Critical_Infrastructure_Governance`, `Grid_India`. **Correcting the origin and the two obvious dependants left seven live copies standing.** All nine are now corrected. |
| **Detection method — reusable** | Found by scanning `05_Concepts/`, `06_Frameworks/`, `03_Domains/` and `04_Knowledge_Products/` for prose claims about institutional conduct that cite an **institution root file** (`[[NPCI]]`) rather than a **corpus node**. That is the signature of a claim with no primary source behind it. The sweep returned **134 such citations across 34 files**; most are benign "Linked Institutions" navigation lists, but the live NPCI copies were all in this set. |
| **Status** | Vault fully corrected 2026-08-15. **No external circulation identified** — unlike C-02 and C-03, this claim does not appear in carousel or LinkedIn material reviewed to date. **Vivek: confirm against P2/P3 draft text**, where the infrastructure-layer argument is likeliest to have been used. |

**The rule this yields, and it is the third of the series:** C-02 — partial extraction cannot support an absence claim. C-03 — a stale listing page cannot either. **C-04 — a claim sourced to secondary reporting will propagate at roughly one note every one to two days, and correcting its origin does not correct its copies.** Grep the distinctive phrase, not the concept.
