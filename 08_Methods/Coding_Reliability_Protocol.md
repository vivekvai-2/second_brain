---
type: Method
tags:
  - type/method
  - status/active
  - paper/p2
  - paper/p3
  - paper/fsqca-primary
  - gate/open
  - engine/phd
---

# Coding Reliability Protocol

**Type:** Method **Status:** Active — created 2026-08-02 (methods sourcing pass)
**Role:** the reliability layer beneath [[Institutional_Grammar_IG2]]; ⚠ **contains two corrections to the vault's stated protocol**

---

## Core Synthesis

PRIS records its reliability protocol as "20% random subsample double-coded by second coder; Cohen's κ reported… κ ≥ 0.75." This note records what the methodological literature and the Institutional Grammar field itself actually specify — which differs in two respects that need deciding before Q3 2026 coding begins, not defended afterwards.

## ⚠ Correction 1 — the terminology is wrong

**Halpin (2024, *American Journal of Qualitative Research*)** distinguishes:

- **Inter-Coder Agreement (ICA)** — for **pre-established deductive codebooks**
- **Inter-Rater Reliability (IRR)** — for inductive/emergent coding

ADICO/IG 2.0 is a pre-established deductive schema. **ICA is the technically correct framing; the vault currently says "inter-coder reliability" throughout.** A minor point in substance, a real one to a methods reviewer, and free to fix.

## ⚠ Correction 2 — PRIS departs from IG field practice, and hasn't said so

**The IG field standard is simple percent agreement, not kappa.** From the IG 1.0 Codebook (Brady et al., 2018), verbatim:

> "It is recommended that coding be assessed by another coder. Preferably 20% of the coded statements should be subject to intercoder reliability testing. At this time, coder agreement is generally assessed through **simple percent agreement**… intercoder agreement ≤85% is evidence of low coder agreement and should result in codebook revisions and re-testing"

citing Guest & MacQueen (2008) generally, and **Basurto et al. (2010)** and **Siddiki et al. (2011)** for the ≥80% threshold specific to IG. Siddiki (2009) states the iterative requirement: "Coding method should be iteratively revised until the eighty percent criterion is met."

**PRIS's 20% subsample matches the field standard exactly. Its choice of Cohen's κ does not.**

**The departure is defensible and arguably superior** — percent agreement does not correct for chance agreement, which is a real weakness — but it must be **stated and justified**, not left implicit. The single sentence to write: *the IG field standard is percent agreement at ≥80% (Brady et al. 2018; Basurto et al. 2010; Siddiki et al. 2011); this study reports a chance-corrected statistic instead because percent agreement is inflated under the skewed component distributions characteristic of ADICO coding.*

## ⚠ Correction 3 — kappa is the wrong chance-corrected statistic for this data

Cohen's κ is **unstable under prevalence imbalance** — skewed category distributions depress κ even at high agreement (the kappa paradox). ADICO coding is exactly that: **Or-else components are rare** relative to Attributes and Aims. PRIS's own P2 finding — "of 11 Rules, 0 govern citizen-facing fallback procedures" — is an extreme-skew result. κ will behave badly on this corpus and may report poor reliability where coding is in fact consistent.

**Gwet's AC1** is the standard remedy, being robust to prevalence imbalance. **Precedent: Schlager et al. (2021) — the first published IG-QCA study — cited a Cohen's κ vs Gwet's AC1 comparison in its own reliability reporting.** The field's leading combined IG-QCA application engaged this exact question. Following it is a defensible, precedented choice rather than an idiosyncratic one.

**Recommendation:** report **percent agreement (field comparability) + Gwet's AC1 (chance correction robust to skew)**, and report κ alongside only if the distribution is not badly skewed. State the reasoning. This is stronger than any single statistic and pre-empts the obvious methods challenge.

## Thresholds Reference

| Statistic | Threshold | Source |
|---|---|---|
| **IG percent agreement** | **≥80%** acceptable; ≤85% triggers codebook revision and re-test | Brady et al. 2018; Basurto et al. 2010; Siddiki et al. 2011 |
| Cohen's κ | 0.00–0.20 none/slight · 0.21–0.40 fair · 0.41–0.60 moderate · **0.61–0.80 substantial** · 0.81–1.00 almost perfect | McHugh 2012; Landis & Koch 1977. κ = [Pr(a) − Pr(e)] / [1 − Pr(e)] |
| Krippendorff's α | **≥0.80** reliable · 0.67–0.79 tentative · <0.67 unreliable | Krippendorff (k-alpha.org) |
| IG-adjacent machine coding | 70–90% is the "acceptable" band; Rice et al. achieved 70% | Rice et al. 2021, *Public Administration*; Quinn et al. 2010 |

## Procedure

1. Code the full corpus against the IG 2.0 codebook (Frantz & Siddiki v1.4; IG Core / Extended / Logico levels)
2. Draw a **20% random subsample** for double-coding by a second coder — matches both the IG standard and PRIS's locked design
3. Compute **percent agreement** and **Gwet's AC1**; report κ where distribution permits
4. Where the threshold is not met: identify discrepant codes → gather coder explanations → generate a revised coding solution → **revise the codebook and re-test iteratively** (Halpin's remediation protocol; Siddiki's iterative requirement)
5. Report the procedure in enough detail to replicate — Siddiki (2009/2011) is the template: multi-coder requirement as an explicit numbered step in the protocol, not an afterthought

## Literature Anchors

- **Brady, U. et al.** (2018). *IG 1.0 Codebook*, institutionalgrammar.org — **the authoritative IG-specific reliability standard**
- **Frantz, C.K. & Siddiki, S.** *IG 2.0 Codebook* v1.4, newinstitutionalgrammar.org — coding procedure; not a reliability-statistics guide, pair with Brady
- **Siddiki, S.** (2009; 2011). *Dissecting Policy Designs* / *An Application of the Institutional Grammar Tool* — the 8-step protocol with reliability as step 7; the replicable reporting template
- **Siddiki, S. & Frantz, C.K.** (2022). *Institutional Grammar: Foundations and Applications.* Palgrave Macmillan — fullest book-length treatment; ⚠ methods chapter not retrieved, recommend direct acquisition
- **Halpin, S.N.** (2024). *Inter-Coder Agreement in Qualitative Coding.* AJQR — ICA/IRR distinction; remediation protocol
- **McHugh, M.L.** (2012). *Interrater Reliability: The Kappa Statistic.* Biochemia Medica
- Krippendorff, K. — methodological notes, k-alpha.org
- **Rice, D. et al.** (2021). *Machine Coding of Policy Texts with the Institutional Grammar.* Public Administration — relevant if any machine-assisted validation is used

## Linked Methods

[[Institutional_Grammar_IG2]] — the coding scheme this protocol governs

[[fsQCA]] — coded output feeds calibration

[[Comparative_Regulatory_Analysis]]

## Linked Projects

[[P2_DPI_JSIS]] · [[P3_BFSI_JEIM]] · [[fsQCA_Thesis_Chapter]]

---

_Back to [[_Methods_MOC]]_
