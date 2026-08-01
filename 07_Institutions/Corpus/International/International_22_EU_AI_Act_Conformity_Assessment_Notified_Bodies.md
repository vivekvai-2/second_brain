---
type: Corpus Node
tags:
  - type/corpus-node
  - status/active
  - series/format-a
  - section/S3
  - section/S2
  - tier/high
  - project/p1
  - project/p4
  - project/fsqca
  - institution/european-commission
  - institution/european-parliament
  - jurisdiction/EU
  - engine/phd
---

# International_22 — EU AI Act: Conformity Assessment & Notified Body Regime (Regulation (EU) 2024/1689, Arts. 28–34, 43–49; Annexes V–VII) + Digital Omnibus on AI Amendment

**Type:** Corpus Node (Format A)
**Vault path:** `07_Institutions/Corpus/International/International_22_EU_AI_Act_Conformity_Assessment_Notified_Bodies.md`
**Institution:** European Parliament + Council of the European Union (co-legislators, Regulation (EU) 2024/1689); European Commission / DG CONNECT (implementation, Digital Omnibus proposal, AI Act Service Desk)
**Issuing body:** European Union (Regulation, directly applicable in all Member States)
**Document date:** Regulation adopted 2024; conformity-assessment/notified-body provisions (Ch. IV, Arts. 28–39) applicable from 2 August 2025; Digital Omnibus on AI (amending regulation) finally approved by Council **29 June 2026**, entry into force July 2026
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/International_Comparators]]
**Batch:** Ad hoc — gap-directed sourcing (Perplexity Deep Research), pre-Batch 19/20 session
**Source corpus:** Gap-fill for AIGP BoK (F055) Domain II (Laws & Standards) gap — Gap #4, the vault's first dedicated node on the EU AI Act's conformity-assessment/notified-body mechanism specifically (distinct from the existing framework-level synthesis at [[06_Frameworks/EU_AI_Act]] and from [[04_Knowledge_Products/Wiki_Intake/FRA_EU_Assessing_High_Risk_AI_Fundamental_Rights|F053]]'s FRIA/Art. 27 focus)

**⚠ Source-method note (methodological deviation from standard pipeline):** Unlike the vault's usual NotebookLM PROMPT 0b single-document extraction relay, this node is built directly from a Perplexity Deep Research synthesis that cites and quotes specific articles, annexes, and dates across the primary Regulation text (EUR-Lex), the Digital Omnibus legislative record, the NANDO database, and named secondary sources. Article/annex citations below are reproduced as given by that research pass and have **not** been independently verified against the EUR-Lex primary text by a NotebookLM extraction of the Regulation itself. Treat all specific article numbers and dates as citation-grade but not yet primary-source-verified in this vault's usual sense — see VERIFY flags.

---

## Instrument Identity

**Primary text:** Regulation (EU) 2024/1689 (the EU AI Act) — EUR-Lex: `https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng`
**Amending instrument:** Digital Omnibus on AI — *Regulation amending Regulation (EU) 2024/1689 and Regulation (EU) 2018/1139 as regards the simplification of the implementation of harmonised rules on artificial intelligence*, COM(2025) 836 final — EUR-Lex proposal: `https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=celex:52025PC0836`
**Type:** Regulation (directly binding EU law) + amending Regulation (legislative procedure complete as of 29 June 2026; Official Journal publication reference not yet confirmed as of the sourcing date)
**Scope of this node:** Articles 28–34 (notified-body designation, competence, operational obligations), Articles 43–49 (conformity assessment procedure, certificates, EU Declaration of Conformity, CE marking, database registration), Annexes V–VII (DoC content, internal-control procedure, notified-body procedure)

---

## Framework Architecture

### Two-Route Conformity Assessment Design (Article 43)

| Route | Applies to | Mechanism | Trigger |
|---|---|---|---|
| **Internal control (Annex VI)** | Annex III Point 1 (biometrics) systems where harmonised standards (Art. 40) or common specifications (Art. 41) are fully applied | 3-step: QMS verification (Art. 17) → technical documentation review (Ch. III §2) → design/development and post-market monitoring consistency check | Default when applicable standards exist and are fully applied |
| **Third-party assessment (Annex VII)** | Annex III Point 1 systems where standards/specifications don't exist, are only partially applied, or are restricted | QMS assessment (incl. on-site audit) + technical documentation assessment by a **notified body**, issuing an EU technical documentation assessment certificate | Mandatory default until harmonised standards are published and applied |
| **Self-assessment only, no notified body option** | Annex III Points 2–8 (critical infrastructure, education, employment, essential services access, law enforcement, migration/asylum/border, administration of justice) | Annex VI internal control only | Always, regardless of standards availability (Art. 43(2)) |
| **Sectoral legislation route** | Annex I product-embedded AI (medical devices, machinery, etc.) | Follows applicable sectoral conformity-assessment law; existing sectoral notified bodies may cover AI Act compliance | Art. 43(3) |

Article 43(6) empowers the Commission to extend the third-party-assessment requirement to further high-risk categories by delegated act — not yet exercised as of the sourcing date. Article 43(4): substantial modification triggers a fresh conformity assessment, subject to a predetermined-change documentation exemption.

### Notified Body Regime (Chapter IV, Arts. 28–39)

| Article | Subject |
|---|---|
| Art. 28 | Notifying authorities — each Member State establishes at least one; independence/impartiality requirements |
| Art. 29 | Application for notification — accreditation certificate or documentary evidence; re-use of designations under other EU legislation (e.g., MDR, Machinery Regulation) permitted |
| Art. 30 | Notification procedure — Commission/Member State notification via electronic tool; standstill period for objections |
| Art. 31 | **Requirements for notified bodies** — legal personality, financial/organisational independence, permanent AI/data/software/cybersecurity-competent staff, liability insurance, impartiality documentation |
| Art. 32 | Presumption of conformity for nationally-accredited notified bodies |
| Art. 33 | Subsidiaries/subcontracting — permitted with notification; 5-year documentation retention |
| Art. 34 | Operational obligations — conformity verification per Art. 43; SME burden-minimisation; documentation access for authorities |
| Art. 44 | Certificates — max validity 5 years (Annex I) / 4 years (Annex III); suspension/withdrawal power; appeal procedure required |
| Art. 45 | Information obligations — notify authority and other notified bodies of certificates issued/refused/withdrawn; share negative results |
| Art. 46 | Derogation — market surveillance authority may authorise limited-period market placement pending full assessment, for public-security/life/health/environment/infrastructure reasons; Commission oversight, 15-day objection window |

### CE Marking and EU Declaration of Conformity

| Provision | Content |
|---|---|
| Art. 47 + Annex V | Written, machine-readable EU Declaration of Conformity; 10-year retention; single DoC where AI system also subject to other EU harmonisation law; must state system identity, provider details, sole-responsibility statement, GDPR compliance statement where applicable, standards applied, notified-body ID and certificate reference where applicable |
| Art. 48 | CE marking — visible/legible/indelible; digital marking for digital-only systems; notified body's identification number appended where Annex VII applies |
| Art. 49 | Registration in the EU AI database (Art. 71) required before market placement, for Annex III systems |

---

## ⚠ Critical Update — Digital Omnibus on AI Timeline Deferral

The Digital Omnibus on AI (Commission proposal 19 Nov 2025 → Council general approach 13 Mar 2026 → trilogue agreement 7 May 2026 → EP adoption 16 Jun 2026 → Council final approval **29 Jun 2026**) materially defers the conformity-assessment-relevant deadlines:

| Provision | Original date | **Amended date (per Digital Omnibus)** |
|---|---|---|
| Art. 5 prohibited practices | 2 Feb 2025 | Unchanged — in force |
| AI literacy (Art. 4) | 2 Feb 2025 | Unchanged — in force; SME obligation simplified |
| GPAI obligations (Arts. 51–55) | 2 Aug 2025 | Unchanged — in force |
| Chapter IV notified-body rules (Arts. 28–39) | 2 Aug 2025 | Unchanged — in force; designation applications open since this date |
| Art. 50(1)(3)(4) transparency (chatbot disclosure) | 2 Aug 2026 | Unchanged |
| Art. 50(2) watermarking/synthetic content | 2 Aug 2026 | Deferred to 2 Dec 2026 for systems already on market |
| **High-risk Annex III obligations (Arts. 9–15, 17, 43–49 — conformity assessment)** | **2 Aug 2026** | **Deferred to 2 Dec 2027** |
| **Art. 27 (FRIA, deployer-side)** | 2 Aug 2026 | **Not textually amended, but practically deferred to 2 Dec 2027** — FRIA only bites once a system is in-scope as high-risk under Annex III, and that trigger date moved (confirmed 2026-07-31, see VERIFY #226 resolution) |
| High-risk Annex I (product-embedded AI) | 2 Aug 2027 | Deferred to 2 Aug 2028 |

**Direct implication:** the conformity-assessment obligations that are the subject of this node (Arts. 43–49, for standalone Annex III systems) do not bind until **2 December 2027** — 16 months later than the date most secondary literature (including this vault's own prior references, see cross-node flag below) has assumed. The notified-body *designation infrastructure* (Ch. IV) remains live from 2 August 2025, so bodies are being assessed and designated now, ahead of the deferred compliance deadline.

---

## NANDO Designation Status

As of the sourcing date, **no or very few notified bodies had been formally designated and listed in NANDO specifically for the AI Act** (Regulation (EU) 2024/1689) — the designation process opened 2 August 2025 but is still in early stages. Existing notified bodies designated under sectoral legislation (Medical Devices Regulation, Machinery Regulation) may leverage existing accreditation to seek AI Act designation under Art. 29(4). Public register: `https://webgate.ec.europa.eu/single-market-compliance-space/notified-bodies/by-legislation` (search "Regulation (EU) 2024/1689").

---

## Companion Practitioner Source (candidate for future Format B ingestion)

**"Conformity Assessments under the EU AI Act: A Step-by-Step Guide"** — Serban, Rovilos, Demetzou; Future of Privacy Forum (FPF) + OneTrust, April 2025. 41-page article-referenced walkthrough of the CA-applicability decision tree, documentation requirements, timeline mapping, and notified-body engagement. `https://fpf.org/wp-content/uploads/2025/04/OT-comformity-assessment-under-the-eu-ai-act-WP-1.pdf` — flagged as a strong Format B companion candidate, not yet ingested as its own node.

Secondary triangulation sources cited but not ingested: VDE (German standardisation/testing body) blog, Feb 2026; EC AI Act Service Desk (`https://ai-act-service-desk.ec.europa.eu/`); Draft Commission Guidelines on Classification of High-Risk AI Systems (Art. 6(5)), published 19 May 2026 by DG CONNECT.

---

## Regulatory Significance

### Comparison with China GenAI Measures (International_21) and Australia AIIA Tool (International_20)

| Dimension | EU AI Act conformity assessment | China GenAI Interim Measures (International_21) | Australia AIIA Tool (International_20) |
|---|---|---|---|
| Legal form | Regulation (directly binding statute) | Departmental regulation (sub-statutory) | Internal APS policy/guidance |
| Third-party verification | Notified-body assessment for a defined subset (Annex III Pt. 1 without applied standards) | None — no third-party conformity body concept | None — internal assessment only |
| Self-certification default | Only where harmonised standards fully applied (narrow) | N/A (different regulatory design — content/process obligations, not product certification) | Yes — agency self-assessment throughout |
| Enforcement infrastructure maturity | Designation process live since Aug 2025; near-zero bodies designated as of mid-2026; compliance deadline itself deferred to Dec 2027 | Multi-regulator (7 ministries) but no product-certification infrastructure | Mature — DTA-operated since Dec 2025 |
| Direct sanction | Up to 3%/EUR 35m turnover-based fines (Art. 99, not detailed in this node) | No self-contained fine (deleted from draft) | No external fine — internal APS accountability only |

This is the corpus's first instance of a **product-certification-style conformity assessment regime** (CE marking, notified bodies, technical documentation certificates) — structurally distinct from the process/principles-based obligations that dominate the rest of the corpus (RBI FREE-AI's "should" principles, India's advisory frameworks, even China's process obligations). It is the closest analogue in the corpus to traditional EU product-safety regulation (medical devices, machinery) applied to AI.

---

## Implications for Indian Governance

India has no conformity-assessment or notified-body equivalent for AI systems in any form — not even a voluntary certification scheme comparable to a CE-marking-adjacent mechanism. The DPDP Act's DPIA requirement (draft Rules) is process-based, not product-certification-based. This node sharpens a previously implicit corpus gap: India's AI governance architecture has never contemplated third-party pre-market certification as a governance tool, whereas the EU (product-safety tradition), and to a lesser extent existing sectoral regimes cited in International_12/HCJP (medical devices, machinery notified bodies now extending to AI), treat this as a standard governance instrument.

**⚠ Cross-node consistency flag — CONFIRMED STALE, action needed:** [[04_Knowledge_Products/Wiki_Intake/F039_ICAAD_KWM_AI_Harm_Human_Rights]] (line ~100/147) states the EU AI Act Art. 27 FRIA obligation applies "from 2 August 2026," including a "six weeks away" urgency framing. This is now **confirmed incorrect** as of the #226 resolution above (2026-07-31): Art. 27's practical application date has shifted to 2 December 2027 alongside the rest of the Annex III cluster. **F039 should be corrected in a future session** — this node flags the discrepancy but has not edited F039 directly, consistent with this session's practice of not silently correcting other nodes without a dedicated pass.

---

## Connections

**[[P1_SLR_RG]]:** S3 (international frameworks) — closes Gap #4 of the AIGP BoK gap analysis; the vault's first dedicated conformity-assessment/notified-body node.

**[[P4_Doctrinal_IJLIT]]:** Product-certification governance design (CE marking, notified bodies) as a doctrinal comparator to India's complete absence of any AI product-certification concept — a sharper doctrinal contrast than the process/principles comparisons already in the corpus.

**[[fsQCA_Thesis_Chapter]]:** Refines the EU AI Act's RL (Regulatory Logic) and EA condition scores at [[06_Frameworks/EU_AI_Act]] — the Digital Omnibus deferral is directly relevant to the "prior" calibration note in that framework file, which was written assuming the original 2026–2027 phase-in and should be revisited before Q3 2026 coding.

**Concept links:**
- [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — the Digital Omnibus itself is a within-EU instance of the "layering/elaboration" pattern also seen in China's GB 45438-2025 (International_21) — a binding base regulation progressively amended/deferred by a second legislative act, distinct from cross-regulator parallelism.
- [[05_Concepts/05_Concepts_Standard/Accountability]] — notified-body certification is a third-party accountability mechanism, structurally distinct from the self-attestation/regulator-reporting accountability model dominant elsewhere in the corpus.
- [[05_Concepts/05_Concepts_Standard/Legitimacy]] — third-party certification is a stronger legitimacy-conferring mechanism than self-assessment; relevant to LG condition calibration.

**Related nodes:**
- [[06_Frameworks/EU_AI_Act]] — the vault's existing framework-level synthesis note; **needs a dated annotation** reflecting the Digital Omnibus deferral (see below).
- [[04_Knowledge_Products/Wiki_Intake/FRA_EU_Assessing_High_Risk_AI_Fundamental_Rights|F053]] — FRIA/Art. 27 companion; see cross-node consistency flag above.
- [[04_Knowledge_Products/Wiki_Intake/F039_ICAAD_KWM_AI_Harm_Human_Rights]] — contains the now-potentially-stale "2 August 2026" FRIA date; flagged, not corrected.
- [[04_Knowledge_Products/Wiki_Intake/International_12_HCJP_Legal_AI_BFSI_2025]] — existing lex specialis mapping between EU AI Act and sectoral financial regulation (MiFID II, CRD, Solvency II); this node's Art. 43(3) sectoral-legislation route is directly relevant to that mapping.
- [[07_Institutions/Corpus/International/International_21_China_CAC_GenAI_Interim_Measures_2023]] — comparator; see Regulatory Significance table above.
- [[07_Institutions/Corpus/International/International_20_Australia_DTA_AI_Impact_Assessment_Tool]] — comparator; see Regulatory Significance table above.

---

## VERIFY Flags

**#226 — RESOLVED (2026-07-31, Perplexity Deep Research), sub-items (2) and partially (3):**

**(2) Art. 27 FRIA deferral — RESOLVED, Medium-High confidence.** The Digital Omnibus on AI was formally published in the Official Journal and became effective **Monday, 27 July 2026**. Article 27 itself was **not textually amended** — it still requires a FRIA before a high-risk AI system goes into use, and Annex III still classifies the same systems as high-risk. What moved is the **Annex III high-risk classification/application date itself**, from 2 August 2026 to **2 December 2027** (standalone Annex III systems) / **2 August 2028** (Annex I product-embedded AI). Since Art. 27's FRIA obligation only bites once a system is actually in-scope as high-risk under Annex III, and that trigger date is now 2 December 2027, the **practical effect is that FRIA obligations are pushed out to 2 December 2027 alongside the rest of the Annex III cluster** — confirming the "plausible but not confirmed" hypothesis this flag originally raised. **F039's "2 August 2026" / "six weeks away" framing is now confirmed stale and should be corrected** — see cross-node action below.

**(3) Official Journal citation — partially resolved, Low confidence.** The 27 July 2026 effective date is confirmed via secondary legal-alert sources, but the specific OJ citation number (e.g., "OJ L ..., 2026") could not be retrieved from those sources — recommend pulling the exact citation from eur-lex.europa.eu directly before formal publication-track use.

**(1) remains open** — article/annex numbers in this node are still Perplexity-synthesis-sourced, not NotebookLM-extracted from the primary EUR-Lex text; cross-check before citing in publication-track material.

**#227 — INVESTIGATED, still open (2026-07-31, Perplexity Deep Research).** (1) A live NANDO count and (2) confirmation of Article 43(6) delegated-act exercise status were both searched but **not found** in available secondary sources — Perplexity reports Low confidence/unverified for both and recommends checking the NANDO database (ec.europa.eu/growth/tools-databases/nando) directly, since a live regulatory database is not well-indexed by general web search. **Remains open** — this is a genuine "needs a direct database check" item, not resolvable via literature search; lower priority given (a) the underlying Annex III compliance deadline is now confirmed deferred to 2 Dec 2027 (see #226), reducing the practical urgency of an exact NANDO count today, and (b) #227's original severity was already LOW. (3) FPF/OneTrust staleness caveat remains valid and unaddressed by this pass.

---

*Node written: 2026-07-15 | Gap-directed sourcing (Gap #4, EU AI Act conformity assessment / notified bodies) — Perplexity Deep Research direct-citation method (methodological deviation from standard NotebookLM relay, see Source-method note above) | PRIS v2.2*
