---
type: Corpus Node
status: active
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/uidai
---

# UIDAI_1 — Circular No. 8 of 2025: Aadhaar Data Vaults, HSMs, and Authentication Application Security

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/UIDAI/UIDAI_1_Circular_8_2025_Data_Vaults_HSM.md`
**Institution:** [[07_Institutions/UIDAI]]
**Issuing body:** Unique Identification Authority of India (UIDAI)
**Document date:** 2025 (secondary source dates coverage 22 September 2025; exact circular date **not independently confirmed against uidai.gov.in** — flag below)
**Pages:** Not determinable from this extraction
**Domain:** [[03_Domains/Privacy_DataProtection]] | [[03_Domains/DPI_Governance]]

---

## Instrument Identity

**Full title:** UIDAI Circular No. 8 of 2025 (exact full title not independently confirmed — reconstructed from secondary summary)
**Type:** UIDAI Circular (security/compliance directive)
**Target entities:** Authentication User Agencies (AUAs), KUAs, and other entities operating Aadhaar authentication applications
**Legal basis:** UIDAI's regulatory authority under the Aadhaar Act, 2016
**Companion documents:** UIDAI circulars index (https://uidai.gov.in/en/about-uidai/legal-framework/circulars.html) — lists circulars through June 2026; no circular in the visible listing is explicitly titled around "AI" or "automated decision-making," making this the closest available match for Aadhaar-authentication automated-system accountability

**Primary source link (unconfirmed — flag):** Secondary summary at https://jisasoftech.com/uidai-2025-guidelines-ensuring-aadhaar-data-compliance/; primary circulars index at https://uidai.gov.in/en/about-uidai/legal-framework/circulars.html

**⚠ Sourcing caveat — this node is intaken from a secondary summary, not the primary UIDAI PDF.** The exact circular number, date, and full text should be independently verified directly against the UIDAI circulars index before this node is used in any publication-facing analysis. Treat as provisional pending verification.

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S5 (Data, Privacy & Security)
**Jurisdiction:** India
**Confidence:** Low-Medium — secondary-sourced only; primary text not independently retrieved
**AI explicit:** Partial — framed as a security/data-protection circular (encryption, HSMs, audit trails for authentication applications) rather than an explicit "AI governance" instrument, but authentication applications increasingly rely on AI/ML-based matching (see UIDAI's own confirmed statement on AI/ML-based Face Authentication, below)
**Tier classification:** Tier C — AI-adjacent; security controls for systems that increasingly incorporate AI/ML authentication methods
**AI Governance Wiki relevance:** LOW-MEDIUM — closest available UIDAI-sourced anchor for automated-authentication accountability, but does not itself regulate AI/ML use

---

## Substantive Content

### Reported requirements (per secondary summary — unverified against primary text)
Mandates AES-256 encryption, high-availability Hardware Security Modules (HSMs), and audit trails for Aadhaar authentication applications.

### UIDAI's own confirmed AI/ML statement (higher-confidence companion fact)
UIDAI's official social-media channel (not a formal circular) states that UIDAI's **AI/ML-based Face Authentication solutions were developed in-house**, referencing 231 crore authentication transactions as of November 2025. This is the clearest UIDAI-sourced confirmation that AI/ML methods are now embedded in Aadhaar's core authentication infrastructure — but it is a social-media post, not a citable regulatory document, and should not be treated as equivalent to a circular.

### Confirmed gap
No UIDAI circular explicitly titled or scoped around "AI" or "automated decision-making" was located in the visible circulars index (through June 2026). Aadhaar's AI/ML authentication capability is confirmed to exist (per UIDAI's own social-media statement) but is **not yet governed by a dedicated UIDAI AI-governance circular** — a documented regulatory lag between AI/ML deployment and AI-specific UIDAI rulemaking, distinct from (but structurally similar to) the DPDP/SDF algorithmic-due-diligence pattern already documented in [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]].

---

## Analytical Significance for PRIS Research

### For P2 (DPI Governance) and Records_Rules_Asymmetry
If confirmed, this circular's security-only framing (HSMs, encryption, audit trails) without AI-specific accountability language is consistent with the domain's existing "records vs rules asymmetry" and "infrastructure governance vs service governance" findings — Aadhaar governance instruments remain system/infrastructure-facing even as the underlying authentication technology becomes AI/ML-based.

### Regulatory Parallelism
UIDAI's silence on AI-specific authentication governance, set against DPDP's SDF algorithmic-due-diligence clause and SEBI/RBI's AI/ML reporting obligations, extends the existing cross-regulator parallelism finding: **each institution touching AI is either building its own narrow algorithmic-accountability hook (SEBI, RBI, MeitY/DPDP) or has not yet built one at all (UIDAI)** — a spectrum, not a uniform pattern.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (SDF algorithmic due-diligence comparator), [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Records_Rules_Asymmetry]], [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]
**Related frameworks:** None directly — UIDAI has no dedicated 06_Frameworks node in this vault
**Related projects:** [[02_Projects/P2_DPI_JSIS]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** Not applicable (not a BFSI instrument)
- **Wiki intake status:** Pending — Normal priority; upgrade to High once primary text verified

---

## Log

- 2026-08-02: Corpus node created. Sourced via Perplexity Deep Research per [[Thin_Node_Perplexity_Prompts_2026-08-02]] Privacy_DataProtection prompt. First node in a new UIDAI institution folder. Flagged for primary-source verification before publication use.
