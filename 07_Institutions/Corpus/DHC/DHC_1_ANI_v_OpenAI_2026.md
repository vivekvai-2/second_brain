---
type: corpus-node
node-id: DHC_1
institution: DHC
date: 2026-07-24
wiki-section: S2
tier: A
ai-explicit: true
status: active
instrument-class: judicial
binding-status: interim-prima-facie
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - institution/DHC
  - wiki-section/S2
  - tier/A
  - instrument-class/judicial
  - batch/ad-hoc-20260802
  - concept/Evidentiary_Governance
  - concept/Regulatory_Parallelism
  - concept/Institutional_Coherence
  - concept/Accountability
  - concept/Transparency
  - concept/Legitimacy
  - project/P4
  - project/P1
  - project/P5
  - jurisdiction/india
---

# DHC_1 — ANI Media Pvt. Ltd. v. OpenAI OpCo LLC, CS(COMM) 1028/2024

**Node ID:** DHC_1
**Institution:** High Court of Delhi ([[07_Institutions/DHC]])
**Document type:** Judgment on interlocutory application (Order XXXIX Rules 1 and 2 CPC)
**Coram:** Hon'ble Mr Justice Amit Bansal
**Reserved:** 27 March 2026 · **Pronounced:** **24 July 2026**
**Jurisdiction:** India — Delhi High Court, original commercial jurisdiction
**Wiki Section:** S2 — India Regulatory
**Tier:** A — full judgment text supplied and read
**Length:** 135 pages, 275 paragraphs

> ## ⚠ STATUS CAVEAT — READ BEFORE CITING
>
> This is an **interim order on an application for temporary injunction**, not a final determination. Every holding is expressly **prima facie**. Para 274: *"Needless to say, any observations made herein are only for the purpose of adjudication of the aforesaid application and would have no bearing on the final outcome of the suit."*
>
> - I.A. 45300/2024 was **dismissed**; the suit CS(COMM) 1028/2024 **continues**.
> - The order is **appealable** to a Division Bench. ✅ Confirmed 2026-08-02: no appeal filed or decided as of verification date (was V-DHC1-1).
> - The **RAG question was left expressly undecided** — not pleaded in the plaint (paras 84, 65.5).
> - The s.52 holding rests on OpenAI's **admitted temporary storage**, the Court having found "no factual foundation in the plaint to reach a finding of infringement in respect of the training claim" (para 202).
>
> **Do not cite as settled Indian law on AI training and copyright.**

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Cause title | ANI Media Pvt. Ltd. v. OpenAI OpCo LLC |
| Case number | CS(COMM) 1028/2024; I.A. 45300/2024, I.A. 45301/2024, I.A. 26192/2025 |
| Court | High Court of Delhi at New Delhi |
| Judge | Amit Bansal J. |
| Issues framed | 19 November 2024 (four issues) |
| Hearing dates | 21 hearings, 21 Feb 2025 – 27 Mar 2026 |
| Amici Curiae | Mr Adarsh Ramanujan; Professor Arul George Scaria |
| Intervenors (pro-ANI) | Federation of Indian Publishers (I.A. 470/2025); Digital News Publishers Association (I.A. 2199/2025); Indian Music Industry (I.A. 4027/2025) |
| Intervenors (pro-OpenAI) | Flux Labs AI (I.A. 4615/2025); IGAP Project LLP (I.A. 4616/2025); Broadband India Forum (I.A. 10766/2025) |
| Governing statute | Copyright Act, 1957 (ss. 2(ff), 2(m), 13, 14, 17, 51, 52, 62); Code of Civil Procedure, 1908 (s. 20) |
| Outcome | Application dismissed — no interim injunction |

---

## S2. Holdings by Issue

### Issue 4 — Territorial jurisdiction: **held for ANI**

Jurisdiction established under **s.62(2) Copyright Act** (ANI's registered and principal office within jurisdiction) and **s.20 CPC** (OpenAI targets Indian subscribers; alleged infringing responses generated within jurisdiction). ChatGPT's terms of use nominating San Francisco courts did not oust statutory remedies.

On extraterritoriality, the Court refused to sever training from output (para 51):

> "the storing of ANI's works on the US servers is a terminal step in the chain of events which begin from access of copyrighted works from India and transmission of the same abroad… the Copyright Act does not require this Court to sever the chain of events and examine only the last step. On a prima facie view, Open AI's argument is untenable as it would lead to evasion of Indian copyright law by infringers who shift the terminal link to servers abroad."

Following *Neetu Singh v. Telegram*, quoted at para 52: *"In the present age of cloud computing and diminishing national boundaries in data storage, conventional concepts of territoriality cannot be strictly applied."*

### Issue 2 — Output claim: **held for OpenAI**

Two sub-questions, both answered against ANI.

**(i) Memorisation and regurgitation — not established.** The dispositive finding is chronological. Training cut-offs were April 2022 (GPT-4) and April 2024 (GPT-4o); all illustrative articles pleaded were published August–September 2024. Para 83:

> "it is apparent that the illustrations of ChatGPT responses relied upon in the plaint could not have been produced on account of training of Open AI's LLMs on the ANI's literary works, as the literary works in question were published only after the completion of the training process."

The Court inferred the outputs were RAG-derived (para 84): *"the instances given in the plaint alleging infringement are not a result of memorisation, rather they are in the nature of live links, perhaps reflecting RAG technique."* RAG was unpleaded and therefore not adjudicated.

**(ii) Substantial reproduction — not established.** Applying *R.G. Anand* (works compared as a whole, not dissected) and *Leo Burnett*. On the Neeraj Chopra interview, the Court made a holding of independent significance (para 106): applying **s.17(cc)**, the person delivering a public address owns copyright in it, so *"Neeraj Chopra's mother would be first owner of the copyright in the said quotation"* and the translation right vested in her, not ANI. ANI produced no assignment.

The Court expressly distinguished **GEMA v. OpenAI** (Munich Regional Court, case 42 O 14139/24, 11 Nov 2025) on prompting method — see §S4 below.

### Issues 1 and 3 — Storage, training and fair dealing: **held for OpenAI**

**Storage is reproduction.** s.14(a)(i) covers "storing of it in any medium by electronic means"; the Court held the provision draws **no distinction between temporary and permanent storage**, and that purpose is irrelevant under s.51 (para 149).

**But s.52 is not an exception.** Para 167:

> "Section 52 independently defines the rights/privileges of a user in respect of copyrighted works and must not be interpreted in a restrictive manner. It is an integral part of the Copyright Act and therefore, it has to be given broad and liberal interpretation."

Following *CCH Canadian*: the fair dealing exception is *"a user's right… it must not be interpreted restrictively."*

Then a **two-step test**: Purpose Test, then Fairness Test. Both satisfied.

---

## S3. The Four Doctrinal Moves (P4's primary material)

**1. Commercial use is not excluded from s.52(1)(a)(i).** The Court reasoned from legislative drafting (paras 176–177): the legislature expressly confined ss. 52(1)(ad), (k)(ii), (l), (n) and (o) to non-commercial use, and *"the requirement of non-commercial use is conspicuously absent in Section 52(1)(a)."* Supported by *CCH Canadian*: *"research is not limited to non-commercial or private contexts."* *Jiwan Publishing House* and *TIPS v. Wynk* distinguished on the ground that in both the defendant supplied copyrighted material to third parties, whereas OpenAI's storage is internal (para 189).

**2. "Private" is not "personal".** Paras 207–209. Dictionary meanings show "private" extends to a group, class or company. If the two were synonyms *"the word 'private' would be rendered otiose."* Supported by *B. Malini Mallya*. Para 211: OpenAI stores works *"in a closed space without access to the public… accessible only to the LLM models themselves."*

**3. The Explanation's "non-infringing copy" limitation attaches only to computer programmes.** Paras 192–201, turning on comma placement in the Explanation to s.52(1)(a). The Court reinforced this with a reductio (para 197): otherwise a researcher photocopying a library page would be protected but the same researcher scanning it would not. Also noted (para 200) that ANI never alleged OpenAI breached a paywall or used unauthorised sources — distinguishing *Bartz v. Anthropic* on shadow libraries.

**4. "Research" extended to machine learning by updating construction.** The centre of gravity of the judgment. Applying *State (CBI) v. S.J. Choudhary* and Bennion's *Statutory Interpretation* ("an ongoing Act is regarded as 'a living Act'"), para 218:

> "With the advent of these technologies, research/ learning is no longer confined to humans. It is now being done through Artificial Intelligence. However, ultimately the research is at the behest of humans and for the benefit of humans… If tomorrow a human teacher is replaced by an AI bot or Robot to say that the said exception could only be used by a human would be a regressive view. Such an approach would limit societal progress. Therefore, the acts of further research cannot be confined to acts of human being alone and the same would extend to machine learning as well."

---

## S4. The Fairness Test — a bespoke Indian three-factor test

The Court surveyed Indian authority and found **no uniform test** (para 234), recording consensus among counsel that the **US four-factor test does not apply in India**. It then formulated its own (para 236):

| Factor | Finding |
|---|---|
| a. Whether OpenAI's use of ANI's works is limited to training its LLMs | Yes — no instance of any other use shown (para 243) |
| b. Whether the use produces economic competition, prejudice to ANI's legitimate interests, or actual or potential damage | No — functions "fundamentally different"; ChatGPT not a substitute for a news wire; *"Except for bare averments, nothing has been placed on record… to show that they have lost any market share"* (paras 246, 250) |
| c. Whether the functions performed serve the overall public interest | Yes — education, accessibility, research, translation, software development (paras 252–254) |

Anchored to **Berne Convention Article 9(2)** (paras 238–239) — reproduction permitted where it "does not conflict with a normal exploitation of the work and does not unreasonably prejudice the legitimate interests of the author."

**Foreign authority relied on:** *Bartz v. Anthropic* and *Kadrey v. Meta* (training as quintessentially transformative); *Authors Guild v. Google*. **Foreign authority distinguished:** *GEMA v. OpenAI*; *Associated Press v. Meltwater*; *Cohere*; *Infopaq*; *Newspaper Licensing Agency v. Meltwater*; *Positive Black Talk*.

---

## S5. Analytical Notes

### S5.1 — Evidentiary reconstruction of model behaviour, without artefacts (the corpus finding)

The output claim was decided entirely by **inference from metadata about the model**, not from evidence of what the model did. The Court had no training-data manifest, no inference logs, no retention record and nothing from OpenAI's systems. It reasoned from published training cut-off dates against article publication dates and concluded memorisation was impossible.

This is a direct and unusually clean illustration of [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]]. Where no evidentiary layer exists, a court will reconstruct system behaviour from whatever is available — and what was available here was a **vendor-published date**. The party bearing the burden could not test the assertion because the artefacts that would have tested it were never required to exist.

Note what the judgment does **not** contain: no reference to the Bharatiya Sakshya Adhiniyam, no s.63 certification analysis, no discussion of what evidence of AI system behaviour should look like, no direction on preservation. The evidentiary question was resolved without the evidentiary law being engaged at all. **OQ-EG-01 is not merely unanswered — the first Indian AI case reached final interlocutory disposal without anyone raising it.**

### S5.2 — Prompt design as an evidentiary standard

Para 104 introduces adversarial prompting as a legal test, with an academic citation:

> "in the second prompt, ANI used the word 'exactly', which clearly shows that ANI was seeking to elicit a response from ChatGPT in exact terms i.e. an **adversarial prompt** ('carefully designed inputs that manipulate model outputs')"

This became the basis for distinguishing *GEMA* (para 119): the Munich court found memorisation on **non-adversarial** prompts; ANI's prompts were adversarial and still failed to produce substantial reproduction.

**The consequence is that in Indian law the provenance and construction of a prompt is now a question of evidentiary weight.** A rights-holder who obtains a reproduction by adversarial prompting has weaker evidence than one who obtains it incidentally. This is a genuinely new dimension for the construct: the *method of interrogating* the system is itself governed, and no instrument in the corpus addresses how prompt-elicited evidence should be captured, logged or authenticated.

### S5.3 — Executive–judicial parallelism

[[07_Institutions/Corpus/DPIIT/DPIIT_1]] records the DPIIT working paper on a text-and-data-mining exception, with Nasscom formally dissenting in favour of the TDM model. That consultation concerns whether India should legislate a TDM exception. **While it ran, the Delhi High Court decided that the existing s.52(1)(a)(i) already covers LLM training.**

Neither track references the other. This extends [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] beyond its current scope in two ways: it is **inter-branch** rather than inter-regulator, and the outputs are potentially **substitutive** — a legislated TDM exception may now be partly redundant, or alternatively may be drafted to displace this reading. Every prior parallelism instance in the corpus involves regulators operating in ignorance of one another; this involves two branches producing answers to one question on different constitutional footings.

### S5.4 — Opt-out non-exercise weighed against the rights-holder

Paras 262–263: ANI had the ability to block crawlers and did not; OpenAI had blocked ANI's site voluntarily for both training and RAG. The Court also observed that ANI's subscribers could block their own sites and had presumably chosen not to "for their own commercial reasons."

**Crawler control has become a governance control with litigation consequences.** This is the judgment's most directly operational holding for consulting work, and it has no counterpart in any regulatory instrument in the corpus.

### S5.5 — Quantifiability defeated irreparable injury

ANI's own 3 October 2024 letter offering a licence at **USD 7.5 million** was held to establish that its claim was quantifiable and compensable in damages (para 265). A pre-litigation licence demand became the evidence that no injunction was needed.

---

## S6. Regulatory Units — codeable ratio

| RU | Proposition | Deontic | ADICO summary |
|---|---|---|---|
| RU1 | Electronic storage, temporary or permanent, is reproduction under s.14(a)(i) | SHALL (declaratory) | A=any person; D=prohibited absent licence; I=store work in any medium by electronic means; C=copyrighted literary work; O=s.51 infringement |
| RU2 | s.52 is a user-rights provision, liberally construed, not an exception to s.51 | Interpretive | — |
| RU3 | Commercial purpose does not defeat s.52(1)(a)(i) | MAY | A=user incl. body corporate; D=MAY; I=deal fairly for private use incl. research; C=commercial character immaterial |
| RU4 | "Private" includes corporate and closed-group use; distinct from "personal" | Interpretive | — |
| RU5 | Machine learning is "research" for s.52(1)(a)(i) | MAY | A=AI developer; D=MAY; I=store works for LLM training; C=data closed, not publicly accessible |
| RU6 | Non-infringing-copy condition in the Explanation applies only to computer programmes | Interpretive | — |
| RU7 | Fair dealing determined by the three-factor test at para 236 | Test | Limited use + no market substitution + public interest |
| RU8 | Copyright in a public address vests in the speaker (s.17(cc)), not the reporting agency | SHALL | A=speaker; I=first ownership incl. translation right; C=address or speech delivered in public |
| RU9 | Offshore server location does not defeat jurisdiction where access and transmission originate in India | SHALL | A=court; I=exercise jurisdiction; C=chain of events originating in India |

---

## S7. Concept Linkages

| Concept | Linkage |
|---|---|
| [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | **Major.** Model behaviour reconstructed from vendor-published training dates in the total absence of retained artefacts (S5.1). Prompt design established as an evidentiary standard (S5.2). BSA and admissibility never engaged. |
| [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | **New inter-branch variant** — judicial resolution concurrent with executive TDM consultation (S5.3). |
| [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] | Judiciary as a fifth instrument-issuing institution, now adjudicating rather than advising. Contrast [[07_Institutions/SCI]]. |
| [[05_Concepts/05_Concepts_Standard/Accountability]] | s.17(cc) reallocates ownership to the speaker — accountability for content attribution does not follow the publisher. |
| [[05_Concepts/05_Concepts_Standard/Transparency]] | Court treated ChatGPT's source-linking as weighing against substitution. |
| [[05_Concepts/05_Concepts_Standard/Legitimacy]] | Public-interest factor made societal benefit an explicit component of the fairness determination. |
| [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] | Para 268: *"It would be economically unviable to develop an LLM if training of an LLM would require licenses from multiple sources."* |

---

## S8. Project Relevance

| Project | Relevance |
|---|---|
| [[02_Projects/P4_Doctrinal_IJLIT]] | **Highest in corpus.** Four doctrinal moves (§S3) plus a bespoke Indian fairness test (§S4) are directly on P4's subject matter. IJLIT is an OUP law-and-IT journal; a first-instance Indian AI copyright judgment is squarely in scope. ⚠ P4's declared scope is RBI + SEBI BFSI doctrinal — **a scope decision is required** (see S9). |
| [[02_Projects/P1_SLR_RG]] | Comparative material: the judgment surveys and distinguishes US, German, UK and EU authority. |
| [[02_Projects/P5_AI_Ethics]] | Public-interest reasoning and the human-benefit framing at para 218. |
| [[03_Domains/Judicial_Governance]] | Second corpus node and the first adjudication; supports promotion beyond seeded status. |
| [[08_Methods/Doctrinal_Analysis]] | Model of statutory construction: legislative history, expressio unius, updating construction. |

---

## S9. ⚠ VERIFY Flags

- **✅ RESOLVED 2026-08-02 (was V-DHC1-1, HIGH).** **No Division Bench appeal has been filed or decided as of the verification date.** Confirmed via Cyril Amarchand Mangaldas (29 July 2026) and SCC Online (26 July 2026), both describing the order purely as a single-judge interlocutory ruling with the underlying suit (CS(COMM) 1028/2024) continuing at trial. This confirms the order's treatment as unsettled/interlocutory throughout this node remains accurate — no appellate development is on record. Re-check periodically; a future appeal would materially change this node's weight and require re-flagging.
- **⚠ V-DHC1-2 (HIGH — scope decision, not a defect).** P4's declared scope is RBI + SEBI BFSI doctrinal analysis, IRDAI excluded. This judgment is copyright and IP, not BFSI. Either P4's scope widens to Indian AI doctrinal analysis generally, or **this judgment anchors a separate paper**. It is strong enough to carry one. Decision required before P4 activation in Q4 2026 — log in [[12_Decision Journal/Decision_Journal]].
- **⚠ V-DHC1-3 (MEDIUM).** Paragraph numbers cited here are from the supplied judgment text. Verify against the official Delhi HC copy (`2026:DHC:____`) before quoting; neutral citation not yet captured.
- **⚠ V-DHC1-4 (MEDIUM).** The Court's summary of *Bartz v. Anthropic* at para 80 quotes a passage referring to **Meta** and Llama, not Anthropic — an apparent conflation of *Bartz* with *Kadrey v. Meta* in the source text. Do not reproduce that quotation without checking both US judgments.
- **⚠ V-DHC1-5 (LOW).** GEMA v. OpenAI (Munich Regional Court, 42 O 14139/24, 11 Nov 2025) is not a corpus node. Worth intake as an international comparator — it reached the **opposite** conclusion on memorisation.
- **⚠ V-DHC1-6 (LOW).** RAG expressly undecided. Any claim about RAG liability in India remains open.

---

## Backlinks

**Related corpus nodes:** [[07_Institutions/Corpus/DPIIT/DPIIT_1]] (executive TDM track — parallelism pair) | [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]] (judicial-branch comparator) | [[04_Knowledge_Products/Wiki_Intake/F046_UK_LawCommission_AI_and_Law_DiscussionPaper_2025]] | [[07_Institutions/Corpus/MeitY/MeitY_7_IT_Intermediary_Guidelines_Digital_Media_Ethics_Code_Rules_2021]] | [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] | [[05_Concepts/05_Concepts_Standard/Accountability]] | [[05_Concepts/05_Concepts_Standard/Transparency]] | [[05_Concepts/05_Concepts_Standard/Legitimacy]] | [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Related domains:** [[03_Domains/Judicial_Governance]] | [[03_Domains/AI_Governance]] | [[03_Domains/Privacy_DataProtection]]
**Related institutions:** [[07_Institutions/DHC]] | [[07_Institutions/SCI]] | [[07_Institutions/DPIIT]]
**Related methods:** [[08_Methods/Doctrinal_Analysis]] | [[08_Methods/Institutional_Grammar_IG2]]
**Related projects:** [[02_Projects/P4_Doctrinal_IJLIT]] | [[02_Projects/P1_SLR_RG]] | [[02_Projects/P5_AI_Ethics]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Log

- 2026-08-02: Node created from full judgment text (135pp, 275 paras) supplied by Vivek, nine days after pronouncement. First judicial corpus node filed as Format A; opens the DHC institution track. All quotes verbatim from supplied text. Interim/prima facie status flagged prominently at head of node. Two HIGH VERIFY flags: appeal status unknown, and P4 scope decision required. Apparent Bartz/Kadrey conflation in the judgment's own text flagged at V-DHC1-4.
