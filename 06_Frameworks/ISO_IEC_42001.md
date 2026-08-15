---
type: Framework
tags:
  - type/framework
  - status/active
  - paper/p3-primary
  - paper/p4
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - engine/knowledge-product
  - content/wiki-entry
  - content/carousel-ready
---

# ISO/IEC 42001 — AI Management System Standard

**Type:** Framework **Status:** Active **Last Updated:** 2026-08-15 (⚠#304 resolved against this node — ISO/IEC 42006 published, NABCB scheme exists; accreditation-gap finding reversed, fsQCA recalibration withdrawn, consulting recommendation inverted. Originally created 2026-08-02)

---

## Core Synthesis

ISO/IEC 42001:2023 is the first international management-system standard for artificial intelligence, and within PRIS its analytical value lies almost entirely in what it **cannot** do. The sourcing pass that created this node was designed to answer one question: does any regulator, anywhere, recognise ISO/IEC 42001 certification as evidence of regulatory compliance? The answer is a confirmed global no — and the reason is not administrative lag but a **unit-of-certification mismatch**. ISO/IEC 42001 certifies that an *organisation* operates a functioning AI management system. The EU AI Act regulates *individual AI systems as products*, assessed at market placement. These are different objects of assessment, and no amount of mapping reconciles them. This finding converts [[Assurance_Reuse_Gap]] from an India-specific coordination failure into a structural property of the global AI assurance market, and it corrects a claim previously held in that note (see below).

## Framework Identity

- **Full title:** ISO/IEC 42001:2023, *Information technology — Artificial intelligence — Management system*
- **Issuing body:** ISO/IEC JTC 1/SC 42
- **Publication:** December 2023 (secondary sources converge on 18 December 2023; the ISO catalogue displays month precision only). First edition
- **Status:** Stage 60.60, published, current. **No amendment or corrigendum located; no revision cycle initiated**
- **Binding status:** Voluntary consensus standard; certifiable
- ⚠ **Link defect:** the sourcing return gave the ISO catalogue link as a generic Russian-language OBP root (`iso.org/obp/ui/ru/`) rather than a record URL. Retrieve the canonical record from `iso.org/standard/` before citing

**Companion standards:**

| Standard | Title | Published | Status |
|---|---|---|---|
| ISO/IEC 23894:2023 | AI — Guidance on risk management | Feb 2023, 26pp | Stage 60.60, current |
| ISO/IEC 22989:2022 | AI concepts and terminology | Jul 2022, 60pp | Stage 60.60, current. ⚠ A secondary source claims "2025 updates" adding foundation-model terminology; **unverified against the ISO catalogue** — treat as commentary, not a formal amendment |
| **ISO/IEC 42006** | Requirements for bodies auditing/certifying AIMS | **Published 2025-07, Ed. 1, 31pp** | **Stage 60.60, current.** ✅ **CORRECTED 2026-08-15** — the earlier "not published / in development (confirmed by UKAS)" entry was **wrong**. Confirmed against the ISO catalogue, IEC Webstore, ANSI, BSI (BS ISO/IEC 42006:2025, adopted 31 Jul 2025) and a Standards Council of Canada **transition bulletin** — a national accreditation body would not issue a transition bulletin for an unpublished standard |

## The Core Finding — no presumption of conformity anywhere

**Confirmed absent, not merely unconfirmed.** Three independent lines of evidence:

1. **The European Commission's own position.** Its AI Act standardisation page states that harmonised standards — CEN-CENELEC JTC 21 deliverables — are the mechanism that "will offer legal certainty under the AI Act." ISO/IEC 42001 is not among them.
2. **The European AI Office signalled in May 2024** that ISO/IEC 42001 is *not fully aligned* with the final AI Act text and is not part of the EU harmonisation process.
3. **The legal mechanism forecloses it.** AI Act **Article 40** grants presumption of conformity only to harmonised standards published and cited in the *Official Journal*. As of June 2026, **zero AI-specific harmonised standards have been cited in the OJ.** Presumption of conformity currently attaches to nothing at all.

**Why it is structural, not temporal.** ISO/IEC 42001 is an organisational management-system standard; the AI Act assesses individual systems as products at market placement. A categorical mismatch in the unit of assessment. Even a perfect crosswalk cannot make an organisation-level certificate discharge a system-level conformity obligation. This is the analytically important point and the one worth publishing.

**No ISO-issued crosswalk exists.** Every located mapping is third-party: a Microsoft-authored NIST AI RMF ↔ 42001 crosswalk hosted on NIST's AIRC index (NIST explicitly disclaims endorsement), and a commercial tool claiming 99 ISO 42001 mappings. NIST's own January 2023 crosswalk maps AI RMF to the OECD Recommendation, the proposed AI Act, EO 13960 and the AI Bill of Rights — not to 42001.

## The EU Harmonised-Standards Track (CEN-CENELEC JTC 21)

**prEN 18286** — *AI — Quality Management System for EU AI Act Regulatory Purposes*. Maps to AI Act Art. 17; informative Annex ZA maps to Arts. 11, 17 and 72. Public enquiry 30 Oct 2025–22 Jan 2026; at **Approval (Formal Vote)** stage as of June 2026; target availability Q4 2026. Will be the **first standard anywhere to carry Article 40 presumption of conformity** once cited in the OJ.

| Deliverable | Subject | AI Act Article | Stage (Jun 2026) |
|---|---|---|---|
| prEN 18228 | AI risk management | Art. 9 | Enquiry |
| prEN 18229-1 | Trustworthiness — logging | Art. 12 | Enquiry |
| prEN 18282 | Cybersecurity specifications | Art. 15 | Enquiry |
| prEN 18229-3 | Transparency and human oversight | Arts. 13, 14 | Drafting |
| prEN 18283 | Managing bias in AI systems | (bias) | Drafting; WD consultation closed 30 Apr 2026 |

**Zero published; zero cited in the OJ.** Commission mandate deadline amended to 28 February 2027. These are drafted as distinct EU instruments, **not** as adoptions of ISO/IEC 42001.

## India — adoption without a scheme

Three layers, and only two are built:

| Layer | Status |
|---|---|
| **Standard adopted** | ✅ **IS/ISO/IEC 42001** — BIS has adopted the ISO text under Indian Standard numbering |
| **Auditor training** | ✅ BIS's National Institute of Training for Standardization (NITS, Noida) runs a 5-day Lead Auditor course against it (course held 15–19 Dec 2025) |
| **Accreditation scheme** | ✅ **EXISTS — finding reversed 2026-08-15.** **NABCB 220, *Accreditation Criteria for Artificial Intelligence Management System (AIMS)*, April 2026** (nabcb.qci.org.in), clause 2.0 requiring compliance with ISO/IEC 17021-1 **and ISO/IEC 42006:2025**; amendment record reads "Apr 2026 — CEO — Criteria aligned with ISO/IEC 42006:2025". **Three accredited certification bodies** on the public register: **AI 001** TUV India (11 Feb 2025–10 Feb 2028), **AI 002** TUV SUD South Asia (5 Aug 2025–4 Aug 2028), **AI 003** Maverick Quality Advisory (31 Mar 2026–30 Mar 2029). Scheme is **operational, not paper**: Mphasis announced NABCB-accredited ISO/IEC 42001 certification from TÜV SÜD South Asia in October 2025 (i.e. under AI 002) |
| **Regulatory recognition** | ❌ No Indian regulator recognises **ISO/IEC 42001** certification as compliance evidence. **This row survives** — it is the accreditation row that was wrong, not this one. See the corrected ISO 27001 block below |

> ### The ISO 27001 contrast — narrowing this finding, 2026-08-09
>
> The claim "no Indian regulator recognises certification as compliance evidence" was stated too broadly and should be read as specific to **ISO/IEC 42001**. [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] reg 5(24) **mandates** that power-sector entities "ensure compliance with and acquire **ISO/IEC 27001 certificate or Technical Criteria Certificate** encompassing all critical systems," with a bar on four consecutive certification audits by the same agency or personnel, and places the certificate in the CISO's mandatory custody under the First Schedule.
>
>> 🔴 **CORRECTION 2026-08-15 — reg 5(24) is NOT in force.** Verified against the CEA-hosted notified PDF (`cea.nic.in/wp-content/uploads/notification/2026/08/Cyber_Regulations_Notification.pdf`): **reg 1(2) defers 5(9), 5(24), 5(33), 5(39), 6(2) and 6(7)** to dates "as may be specified by the Authority through separate orders with prior approval of the Central Government." **No such order had issued as at 15 August 2026.** CEA_3 recorded this deferral correctly in three places and then reasoned from 5(24) as though it were operative in a fourth — which is precisely what its own ⚠#312 warns against.
>
> **Restated:** India has *enacted* a mandate for a management-system certificate as a binding compliance obligation, and has **not brought it into force**, with no commencement date. The correct comparison is therefore enacted-but-dormant ISO 27001 recognition against wholly absent ISO 42001 recognition — a weaker contrast than the one originally drawn, though it points the same way.
>
> **This still sharpens the "certification without recognition" thesis, but less sharply than claimed on 2026-08-09** (see correction immediately above). The contrast is now internal to India and internal to the ISO management-system family, which is a cleaner comparison than the cross-jurisdictional one: the same regulator, in the same instrument, mandates ISO 27001 and says nothing about AI management systems. The unit-of-certification argument explains why — ISO 27001 certifies an organisational security posture that maps directly onto CEA's entity-level obligations, whereas ISO 42001 would have to discharge system-level AI conformity obligations **that do not exist anywhere in Indian law**. There is nothing for a 42001 certificate to be recognised *against*.
>
> **A second Indian accreditation regime also appears here.** CEA_3 reg 3(1)(jj) defines the **Technical Criteria Certificate** as one "issued to an organisation by a designated certification body **accredited** for ensuring conformance to cyber security standards specified by the Central Government." That sits alongside the unresolved NABCB/AIMS accreditation question at ⚠ #304 (see the India section below) and is worth checking when that flag is resolved — the two may share an accreditation body.

> 🔴 **REWRITTEN 2026-08-15 — the original paragraph rested on the accreditation gap, which was false.**

India has adopted an AI management-system standard, trains lead auditors against it, **and operates a national accreditation scheme through NABCB with three accredited certification bodies and certificates already issued to clients** — while **no Indian regulator treats the resulting certificate as evidence of anything.**

**This is a stronger finding than the one it replaces, not a weaker one.** The original read as capacity lag: India had not yet built the scheme. The corrected reading is that India built the full assurance apparatus — standard, auditor training, accreditation criteria, accredited bodies, live certifications — and then attached **no regulatory consequence** to its output. That is not lag; it is a completed institutional investment with a missing final link, and it is a much better instance of [[Assurance_Reuse_Gap]] than the gap version was.

**The sequencing pattern also inverts.** This is *not* a fourth "institution before regulation" instance in the CSIRT-Power / AA / Sahamati sense. Those are institutions built ahead of the rules that would govern them. Here the **entire assurance chain** — standard → scheme → accredited bodies → certificates — was completed ahead of any rule that would *use* it. Propose recording it as a distinct variant: **assurance before demand**.

**Accreditation ran ahead of the standard, too.** NABCB accredited **AI 001 (TUV India) on 11 February 2025** — five months before ISO/IEC 42006 was published in July 2025 — against the **DIS**. NABCB's public scheme-listing webpage still carries the stale "ISO/IEC DIS 42006" caption, which is what the 2 August 2026 pass appears to have read. India accredited AIMS certification bodies against a draft international standard and transitioned to the published text in April 2026. ⚠#355.

⚠ The IS/ISO/IEC 42001 adoption is confirmed from a BIS-hosted NITS course brochure, not from a gazette or catalogue entry. **The exact adoption date is not pinned.** Verify against Manakonline before citing a date.

> ✅ **RESOLVED 2026-08-15 — Parliament_2 was right on the substance; this node was wrong.** ISO/IEC 42006 **is** published (July 2025) and NABCB **does** operate a dated, named AIMS accreditation scheme (NABCB 220, April 2026) with three accredited bodies. The Framework Identity and India tables above have been corrected. **⚠#304 is closed on the substance but a residual remains: the underlying Lok Sabha document itself could not be located** — see ⚠#354 below. The 2026-08-09 instruction not to silently prefer one source was correct and was followed: both were checked against third sources, and the third sources vindicate Parliament_2.
>
> **Original addendum retained below for the audit trail.**
>
> ⚠ **ADDENDUM (2026-08-09) — unresolved contradiction, do not silently update the table above.** [[07_Institutions/Corpus/Parliament/Parliament_2_Unstarred_Question_2988_Institutional_Framework_Auditing_AI_2026]] (Lok Sabha answer, 5 August 2026 — three days after this node's "confirmed gap" finding) states as government fact that "National Accreditation Board for Certification Bodies (NABCB)... has developed accreditation framework for Artificial Intelligence Management System (AIMS) certification as per ISO/IEC 42001:2023," accrediting bodies "as per ISO/IEC 17021-1:2015 and ISO/IEC 42006:2025" — which would mean both the NABCB accreditation scheme *and* ISO/IEC 42006 itself are further along than this node's UKAS-sourced finding shows. **This directly contradicts the "❌ confirmed gap" row above and is not yet resolved.** Do not treat either source as settling the question; check NABCB's own website/gazette for a dated, named AIMS accreditation scheme document before revising the table. See VERIFY #304 on the Parliament_2 node for the full reasoning.

## Assurance Quality Gap

ISO/IEC 42006 — the scheme-specific standard defining auditor competence for AIMS certification — **is not published**. Certification bodies are therefore accrediting and auditing against ISO/IEC 42001 under the generic requirements of ISO/IEC 17021-1, with no AI-specific competence standard in force. UKAS confirms 42006 is "currently being developed" and will "help accreditation bodies assess the technical competence of these bodies in a harmonised manner" — future tense.

No dedicated IAF mandatory document specific to ISO/IEC 42001 was located. ANAB is the largest accreditor (early accredited bodies: Schellman first, then A-LIGN, SGS, DEKRA, Coalfire, TÜV, Sensiba); BSI became the first UKAS-accredited body in late 2025.

**Consequence:** a market in AI management-system certificates is operating ahead of the competence standard that would make those certificates comparable. That is [[Evidentiary_Governance]] territory — certificates are being produced whose evidentiary weight is undefined.

## fsQCA Calibration

The [[Assurance_Reuse_Gap]] note proposes cross-recognition (specifically "ISO/IEC 42001 mapped to sectoral audit requirements") as a candidate calibration point for the **SR (Structural Readiness)** condition. **That calibration is not currently viable**: the condition would score at or near full non-membership for every case in the corpus, including the EU, because no jurisdiction grants recognition. A condition with no cross-case variance carries no configurational information.

> 🔴 **WITHDRAWN 2026-08-15.** The recommendation below rested on the false premise that NABCB has no scheme. **It does** — NABCB 220 (April 2026), three accredited bodies. Recalibrating SR on scheme existence would have scored India at **full non-membership on a condition where it is actually a member**, mis-specifying the fsQCA condition for the Indian case. Flagged as ⚠#356; this would have propagated into the fsQCA chapter had it not been caught.
>
> ~~Recommended: recalibrate SR on *whether a national accreditation scheme exists* rather than on regulatory recognition. That does vary — ANAB and UKAS have operating schemes, NABCB does not — and it is the layer where institutional capacity actually differs.~~
>
> **Replacement recommendation:** SR does not vary usefully on either recognition *or* scheme existence — India, the EU, the US and the UK all now have operating accreditation schemes and none grants recognition. Recalibrate on a layer that does vary, or drop SR and re-derive the condition set.

## 🔷 Standards-Setting Participation Asymmetry, Quantified (2026-08-09)

Source: [[07_Institutions/Corpus/International/International_38_World_Bank_WDR2026_AI_Governance]] Ch.9, primary text; drawing on Hennessy, Radu and von Ingersleben-Seip (2026) and Galvagna (2023).

This note has carried the participation problem as a qualitative assertion. WDR 2026 supplies numbers.

| Finding | Value |
|---|---|
| AI-related standards published or under development, across all bodies | **more than 800** |
| Share of **ISO/IEC** AI standards-committee members from developing countries | **one-third** |
| Countries party to **all seven** sampled non-UN AI governance initiatives | **7** — Canada, France, Germany, Italy, Japan, UK, US. All high income. |
| Countries party to **none** | **118** |
| African Group members involved in none | **48 of 54** |

The report is explicit that standards are not neutral instruments: *"Whoever writes these standards determines the definitions of value-laden terms like fairness, safety, and risk"* (Hennessy et al. 2026; Solow-Niederman 2023). Barriers to participation for civil society and developing-country policy makers are named as the time commitment, opacity of standards-development processes, and industry dominance within them.

**The Seoul Statement — a live commitment worth tracking.** In **December 2025**, the **IEC, ISO and ITU** jointly issued a statement committing to *"deepening their understanding of the relationship between international standards and human rights, incorporating sociotechnical dimensions into the development of standards, and strengthening the multistakeholder community for developing and applying AI standards."* Whether this produces procedural change in SC 42 is the thing to watch, and it is the natural place to look for movement on the accreditation and competence layers this note tracks.

**Bearing on ⚠#304 (the NABCB / ISO/IEC 42006 contradiction).** WDR 2026 does not resolve it — the report says nothing about NABCB or 42006 specifically. But it does establish two things that shift the priors slightly:
1. **BIS is a P-member of SC 42 and hosted the 15th plenary in New Delhi (April 2025).** India's participation in the standards layer is active, not nominal — which makes it more plausible, not less, that NABCB has moved on an AIMS scheme ahead of UKAS-sourced visibility.
2. **The report treats ISO/IEC 42005 (AI System Impact Assessment) as published**, alongside ISO/IEC 42001 and the NIST AI RMF, in its list of standards giving organisations operational guidance. If 42005 is out, the 42006 timeline warrants a fresh direct check rather than reliance on the UKAS "currently being developed" language recorded above.

**Neither point settles the contradiction.** The instruction stands: retrieve a dated, named NABCB AIMS accreditation scheme document, and check the ISO catalogue entry for 42006 directly, before revising the Framework Identity table.

## Key Tensions & Gaps

- **The India-lags framing does not hold here.** On ISO/IEC 42001 recognition, India, the EU, the US and the UK are all at zero. India lags on the *accreditation* layer, not the recognition layer.
- **⚠ The "no jurisdiction grants recognition" finding needs narrowing as of 2026-08-09.** It is accurate for ISO/IEC 42001 specifically. It is **not** accurate as a general statement about voluntary-standards recognition: WDR 2026 Ch.9 records that **Colorado and Texas grant liability safe harbour for NIST AI RMF compliance**, and that the EU AI Act treats CEN-CENELEC harmonised standards as a route to demonstrating conformity. So the correct statement is: *no jurisdiction grants recognition to **ISO/IEC 42001**; two US states grant it to **NIST AI RMF**; the EU has built the mechanism for **harmonised standards** but has cited none.* See [[Assurance_Reuse_Gap]], which now carries this as a four-way typology. **This materially affects the fsQCA SR calibration discussion above** — the recognition condition varies after all, just not on the standard this note tracks.
- **BIS LITD 30 is active but has published nothing.** Scope: "Standardization in the area of Artificial Intelligence and Big Data"; P-member of ISO/IEC JTC 1/SC 42; 46th sectional committee meeting scheduled **5 August 2026**. Only two potential proposals located — "Reliability of AI systems" and "Guidance for Generative AI Applications" — neither a published standard nor a draft under public comment.
- SC 42 had published 35 AI standards with 47 under development as of its 15th plenary (New Delhi, hosted by BIS, April 2025).

## Linked Projects

[[P3_BFSI_JEIM]]

[[P4_Doctrinal_IJLIT]]

[[fsQCA_Thesis_Chapter]]

## Linked Domains

[[AI_Governance]]

[[BFSI_Governance]]

[[Cybersecurity_Governance]]

[[International_Comparators]]

## Linked Concepts

[[Assurance_Reuse_Gap]]

[[Evidentiary_Governance]]

[[Governance_Debt]]

[[Governance_Capacity]]

[[Institutional_Coherence]]

[[Proportionality]]

[[Accountability]]

## Linked Frameworks

[[EU_AI_Act]]

[[NIST_AI_RMF]]

## Linked Institutions

[[BIS]]

## Linked Corpus Nodes

[[07_Institutions/Corpus/BIS/BIS_1_LITD30_and_IS_ISO_IEC_42001_Adoption]]

[[07_Institutions/Corpus/International/International_33_CEN_CENELEC_JTC21_Harmonised_Standards_2026]]

[[04_Knowledge_Products/Wiki_Intake/F034_Buscemi_Assessing_High_Risk_AI_2025]]

## Future Research / Reuse Opportunities

- **"Certification without recognition"** is a publishable paper on its own — a global market in AI management-system certificates with no regulator anywhere granting them evidentiary status, and a structural (not temporal) reason why. Target: *Regulation & Governance*.
- The unit-of-certification mismatch (organisation-level standard vs system-level regulation) is a clean theoretical contribution and generalises beyond AI to any management-system standard facing product regulation.
- Practitioner angle with immediate consulting value: clients pursuing ISO 42001 for EU AI Act readiness are frequently sold it as compliance. It is not, and the EU AI Office said so in May 2024. A short corrective piece would land well with CROs and GCs.
- ~~India-specific: the NABCB accreditation gap is an actionable policy recommendation with a named recipient~~ 🔴 **WITHDRAWN 2026-08-15 — the gap does not exist.** Recommending that NABCB build a scheme it published in April 2026 would have been a credibility failure in front of the named recipient. **The defensible India recommendation is the opposite one:** NABCB has built the accreditation layer and no Indian regulator uses its output — the ask is *regulatory recognition*, addressed to RBI/SEBI/IRDAI/MeitY, not scheme creation addressed to NABCB. BIS LITD 30's 5 August 2026 meeting remains a live engagement window. Logged as **C-03** at [[11_Content/Content_Correction_Register]].

---

_Back to [[_Frameworks_MOC]]_
