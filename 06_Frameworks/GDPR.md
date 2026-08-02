---
type: Framework
tags:
  - type/framework
  - status/active
  - paper/p2
  - paper/p3
  - paper/p4-primary
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - content/wiki-entry
  - content/carousel-ready
---

# GDPR — Automated Decision-Making and AI Provisions

**Type:** Framework **Status:** Active **Last Updated:** 2026-08-02 (created — closes the vault's longest-standing forward reference)

**Scope note:** this node is deliberately scoped to GDPR's **automated decision-making, profiling and AI-relevant layer**, not to GDPR generally. General data-protection provisions are covered adequately at [[Privacy_DataProtection]] and by comparison against [[DPDP_Act_2023]]. What this node exists to hold is the material India does not have.

---

## Core Synthesis

GDPR Article 22 is the provision India's data-protection statute does not contain, and this node's analytical purpose in PRIS is to make that absence precise. The corpus has recorded for some time that DPDP 2023 has no ADM provision; what was missing was a specification of *what exactly* is absent — a general prohibition on solely-automated decisions with legal or similarly significant effect, four transparency hooks requiring "meaningful information about the logic involved," a statutory right to contest, and, since **SCHUFA (2023)**, a CJEU doctrine that pushes the regulated moment upstream from the lender's decision to the **score generator's** output. That last element is the one with the sharpest Indian application: it is precisely the seam left open by the Account Aggregator architecture.

## Framework Identity

- **Instrument:** Regulation (EU) 2016/679
- **Dates:** adopted 27 April 2016; applicable 25 May 2018
- **Consolidated text:** CELEX 02016R0679-20160504 — https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:02016R0679-20160504
- **Official Journal (canonical):** https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng
- **Binding status:** Binding EU Regulation, directly applicable

## Operative Text — the ADM layer

| Provision | Operative text / effect |
|---|---|
| **Art. 22(1)** | "The data subject shall have the right not to be subject to a decision based solely on automated processing, including profiling, which produces legal effects concerning him or her or similarly significantly affects him or her." **Per WP251 this is a general prohibition, not a right that must be actively invoked** — an important reading, and the one India lacks entirely |
| **Art. 22(2)** | Three exceptions: contractual necessity; Union/Member State law with safeguards; explicit consent |
| **Art. 22(3)** | Safeguards must include "the right to obtain human intervention on the part of the controller, to express his or her point of view and **to contest the decision**" |
| **Art. 22(4)** | Restricts special-category data in such decisions |
| **Art. 13(2)(f)** | Where data collected from the subject: inform of the existence of ADM and "at least in those cases, **meaningful information about the logic involved**, as well as the significance and the envisaged consequences" |
| **Art. 14(2)(g)** | Identical substantive obligation where data obtained from another source |
| **Art. 15(1)(h)** | Same disclosure, triggered by an access request rather than at collection |
| **Recital 71** | Interpretive: names "automatic refusal of an online credit application or e-recruiting practices without any human intervention" as paradigm cases; defines profiling as automated evaluation of "performance at work, economic situation, health, personal preferences or interests, reliability or behaviour, location or movements" |

**Architecture worth noting for coding:** the ADM right is delivered through **four separate provisions** — one prohibition (22), three transparency hooks (13/14/15) — plus a recital. India's DPDP delivers none of the four. This is not one missing clause but a missing sub-architecture, and stating it that way is more precise than "DPDP has no Article 22."

## Interpretive Layer

**WP29 Guidelines on Automated Individual Decision-Making and Profiling (WP251).** Adopted 3 October 2017; revised final 6 February 2018; **endorsed by the EDPB on 25 May 2018** and never superseded — it remains operative by carry-over rather than replacement.
https://www.edpb.europa.eu/documents/guideline/automated-decision-making-and-profiling_en
Two holdings that matter here: Art. 22 is a **general prohibition**; and "solely automated" excludes any *meaningful* human involvement — rubber-stamping does not take a decision outside Art. 22. That second point is the legal counterpart of the nominal-vs-effective distinction recorded at [[Human_Oversight]], and it is the only place in the corpus where that distinction has been given operative legal content by a supervisory authority.

## CJEU — SCHUFA and the upstream shift

**Case C-634/21, *OQ v Land Hessen*, 7 December 2023** — see [[07_Institutions/Corpus/International/International_36_CJEU_SCHUFA_C634_21]] for full treatment.

Three cumulative conditions for Art. 22: a decision; based solely on automated processing including profiling; producing legal effects or similarly significant effect. The Court held that a credit information agency's generation of a **probability value** is itself Art. 22 decision-making **where a third party draws strongly on it** — rejecting the argument that scoring is a mere "preparatory act." The regulated moment moves upstream from the lender to the scorer.

⚠ **No second CJEU judgment elaborating Art. 22 was located.** A source referring to "recent automated decision-making rulings" in the plural appears to discuss SCHUFA as the sole substantive ruling. Treat SCHUFA as the single leading authority.

## Enforcement — AI/algorithmic decisions (2020 onward)

| Authority | Target | Date | Fine | Doctrinal weight |
|---|---|---|---|---|
| Irish DPC | LinkedIn | Oct 2024 | **€310m** | Hidden behavioural profiling for targeted advertising without valid basis; corrective order to rebuild the profiling system. **Most significant for profiling doctrine** |
| Dutch AP | Clearview AI | Sep 2024 | **€30.5m** | Biometric facial-recognition collection without legal basis; processing ban with escalating penalties |
| Garante (IT) | OpenAI / ChatGPT | 20 Dec 2024 | **€15m** | Arts. 5, 6, 13, 14 — unlawful and non-transparent training-data processing, incl. minors' data. **Generative-AI training transparency, a distinct doctrinal category from Art. 22 profiling** |
| Hamburg DPA (DE) | financial services provider | 2025 | €492k | **Explicitly targets algorithmic decision-making** and inadequate transparency/accountability in an AI-driven process at an FI. Small fine, **highest relevance to [[P3_BFSI_JEIM]]** of any enforcement action located |
| Irish DPC | Meta | 22 May 2023 | €1.2bn | ⚠ **International transfers, not ADM.** Included only as a general GDPR benchmark — do not cite as ADM precedent |

## GDPR × AI Act — supervisory competence

See [[07_Institutions/Corpus/International/International_37_EDPB_AI_Opinions_and_Competence_2024_2026]].

- **EDPB Opinion 28/2024** (adopted 17–18 Dec 2024, Art. 64(2) GDPR): when AI models can be considered anonymous; whether legitimate interest can ground model development and use; consequences where a model was developed on unlawfully processed data. The most substantive EDPB document on AI–GDPR interaction to date.
- **EDPB–EDPS Joint Opinion 1/2026** (adopted 19–20 Jan 2026) on the Digital Omnibus on AI: **DPAs retain primary supervisory competence** over personal-data processing under AI Act Art. 2(7); the **AI Office** holds competence under Art. 75 only for AI systems built on a GPAI model **where model and system share a provider**, extending to systems integrated into VLOPs/VLOSEs under the DSA. Also flags that the EDPS's exclusive competence over EU-institution AI systems (Art. 74(9)) sits in recitals rather than operative text and should be codified.
- **Joint EDPB–Commission guidelines on AI Act–GDPR interplay: not yet published.** Confirmed in progress, expected 2026, modelled on the DMA–GDPR joint guidelines (draft 9 Oct 2025). Track.

**For [[Institutional_Coherence]]:** the EU has an explicit, published, statutorily-grounded allocation of supervisory competence between its data-protection and AI regulators, plus joint interpretive guidelines in preparation. India has four financial regulators plus MeitY issuing AI instruments with **zero cross-references** and no competence-allocation instrument of any kind. This is the sharpest available contrast on coordination — and unlike the ISO 42001 and Singapore comparisons, **this one survives inspection**: the EU really does have something here that India does not. Worth stating in P4 precisely because the other two benchmarks collapsed.

## India Comparison — what is actually missing

| Element | GDPR | DPDP 2023 |
|---|---|---|
| Prohibition on solely-automated significant decisions | Art. 22(1) | **None** |
| Right to human intervention | Art. 22(3) | **None** |
| Right to contest the decision | Art. 22(3) | **None** |
| Notice of ADM existence + logic (collection) | Arts. 13(2)(f), 14(2)(g) | **None** |
| Disclosure of ADM + logic on access request | Art. 15(1)(h) | **None** |
| Interpretive guidance on "solely automated" | WP251 | **None** |
| Judicial doctrine locating the decision at the scorer | SCHUFA | **None** |

**The Indian application of SCHUFA is the finding to carry forward.** [[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]] records that an Account Aggregator may lawfully deliver a complete financial profile to a Financial Information User which then runs an unregulated credit model on it — the consent layer is governed, the inference layer is not. **SCHUFA is precisely the doctrine that governs the inference layer, and India has no equivalent.** Under SCHUFA reasoning an Indian bureau generating a probability value that lenders draw strongly on would be engaged in regulated ADM. It is not, because no such provision exists. That is a concrete, doctrinally grounded, India-specific consequence of the Art. 22 gap, and it is considerably stronger than asserting the gap in the abstract.

## Confirmed Literature Gap

No dedicated law-journal article treats the DPDP's ADM absence as its **primary analytical focus**. The strongest located sources are an IJSSHR comparative paper (Feb 2026 — peer-reviewed but low-tier) and a Latham & Watkins comparison (12 Nov 2025) which states plainly: "The DPDPA does not provide the right to not be subject to automated decision-making," listed as a "No-action gap."

**Third confirmed white space located today**, after the fsQCA-DPI gap and the four-jurisdiction comparative gap. A paper built around *the missing ADM right in Indian data law* — DPDP's silence, read against Art. 22 + SCHUFA, applied to the AA/credit-bureau inference layer — has no incumbent. This is the most concrete P4 spin-off identified in the whole audit sequence.

## fsQCA Calibration

GDPR scores at or near full membership on RL for the ADM dimension: binding, prohibition-framed, with transparency hooks, an enforcement record, and judicial elaboration. It is the natural RL benchmark case for any EA constituent involving [[Contestability_Redress]] or [[Explainability]] — more so than the EU AI Act, whose conformity architecture does not yet operate (see [[07_Institutions/Corpus/International/International_33_CEN_CENELEC_JTC21_Harmonised_Standards_2026]]). **Where the thesis needs a case of a working binding AI-relevant regime, GDPR is it, and the AI Act is not.**

## Linked Projects

[[P4_Doctrinal_IJLIT]]

[[P3_BFSI_JEIM]]

[[P2_DPI_JSIS]]

[[fsQCA_Thesis_Chapter]]

## Linked Domains

[[Privacy_DataProtection]]

[[BFSI_Governance]]

[[AI_Governance]]

[[International_Comparators]]

## Linked Concepts

[[Contestability_Redress]]

[[Explainability]]

[[Transparency]]

[[Human_Oversight]]

[[Fairness]]

[[Accountability]]

[[Institutional_Coherence]]

[[Governance_Debt]]

## Linked Frameworks

[[DPDP_Act_2023]]

[[EU_AI_Act]]

[[DEPA]]

## Linked Corpus Nodes

[[07_Institutions/Corpus/International/International_36_CJEU_SCHUFA_C634_21]]

[[07_Institutions/Corpus/International/International_37_EDPB_AI_Opinions_and_Competence_2024_2026]]

[[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]]

## Future Research / Reuse Opportunities

- **"The missing ADM right in Indian data law"** — confirmed white space, concrete Indian application through the AA/bureau inference layer, and a live SCHUFA doctrine to anchor it. Strongest standalone P4 spin-off identified in this audit sequence.
- The four-provision architecture table (prohibition + three transparency hooks) is a clean carousel and reframes the India gap from "one missing clause" to "a missing sub-architecture."
- The EU competence-allocation material is the one benchmark comparison that has *survived* scrutiny this week — use it in P4 where the ISO 42001 and Singapore comparisons had to be softened.
- WP251's "solely automated excludes meaningful human involvement" is the only operative legal content the corpus holds for the nominal-vs-effective oversight distinction; feed into [[Human_Oversight]] and the Art. 14(4) coding scheme.

---

_Back to [[_Frameworks_MOC]]_
