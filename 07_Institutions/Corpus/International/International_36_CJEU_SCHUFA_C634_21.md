---
type: Corpus Node
status: active
tags:
  - type/corpus-node
  - status/active
  - institution/international
  - paper/p4-primary
  - paper/p3
  - gate/open
  - engine/phd
---

# International_36 — CJEU C-634/21, *OQ v Land Hessen* (SCHUFA), 7 December 2023

**Framework:** [[GDPR]] | **Added:** 2026-08-02 (GDPR sourcing pass)

The corpus's **first CJEU judgment**, and the leading authority on GDPR Article 22.

---

## Document Identity

- **Court:** Court of Justice of the European Union, First Chamber
- **Procedure:** preliminary reference from the Verwaltungsgericht Wiesbaden (Germany)
- **Date:** 7 December 2023
- **Link:** https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=celex:62021CJ0634
- **Status:** final and binding; CJEU judgments are not subject to appeal

## Holding

The **automated establishment by a credit information agency of a probability value** concerning a person's ability to meet future payment commitments **constitutes "automated individual decision-making" within Article 22(1)** where a third party to which that value is transmitted **draws strongly on it** to establish, implement or terminate a contractual relationship.

Three cumulative conditions for Art. 22 to apply:

1. there is a **decision**;
2. it is based **solely on automated processing**, including profiling;
3. it produces **legal effects** or **similarly significantly affects** the individual.

The Court **rejected SCHUFA's "preparatory acts" argument**. The scoring agency itself — not only the downstream lender — engages in Art. 22-regulated decision-making.

## Doctrinal Significance

**The regulated moment moves upstream.** Aza (*International Journal of Law and Information Technology*, 30 Dec 2024) characterises this as a "dynamic reading" ascribing Art. 22(1) an **anticipatory element**: the "decision" is located in the generation of the score, not only in the human act of refusing credit. The practical effect is that an entity which never contracts with the data subject, never communicates with them, and formally only supplies a number to a client, is nonetheless the regulated decision-maker.

## The Indian Application — the finding to carry into P4

This is the corpus's clearest instance of a foreign doctrine that would, if it existed in India, close a gap the corpus has already independently identified.

[[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]] records that an Account Aggregator may lawfully deliver a complete financial profile to a Financial Information User, which then runs an unregulated model on it: **the consent layer is governed; the inference layer is not.** SCHUFA is precisely the doctrine that governs the inference layer.

Under SCHUFA reasoning, an Indian credit bureau or FIU generating a probability value on which lenders draw strongly would be conducting regulated automated decision-making, owing the data subject human intervention, a hearing, and a right to contest. **In India it owes none of these**, because [[DPDP_Act_2023]] contains no ADM provision at all — no prohibition, no right to contest, no obligation to disclose the logic. See [[GDPR]] for the full four-provision comparison.

This converts an abstract gap ("India has no Article 22") into a specific, sectorally located, doctrinally grounded claim about India's credit infrastructure — and it lands on the exact seam that [[DEPA]] and the AA architecture create. It is the strongest single argument available for a P4 spin-off paper.

## Connections

- **[[Contestability_Redress]]** — SCHUFA extends the *scope* of the Art. 22(3) contest right by widening who counts as the decision-maker. Note that Art. 22(1) is a **general prohibition** per WP251, not merely a right to be invoked; that reading should be reflected wherever the corpus treats Art. 22 as a "right."
- **[[Explainability]]** — where Art. 22 applies, Arts. 13(2)(f)/14(2)(g)/15(1)(h) attach, requiring "meaningful information about the logic involved." SCHUFA therefore expands explainability obligations upstream to score generators.
- **[[Human_Oversight]]** — the "solely automated" limb turns on whether human involvement is *meaningful*; WP251 confirms rubber-stamping does not exempt. This is the only operative **legal** content the corpus holds for the nominal-vs-effective oversight distinction, which that note treats as its defining boundary condition but had grounded only in Art. 14(4)(b)'s automation-bias clause.
- **[[Records_Rules_Asymmetry]]** — a subject scored by an agency they have no relationship with is the paradigm of being extensively represented as a data subject and not at all as a rule-bearing actor.

## Coding Notes (IG 2.0)

A judgment rather than an instrument, so ADICO extraction applies to the **rule it establishes** rather than to the text: Attributes = credit information agencies and comparable scorers; Deontic = must not (prohibition, per WP251); aIm = subject a person to a solely-automated significant decision; Conditions = where a third party draws strongly on the value; Or-else = supervisory enforcement under Ch. VIII. A complete ADICO — useful as a **fully-specified rule control case** against the corpus's many Indian ADIC norms with no Or-else.

Second judgment in the corpus after [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]], and the first from a supranational court. Note the contrast: DHC_1 is interim, prima facie and appealable; SCHUFA is final and binding. The corpus now has one settled and one unsettled judicial data point.

## Verification Notes

⚠ **No second CJEU judgment elaborating Article 22 was located.** One source referred to "recent automated decision-making rulings" in the plural but appears to discuss SCHUFA alone. Treat as the single leading authority; do not imply a line of cases.

## Related Nodes

- [[06_Frameworks/GDPR]] — parent framework
- [[07_Institutions/Corpus/International/International_37_EDPB_AI_Opinions_and_Competence_2024_2026]] — the interpretive/supervisory layer
- [[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]] — the Indian seam this doctrine would close
- [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] — the corpus's other judgment

## Linked Concepts

[[Contestability_Redress]] · [[Explainability]] · [[Human_Oversight]] · [[Records_Rules_Asymmetry]] · [[Accountability]] · [[Governance_Debt]]

## Linked Domains

[[BFSI_Governance]] · [[Privacy_DataProtection]] · [[DPI_Governance]] · [[International_Comparators]]

---

_Back to [[International]] | [[Corpus_Index_MOC]]_
