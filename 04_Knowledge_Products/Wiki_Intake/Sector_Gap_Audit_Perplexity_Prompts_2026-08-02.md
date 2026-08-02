---
type: Process Document
status: active
last_updated: 2026-08-02
tags:
  - type/process-document
  - status/active
  - engine/phd
---

# Sector Gap Audit — Healthcare, Judiciary, Insurance, Telecom, Power Grid/Critical Infrastructure Cyber-AI Assurance (2026-08-02)

**Method:** Checked whether each sector has a Domain-level node, how many corpus-node anchors it has, and whether the relevant sectoral institution note itself already flags the gap. Your instinct was right on all five, but the *kind* of thin varies a lot — two of these already have live, self-diagnosed intake queues from earlier today; three have no dedicated treatment at all.

**Parent:** [[Thin_Node_Perplexity_Prompts_2026-08-02]] (the first sourcing pass — DPDP/OECD/UNESCO/NIST/Privacy/DPI/BFSI/Legitimacy/Deontic_Bifurcation)

---

## 1. Diagnosis — five sectors, three different problems

| Sector | Domain node? | Corpus anchors | Actual problem |
|---|---|---|---|
| **Healthcare** | Yes — `status/stub`, 489 words, 1 evidence link | 1 (ICMR) | **Already diagnosed and queued.** Stub written 2026-07-31 with a 6-document candidate table (ICMR Ethical Guidelines, CDSCO Medical Device Software Guidance final + draft, WHO x2, FDA SaMD Action Plan) — titles/dates/links confirmed, nothing read/coded yet. |
| **Judiciary** | Yes — `status/seeded` (promoted from stub today, 2026-08-02), ~1,500 words | 2 (SCI White Paper, DHC ANI v. OpenAI) | **Already diagnosed and queued, more urgently.** Has a priority-1 *blocking* gap: no Bharatiya Sakshya Adhiniyam (BSA) 2023 corpus node exists — the evidence-admissibility statute the whole domain's "evidentiary forum" argument depends on. Five more candidates queued (UK judicial AI guidance, CEPEJ Charter, three eCourts phase documents). |
| **Insurance** | **No domain node at all.** IRDAI exists only as an institution note | 3 (IRDAI_1/2/3) | IRDAI's own institution note self-describes as "a fourth silo," "Regulatory Parallelism through omission," and insurance as "the sector with the weakest sectoral AI-governance overlay." Currently folded into BFSI_Governance as an afterthought, not treated as its own domain. |
| **Telecom** | **No domain node at all.** TRAI exists only as an institution note | 2 (TRAI_1/2) | TRAI's own institution note literally calls itself "a forward intelligence note — research relevance is anticipatory, not current." Two AI-relevant corpus nodes exist (UCC/spam AI direction) but nothing pulls them into a synthesised domain. |
| **Power grid / critical infrastructure cyber-AI assurance** | **Zero presence anywhere in the vault** — not a stub, not a mention, not an institution note | 0 | Confirmed by direct search: no CEA (Central Electricity Authority), no Ministry of Power, no NCIIPC (National Critical Information Infrastructure Protection Centre), no POSOCO/Grid-India, no SCADA/OT-security content anywhere. `Cybersecurity_Governance.md` is entirely BFSI-scoped (CERT-In + RBI + SEBI + DPDP) and never once mentions critical infrastructure outside finance. This is the only true **blank spot** of the five — everything else is thin; this is absent. |

---

## 2. What to do differently for each

Healthcare and Judiciary don't need *discovery* prompts — the documents are already named, dated, and linked. What they need is either (a) direct retrieval/reading via the standard [[PRIS_Corpus_Intake_Prompts]] pipeline, or (b) a short verification pass to confirm links still resolve and nothing newer has superseded them. I've written (b) below since it's cheap and catches drift.

Insurance, Telecom, and Power Grid genuinely need fresh discovery — full sourcing prompts below.

---

## 3. Verification Prompts (Healthcare, Judiciary — discovery already done)

### PROMPT — Healthcare_Governance candidate-source refresh

```
I have a confirmed list of six candidate primary sources for an Indian healthcare-AI-governance research node, sourced 2026-07-31. Before I read and code them, please verify each is still current and provide a working direct link:

1. ICMR "Ethical Guidelines for Application of Artificial Intelligence in Biomedical Research and Healthcare" (March 2023, ISBN 978-93-5811-343-3)
2. CDSCO "Guidance Document on Medical Device Software" (Final, 21 July 2026, Doc No. CDSCO/MD/GD/MDSW/01/2026)
3. CDSCO Draft Guidance Document on Medical Device Software (21 October 2025 — superseded by #2, confirm this)
4. WHO "Ethics and Governance of Artificial Intelligence for Health" (28 June 2021, ISBN 978-92-4-002920-0)
5. WHO "Ethics and Governance of AI for Health: Guidance on Large Multi-Modal Models" (2024)
6. US FDA "AI/ML-Based Software as a Medical Device (SaMD) Action Plan" (12 January 2021, updated December 2024)

For each: confirm the link resolves, confirm the document has not been further superseded since the date above, and flag if any part of the ABDM/NDHM ecosystem has since published an AI-specific data-governance instrument (as of 2026-07-31 no such document existed — check if that has changed). Do not summarize content — I will read these myself.
```

### PROMPT — Judicial_Governance: BSA text + candidate-link verification (priority: blocking)

```
I need the primary legal text and a working direct link for the Bharatiya Sakshya Adhiniyam, 2023 — specifically Section 63 and its accompanying Schedule (electronic-record admissibility and certification requirements). This is blocking a research analysis of whether Indian regulatory logging/audit-trail obligations (RBI, SEBI, CERT-In, MeitY) satisfy the certification standard this section sets for admitting AI-system-generated records as evidence.

Also verify working direct links for these five already-identified sources:
1. "Artificial Intelligence (AI) Guidance for Judicial Office Holders" — Courts and Tribunals Judiciary, UK (31 October 2025 edition, supersedes April 2025 and December 2023 editions)
2. "European Ethical Charter on the Use of AI in Judicial Systems" — CEPEJ, Council of Europe (3–4 December 2018)
3. "Vision Document for Phase III of the eCourts Project" — e-Committee, Supreme Court of India (26 November 2022)
4. "Policy and Action Plan Document, Phase II" (eCourts) — e-Committee, Supreme Court of India (8 January 2014)
5. "Policy and Action Plan Document, Phase I" (eCourts) — e-Committee, Supreme Court of India (1 August 2005)

Additionally: has any Division Bench appeal been filed or decided in ANI Media Pvt Ltd v. OpenAI (Delhi High Court, interim order 24 July 2026)? That order is currently being treated as unsettled/interlocutory — flag any appellate development. Do not summarize the BSA's substantive content beyond confirming s.63's scope — I will read the primary text myself.
```

---

## 4. Discovery Prompts (Insurance, Telecom, Power Grid — genuine new sourcing)

### PROMPT — Insurance sector AI governance (India + comparative)

```
I am building a new research domain on AI governance in India's insurance sector — currently the weakest-covered financial sub-sector in my corpus (IRDAI has no AI-specific regulatory instrument as of mid-2026, only a general data-governance regulation). I need primary sources, not commentary.

Find and list, with exact title, issuing body, date, and direct link:
1. Any IRDAI circular, guideline, or regulation issued after mid-2026 that explicitly addresses AI, ML, or algorithmic underwriting/claims/fraud-detection systems (check specifically whether the IRDAI AI Working Group, constituted to study this, has published any output or draft guidelines yet)
2. IRDAI's Insurtech Regulatory Sandbox (operational since 2019) — any published outcomes, approved cohort details, or lessons-learned reports specifically involving AI-based products
3. Comparative insurance-AI regulatory material: US NAIC (National Association of Insurance Commissioners) Model Bulletin on the Use of AI Systems by Insurers (2023) and any state-level implementing adoptions; EIOPA (EU) AI governance guidance for the insurance sector; UK PRA/FCA insurance-specific AI supervisory statements (distinct from general FCA/PRA banking AI guidance)
4. IAIS (International Association of Insurance Supervisors) any published AI governance application papers or holistic framework updates
5. Academic or think-tank literature (2023 onward) specifically on algorithmic underwriting fairness, claims-denial automation, or insurance fraud-detection AI governance, with India as a case if available, otherwise global

For each item confirm exact date, issuing body, and working link. Flag anything still in draft/consultation vs. finalized. Do not summarize — I will read and code these myself.
```

### PROMPT — Telecom sector AI governance (India + comparative)

```
I am building a new research domain on AI governance in India's telecommunications sector — currently only two AI-relevant corpus nodes exist (a TRAI direction on AI/ML for UCC spam detection and inter-operator intelligence sharing, February 2026, and one other TRAI node), with no synthesised sectoral treatment.

Find and list, with exact title, issuing body, date, and direct link:
1. Any TRAI recommendation, direction, or consultation paper (beyond the UCC/spam AI direction already known) addressing AI in network management, automated customer service/chatbots, telecom data analytics, or algorithmic spectrum/traffic management
2. Department of Telecommunications (DoT) rules or notifications issued under the Telecommunications Act 2023 that reference AI, automated decision-making, or algorithmic systems
3. Any TRAI consultation paper specifically on AI governance in telecom, even in draft/consultation stage
4. Comparative telecom-AI regulatory material: Ofcom (UK) guidance on AI use by telecom operators; FCC (US) any AI-specific telecom rulemaking (robocall/AI-voice detection rules are a likely candidate — check for a confirmed primary FCC order); EU's approach to AI within the European Electronic Communications Code framework
5. ITU (International Telecommunication Union) or GSMA published AI governance frameworks specifically for telecom operators/networks (not general AI ethics documents — telecom-specific)
6. Any Indian telecom-sector data-localisation or AI-specific data governance requirement that interacts with DPDP obligations for telecom companies as Significant Data Fiduciaries

For each item confirm exact date, issuing body, and working link. Flag draft vs. final status. Do not summarize — I will read and code these myself.
```

### PROMPT — Power grid / critical infrastructure cyber-AI assurance (India + comparative) — highest priority, true blank spot

```
I am building an entirely new research domain on cybersecurity and AI-assurance governance for power grids and critical infrastructure in India. This currently has zero coverage in my corpus — my existing Cybersecurity_Governance domain is scoped only to BFSI (CERT-In + RBI + SEBI + DPDP) and has never addressed energy/grid infrastructure. I need primary regulatory and institutional sources.

Find and list, with exact title, issuing body, date, and direct link:
1. Any Central Electricity Authority (CEA) regulation, guideline, or notification on cybersecurity for the power sector — specifically the "Cyber Security in Power Sector" guidelines (originally 2021) and any updates or amendments since
2. Ministry of Power notifications or advisories on grid cybersecurity, AI-based grid management, or smart-grid automated decision systems
3. National Critical Information Infrastructure Protection Centre (NCIIPC) — any published sector-specific guidelines for power/energy as a designated Critical Information Infrastructure sector, and whether NCIIPC has issued anything addressing AI-specific risks (as opposed to general OT/ICS cybersecurity)
4. POSOCO / Grid Controller of India (Grid-India) — any published cybersecurity or automated grid-management governance documents
5. CERT-In sector-specific advisories for power/energy (as distinct from the general CERT-In 2022 Directions already coded in my corpus) — check for a dedicated power-sector CERT (if one exists, e.g. a Power Sector CERT or "CSIRT-Power")
6. Comparative material: NERC CIP (Critical Infrastructure Protection) standards (US) — confirm current version and any AI/ML-specific updates; ENISA (EU) guidance on AI in energy-sector critical infrastructure; IEC 62443 (industrial automation/control systems security) — confirm whether any AI-specific extension or supplementary guidance exists
7. Any documented incident, advisory, or academic case study on AI/ML use in Indian grid load-forecasting, demand-response, or fault-detection systems and the governance (or absence of governance) surrounding them

For each item confirm exact date, issuing body, and working link. This sector may have very little AI-specific material yet — if so, explicitly confirm the absence rather than reaching for tangential documents, and note whether general OT/SCADA cybersecurity governance (non-AI-specific) is the closest available primary-source anchor. Do not summarize — I will read and code these myself.
```

---

## 5. Recommended sequence

1. **Power grid / critical infrastructure** first — it's the only true blank spot, and even a thin first node here is more valuable than incremental depth elsewhere.
2. **Insurance** second — IRDAI's own institution note already argues this is the weakest-governed high-AI-adoption financial sub-sector; closing it strengthens the existing BFSI/Regulatory_Parallelism argument directly.
3. **Telecom** third — lower urgency; TRAI's own note calls itself "anticipatory," so there may genuinely be little to find yet.
4. **Judiciary BSA verification** — cheap, and it's explicitly blocking further work on that domain per its own log.
5. **Healthcare verification** — cheap, lowest urgency since the candidate list is only a week old.

Paste each response back with the vault MCP active and I'll create the Domain node (Insurance, Telecom, Power Grid — none currently exist) or Corpus nodes (Healthcare, Judiciary — domains exist, need document intake) following the same pattern as the first sourcing pass.

---

## Log

- 2026-08-02: Telecom prompt run and intaken — new domain [[03_Domains/Telecom_AI_Governance]] built. Discovered TRAI is the most analytically developed of the three thin sectors: TRAI_2 (existing node, July 2023 cross-sector Recommendations) had two open VERIFY flags, both addressed — V-TRAI4 (primary link) fully resolved, V-TRAI6 (did DoT act on the recommendation) partially resolved via confirmed absence of AI references in DoT's own June 2026 Telecommunications Act rule-making. New international comparator nodes: [[07_Institutions/Corpus/International/International_30_Ofcom_Strategic_Approach_AI_Telecom]] (UK, monitoring-only), [[07_Institutions/Corpus/International/International_31_FCC_AI_Robocall_Voices_Ruling_2024]] (US, narrow but genuinely binding), [[07_Institutions/Corpus/International/International_32_GSMA_Responsible_AI_Roadmap_Telecom_2024]] (industry self-governance, consolidates GSMA/ETSI/3GPP/ITU findings). **Central finding: neither pure silence (Power Grid) nor study-in-progress (Insurance) — telecom is a case of institutional vision (TRAI's 2023 cross-sector ambition) exceeding institutional reach** (only a narrower binding instrument, TRAI_1, was ever built). Cross-linked from TRAI institution note and DPI_Governance.
- **All five sector-gap prompts now run and intaken (Power Grid, Insurance, Telecom — new domains built; Healthcare and Judiciary verification prompts remain queued but are low-cost/low-urgency since both already have fresh, self-diagnosed intake queues).**
- 2026-08-02: Insurance prompt run and intaken — new domain [[03_Domains/Insurance_AI_Governance]] built. Resolved two pending VERIFY flags on the existing [[07_Institutions/Corpus/IRDAI/IRDAI_2_Working_Group_AI_Governance_2026]] node (order reference IRDAI/GA&HR/ORD/MISC/90/06/2026 confirmed; date corrected to 17 June 2026). New corpus nodes: [[07_Institutions/Corpus/IRDAI/IRDAI_4_Regulatory_Sandbox_Regulations_2025]], and three international comparators — [[07_Institutions/Corpus/International/International_27_NAIC_Model_Bulletin_AI_Insurers_2023]] (US, decentralised state-adoption), [[07_Institutions/Corpus/International/International_28_EIOPA_Opinion_AI_Governance_Insurance_2025]] (EU, interpretive layering on the binding AI Act), [[07_Institutions/Corpus/International/International_29_IAIS_Application_Paper_AI_Supervision_2025]] (Global, "existing ICPs suffice, no new standards"). **Unlike Power Grid, this is a genuine "India lags its peers" case** — three live substantive international comparators exist against which IRDAI's WG-AI recommendations (due ~18 Sep 2026) can be benchmarked once published. Confirmed gap: no India-specific academic literature on algorithmic underwriting/claims/fraud-AI governance exists. Cross-linked from IRDAI institution note and BFSI_Governance.
- 2026-08-02: Power Grid/Critical Infrastructure prompt run and intaken — this is a brand-new Domain (no prior node existed at all). Created: institutions [[07_Institutions/CEA]] and [[07_Institutions/NCIIPC]]; corpus nodes [[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]] (sole binding Indian anchor), [[07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025]] (draft, folds in CSIRT-Power), [[07_Institutions/Corpus/NCIIPC/NCIIPC_1_Guidelines_Protection_NCII_V2_2015]], and [[07_Institutions/Corpus/International/International_26_NERC_CIP_ENISA_IEC62443_AI_Gap_2026]] (consolidates NERC/ENISA/IEC 62443 — all three confirm the identical AI-specific gap). New domain note at [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]]. **Central finding: this is the only domain in the vault where India tracks global peers rather than lagging — a genuine, unsolved regulatory frontier, not a capacity gap.** Second confirmed instance of the "institution before regulation" sequencing pattern (CSIRT-Power operational since Sept 2024, formalising regulation still draft). Explicit methodological caution logged against folding this sector into the existing fsQCA model (near-zero cross-case variance on any AI-specific-regulation condition). Cross-linked from Cybersecurity_Governance (scope note distinguishing BFSI-parallelism from critical-infrastructure-silence) and CERT_IN (CSIRT-Power coordination role).
- 2026-08-02: Sector gap audit run across Healthcare, Judiciary, Insurance, Telecom, and Power Grid/Critical Infrastructure. Confirmed: Healthcare and Judiciary already have live, self-diagnosed intake queues (written 2026-07-31 and 2026-08-02 respectively) — verification prompts only. Insurance and Telecom have institution notes but no Domain node — full discovery prompts written. Power Grid/Critical Infrastructure has zero presence anywhere in the vault — confirmed true blank spot, highest-priority discovery prompt.
- 2026-08-02: **Judiciary + Healthcare verification prompts run and intaken — closes out this entire five-sector audit.** Judiciary: created [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] (Bharatiya Sakshya Adhiniyam 2023, s.63 + Schedule — full text and both certificate-format parts coded), which **closes the priority-1 blocking gap** flagged in [[03_Domains/Judicial_Governance]]'s prior log entry; new institution note [[07_Institutions/Parliament]] and corpus node [[07_Institutions/Corpus/Parliament/Parliament_1_Standing_Committee_48th_Report_2023]] created in the same pass. [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]]'s open appeal flag (V-DHC1-1) resolved — no Division Bench appeal filed or decided as of verification (Cyril Amarchand Mangaldas 29 Jul 2026; SCC Online 26 Jul 2026). BSA_1's existence sharpens rather than resolves DHC_1's silence: s.63 was in force throughout the entire ANI v. OpenAI proceeding and was never invoked by any party. Judicial_Governance's candidate-source table updated with verified links; remaining 5 items (UK judicial AI guidance, CEPEJ Charter, three eCourts phase documents) marked link-verified but still unread/uncoded. Healthcare: all 6 candidate links in [[03_Domains/Healthcare_Governance]] re-verified live and current, with two discrepancies flagged rather than silently resolved (WHO 2021 ISBN conflict; FDA's "December 2024 update" reframed as a sequence of implementing guidances, not a revision to the 2021 Action Plan itself). Healthcare's "no ABDM/NDHM AI instrument exists" gap is now closed: [[04_Knowledge_Products/Wiki_Intake/MoHFW_1_SAHI_Healthcare_AI_Strategy_2026]] updated with BODH benchmarking platform, ABDM architectural linkage (860M+ IDs), pending DPDP Phase II Consent Manager rollout, and cross-tagged into Healthcare_Governance, Privacy_DataProtection, and DPI_Governance — with two new discrepancies flagged there too (launch date, pillar count) rather than resolved. **This closes all five sectors opened by this audit** (Power Grid, Insurance, Telecom fully built as new domains; Judiciary's blocking gap cleared; Healthcare's candidate queue link-verified).
