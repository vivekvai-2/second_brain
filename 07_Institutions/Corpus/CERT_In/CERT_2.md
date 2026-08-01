---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/cert-in
---

# CERT_2 — CERT-In Advisory CIAD-2025-0013: Best Practices Against Vulnerabilities While Using Generative AI Solutions

**Type:** Corpus Node  
**Vault path:** `07_Institutions/Corpus/CERT_In/CERT_2.md`  
**Institution:** [[07_Institutions/CERT_IN]]  
**Issuing body:** Indian Computer Emergency Response Team (CERT-In), MeitY  
**Document date:** March 26, 2025  
**Pages:** 2  
**Domain:** [[03_Domains/AI_Governance]]  

---

## Instrument Identity

**Full title:** CERT-In Advisory CIAD-2025-0013: Best Practices against vulnerabilities while using Generative AI solutions  
**Type:** Advisory Note  
**Target scope:** General — organisations and individuals using generative AI tools  
**Companion to:** [[07_Institutions/Corpus/CERT_In/CERT_1]] (CIAD-2023-0015 is cited as a reference)

---

## Analytical Classification

**P3 corpus role:** Screening corpus — CERT-In null finding for AI-relevant RUs in P3 context (advisory, not binding mandate on financial regulated entities). Confirmed in SOM.  
**AI Governance Wiki relevance:** HIGH — 2025 advisory on GenAI vulnerabilities provides current Indian regulatory stance on AI security risks; extends CIAD-2023-0015.  
**Tier classification:** Tier C (AI-adjacent governance — advisory, no binding mandate)

---

## Substantive Content

### AI Vulnerability Taxonomy (GenAI-Specific — 2025)

**Data Poisoning:** Manipulation of AI model training data to induce incorrect patterns, misclassification, biased or malicious outputs. Attack vectors: inserting deceptive data, modifying existing data, using compromised training sources.

**Adversarial Attacks:** Input perturbations that change AI model predictions while appearing unchanged to human observers.

**Model Inversion:** Extraction of sensitive training data by analysing model outputs — allows deduction of individual training samples and identification of data patterns.

**Model Stealing:** Replication of a machine learning model by repeatedly querying it and using outputs to construct a substitute model (avoids training costs; IP theft).

**Prompt Injection:** Input manipulation attack introducing malicious instructions into AI systems — enables hijacking of model output and bypassing of content filters/safeguards.

**Hallucination Exploitation:** Exploitation of AI tendency to generate inaccurate/fabricated outputs to propagate false information, conduct phishing, execute fraudulent transactions, or compromise security.

**Backdoor Attacks:** Hidden triggers implanted during AI model training — triggered by specific inputs to induce malicious or incorrect behaviour.

### Best Practices Framework (Seven Categories)

1. **Choose AI Apps Carefully** — Use only organisationally-approved and verified AI tools; avoid fake AI applications (malware vector)
2. **Avoid Sharing Personal & Sensitive Information** — No sensitive data to public GenAI services (client cannot control GenAI provider's data handling)
3. **Carefully Configure AI Tools' Access Rights** — Review default permissions when first activated; periodic review of access rights to emails, documents, source code repositories, AV conferencing
4. **Don't Rely on AI for Accuracy** — Fact-check AI outputs; verify against reliable sources; do not use for critical business decisions without validation
5. **Use the System for Its Intended Purpose** — AI tools not for critical decisions in legal or medical contexts; scope limitation
6. **Use a Strong Password/Secure Access** — MFA; avoid credential sharing; review access permissions regularly
7. **Use an Anonymous Account** — Where possible, anonymise input; do not link AI accounts to personal/professional identity for sensitive work
8. **Don't Use Plagiarised Content** — Verify AI-generated content for plagiarism
9. **Stay Alert for Suspicious Activity** — Monitor for deepfakes, phishing emails, malicious code generated via AI

---

## Analytical Significance for PRIS Research

### Evolution of CERT-In AI Advisory Framework
- CIAD-2025-0013 extends CIAD-2023-0015 to GenAI-specific vulnerabilities (2025 = post-widespread GenAI deployment)
- New taxonomy (2025 vs 2023): Adds model inversion, model stealing, prompt injection, hallucination exploitation, backdoor attacks — reflects maturation of AI threat landscape
- Still advisory-only in March 2025, despite CERT-In's binding incident reporting powers under IT Act 2000
- Gap: CERT-In has not issued a binding mandate on GenAI security for regulated entities — advisory-only status contrasts with SEBI's binding AI reporting mandates (2019)

### Regulatory Parallelism Evidence
- CERT-In (March 2025) addresses GenAI security without referencing SEBI's 2019 AI reporting regime or RBI's 2023 IT governance directions
- Access rights configuration requirement (Best Practice 3) overlaps with RBI third-party IT outsourcing due diligence requirements — no cross-reference
- Pattern: Parallel governance of GenAI risks across CERT-In, SEBI, and RBI silos without coordination mechanism

### Governance Debt Indicator
- Adversarial AI threat taxonomy (data poisoning, prompt injection, backdoor attacks) documented in 2025 advisory but no corresponding mandatory control requirements issued for financial sector
- Contrast with CERT_4 AIBOM (July 2025) which introduces binding AIBOM mandate for government procurement — evolution from advisory to mandate within same regulator

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/CERT_In/CERT_1]] | [[07_Institutions/Corpus/CERT_In/CERT_4]] | [[07_Institutions/Corpus/SEBI/SEBI_9]] | [[07_Institutions/Corpus/RBI/RBI_1]]  
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]]  
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] | [[02_Projects/P4_Doctrinal_IJLIT]]  
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]  
**Zotero key:** CERT-In_CIAD-2025-0013

---

## Coding Status

- **P3 NVivo coding:** Not in canonical corpus — CERT-In null finding
- **AI Governance Wiki:** Flag for adversarial AI section and Indian regulatory chronology
- **Future coding:** If CERT-In issues binding GenAI mandates, this advisory becomes the interpretive baseline

---

## Log

- 2026-06-13: Corpus node created from source extraction. S5 session.
