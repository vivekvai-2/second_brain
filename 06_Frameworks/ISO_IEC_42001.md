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

**Type:** Framework **Status:** Active **Last Updated:** 2026-08-09 (addendum — unresolved NABCB/ISO 42006 contradiction flagged, see India section; originally created 2026-08-02, 32 referencing notes, no node)

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
| **ISO/IEC 42006** | Requirements for bodies auditing/certifying AIMS | **Not published** | **Work item in development** (confirmed by UKAS) |

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
| **Accreditation scheme** | ❌ **No NABCB published accreditation programme, scheme document, or auditor-competence guidance located** — confirmed gap |
| **Regulatory recognition** | ❌ No Indian regulator recognises certification as compliance evidence |

India has adopted an AI management-system standard and is training lead auditors against it, with no confirmed national accreditation scheme for the certification bodies those auditors would work for, and no regulator that treats the resulting certificate as meaning anything. **A fourth instance of the "institution before regulation" sequencing pattern** already recorded for CSIRT-Power, the AA regime, and Sahamati — here in the form *standard before scheme before recognition*.

⚠ The IS/ISO/IEC 42001 adoption is confirmed from a BIS-hosted NITS course brochure, not from a gazette or catalogue entry. **The exact adoption date is not pinned.** Verify against Manakonline before citing a date.

> ⚠ **ADDENDUM (2026-08-09) — unresolved contradiction, do not silently update the table above.** [[07_Institutions/Corpus/Parliament/Parliament_2_Unstarred_Question_2988_Institutional_Framework_Auditing_AI_2026]] (Lok Sabha answer, 5 August 2026 — three days after this node's "confirmed gap" finding) states as government fact that "National Accreditation Board for Certification Bodies (NABCB)... has developed accreditation framework for Artificial Intelligence Management System (AIMS) certification as per ISO/IEC 42001:2023," accrediting bodies "as per ISO/IEC 17021-1:2015 and ISO/IEC 42006:2025" — which would mean both the NABCB accreditation scheme *and* ISO/IEC 42006 itself are further along than this node's UKAS-sourced finding shows. **This directly contradicts the "❌ confirmed gap" row above and is not yet resolved.** Do not treat either source as settling the question; check NABCB's own website/gazette for a dated, named AIMS accreditation scheme document before revising the table. See VERIFY #304 on the Parliament_2 node for the full reasoning.

## Assurance Quality Gap

ISO/IEC 42006 — the scheme-specific standard defining auditor competence for AIMS certification — **is not published**. Certification bodies are therefore accrediting and auditing against ISO/IEC 42001 under the generic requirements of ISO/IEC 17021-1, with no AI-specific competence standard in force. UKAS confirms 42006 is "currently being developed" and will "help accreditation bodies assess the technical competence of these bodies in a harmonised manner" — future tense.

No dedicated IAF mandatory document specific to ISO/IEC 42001 was located. ANAB is the largest accreditor (early accredited bodies: Schellman first, then A-LIGN, SGS, DEKRA, Coalfire, TÜV, Sensiba); BSI became the first UKAS-accredited body in late 2025.

**Consequence:** a market in AI management-system certificates is operating ahead of the competence standard that would make those certificates comparable. That is [[Evidentiary_Governance]] territory — certificates are being produced whose evidentiary weight is undefined.

## fsQCA Calibration

The [[Assurance_Reuse_Gap]] note proposes cross-recognition (specifically "ISO/IEC 42001 mapped to sectoral audit requirements") as a candidate calibration point for the **SR (Structural Readiness)** condition. **That calibration is not currently viable**: the condition would score at or near full non-membership for every case in the corpus, including the EU, because no jurisdiction grants recognition. A condition with no cross-case variance carries no configurational information.

Recommended: recalibrate SR on *whether a national accreditation scheme exists* rather than on regulatory recognition. That does vary — ANAB and UKAS have operating schemes, NABCB does not — and it is the layer where institutional capacity actually differs.

## Key Tensions & Gaps

- **The India-lags framing does not hold here.** On ISO/IEC 42001 recognition, India, the EU, the US and the UK are all at zero. India lags on the *accreditation* layer, not the recognition layer.
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
- India-specific: the NABCB accreditation gap is an actionable policy recommendation with a named recipient, and BIS LITD 30's 5 August 2026 meeting is a live engagement window.

---

_Back to [[_Frameworks_MOC]]_
