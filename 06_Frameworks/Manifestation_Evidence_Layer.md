---
type: Framework
status: partial
last_updated: 2026-08-02
tags:
  - type/framework
  - status/partial
  - project/p3
  - engine/phd
---

# Manifestation Evidence Layer

**Type:** Framework **Status:** Partial — intent confirmed 2026-08-02, taxonomy still incomplete **Last Updated:** 2026-08-02

---

## Intent — CONFIRMED 2026-08-02

The 2026-07-31 stub inferred that this framework classified "how a regulatory obligation manifests as evidence" and explicitly warned against assuming that framing without checking RBI_1/RBI_2 usage context. **That check has now been done, and the inference was wrong.**

The actual usage is narrower and different. "Manifestation" here refers to the empirical manifestation of a **cross-regulator coordination pattern**, not to an obligation manifesting as an evidentiary artefact. The Manifestation Evidence Layer is the **P3 empirical evidence layer, held at SOM Tables S17–S21**, that documents where each coordination pattern is observed in the corpus. "Evidence" in this name means *research evidence for a coordination claim* — not evidence in the regulatory or forensic sense.

Confirmed from the two citing nodes:

- [[07_Institutions/Corpus/RBI/RBI_1]] — "§27(d) dual CERT-In + RBI incident reporting = M1 evidence"; and: "a concrete manifestation of Coordination Pattern M1 (Separate regulatory reporting channels for one event). This is a core evidence element in the Manifestation Evidence Layer (Tables S17–S21 of SOM)."
- [[07_Institutions/Corpus/RBI/RBI_2]] — "§17(h) three-level reporting chain... This is a concrete M1 pattern manifestation: same incident reported through multiple parallel channels to multiple regulators. Strong Manifestation Evidence Layer evidence."

---

## Pattern Taxonomy — INCOMPLETE

| Pattern | Definition | Evidence in vault |
|---|---|---|
| **M1** | Separate regulatory reporting channels for one event | **Current (2026):** [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] para 182 — "report cyber incidents within six hours of detection on DAKSH platform... shall also pro-actively notify CERT-In." Hardens the pattern with an explicit six-hour clock and a named platform; CERT-In leg remains loosely framed, preserving the specification asymmetry. **Antecedents (2023, superseded for Commercial Banks):** [[07_Institutions/Corpus/RBI/RBI_1]] §27(d) — RE shall notify both CERT-In and RBI for the same cyber incident; [[07_Institutions/Corpus/RBI/RBI_2]] §17(h) — three-level chain: service provider → RE → RBI within 6 hours → RBI/CERT-In. The three together give M1 a **2023 → 2026 time series with hardening at each step**, which is stronger evidence than any single instance. |
| **M2–M5** | ⚠ **Not recorded anywhere in the vault** | — |

⚠ **VERIFY / GAP.** Only M1 is defined in any vault note. The M2–M5 definitions exist, if at all, in `fsqca_SOM_V2.docx` Tables S17–S21 outside the vault. **They have not been reconstructed or inferred here.** Do not populate M2–M5 from memory or plausible guesswork — read them from the SOM and transcribe. Until then this framework supports M1 claims only.

---

## Relationship to Adjacent Infrastructure

**[[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]]** — the analytical companion. That matrix identifies and characterises coordination patterns across regulator pairs; this layer holds the corpus evidence substantiating each pattern claim. The matrix already cites this framework specifically for "RBI↔CERT-In M1 evidence." Matrix = claim; this note = evidence for the claim.

**[[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]]** — **no relationship despite the similar name, and the two must not be conflated in drafting.** That concept treats evidence as a *regulated artefact class* subject to specification, retention and custody obligations. This framework treats evidence as *research support for a coordination-pattern claim*. The name collision is unfortunate and pre-existing; both notes now carry a reciprocal disambiguation warning.

**[[08_Methods/Institutional_Grammar_IG2]]** — the stub asked whether this framework had been superseded by ADICO coding infrastructure. It has not. ADICO codes the internal grammar of individual institutional statements; this layer records cross-instrument coordination observations. Different units of analysis, both live.

---

## Linked Corpus Nodes

[[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] (current M1 instance) | [[07_Institutions/Corpus/RBI/RBI_1]] | [[07_Institutions/Corpus/RBI/RBI_2]]

## Linked Frameworks

[[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]]

## Linked Concepts

[[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — the M-patterns are the empirical manifestations of this construct at the BFSI-instrument level
[[05_Concepts/05_Concepts_Signature/Governance_Debt]] — dual-channel reporting is a cost borne by the regulated entity

## Linked Projects

[[02_Projects/P3_BFSI_JEIM]] (primary)

---

## Log

- 2026-08-02: Intent confirmed against RBI_1/RBI_2 usage context; the 2026-07-31 inferred framing ("obligation manifesting as evidentiary artefact") was **incorrect** and has been replaced. M1 populated from verified node text. M2–M5 left empty pending SOM transcription. Reciprocal disambiguation added against the newly created [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]], which the incorrect inferred framing closely resembled — had the stub been built out on that inference, the two would have silently merged.

---

*Back to [[_Frameworks_MOC]]*
