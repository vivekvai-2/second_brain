---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/meity
---

# MeitY_6 — Standard Operating Procedure to Curtail Dissemination of Non-Consensual Intimate Imagery (NCII) Content

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/MeitY/MeitY_6_SOP_NCII_Takedown_2025.md`
**Institution:** [[07_Institutions/MEITY]]
**Issuing body:** Ministry of Electronics and Information Technology, Government of India (in coordination with Ministry of Home Affairs/I4C, Ministry of Women and Child Development, Department of Telecommunications)
**Document date:** October 2025 (SOP document, "SOP NCII vers.1"); publicly announced via PIB press release dated 11 November 2025 (Release ID 2188886)
**Pages:** 9 (SOP) + 2 (PIB press release)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/DPI_Governance]]

**⚠ 2026-07-15 backlink:** [[07_Institutions/Corpus/MeitY/MeitY_7_IT_Intermediary_Guidelines_Digital_Media_Ethics_Code_Rules_2021]] is now the vault's dedicated primary-source node for the base 2021 Rules (including Rule 3(2)(b), which this SOP operationalises) — reference it for baseline Part II obligations rather than re-deriving them from this SOP node.

---

## Instrument Identity

**Full title:** Standard Operating Procedure to curtail dissemination of Non-Consensual Intimate Imagery (NCII) content, under Clause (b) of sub-rule (2) of Rule 3 of the Information Technology (Intermediary Guidelines and Digital Media Ethics Code) Rules, 2021
**Type:** Standard Operating Procedure (SOP) / implementation guidance document — explicitly **not** a rule, amendment, or independent source of obligation. Disclaimer (para 4) states the SOP "does not seek to replace, amend or alter any part of the IT Rules, 2021 and in no manner should be considered as part of the IT Rules, 2021."
**Target entities:** Individuals (victims, described in the document predominantly as "female victims"), intermediaries (including Significant Social Media Intermediaries — SSMIs), Content Delivery Networks (CDNs) and Domain Name Registrars (DNRs), One Stop Centres (OSCs, under Ministry of Women and Child Development), Indian Cybercrime Coordination Centre (I4C, under MHA), Department of Telecommunications (DoT), and Law Enforcement Agencies (LEAs)
**Legal basis:** Issued "in line with" directions of the Hon'ble High Court of Judicature at Madras in WP 25017/2025 (order dated 15.07.2025), directing MeitY to "provide a prototype as to what a victim girl must do when faced with situations of dissemination of NCII content." Operationalises Rule 3(2)(b) and 3(2)(c) of the IT (Intermediary Guidelines and Digital Media Ethics Code) Rules, 2021, with reference also to Section 79 (intermediary safe harbour) of the IT Act 2000, Rule 3(1)(d) (court/government takedown notifications), Rule 4(4) (SSMI proactive technology measures), the Indecent Representation of Women (Prohibition) Act 1986, and the Bharatiya Nyaya Sanhita 2023.
**Companion documents:** Operationalises the same base instrument as [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]] (IT Rules 2021) — MeitY_5 addresses the *draft* SGI/deepfake-labelling amendment to that base instrument, while MeitY_6 is a *notified, operative* SOP implementing an *existing* provision (Rule 3(2)(b)) of the same Rules. References the Grievance Appellate Committee (Rule 3A, in force since October 2022, discussed in MeitY_5) as the appeal mechanism (www.gac.gov.in). Also references the Sahyog Portal (I4C/MHA) as the inter-agency coordination platform for hash-sharing and URL-blocking referrals.

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S4 (Agentic AI Governance — deepfake/synthetic-content harms) / S5 (Data, Privacy & Security)
**Jurisdiction:** India
**Confidence:** HIGH for the SOP's procedural content (primary MeitY document, version-controlled "SOP NCII vers.1," October 2025, publicly released via PIB November 2025) — but ⚠ VERIFY BEFORE PUBLISHING: the SOP itself states it "is an evolving document and hence the versions of this document may undergo change," and instructs stakeholders to verify the latest version on the MeitY website before reliance. Any citation should note the version number (vers.1) and date.
**AI explicit:** PARTIAL — the SOP's operative legal basis (Rule 3(2)(b) IT Rules 2021) covers "artificially morphed images" generally and is not confined to AI-generated content; however, the PIB press release explicitly frames the SOP within the broader "deepfakes" governance conversation (the source filename itself pairs "Intimate Photos/Videos" with "deepfakes"), and the underlying harm category — non-consensual intimate imagery — is one of the most consequential real-world application domains for generative-AI/deepfake misuse. ⚠ VERIFY BEFORE PUBLISHING — the SOP text itself does not use the term "deepfake" or "AI-generated"; "artificially morphed images" (Rule 3(2)(b) language, reproduced verbatim from the 2021 Rules) is the operative term, and predates the generative-AI wave. Treat this node as **AI-adjacent** (covering a harm category increasingly produced via generative AI) rather than an AI-specific instrument.
**Tier classification:** Tier C — AI-adjacent governance (content-harm takedown procedure applicable to, but not exclusively concerned with, AI/deepfake-generated content)
**AI Governance Wiki relevance:** HIGH — this is the corpus's most operationally detailed **multi-agency incident-response/takedown workflow** for AI-relevant content harms, directly complementing [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]]'s draft SGI-labelling regime: MeitY_5 addresses *prevention/labelling at the point of upload*, while MeitY_6 addresses *post-publication takedown* — together forming a lifecycle pair for synthetic/non-consensual content governance in India.

---

## Substantive Content

### Origin and Judicial Mandate
The SOP was developed in direct response to a Madras High Court order (WP 25017/2025, dated 15.07.2025) directing MeitY to produce "a prototype as to what a victim girl must do when faced with situations of dissemination of NCII content." This is a notable instance of **judicially-prompted procedural rulemaking** — the SOP did not originate from MeitY's own regulatory cycle but from a specific writ petition, illustrating how India's content-governance procedures can be shaped by individual case litigation rather than only top-down policy design. ⚠ VERIFY BEFORE PUBLISHING — confirm whether WP 25017/2025 has any other reported orders/commentary that might further contextualise the SOP's scope or any subsequent compliance reporting to the Madras High Court.

### Scope of Covered Content (para 1(b), reproducing Rule 3(2)(b))
Four categories of content qualify for the 24-hour takedown mechanism when reported by the affected individual, an authorised representative, or an appropriate government/agency: (i) content prima facie exposing the individual's private area; (ii) content showing the individual in full or partial nudity; (iii) content showing/depicting the individual in any sexual act or conduct; and (iv) "artificially morphed images of such individual." The SOP explicitly **excludes** content relating to third persons that may be obscene or unlawful (para 1(d)) — i.e., this SOP is scoped strictly to first-person NCII victims, not general obscenity/content-moderation requests.

### Dual Takedown Pathways (para 1(c))
Two distinct legal triggers for intermediary takedown are reproduced in full: **Pathway A** — government/agency notification under Section 79(3)(b) read with Rule 3(1)(d), carrying a **36-hour** removal deadline from receipt of a court order or government notification (the SOP reproduces the full text of Section 79 and Rule 3(1)(d), including the safe-harbour-preserving proviso that voluntary removal under Rule 3(2)(b) "shall not amount to a violation" of Section 79(2) conditions). **Pathway B** — individual grievance under Rule 3(2)(b)/(c), carrying a **24-hour** removal deadline from receipt of complaint. ⚠ VERIFY BEFORE PUBLISHING — the SOP juxtaposes a 36-hour statutory deadline (Pathway A, government-triggered) against a 24-hour deadline (Pathway B, individual-triggered) without explicitly reconciling the two; both figures are reproduced directly from existing 2021 Rules text (not new to this SOP), but the practical interaction (e.g., whether the shorter 24-hour clock applies once an individual complaint is also lodged for content already subject to a government notification) is not addressed.

### Reporting Channels for Victims
Four parallel channels are detailed: (1) **One Stop Centres (OSCs)** under the Ministry of Women and Child Development (contact details via the Mission Shakti Portal), which can assist with NCRP filing, legal/psychological counselling, and LEA liaison; (2) **direct approach to intermediaries** via in-app reporting, Grievance Officers (Rule 3(2)(a)), or Trusted Content Flaggers, with escalation to the Grievance Appellate Committee (Rule 3A, www.gac.gov.in) if unresolved; (3) **National Cybercrime Reporting Portal (NCRP)** at cybercrime.gov.in or helpline 1930, under I4C/MHA; and (4) **direct complaint to local police stations (LEAs)**. The OSC pathway is notable for embedding NCII takedown within India's existing gender-based-violence support infrastructure (Mission Shakti) rather than creating a parallel dedicated mechanism — a "channel integration" design choice.

### Intermediary Obligations Beyond Basic Takedown
Beyond the core 24-hour removal, the SOP specifies: (a) **SSMI hash-matching/crawler obligations** under Rule 4(4) to prevent re-upload of identified NCII content across the platform; (b) **hash-sharing with I4C via the Sahyog Portal** for a centralised "secure NCII hash bank" intended to prevent resurfacing across *different* intermediaries — a cross-platform deduplication mechanism; (c) **periodic victim notification** of both removal and any resurfacing of flagged content; (d) **search-engine de-indexing** obligations; (e) **CDN/DNR obligations** to render flagged content inaccessible (deregistration or source-removal direction) within 24 hours of detection, including across multiple URLs hosting the same content. Note (e) extends the 24-hour takedown clock to infrastructure-layer actors (CDNs/DNRs) who are not "intermediaries" in the conventional platform sense — a notable expansion of the takedown ecosystem's scope of obligated parties.

### Inter-Agency Coordination Architecture
I4C (MHA) is positioned as the central aggregation point for both (a) NCII removal requests/grievances from OSCs, LEAs, and direct NCRP reports, and (b) the secure NCII hash bank. DoT coordinates ISP-level URL blocking based on referrals from government/LEAs/I4C. MeitY's own role is described narrowly as coordination with intermediaries "for compliance in a timely manner" — i.e., MeitY is positioned as a coordinating/oversight node rather than the primary operational actor, with MHA/I4C performing the operational aggregation function. This is a notable **inter-ministerial division of labour** (MeitY: rules/intermediary compliance; MHA/I4C: victim-facing aggregation and hash-bank infrastructure; MWCD: victim support via OSCs; DoT: ISP-level blocking) for a single harm category.

---

## Analytical Significance for PRIS Research

### For P1 (AI Governance SLR) and Synthetic-Media Governance Comparative Analysis
MeitY_6 and [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]] together form a **two-part lifecycle governance pair** for synthetic/non-consensual visual content in India: MeitY_5 (draft) targets *ex ante* prevention via mandatory SGI labelling at the point of creation/upload by SSMIs; MeitY_6 (operative) targets *ex post* takedown via a 24-hour multi-channel removal/hash-banking mechanism for already-published NCII content (a category substantially overlapping with, but broader than, "artificially morphed images"/deepfakes). For P1's comparative regulatory-configuration analysis, this pairing illustrates India's approach to one of the most consequential AI-harm categories (non-consensual sexual deepfakes) as **two separate instruments at two different stages of legislative maturity** (one notified/operative SOP under existing 2021 Rules; one draft amendment not yet gazetted) — a useful fsQCA configurational observation: "operative ex post remedy + draft ex ante prevention" as a transitional governance state for an emerging AI-harm category.

### For Institutional Coherence / Governance Capacity
The inter-agency coordination architecture (MeitY–MHA/I4C–MWCD–DoT, mediated via the Sahyog Portal and NCRP) is one of the corpus's most developed examples of **explicit, named, multi-ministry coordination for a single harm category** — a notable counterpoint to the largely siloed sectoral patterns observed in RBI/SEBI/IRDAI/MeitY data-governance instruments ([[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]], [[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025]]). If this NCII coordination model (single aggregation point at I4C, shared hash bank, defined ministry-to-ministry referral pathways) is generalisable, it could represent a positive [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] template for other AI-harm categories (e.g., AI-generated financial fraud content, election misinformation) — worth flagging as a candidate "coordination architecture" exemplar for any policy-recommendation output.

### Judicial-Origin Rulemaking as a Pattern
The SOP's origin in a specific High Court writ petition (rather than MeitY's own rulemaking cycle) is a distinct **regulatory-pathway** observation worth tracking across the corpus: whereas MeitY_4 (DPDP Rules) and MeitY_5 (draft IT Rules SGI amendment) originated through conventional notification/consultation cycles, MeitY_6 originated through **court-directed procedural compliance**. This raises a question (flagged for future batches) of whether other corpus instruments have similarly judicial origins not evident from the instrument text alone — relevant to any discussion of India's AI/digital-governance development as partly **reactive-judicial** rather than purely **proactive-administrative**.

### Coordination / Parallelism Pattern
**Existing nodes:** [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]] (same base instrument — IT Rules 2021 — different provisions: Rule 3(2)(b)/Rule 4(4) operative takedown vs. draft Rule 3(3)/4(1A) SGI labelling).
**Pattern:** **Within-instrument lifecycle complementarity** — both nodes operationalise different parts of the same 2021 Rules to address overlapping harm categories (synthetic/morphed imagery) at different lifecycle stages (pre-publication labelling vs. post-publication takedown), via different instrument types (draft amendment vs. operative SOP) and different originating triggers (regulatory cycle vs. judicial direction). This is a richer within-MeitY pattern than simple "parallelism" — it is closer to **complementary layering**, in contrast to the largely uncoordinated cross-regulator parallelism observed for BFSI algorithmic-governance provisions (MeitY_4/RBI_6/SEBI_9-11).

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]] (same base instrument — IT Rules 2021; lifecycle-complementary pairing on synthetic/morphed media governance), [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (same issuing ministry; different domain — data protection vs. content takedown)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] (multi-ministry NCII coordination architecture as a candidate positive exemplar), [[05_Concepts/05_Concepts_Standard/Accountability]] (intermediary/CDN/DNR takedown obligations with defined timelines), [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] (I4C hash-bank infrastructure as institution-building), [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] (AI-harm content lifecycle — labelling + takedown)
**Related frameworks:** Candidate component of a future "India Synthetic Media / Deepfake Governance" framework synthesis node, alongside MeitY_5 (per MeitY_5's Connections section)
**Related projects:** [[02_Projects/P1_SLR_RG]] (AI Governance SLR — synthetic-media/deepfake harm governance comparative element), [[08_Methods/Institutional_Grammar_IG2]] (the 24-hour/36-hour dual-deadline structure and multi-actor obligation chain (intermediary/SSMI/CDN/DNR/I4C/DoT) is a strong ADICO multi-Attribute coding candidate)
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] (S4 — synthetic media/deepfake governance, paired with MeitY_5)
**Related consulting:** Potentially relevant to AEGIS_OS if engagement scope expands to platform/intermediary clients requiring NCII/deepfake takedown-compliance workflow design (cross-reference MeitY_5's consulting note).

---

## Coding Status

- **P3 NVivo:** Not primary BFSI evidence — flag for P1 SLR screening corpus given direct relevance to synthetic/non-consensual content governance
- **Wiki intake status:** Pending — HIGH priority for S4, to be processed alongside MeitY_5 as a lifecycle pair

---

## Log

- 2026-06-15: Corpus node created. Batch 7. Cowork session. Document 7 of 9. Source comprises a 2-page PIB press release (11 Nov 2025) plus the 9-page SOP (Oct 2025, "SOP NCII vers.1"). Flagged as version-controlled/evolving document per the SOP's own disclaimer — re-verify current version before citation in future sessions.
