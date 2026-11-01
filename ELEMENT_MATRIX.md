# ELEMENT MATRIX — behaviors (a)–(h) × elements (charter step 5)

Draft 1 · 2026-11-01 · Spiegel thread · written read-only. This is the only file written. No git command was run and no one was contacted.

**What this is.** For each behavior in `BEHAVIOR_LEDGER.md`, this file lists the elements of the candidate provisions, numbered as in `LAW/`, against the register documents (SP-ids). It names each gap, who holds the missing fact and the lawful way to get it, and the forum the jurisdiction file points to. **It draws no verdict.** That is ASSESSMENT_v1, a later step. Halsey Minor is the victim and the reporting party. His account is carried as his account, and it is never treated as a possible untruth.

**Inputs read in full:**
- `BEHAVIOR_LEDGER.md`: L-01…L-81, X-01…X-09, G-0…G-10 and "WHAT NO DOCUMENT SHOWS".
- All of `LAW/`: INDEX and the nine `VERIFIED_AT_SOURCE_2026-11-01_*` files, including `jurisdiction_and_intake`. Also `FAM_disclosure_timing_and_waiver`, which landed at 04:01, after this work began, and is used in (e).
- `FORENSIC_BRIEF_v1.md`, `OPEN_REQUESTS.md`, `QUESTIONS_FOR_HALSEY.md`, `COLLISION_GATE.md` and `EVIDENCE_REGISTER_NOTES.md`.
- From READING_NOTES:
  - two files the coordinator sent after this work began: `GOOGLE_NOTICES_and_KALE_denial` and `ASKS_TO_FIRM_2024` (with `INVENTORY/asks_to_firm_2024.tsv`);
  - `FIRST_CONVERSATIONS_2024_promised_disclosures`, `COURT_ORDERS_and_FL141`, `MO_2026-04-21_compel_disclosures`, `JURISDICTION_SPLIT_2026-09-28`, `BRIEF_and_DECL_2026-03-27_text` and `BEHAVIOR_c_proofs_of_service`;
  - `ASKS_TO_FIRM_2025_2026`, §§1–3 only. It landed at 04:11; its §§4–6 were not read.

**Searched, not read in full:**
- `EVIDENCE_REGISTER.tsv`, searched by pointer.
- From READING_NOTES, searched for single facts only: DOCKET_24STFL00432, PDD_2024-06-17_content, SPIEGEL_DECLARATIONS_2025-12, BEHAVIOR_b_e_primary, ALLY_2026-09-04, COURT_OF_APPEAL_docket_check, D3 and SERVICE_VIOLATIONS_LOG.
- The 63K, 81B and 85_V3 notes were searched only to trace where a ledger quotation came from.

---

## 1. LEGEND — how to read a cell

Each cell has three parts: **Status · Pointers (SP-ids / L-ids) · Operative words** (verbatim from the document cited, or the missing fact).

| Status | Meaning |
|---|---|
| **SHOWN** | The element's fact appears in a document of class COURT, SWORN, CORRESPONDENCE or ACCOUNT-record. A thread reader read that document, or the part of it that the cell relies on, in full. The read is recorded either as register read_status `full`, or in a READING_NOTES file that records a full read (for example, the POS page of a longer filing). |
| **PARTLY** | Part of the fact is shown. The cell says which part, by which SP-ids, and what is missing. |
| **NOT SHOWN** | No document read shows the fact. The cell names the missing fact. |
| **ACCOUNT-ONLY** | Only Halsey's statement carries the fact (L-id). It is his account, pending the document named in GAPS. |
| **AI-LEAD-ONLY** | Only AI material or WORK-PRODUCT points to the fact. That is never evidence. |
| **n/a** | The element does not arise on these facts. The cell says why. |

Rules applied:
1. **AI-LEAD and WORK-PRODUCT rows** (register class) can never make a cell SHOWN or PARTLY. Where the ledger's quotation comes only from an AI-LEAD or WORK-PRODUCT transcription, the cell says **"not read at source"**.
2. **[F] marks every email-dependent cell.** The 4/21/2026 §271 finding (EV-003: **SP-0659**, preserved copy SP-0668, COURT, read in full) stands in front of each such cell: "The Court finds that Respondent submitted Exhibit F to the Court and analyzed it as if it were an authentic set of email communications, knowing that it was not. … Because critical evidence in support of the RFO was fabricated, the Court finds that the submission of the RFO was a violation of Family Code Section 271".
   - [F] does not say the cited email is inauthentic. It says the finding meets any report that rests on emails "in the Department's hands on day one" (JURISDICTION_SPLIT E.4).
3. **No verdict words.** "PC 118 el.5" means element 5 in the LAW file's ELEMENTS list for that section.
   - The ELEMENTS lists in `FAM_disclosure_timing_and_waiver` are described by that file as AI-written indexes to quoted words. Here they are used only for their numbering; the operative words quoted are the statute's.
4. **Register lag.** Several documents were read in full by notes files that landed after the register's pass 2, so their register rows still say `not-read` or `metadata-only`. The cells cite the SP-id, and **Appendix A** names the notes file that holds the full read.
5. **Counting** (for §6): an element counts as shown only if SHOWN. PARTLY is counted separately, and n/a counts as not shown. **The elements that are SHOWN are mostly formal ones** (actor, oath, statement, place). For every criminal provision below, the falsity, knowledge, intent and materiality elements are NOT SHOWN.
6. **Abbreviations.**
   - Decl. 3/27 = Halsey's declaration of 3/27/2026 (SP-0590).
   - POS P1–P22 = BEHAVIOR_c §2.1. D1–D27 = BEHAVIOR_c §1.
   - Register = LASC register of actions: printout A (SP-0705) and B (SP-0712), both read in full; F (SP-0146); E (SP-0243).
   - D-66 = the existing system's split. The civil process owns "discovery and subpoenas to private parties and providers — … Lance Spiegel's firm, Shannon Minor, … preservation letters to any of them; any spoliation motion; the 21 April 2026 section 271 order and Exhibit F". Front 4 owns police, DA, AG and federal contact, and the City PRA request.

**Lawful routes used in GAPS:**

| Code | Route |
|---|---|
| **H** | Halsey's own records and accounts |
| **CLK** | Certified copies from the LASC clerk, 24STFL00432 ("any member of the public may request", FORENSIC_BRIEF §3) |
| **CSR** | Reporter's transcript, ordered from the court reporter |
| **PRA** | Public Records Act request. Front 4 owns PRA contact with the City (D-66; OPEN_REQUESTS R-6), so this is a pointer only. |
| **SUBP** | The civil process's subpoena. D-66 assigns subpoenas to the firm, to Shannon and to providers to the civil process. |
| **WAR** | Police warrant or other law-enforcement process |
| **GLP** | "valid legal process" to Google (EV-053, SP-0379: "Google only takes steps to preserve data upon being properly served with valid legal process.") |
| **FAM** | The family court, by motion |
| **FX** | Forensic examination under FORENSIC_BRIEF §4 custody |

Halsey decides every route. This thread requests nothing.

**Collision gate.** Any destination at beverlyhills.org or da.lacounty.gov is read by the existing routines, which file replies into the Shannon tracker and may auto-reply in Halsey's voice (COLLISION_GATE.md). Each forum note below is subject to W-C1…W-C3.

---

## 2. MATRICES BY BEHAVIOR (each followed by its GAPS and FORUM NOTE)

Sections 3 (GAPS) and 4 (FORUM NOTE) of the requested structure sit directly after each behavior's matrices, so each behavior can be read on its own.

### (a) Unauthorized access, alteration or creation of content in Halsey's accounts

**Entries:** L-01, L-02, L-03, L-04, L-05, L-78 and L-80, all ACCOUNT in the ledger. Context records X-01…X-05.

**Common record:**
- GOOGLE_NOTICES §5 (over SP-0029, SP-0074…SP-0083, SP-0337/0338, SP-0379 and SP-0469): "No document read here names any person as the one who accessed, altered or deleted anything in Halsey's accounts."
- The first firm email in the mailbox is 2024-01-25 (SP-0096). FIRST_CONVERSATIONS §0: "No message from/to/cc/bcc ysfamilylaw.com before 2024-01-25 (search returned none)."
- The 2025-08-04 window: "No Google security notice was found in the window." (GOOGLE_NOTICES §4)
- Thread 18461348b9fe0954 (SP-0042…SP-0046): "It is present in the mailbox now. All 5 messages were returned. None is labelled TRASH".

**A1 · PC 502(c)** (LAW/PC_computer_502 §1(3))

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Lead-in: actor "any person"; an act in (c)(1)–(c)(14); "(h)" exceptions not applying | NOT SHOWN (actor) [F] | L-01–L-05, L-78, L-80; SP-0379; SP-0469 | No document names who accessed, deleted or created anything. Google states a policy only: "Google only takes steps to preserve data upon being properly served with valid legal process." |
| el.2 "Knowingly" | NOT SHOWN | — | With no actor identified, there is no state of mind to show. |
| el.3 "without permission" | ACCOUNT-ONLY [F] | L-01 (SP-0337, read in full: GOOGLE_NOTICES §1); L-03 (SP-0590 ¶8); L-05 | 2025-10-16: emails "were permanently deleted from my mailbox without my knowledge or consent." |
| el.4 Defined terms: (b)(1) "Access", (b)(8) "Data", (b)(12) "Computer contaminant", (b)(14) "Electronic mail" | PARTLY | SP-0042–SP-0046; SP-0323; SP-0326 | The objects named are email messages and a Drive document. "Data may be in any form, in storage media". That any of them was deleted, added or infected by another person is ACCOUNT-ONLY. |
| el.5 (c)(4) "accesses and without permission adds, alters, damages, deletes, or destroys any data": deletions (L-01) | ACCOUNT-ONLY [F] | L-01; SP-0282 (not read at source); WP: EV-079 (SP-1410, WORK-PRODUCT, not read) | 2025-07-28 (via EV-076): "The emails have now been erased in my email account." The absence comparison is WORK-PRODUCT, and its "15/17" figure is marked SUPERSEDED in 85_V3 (§7 item 2). |
| el.5 (c)(4): the date of the deletions | ACCOUNT-ONLY [F] | L-01; SP-0549 | The discovery email is dated 2025-07-28. The complaint gives "4. August 4, 2025: Scalpel deletion executed using police report as blueprint". No Google notice appears in the 8/3–8/5/2025 window. |
| el.5 (c)(4) / (c)(1): documents "created and inserted" (L-03) and the Exhibit F document (L-78) | ACCOUNT-ONLY [F] | SP-0590 ¶8 (SWORN; pp. 1–3 read in full); SP-0323 (Drive metadata only); SP-0326 (read in full) | ¶8: "These fabricated documents were created using my accounts during the period of unauthorized access." Drive: "owner Halsey@realitylab.com"; the self-email's whole body is "Sent from my iPad". No creating person, client, IP address or device is recorded. |
| el.5 (c)(7) "accesses or causes to be accessed any computer, computer system, or computer network": Apple change (L-05) | PARTLY | SP-0547 (quoted at source per L-05; register not-read) | "The following changes to your Apple Account, halsey@minorventures.com, were made on February 27, 2026 at 4:03:08 PM EST: Password". The change is recorded; who made it is not. |
| el.5 (c)(8) "introduces any computer contaminant": L-02 | ACCOUNT-ONLY [F] | SP-0284 (checked at source per L-02; a privileged communication, Halsey's to keep or waive) | "Lance sent the malware." No examined file or device is in the record. |
| el.5 (c)(9) "uses the internet domain name or profile of another … in connection with the sending of one or more electronic mail messages": L-04 and the envelope contents | ACCOUNT-ONLY [F] | SP-0549; SP-3289 | "Lance or his counsel read a "terrible documents" email in court, claiming I sent it." / "I opened a few and saw fakes emails from me". |
| el.5 (c)(7): the video call (L-80) | ACCOUNT-ONLY | L-80 | "Somebody said I'll drop off now and you can go ahead with your call" (relayed 2026-11-01). Interception statutes are not in LAW/. |
| el.6 Employment exception (h)(1) | n/a | — | This arises only once an actor is identified. |
| el.7 (j): "is deemed to have personally accessed … in each jurisdiction" | n/a | — | No record shows where any access came from. |

*Civil action (el.8–9):* "within three years of the date of the act complained of, or the date of the discovery of the damage, whichever is later." On Halsey's discovery date (2025-07-28), that is 2028-07-28 (arithmetic only). Google's log retention is the shorter clock (FORENSIC_BRIEF §6).

**A2 · PC 182, if two persons**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 "If two or more persons conspire" | NOT SHOWN [F] | L-01, L-61; SP-0469 | No second person is identified. Kalé, 1/12/2026: "I would not know how to be a part of a "Scalpel-like hacking" operation." |
| el.2 "conspire" (an agreement) | NOT SHOWN | — | No document read shows any communication between Spiegel or his firm and another person about Halsey's accounts. |
| el.3 Object: (a)(1) "To commit any crime." / (a)(5) "to pervert or obstruct justice" | NOT SHOWN | — | — |
| el.4 Overt act (subd. (b)) | NOT SHOWN | — | — |
| el.5 Venue | n/a | — | — |

**A3 · PC 135 — the L-01 deletions as destruction of evidence**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 "A person who" | NOT SHOWN | L-01 | — |
| el.2 "knowing that any … record … is about to be produced in evidence upon a trial, inquiry, or investigation" | PARTLY [F] | SP-0469; SP-3482 | An investigation existed: Kalé, "we still have that original 567-page document you sent us. That document has not been compromised at all." Lt. Coulter: the case went to the DA on 2/9/2026. Anyone's knowledge is NOT SHOWN. |
| el.3 "willfully destroys, erases, or conceals" | ACCOUNT-ONLY [F] | L-01 | As in A1 el.5. |
| el.4 "with the intent to prevent it or its content from being produced" | NOT SHOWN | — | — |

**A4 · PC 134 — documents created in his files (L-03, L-78)**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 "preparing" | ACCOUNT-ONLY [F] | SP-0590 ¶8; L-78 | "I identified documents that had been created and inserted into my files that I had never authored." / "it was constructed on my computer based on the virus" |
| el.2 "any false or ante-dated … paper" | SHOWN, for Exhibit F only [F] | SP-0659 | "…analyzed it as if it were an authentic set of email communications, knowing that it was not." This finding is about Respondent's submission. It does not say who or what created the 2025-09-24 document. |
| el.3 The preparer's intent: "to produce it, or allow it to be produced for any fraudulent or deceitful purpose, as genuine or true" | NOT SHOWN | — | — |
| el.4 Intended setting: "upon any trial, proceeding, or inquiry whatever" | PARTLY [F] | SP-0659 | Exhibit F was filed with the 11/12/2025 RFO. The preparer's intent is not shown. |

**A5 · PC 132 and BPC 6068(d) — the "terrible documents" email (L-04)**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| PC 132 el.1–2 Actor and setting ("upon any trial, proceeding") | ACCOUNT-ONLY | L-04; SP-0705; SP-0712 | The register shows no hearing on 1/10/2026: "1/9/2026 1:30 PM … Ex Parte Hearing — Not Held - Court's Motion"; "1/12/2026 8:30 AM … RFO - Family Law — Held - Order Made". |
| PC 132 el.3 "offers in evidence, as genuine or true" | ACCOUNT-ONLY [F] | L-04 | "read a "terrible documents" email in court, claiming I sent it" |
| PC 132 el.4 The object (which email) | NOT SHOWN | — | The email used is not in the record. |
| PC 132 el.5 "forged or fraudulently altered or ante-dated" | NOT SHOWN | — | — |
| PC 132 el.6 "knowing the same" | NOT SHOWN | — | — |
| BPC 6068(d) el.3 "never to seek to mislead the judge … by an artifice or false statement of fact" | ACCOUNT-ONLY | SP-0532 (Ex. 1 p. 19: the 1/12/2026 order as filed) | "For the reasons stated on the record, the RFO/MTN - Family Law filed by Respondent on November 12, 2025 is denied." |

**GAPS (a)**

| # | Missing fact | Who holds it | Lawful way to obtain it |
|---|---|---|---|
| a-1 | Who accessed halsey2005@gmail.com (= Halsey@realitylab.com, D-67) and deleted mail, 2025-04→09, including 2025-07-28 and 2025-08-04: sessions, IP addresses, devices, deletion events | Google; first, Halsey as Workspace administrator | **H** first: admin-console audit log and Vault exports, screen-recorded and hashed (FORENSIC_BRIEF §3–4). Then **GLP** (warrant or court subpoena) for server-side records (Q-F3; OPEN_REQUESTS Part B row (a)). Retention limits apply (FORENSIC_BRIEF §6). |
| a-2 | What created "Email Financial Records Chronological Index" at 2025-09-24 06:19:45Z (actor, IP address, client), and its version history | Google Workspace; Halsey is the administrator | **H** (Q-H2; Q-F2; FORENSIC_BRIEF Outcome F) |
| a-3 | Which documents were "created and inserted" (Decl. ¶8): when, and by what account or process | Halsey's devices and Drive | **FX** (device imaging) + **H** (Q-F4) |
| a-4 | Whether any attachment from the firm carried code: the attachments as received, the device image, and the firm's sent copies | Halsey; the firm | **FX**; **SUBP** (D-66) (Q-F4) |
| a-5 | Who changed the Apple password on 2/27/2026 (sign-in, device, IP) | Apple; Halsey as account holder | **H** (Apple account data request); then **WAR** |
| a-6 | The call in L-80: platform, date, meeting id, participant and join log | The provider (Dialpad appears in his mail); Halsey's account | **H** first; then the provider by process (Q-H1; Q-F6) |
| a-7 | The email "read in court" and the hearing at which it was read (L-04) | LASC; the court reporter; the firm | **CSR** (transcript of the 1/12/2026 hearing); **CLK**; **SUBP** |
| a-8 | A second person for PC 182: any Spiegel/firm contact with BHPD | BHPD/City | **PRA** item 6 / 5(d) (R-6; see (f)) |
| a-9 | Any Halsey–firm email before 2024-01-25 (the subject of Exhibit F) | Google; Microsoft; the firm | **GLP**; **SUBP** (Q-F1) |

**FORUM NOTE (a).** No forum can be fixed until the place of any access is known (a-1).
- The jurisdiction file's P2 row: "**LAPD** if inside the City of Los Angeles (Division by address), **BHPD** if inside Beverly Hills, otherwise "your local Sheriff's Station or police department" (**LASD**)".
- PEN 502(j): "is deemed to have personally accessed the computer, computer system, or computer network in each jurisdiction." [3.5]
- DA FAQ: "All crimes should be reported to the police agency in the area where the crime occurred." [2.1]
- LASD: "If you wish to report a non-emergent crime involving the internet please call your local Sheriff's station, law enforcement agency or the LASD Fraud & Cyber Crime Bureau (562) 374-2601." [7.6]
- "No retrieved source identifies an agency in Mexico or a route for a victim located abroad" [7.5].
- If an attorney were ever shown to be the actor: JSID [2.3].
- Federal, note only: IC3 [7.6].

---

### (b) Material from Halsey's accounts appearing in filings

**Entries:** L-06, L-07 and L-08 are DOCUMENTED; L-09 and L-79 are ACCOUNT. L-59 is cross-tagged.

**B0 · The behavior's predicate** (not a LAW element)

| Fact | Status | Pointers | Operative words |
|---|---|---|---|
| Material from communications with Halsey appears in filings | SHOWN | SP-0221 (SWORN; read through Ex. 14); SP-0226 (SWORN; read in full) | L-06: "WhatsApp messages between Respondent and I". L-07: Ex. 9 "From halsey2005@gmail.com To Anna Kralle; Lance Spiegel". L-08: Bates "VL_000060–VL_000079". |
| The source each item shows on its face | SHOWN [F] (L-07) | SP-0221; SP-0226; SP-0180 | L-06: the only senders are "Halsey Minor" and "Shannon". L-07: every email read is addressed to the declarant. L-08: "third-party productions, sources printed on their face"; the producing entities are among the 10/31/2024 subpoena targets. |

**B1 · PC 502(c)(2)** — this arises only if material came from his accounts without permission.

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Actor; an act under (c) | NOT SHOWN | L-79; Q-H3 | No filing read uses information that, at the time, existed only in Halsey's private channels. |
| el.2 "Knowingly" | NOT SHOWN | — | — |
| el.3 "without permission" | NOT SHOWN | SP-0221; SP-0226 | Each source shown is a party to the chat, the addressee of the email, or a subpoena production. |
| el.4 (b)(8) "Data" / (b)(9) "Supporting documentation" | n/a | — | No item is traced to his computer or accounts. |
| el.5 (c)(2) "accesses and without permission takes, copies, or makes use of any data from a computer, computer system, or computer network" | NOT SHOWN; ACCOUNT-ONLY for L-79 | L-79 | "That's how Lance has been so telepathic." (relayed 2026-11-01) |
| el.5: mediation material in the 6/24/2025 DVRO request (L-09) | ACCOUNT-ONLY [F] | SP-0270 (COURT; located, not read); SP-0284; lead: 81B C5 (AI-LEAD) | 8/3/2025: "Somehow, Lance paid off my mediator to share all confidential emails and conversations I had with them." |
| el.5: Exhibit 18 (L-59) | PARTLY | SP-0221 ¶7 (read) | "A copy of correspondence to the Beverly Hills Police Department from Respondent's counsel is attached hereto as Exhibit '18.' I was not copied on the letter from Respondent's counsel." How he obtained it is NOT SHOWN. Ex. 18 itself was not found (16.4 MB file, over the download limit). |
| el.6–el.7 | n/a | — | — |

**B2 · PC 182 — L-09 (Spiegel and the mediator)**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Two or more persons | ACCOUNT-ONLY [F] | L-09; SP-0284 | "Lance paid off my mediator" |
| el.2 Agreement | ACCOUNT-ONLY | L-09 | — |
| el.3 Object | NOT SHOWN | — | Evid. Code § 1119 is not in LAW/. No LAW text makes the use of mediation material a crime. |
| el.4 Overt act | NOT SHOWN | — | There is no payment record. |
| el.5 Venue | n/a | — | — |

**GAPS (b)**

| # | Missing fact | Who holds it | Lawful way to obtain it |
|---|---|---|---|
| b-1 | One filing that used a fact then existing only in his private channels | Halsey, to name it; the LASC file | **H** (Q-H3); **CLK** |
| b-2 | The 6/24/2025 DVRO request with its exhibits | Halsey's Drive (drive:1MXzsfi8…, SP-0270); LASC | **H** (open it outside this toolset); **CLK** |
| b-3 | The mediator's file, and any payment | Jacobson | **SUBP** (D-66) or **FAM** |
| b-4 | Exhibits 15–30, including Exs. 18–19, of the 4/18/2025 Spiegel declaration | LASC; Halsey's served copy (SP-0221, over the download cap) | **CLK**; **H** (OPEN_REQUESTS Part B row (f)) |
| b-5 | The protective order covering the "CONFIDENTIAL" pages (the "Engel PO Certification") | LASC; the firm | **CLK** |

**FORUM NOTE (b).** For computer access, the lines are those of (a). For an attorney's conduct in filings: JSID, "investigates and prosecutes criminal conduct by persons who work within the justice system in Los Angeles County, including attorneys" [2.3]. The mediation-privilege question belongs to the family court; no LAW/ text makes it a criminal matter.

---

### (c) Papers claimed as served on dates other than sent

**Entries:** L-10…L-46 and L-81. The ledger counts 36 DOCUMENTED and 2 ACCOUNT (L-39, L-41).

The fact this behavior turns on is that a paper travelled on a date other than its declared date. That fact is documented for no paper: "No document assigns any paper to any envelope." (ledger (c), common facts).

The POS pages relied on below were read in full (BEHAVIOR_c §2.0–2.1), although several register rows for the whole filing read `partial`:
- **P1** SP-0869
- **P2a/P2b** SP-1143
- **P3** SP-1919 (also SP-0387 p20)
- **P4** SP-0390 (D6, byte-identical)
- **P5** SP-2790 · **P6** SP-1706 · **P7** SP-2760 · **P8** SP-1904 · **P9** SP-1073 · **P10** SP-2683 · **P11** SP-1791 · **P12** SP-1574
- **P13** SP-1228 · **P14** SP-2393 · **P15** SP-1774 · **P16** SP-2503
- **P17** SP-0532 · **P18** SP-1864 · **P19** SP-1857
- **P20** SP-0915 · **P21** SP-1941 · **P22** SP-2583

**C1 · PC 118 — the proofs of service (P1–P22; 2024 POS)**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Actor: "every person who … declares … under penalty of perjury" | SHOWN | P1–P22 (above); L-15 (ALLY notes p.6, SUBP-025 POS read; register SP-2527 lags); L-19 (SP-0199, POS p.97) | The declarants are firm staff: ANNA KRALLE VANMALI (P1, P5–P8, P11–P22) and MATTHEW SIRRIYEH (P2a/b, P3, P4, P9, P10). No POS is signed by Spiegel. |
| el.2 Setting (B): penalty of perjury | SHOWN | same | "I declare under penalty of perjury under the laws of the State of California that the above is true and correct." |
| el.3 "states as true" | SHOWN | same | "On [DATE], I served the within document(s) …"; "A. BY MAIL … on the date shown below"; "D. BY ELECTRONIC COMMUNICATION - I caused a true copy thereof to be transmitted on the date shown". |
| el.4 "any material matter" | NOT SHOWN | SP-0663; SP-0558 | No ruling is shown to turn on a declared date. The 4/21/2026 order: "The Court finds that the Respondent has been provided with notice of these proceedings." |
| el.5 "which he or she knows to be false": the mail leg, P1–P19 | NOT SHOWN [F] | SP-2776 (photographs); SP-2798 (Ex. A); SP-2799 (Ex. B); SP-3513 (Correos) | No envelope is matched to a paper. The labels run "DEC 30, 2025" to "FEB 02, 2026". Correos shows "30/01/2026 12:14: 'Deposito del Cliente en el país de origen'" and "26/02/2026 12:04: 'Entrega'". That is a third-party record transcribed live, with no saved capture. |
| el.5: P20–P22 | PARTLY [F] | SP-0915, SP-1941, SP-2583; SP-0563 (read in full) | The POS say "March 4, 2026" for the mail and email legs. The only firm email is "2026-03-02T21:01Z". BEHAVIOR_c §3 read every ysfamilylaw.com message from 11/1/2025 to 3/15/2026, and none is dated 3/4. The declared date is later than the email, not earlier. Knowledge is NOT SHOWN. |
| el.5: P3 (12/26/2025) | NOT SHOWN [F] | SP-1919; SP-0383 | The email reads "Per the attached, the deposition will not be proceeding …"; "The body says nothing about mail." The four "DEC 30, 2025" labels are 4 days later and are candidates only. |
| el.5: the orange package (L-81) | PARTLY | SP-3513; SP-2776 p-003 | Deposited 30/01/2026, which is 3 days after the 1/27/2026 POS (P10) and 3 days before the 2/2/2026 POS (P11–P12). No POS in hand declares 1/30/2026. No POS was located for the FL-300 dated 1/30/2026. |
| el.5: the bundled delivery (L-39) | ACCOUNT-ONLY (that papers were mailed late); the delivery itself is SHOWN | SP-0590 ¶4; SP-2799 | ¶4: "The papers in that bundled delivery corresponded to documents that had previously been claimed as served on different dates." Ex. B is typed "February 24, 2024" and "early December 2023", as recorded. |
| el.6 "willfully" | NOT SHOWN | — | — |
| el.7 Place | SHOWN | P1–P22 | "Executed on [DATE], at Beverly Hills, California." This element is a scope rule. |
| el.8 Proof limitation | n/a | — | It arises only once falsity is shown. The comparisons available (labels, the Correos record, email headers) are documentary, not one witness's testimony. |

**C2 · PC 132 — POS offered as proof by Spiegel**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Actor | SHOWN | SP-1857 (D24 pp.3–7 read in full); SP-1864; SP-0532 | The MPAs are signed "LANCE S. SPIEGEL". |
| el.2 "upon any trial, proceeding" | SHOWN | same; SP-0663 | The RFO on Respondent's "Objection to Defective Service" (EV-002). |
| el.3 "offers in evidence, as genuine or true" | PARTLY | SP-1857 | "As demonstrated by the Proof of Service By Mail for Petitioner's RFO re Section 271 Sanctions dated December 30, 2025, all papers were mailed to Respondent at his address in Mexico. (Exhibit B, Proof of Service By Mail dated December 30, 2025)." Exhibits A and B are not in the 7-page copy read. |
| el.4 Object: "paper, document, record" | SHOWN | same | A proof of service. |
| el.5 "forged or fraudulently altered or ante-dated" | NOT SHOWN | — | The two 12/30/2025 POS are not in hand. The "DEC 30, 2025" labels fall on the cited date (0 days). |
| el.6 "knowing the same" | NOT SHOWN | — | — |

**C3 · PC 134**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 "preparing" | SHOWN | P1–P22 | Executed by firm staff (DocuSign on P3 and P10; script-font names on the others; handwritten on P2a/b, P4 and P9). |
| el.2 "any false or ante-dated … paper" | NOT SHOWN | — | For the date difference on P20–P22 see C1 el.5. The 12/2x/2025 declaration is in H1. |
| el.3 "with intent to produce it … for any fraudulent or deceitful purpose" | NOT SHOWN | — | — |
| el.4 "upon any trial, proceeding … authorized by law" | SHOWN | P1–P22 | Prepared for LASC 24STFL00432. |

**C4 · PC 127 — Spiegel and the declarants**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Actor / el.3 "another person" | SHOWN (formal) | P1–P22; SP-0400 | The declarants are other persons. Spiegel is copied on transmittals (e.g. SP-0400: "cc … lances@"). |
| el.2 "willfully procures" | NOT SHOWN | — | Being copied on an email is not procurement. No instruction to a declarant is in the record. |
| el.4 "to commit perjury" | NOT SHOWN | — | No perjury is shown. |
| el.5 Result | NOT SHOWN | — | — |

**C5 · BPC 6128(a) and BPC 6068(d) — Spiegel's statements about service**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| 6128 el.1 "Every attorney" | SHOWN | SP-0712 | "SPIEGEL LANCE STEPHEN Attorney for Petitioner" |
| 6128 el.2 "guilty of any deceit or collusion, or consents to any deceit or collusion" | NOT SHOWN | — | — |
| 6128 el.3 "with intent to deceive the court or any party" | NOT SHOWN | — | — |
| 6068(d) el.1 / el.2 / el.3 | SHOWN / NOT SHOWN / NOT SHOWN | SP-1864; SP-1857; SP-0532 | The statements are shown: "As stated in the proof of service, the Notice of Consumer which attached the Subpoena was mailed to Respondent at his address in Mexico." / "the proof of service by mail establishes that Petitioner timely and properly served her response." That either statement is untrue is not shown. |

**C6 · CCP 415.30 — the 2024 summons by acknowledgment** (civil; L-10–L-13)

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 "A summons may be served by mail as provided in this section." | SHOWN [F] | SP-0096 (attachments read in full: FIRST_CONVERSATIONS §0, §3) | 1/25/2024 letter: "Please date and sign the Notice and Acknowledgment of Receipt and return by email to my office." |
| el.2 "shall be mailed (by first-class mail or airmail, postage prepaid)" | NOT SHOWN [F] | SP-0096; SP-0102 | The letter is headed "VIA MAIL ONLY / halsey2005@gmail.com". Both packets went by email. The 2/13 NAR reads "Date of mailing: February 13, 2024". A mailing is not shown. |
| el.3 "two copies of the notice and acknowledgment … and a return envelope, postage prepaid" | NOT SHOWN | — | — |
| el.4 Form | SHOWN | SP-0096 | FL-117 Notice and Acknowledgment of Receipt. |
| el.5 "deemed complete on the date a written acknowledgement … is executed, if such acknowledgement thereafter is returned to the sender" | SHOWN [F] | SP-2835 (read in full: FIRST_CONVERSATIONS §3; register lags); SP-0144 (attachment read: same); SP-0160 (FL-180) | 2024-03-08T07:32:29Z: "Accepted March 7, 11:31 PM Pacific Time", with the signed NAR. Filed "3/8/2024 12:24 PM … By A. Gonzalez, Deputy Clerk". FL-180: "The court acquired jurisdiction of the respondent on (date): 3/8/24". |
| el.6 Failure to return | n/a | — | It was returned. |
| el.7 "A notice or acknowledgment of receipt in form approved by the Judicial Council is deemed to comply" | SHOWN | SP-0096 | FL-117. |

**C7 · CCP 1013b (adjacent) — the form of the proof of electronic service** (civil; the email leg of P1–P22)

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Method: an affidavit showing county of employment and age over 18 | SHOWN | P1–P22 | "I am employed in the County of Los Angeles, State of California. I am over the age of 18" |
| el.2 Contents: sender's address, date, addresses served, statement of e-service | SHOWN | same | "from [SENDER EMAIL]"; the four addresses; "D. BY ELECTRONIC COMMUNICATION" |
| el.3 Signature "as provided in subparagraph (B) of paragraph (2) of subdivision (e) of Section 1010.6" | PARTLY | same | Script-font names appear on 17 POS. The signing procedure behind them is not shown, and rule 2.257 is not in LAW/. |
| el.4 Electronic form allowed | SHOWN | same | — |

**Other (c) entries:**
- **L-41 (notice of the 4/21/2026 hearing):** ACCOUNT-ONLY as to its timing. The court's records: "Notice of this Minute Order is given to Respondent and Petitioner's Counsel via eService." (3/2/2026, SP-0558) and "the Court's tentative ruling was emailed to both Petitioner and Respondent" (SP-0658). [F]
- **Compliance with the trackable-mail order after 4/21/2026 (EV-002, SP-0663):** SHOWN that the transmittals recite USPS numbers: "EH045932903US" (SP-0694), "RF414716216US" (SP-0709), "RF414716220US" (SP-0715) and "RF414694440US" (SP-0717). No filed POS with tracking was read, and no scan history is in the record. [F]

**GAPS (c)**

| # | Missing fact | Who holds it | Lawful way to obtain it |
|---|---|---|---|
| c-1 | Which paper travelled in which envelope, set beside each POS | Halsey (the envelopes and their contents); LASC (the POS images) | **H** (Q-H4); **CLK** (OPEN_REQUESTS Part B rows (c)) |
| c-2 | USPS acceptance and scan history for "LH 265 470 088 US" and for every "00495 BEVERLY HILLS" label | USPS | **WAR** (law-enforcement request) |
| c-3 | An evidentiary capture of the Correos page | Halsey | **H**. The USPS_tracking note says "An evidentiary capture would need a person to save the live page." |
| c-4 | The firm's mail log and postage or meter records, 11/2025–2/2026 | The firm | **SUBP** (D-66) |
| c-5 | The two 12/30/2025 POS cited as D24 Exhibits A and B | LASC | **CLK** |
| c-6 | The POS of the 1/27/2026 Responsive Declaration (drive:181IlSVc…, SP-1066, 9.2 MB, not read) | Halsey's Drive; LASC | **H** (open it outside this toolset); **CLK** |
| c-7 | Any POS for the vexatious-litigant FL-300 dated 1/30/2026, the same day as the orange package's deposit | LASC | **CLK** |
| c-8 | The printed originals bearing original signatures. CCP 1010.6(e)(2)(B)(i): the filer "shall maintain the printed form of the document bearing the original signature … and make it available for review and copying upon the request of the court or any party" | The firm | A party's request in the case. Halsey decides, and the request must never mention any report (§5). |
| c-9 | Materiality: whether any ruling turned on a declared date | LASC; the court reporter | **CLK**; **CSR**. The 3/2/2026 international-service note (SP-0558) cites a Rule of Court that is not in LAW/. |
| c-10 | Knowledge: what the declarants and Spiegel knew of the actual mailing dates | Firm staff; the firm | **SUBP**; **WAR** |
| c-11 | The correct year in the Exhibit B declarations | The declarants | Halsey decides on re-execution (Q-H5) |
| c-12 | Law not in LAW/: CCP 1013(a), which the firm cites, and the presumption printed on the blank CEB block on D8 p48: "service is presumed invalid if postal cancellation date or postage meter date is more than one day after date of deposit for mailing in affidavit" | — | Retrieve at source before any use |

*Cross-file note:* OPEN_REQUESTS Part B ties the envelope preservation ask to "Q-H1". In QUESTIONS_FOR_HALSEY the envelopes are **Q-H4**; Q-H1 is the video call.

**FORUM NOTE (c).**
- The jurisdiction file's P1 row: "Place of signing, 301 N. Canon Dr.: **Beverly Hills Police Department** (City of Beverly Hills), 464 N. Rexford Dr. [1.1–1.4]. Place of filing, 111 N. Hill St.: **LAPD, Central Division** (Central Bureau, Reporting District 122), station 251 E. 6th St. [1.5]. Named on the DA's page for conduct of attorneys and court personnel: **DA Justice System Integrity Division** [2.3] … The sources do not say which of the two police agencies takes a report about an act that spans both places."
- Federal, note only: "Any fraud that uses the U.S. Mail™—whether it originates in the mail, by phone, or online—is mail fraud." [6.1]
- State Bar (SP-0689): "If that court were to find any impropriety by the lawyer, please forward such written findings to our office for review."
- The family court's own instrument going forward is the 4/21/2026 trackable-mail order (SP-0663).

---

### (d) Electronic service without consent

**Entries:** L-47–L-53. Cross-tagged: L-10, L-13, L-24, L-27 and L-41.

**No criminal provision fits (d) on its own.** CCP 1010.6, CRC 2.251 and CCP 473 are "PROCEDURAL / CIVIL … No punishment" (LAW/CCP_service; LAW/CRC_2.251). The only criminal question would be a sworn POS that states an e-service fact known to be false and material. That is PC 118, in matrix C1.

**Representation periods** (register, read in full):
- No attorney is listed for Respondent before the 10/18/2024 substitution (printout F, SP-0146).
- Printout E (SP-0243): "PROVINZIANO ALPHONSE FRANCIS - Attorney for Respondent for Respondent". The withdrawal was "Granted" on 6/5/2025.
- Printouts C, D, A and B list no attorney for Respondent.

**D1 · CCP 1010.6**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Scope: "A document may be served electronically" | SHOWN [F] | SP-0372…SP-0563 (transmittals) | Every POS from P1 to P22 except P2a/b declares "A/D". |
| el.2 "Electronic service" means "electronic transmission or electronic notification" | SHOWN [F] | same; WP: EV-089 (SP-0744) | The four addresses. EV-089 records that minorventures mail delivers into halsey2005; that is WORK-PRODUCT. |
| el.3 Represented person (b): (i)–(iv) shown; (v) "confirm the appropriate electronic service address" | SHOWN (i–iv) / NOT SHOWN (v) | SP-0199 (POS p.97); SP-0243 | L-19, 2/24/2025: "BY ELECTRONIC COMMUNICATION … from mvs@ysfamilylaw.com" to "al@provinziano.com service@provinziano.com". |
| el.4(i) "An unrepresented party may consent to receive electronic service." | SHOWN | SP-0146; SP-0705; SP-0712 | Unrepresented 1/16/2024→10/18/2024 and from 6/5/2025. |
| el.4(ii) Express consent: a notice served on all parties and filed, or affirmative consent "through electronic means with the court or the court's electronic filing service provider" | NOT SHOWN as to any consent document. That absence is what the behavior asserts, and it is documented only as far as the records read reach. [F] | SP-0590 ¶3; SP-2830 (read in full: FIRST_CONVERSATIONS §3); SP-0264; SP-0267; SP-0658 | ¶3: "I have not filed Judicial Council form EFS-005-CV or any other written consent to electronic service." 2/13/2024, to lances@: "I will accept the service of these documents by email." 6/23/2025: "I AGREED TO ACCEPT SERVICE FOR ONLY THE DIVORCE PAPERS". The court's summary of his 1/5/2026 motion: "despite the parties agreeing to email service to exchange declarations of disclosure". None of these is a filed notice. His own e-filing provider's terms were not examined. |
| el.4(iii) "The act of electronic filing shall not be construed as express consent." | SHOWN (the rule applies) | SP-0712 | Respondent's 16 register entries "Proof of Service Electronic" (6/4/2025–3/27/2026) are e-filing acts, not consent. |
| el.4(iv) Withdrawal by Judicial Council form | n/a | — | No consent is on file. |
| el.4(v) "may only be completed by a person entitled to service" | n/a | — | — |
| el.6 When service is complete | SHOWN [F] | SP-0493 | e.g. 2026-01-28T07:04Z (1/27 23:04 PST): "deemed served on that court day". |
| el.7 Proof of e-service | → C7 | — | — |
| el.8 The court's own e-service (d) | PARTLY | SP-0558 | "Notice of this Minute Order is given to Respondent and Petitioner's Counsel via eService." The basis, (b) or (c), is not stated. |

**D2 · CRC 2.251**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Authorization (a): documents that "may be served by mail" | SHOWN | P1–P22 | Each declares a mail leg. |
| el.2 Express consent (b)(1)(A)/(B): a filed notice, provider terms, or "form EFS-005-CV" | NOT SHOWN [F] | SP-0590 ¶3 | No EFS-005-CV appears. Whether his provider's terms "clearly state[]" consent was not examined. |
| el.4 (c)(3)(B): self-represented persons "are to be served by non-electronic methods unless they affirmatively consent" | PARTLY [F] | SP-0712; P1–P22; SP-0123; SP-0262 | The self-represented party is SHOWN. Every POS from P1 to P22 adds mail. Email-only service is shown on the FL-141, "Email: halsey@minorventures.com" (6/18/2024), and in the ex parte notice of 6/23/2025 by calls and email. The rule's trigger, that the server is "required to file documents electronically", is NOT SHOWN: no LASC rule is in LAW/. |
| el.5 (f)(2) "may not be electronically served on a nonparty unless the nonparty consents … or … court order" | PARTLY [F] | SP-0695; SP-0701; SP-0663 | To kat.flds@, 5/8/2026: "please produce all documents … on or before Thursday, 05/14/2026 at 10:00 a.m." Schwenke: "I do not accept service by email." EV-002: "As a backstop, all service shall also be effectuated by electronic means." Whether that order reaches a nonparty is not shown. |
| el.6 (g)(3) An address is "presumed valid … if the party … files electronic documents with the court from that address" | NOT SHOWN | — | Which address his e-filings came from is not shown. |
| el.7 When complete | SHOWN [F] | as D1 el.6 | — |
| After 4/21/2026 | SHOWN | SP-0663 | From that date, e-service rests on the court's order: "As a backstop, all service shall also be effectuated by electronic means." |

**D3 · CCP 473(d)** (civil)

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.3(i) "on motion of either party" | NOT SHOWN | SP-0727 | No 473(d) motion appears. Schwenke's 7/31/2026 notice cites "(CCP § 473(b))" for the 7/21/2026 nonappearance finding. |
| el.3(ii) "after notice to the other party" | n/a | — | There is no motion. |
| el.3(iii) "set aside any void judgment or order" | NOT SHOWN | SP-0663; SP-0658 | "The Court finds that the Respondent has been provided with notice of these proceedings." |
| el.3(iv) Discretionary ("may") | n/a | — | — |
| el.5 Version B (e), from 1/1/2027: "a default judgment that is void for lack of proper service" | n/a on this record | SP-0712; SP-0160 | The 10/23/2024 judgment followed the parties' signed packet (FL-130 "I have previously made a general appearance"; FL-180). No default judgment is shown. |

**GAPS (d)**

| # | Missing fact | Who holds it | Lawful way to obtain it |
|---|---|---|---|
| d-1 | Whether the terms of his or Schwenke's e-filing provider account state consent to e-service (CRC 2.251(b)(1)(B)(i)) | Halsey; Schwenke; the provider | **H** |
| d-2 | Any EFS-005-CV, or a notice of consent, in the court file | LASC | **CLK** (a file search) |
| d-3 | Whether the 6/18/2024 email reached halsey@minorventures.com: the routing in June 2024 | Halsey; the minorventures mailbox; the firm (its sent item with headers) | **H** (Q-H6); **SUBP** |
| d-4 | The 8/18/2025 ex parte email (L-50, lead only) | Halsey's minorventures mailbox; the firm | **H**; **SUBP** |
| d-5 | The 4/21/2026 notice and tentative-ruling emails, with headers (L-41) | Halsey's mailbox; the court; the firm | **H** |
| d-6 | Whether EV-002's backstop covers a nonparty (L-53) | The court | **CLK** (the full order); **FAM** (clarification) |
| d-7 | Halsey's own FL-141 of 7/2/24 (packet SP-0160; pp.3, 4, 8 and 10–19 not read) | Halsey | **H** |
| d-8 | The LASC rule that makes e-filing "required" for the firm, if any (the CRC 2.251(c)(3) trigger) | LASC local rules (public) | Retrieve at source |

**FORUM NOTE (d).** No criminal provision and no police intake line applies to a procedural service defect.
- The forum is the family court, by motion. The 6/18/2026 appeal of the 4/21/2026 orders was "forwarded for consideration to dismiss the appeal" (SP-3433), and no Court of Appeal case number was found (Q-H8).
- State Bar (SP-0689): "If that court were to find any impropriety by the lawyer, please forward such written findings to our office for review."

---

### (e) Petitioner's disclosure and its service

**Entries:** L-54, L-55, L-56, L-57 (ACCOUNT) and L-58. Cross-tagged: L-11, L-19, L-47 and X-06 (the PDD).

**E1 · FAM 2104** (with § 2103 and rule 5.83)

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 "each party" | SHOWN | SP-0117 | Petitioner's PDD: FL-140, FL-142 and FL-150, each "Date: 6/17/2024", signed "SHANNON MINOR". |
| el.2 "shall serve on the other party a preliminary declaration of disclosure, executed under penalty of perjury" | SHOWN (execution, declared service, court finding) / ACCOUNT-ONLY (receipt) [F] | SP-0117; SP-0123; SP-0532 (Ex. 4, image read); SP-0658; SP-0261 | The court: "Petitioner has submitted proof that she has served her PDD on Respondent". Halsey, 6/17/2025: "I have never received the required forms (FL-140, FL-141, FL-142, FL-150, FL-160) for proper service". His then counsel's office emailed him "2024.06.17, P's PDD.pdf" on 2025-06-04 (SP-0255, from bill@provinziano.com; not the firm). |
| el.3 Exceptions: "court order for good cause"; § 2110 | n/a | — | None was claimed. § 2110 concerns default judgments; § 2101(b) excludes stipulated judgments from "Default judgment". |
| el.4 Timing (f): "within 60 days of filing the petition"; "may be extended by written agreement of the parties or by court order" | PARTLY [F] | SP-0712 (filed 1/16/2024); SP-0123 (served 6/18/2024); SP-0096 (FAM 111 order, read in full) | FAM 111: "The Petitioner has 60 days after filing the Petition to complete the PDD and have the other spouse served." / "Exception: You and your spouse can extend the deadline if you agree in writing or get permission from the court." Arithmetic only: day 60 is 2024-03-16, a Saturday, and 6/18/2024 is day 154; the text states no counting rule. A written extension or order is NOT SHOWN; none was found (FIRST_CONVERSATIONS §1, §4). Rule 5.83(c)(4)(C), a case-management milestone: "The petitioner's preliminary declaration of disclosure should be served within 60 days of the filing of the petition". |
| el.5 Content: "the identity of all assets … with sufficient particularity" | PARTLY | SP-0117; SP-0199 (partial) | 6/17/2024 FL-142: WF x0890; four Vanguard 529s; items 5, 10 and 13 "NONE"; total 808,216. The 2/24/2025 FL-142 adds WF x1074, x1530, x4249, x4215 and x5631, four term-life policies, and "FIDELITY ROTH IRA X3347". Whether those existed in Petitioner's name on 6/17/2024 is NOT SHOWN. |
| el.6 Attachments: tax returns of the prior two years; an I&E | PARTLY | SP-0117 | FL-140: "X All tax returns filed by the party in the two years before the date that the party served the disclosure documents. 2023 TAX RETURN ATTACHED". The FL-150 is included. The copy read has "No 2022 return". Whether a return filed in the window was left out is NOT SHOWN. |
| el.7 "the parties shall file proof of service of the preliminary declaration of disclosure" (and § 2103) | SHOWN | SP-0123; SP-0712 | The register for 6/18/2024: "Declaration - Service of Preliminary Dec. of Disclosure" (Petitioner). FL-141 e-filed "6/18/2024 1:42 PM". |
| el.8 Amendment: "Proof of service of an amendment shall be filed with the court" | PARTLY | SP-0199; SP-0712; SP-0390 ¶11.A | The 2/24/2025 "PETITIONER'S SCHEDULE OF ASSETS AND DEBTS" was e-served on Provinziano (POS p.97). The register has no 2/24/2025 entry. Whether it is a § 2104(d) amendment, or an update under the continuing duty in § 2100(c), is NOT SHOWN. |

**E2 · FAM 2105(d) and FAM 2106 — the FL-144 waiver** (LAW/FAM_disclosure_timing_and_waiver §5, §6)

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| 2105 el.9 "The parties may stipulate to a mutual waiver of the requirements of subdivision (a) concerning the final declaration of disclosure" | SHOWN | SP-0161 (read in full) | FL-144 e-filed "8/22/2024 3:55 PM"; "Mediated by Jeffery S. Jacobson, CFLS". |
| 2105 el.10 "by execution of a waiver under penalty of perjury … by separate stipulation" | SHOWN | SP-0161 | "Shannon Minor … DocuSigned by: …"; "Halsey Minor … DocuSigned by: …". |
| 2105 el.11 "The waiver shall include all of the following representations:" | SHOWN | SP-0161; LAW §12 | Items 2.a–2.f of the FL-144 correspond to (d)(1)–(5). |
| 2105 el.12 (d)(1) "Both parties have complied with Section 2104 and the preliminary declarations of disclosure have been completed and exchanged." | SHOWN as a representation. Its truth is NOT SHOWN either way. | SP-0161; SP-0658 | Item 2.a: "We have complied with Family Code section 2104, and the preliminary declarations of disclosure have been completed and exchanged." The court relied on it. |
| 2105 el.13–el.14 (d)(2)–(3): the I&E exchanged; "fully augmented" | SHOWN as representations; augmentation PARTLY | SP-0161; SP-0199 | The later FL-142 lists accounts that are not in the 6/17/2024 FL-142 (E1 el.5). |
| 2105 el.15 (d)(4) "knowingly, intelligently, and voluntarily" | SHOWN as a representation; the circumstances ACCOUNT | SP-0161; SP-0155 | Mediator, 8/5/2024: "the documents are drafted to reflect that you are representing yourself. Let me know if anything has changed." |
| 2105 el.16 (d)(5) "does not limit the legal disclosure obligations … noncompliance … will result in the court setting aside the judgment" | SHOWN | SP-0161 | Item 2.e: "Each party understands that this waiver does not limit the legal disclosure obligations of the parties but rather is a statement under penalty of perjury that those obligations have been fulfilled." |
| What FL-144 waives | SHOWN (by its words) | LAW §12 | It waives the final declaration only. On waiving the preliminary declaration by stipulation, "the text is silent". |
| 2106: judgment on property only with the FDD served or "waived pursuant to subdivision (d) of Section 2105" | SHOWN (dates) | SP-0712 | The waiver was filed 8/22/2024 ("Stipulation - Waiver of Final Declaration of Disclosure", Petitioner), before the Judgment of 10/23/2024. |

**E3 · FAM 2107**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Request step: one party "fails to serve" or fails to give "sufficient particularity", AND "the other party has served the respective declaration"; then "request preparation … or further particularity" | PARTLY [F] | SP-0160 (FL-141 in the packet); SP-0712; SP-0143; SP-2896, SP-2905 (read in full: ASKS_TO_FIRM_2024); SP-3160 (read in full: ASKS_TO_FIRM_2025_2026); SP-0658 | Halsey served his own PDD: "Email on (date): 7/2/24". He asked for Petitioner's financial statements 3 times on 3 days in 2024 (7/19, 10/22 and 10/28), e.g. "I would appreciate you sending me financial documents from Shannon first". He asked 10 times on 9 days from 6/17 to 12/29/2025, e.g. "Please confirm in writing by Monday, January 5, 2026 that Petitioner will serve a complete, verified Preliminary Declaration of Disclosure". "No in-thread firm reply attached any document of category A or B." On "fails to serve", the court found otherwise (SP-0658). On "particularity", there is no finding. |
| el.2 Motions under (b) if the request is ignored | SHOWN | SP-0712; SP-0658 | 1/5/2026 "RFO/MTN - Compel Initial Other: Compel Preliminary/Final Declarations of Disclosure; Monetary Sanctions". Denied: "Respondent's motion for an order compelling these disclosures is unwarranted"; "this court has denied such requests as recently as 1.12.26". |
| el.3 Mandatory sanctions (c) | NOT SHOWN | SP-0658 | There is no finding of non-compliance. Petitioner's request was "justified"; the amount is reserved. |
| el.4 Set-aside (d), including (d)(1) actual fraud and (d)(2) "Perjury, as defined in Section 118 of the Penal Code" | NOT SHOWN | SP-0712; SP-0161 | No set-aside motion is in the record. The Judgment is dated 10/23/2024. |
| el.5 The court may order the exchanged declarations (e) | n/a | — | There is no set-aside motion. |

**E4 · FAM 2120–2129**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| 2121 el.1–3: dissolution; a judgment "adjudicating support or division of property"; "after the six-month time limit of Section 473" | SHOWN (preconditions of the court's power only) | SP-0712 | "10/23/2024 — Judgment"; "Status: Statistical Disposition on 10/23/2024". |
| 2121 el.4–5: a ground in this chapter; "materially affected the original outcome" | NOT SHOWN | — | — |
| 2122(a) Ground: "Actual fraud where the defrauded party was kept in ignorance or … fraudulently prevented from fully participating" | NOT SHOWN | SP-0161; SP-0155 | Halsey DocuSigned the FL-144. |
| 2122(a) Time: "within one year after the date on which the complaining party either did discover, or should have discovered, the fraud" | NOT SHOWN | — | No discovery date is documented. |
| 2122(b) Ground: perjury "in the preliminary or final declaration of disclosure, the waiver …, or in the current income and expense statement" | NOT SHOWN | SP-0117; SP-0161; SP-0189 | The statements are shown. Falsity and knowledge are not. |
| 2122(b) Time | NOT SHOWN | — | — |
| 2122(f) Ground: "Failure to comply with the disclosure requirements of Chapter 9" | NOT SHOWN | SP-0658 | The court found PDD service proven, and FL-144 recites the exchange. |
| 2122(f) Time | NOT SHOWN | — | — |
| 2123 Inequity alone is not a ground | n/a | — | A limit on relief. |
| 2124 Attorney negligence is not imputed | n/a | SP-0146; SP-0155 | Halsey was unrepresented on 6/18/2024 and 8/22/2024. |
| 2129 Judgments on or after 1/1/1993 | SHOWN | SP-0712 | 10/23/2024. |

**E5 · PC 118 — the sworn forms in (e)**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| FL-141 el.1–3: declarant, penalty of perjury, statements | SHOWN | SP-0123 | "Anna Kralle (TYPE OR PRINT NAME)"; "I declare under penalty of perjury"; "I am the X attorney for X petitioner"; "X Other (specify): Email: halsey@minorventures.com on (date): June 18, 2024". |
| FL-141 el.4 Materiality | NOT SHOWN | SP-0658 | The court relied on the email and the FL-141 for service. Whether the "attorney" box mattered is not shown. |
| FL-141 el.5 Falsity and knowledge | PARTLY (the "attorney" box) / NOT SHOWN (service) [F] | SP-0123; SP-0529; SP-0532 Ex. 4 | Every signature block read says "Paralegal" ("Anna Kralle, Paralegal"), and no State Bar number appears for her. Knowledge is NOT SHOWN. |
| FL-141 el.6 "willfully" | NOT SHOWN | — | — |
| FL-141 el.7–el.8 | n/a | — | The FL-141 states no place. Falsity is not shown. |
| PDD (Shannon), FL-150 (1/8/2025) and FL-144 (both parties) el.1–3 | SHOWN | SP-0117; SP-0189; SP-0161 | e.g. FL-142 items 5, 10 and 13 "NONE"; FL-150 item 13s "*LOANS FROM PARENTS"; FL-144 item 2.a. |
| PDD, FL-150 and FL-144 el.4–6 | NOT SHOWN | — | Falsity, materiality and knowledge are not shown (see E1 el.5). The declarants are Shannon, and Halsey for FL-144. |

**E6 · PC 127**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.2 "willfully procures" | NOT SHOWN | SP-0117 | The caption "LANCE S. SPIEGEL … ATTORNEY FOR (Name): PETITIONER, SHANNON MINOR" shows representation, not procurement. |
| el.4 "to commit perjury" | NOT SHOWN | — | — |

**E7 · BPC 6068(d) and BPC 6128(a)** — these apply only with knowledge shown.

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| 6068(d) el.1; 6128 el.1 | SHOWN | SP-0712 | Attorney of record. |
| 6068(d) el.2–3; 6128 el.2–3 | NOT SHOWN [F] | SP-0532 (¶¶7–8, Ex. 4, Ex. 7 read) | ¶7: "Later that same day, Petitioner served her PDD" (6/17/2024). Ex. 4: "Sent: Tuesday, June 18, 2024 12:12 PM". DIFFERS by one day. ¶8: "On June 23, 2024, Respondent emailed both Mr. Jacobson and myself confirming receipt of Petitioner's PDD." Ex. 7 as filed: "Her disclosure is a joke. It's our kids savings accounts." That email is not in halsey2005@gmail.com, which holds only part of that address's June 2024 mail, so its absence proves nothing either way. Knowledge is NOT SHOWN. |
| Spiegel's knowledge of the 529 accounts (L-57) | ACCOUNT-ONLY | L-57; SP-0390 ¶5 | "'how should we divide the Vanguard fund.'" / ¶5: "I responded that Petitioner had no interest in the 529 accounts." |

**GAPS (e)**

| # | Missing fact | Who holds it | Lawful way to obtain it |
|---|---|---|---|
| e-1 | Whether the accounts first listed on 2/24/2025 (WF x1074, x1530, x4249, x4215 and x5631; Fidelity x3347; four policies) existed in Petitioner's name or control on 6/17/2024. Lead: the mediator's 8/13/2024 email names "the 1074 account" (SP-2865; only its first 400 characters were read). | Wells Fargo; Fidelity; the insurers; Petitioner | **FAM** (a § 2107(b)(1) motion or discovery; rule 5.12(b)); **SUBP** (D-66); **H** (read SP-2865 in full) |
| e-2 | A written agreement or court order extending the 60-day PDD deadline | The parties; the mediator's file; LASC | **H**; **SUBP**; **CLK** |
| e-3 | Whether a return filed within two years before 6/18/2024 (e.g. 2022) was left out of the PDD; and whether the copy served matches the copy read (Provinziano's file copy) | Petitioner; Provinziano | **FAM**; **H** |
| e-4 | Whether the 6/18/2024 email reached halsey@minorventures.com | Halsey; the firm | **H** (Q-H6); **SUBP**. The court has already found service proven (SP-0658), so the route is the family court or the appeal (Q-H8). |
| e-5 | Whether the 2/24/2025 FL-142 is a § 2104(d) amendment, and whether its POS was filed | LASC | **CLK** |
| e-6 | What Spiegel knew of the PDD's contents (for BPC 6068(d)/6128(a)) | The firm; Provinziano (L-57; the privilege is Halsey's) | **SUBP**; **H** |
| e-7 | The firm's 11/18/2024 letter, sent 21 days after his 10/28/2024 request that set a 21-day deadline (19340b0eb2056651, SP-0185; attachment drive:1Sr6fgmUNqhXhplaaBnFOwlwMuwfGRWge, not read) | Halsey | **H** (open it) |
| e-8 | The "promised upfront" initial financial statement | Halsey's contemporaneous notes | **H** (Q-H11) |
| e-9 | The discovery date for the FAM 2122 one-year limits | Halsey | **H** |

**FORUM NOTE (e).**
- The forum for FAM 2107 and 2122 is the family court. FAM 2121(a): "the court may, on any terms that may be just, relieve a spouse from a judgment … adjudicating support or division of property, after the six-month time limit of Section 473 of the Code of Civil Procedure has run, based on the grounds, and within the time limits, provided in this chapter."
- FAM 2104(a): perjury on the PDD "may be grounds for setting aside the judgment … in addition to any and all other remedies, civil or criminal".
- The jurisdiction file has no family-court intake line. Its P3 row (a sworn LASC declaration alleged false) reads: "for a filing at 111 N. Hill St., **LAPD Central Division** [1.5]" and JSID [2.3].
- State Bar [4.4]: "provides appropriate deference to civil or criminal court resolution of issues."
- The 4/21/2026 compel order stands (SP-0658); the appeal is in default (SP-3433).

---

### (f) Concert with court or police

**Entries:** L-59, L-60 and L-61. Cross-tagged: L-71. Context records X-07, X-08 and X-09.

**F1 · PC 182**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 "two or more persons" | NOT SHOWN | SP-0221 ¶7; SP-1221; SP-3005 (not read at source); SP-3487 | BEHAVIOR_f: "No document read shows a communication sent by Spiegel or anyone at ysfamilylaw.com to BHPD, the City of Beverly Hills, or the LA District Attorney, or one sent by any of them to Spiegel or his firm." BHPD, 10/9/2026, item 6: "The Department has identified records responsive to this part of the request, however, such communications are exempt from disclosure pursuant to Government Code section 7923.600." The answer does not say whom the records concern. |
| el.2 "conspire" | NOT SHOWN | — | — |
| el.3 Object: (a)(1) "To commit any crime."; (a)(2) "to procure another to be charged or arrested"; (a)(5) "to pervert or obstruct justice" | NOT SHOWN; ACCOUNT-ONLY for L-61 [F] | SP-0549; SP-0469 | "Lance obtained my confidential 567-page police report (only Detective Kale should have this)". Kalé: "That document has not been compromised at all." |
| el.4 Overt act | NOT SHOWN as an act of any agreement | SP-0221 ¶7 | "A copy of correspondence to the Beverly Hills Police Department from Respondent's counsel is attached hereto as Exhibit '18.' … My response dated April 16, 2025, is attached hereto as Exhibit '19.'" Exs. 18 and 19 were not found. |
| el.5 Venue | n/a | — | — |

**F2 · BPC 6128(a), "collusion"**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 | SHOWN | SP-0712 | Attorney of record. |
| el.2 "collusion" | NOT SHOWN | — | — |
| el.3 Intent | NOT SHOWN | — | — |

**F3 · Concert with the court** (no LAW element)

| Fact | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| Any off-record contact between Spiegel and the court | NOT SHOWN | — | No document shows any. |
| Jolie v. Superior Court | context only | SP-0024 | A finding about a private judge in other matters. Never evidence here. |
| Provinziano's letter of 4/17/2025, §V | SHOWN (as his office describes it) | SP-3030 (§V read); SP-3036 | "our office received a communication from opposing counsel, Lance Spiegel, asserting that attorney-client confidentiality has been waived … He has indicated an intent to depose me personally." BEHAVIOR_f: "none says it was sent to the police". |

**GAPS (f)**

| # | Missing fact | Who holds it | Lawful way to obtain it |
|---|---|---|---|
| f-1 | Whom the withheld item-6 records concern; the item-5(d) records (Kalé ↔ Spiegel, Shannon or their representatives); the item-13(b) intake records | City/BHPD | **PRA** PD-2026-677. Front 4 owns it (D-66; R-6, pointer only); the next update is due "by 6 Nov 2026". |
| f-2 | Exhibits 18 and 19 of the 4/18/2025 declaration | LASC; Halsey's served copy | **CLK**; **H** (OPEN_REQUESTS Part B row (f)) |
| f-3 | How Spiegel obtained Ex. 18, and any ruling on the 5/7/2025 objection ("Lacks foundation (Evid. Code § 400, et seq)") | The firm; LASC | **SUBP**; **CLK**; **CSR** |
| f-4 | The 1/29/2026 DA hold request (SP-0494, not read) and Kalé's messages to Provinziano's office (SP-3005, not read at source) | Halsey; Provinziano | **H** |
| f-5 | What BHPD sent to the DA (ECE #719953) | DA; BHPD | Front 4 (D-66), pointer only |

**FORUM NOTE (f).**
- For conduct by attorneys and by law-enforcement personnel: "The District Attorney's Justice System Integrity Division (JSID) investigates and prosecutes criminal conduct by persons who work within the justice system in Los Angeles County, including attorneys, judges, court employees and law enforcement personnel." [2.3]
- BHPD's own records are the subject of f-1. Replies from beverlyhills.org and da.lacounty.gov are caught by the existing routines (COLLISION_GATE).
- State Bar [4.1]: "Refer criminal conduct to law enforcement".

---

### (g) The Ally restriction and the writs

**Entries:** L-62 is DOCUMENTED; L-63 and L-64 are ACCOUNT. Cross-tagged: L-15 (the 2024 Ally subpoenas) and L-77.

**No criminal provision in LAW/ fits the record.**
- The writs are court process, issued by the clerk on an entered order.
- The levy is known only from Halsey's account, Schwenke's statement, and a screenshot inside an AI-drafted package.
- The enforcement statutes printed on the form (CCP §§ 699.520, 712.010, 715.010) and the notice-of-levy rules are not in LAW/.

**G1 · The record**

| Fact | Status | Pointers | Operative words |
|---|---|---|---|
| Three writs were issued on 4/28/2026 on Petitioner's applications | SHOWN | SP-3373, SP-3374, SP-3375 (read in full); SP-0712 | "Writ - Execution Los Angeles - $21,857.00 Spousal Support based on Order 5/12/2025 - Issued 4/28/2026"; "Date: 4/28/2026 Clerk, by /s/ L. Murillo , Deputy"; requester "LANCE S. SPIEGEL [SBN 51625]". |
| The judgment date entered on the writs, compared with the register | SHOWN (DIFFERS) | SP-3373–SP-3375; SP-0712 | EJ-130: "Judgment entered on (date): 05/12/2025". Register: "10/23/2024 — Judgment"; the writ lines read "based on Order 5/12/2025". |
| A levy was served on Ally, and by whom | ACCOUNT-ONLY / AI-LEAD-ONLY | SP-3448; SP-0776; SP-1426 / SP-1416 (an AI-drafted package; ALLY notes: "This is not an Ally document.") | Schwenke: "Lance had writs issued and levied your bank accounts." The screenshot (AI-LEAD): "Ally Bank received a Notice of Levy from Young, Spiegel and Hosp LLP". |
| The amount and date restrained | ACCOUNT-ONLY | SP-0776 | "$4,156.66 restrained on August 6, 2026 across my accounts ending 0942 and 9376, associated with LASD file 2026069969" |
| Ally's referral to Spiegel's office | ACCOUNT-ONLY | SP-3429; L-64 | "My bank has informed me that my accounts are restricted and specifically directed me to your office". |
| A reply from the firm | NOT SHOWN | BEHAVIOR_g §C | None was found from 2026-08-06 to 11-01. |
| A link between the 2024 subpoenas and the 2026 restriction | NOT SHOWN | SP-0180; SP-2706 (ALLY notes §2b) | "Records Subpoenaed from Ally Bank Account No.: xxxxxx0942, xxxxxx9376, xxxxxx0931" (11/27/2024). |

**G2 · What would have to be shown**

| Provision | What would have to be shown | The record now |
|---|---|---|
| PC 118 / PC 132 | A writ application ("Application - Issue Writ E/P/S") stating, under oath, a material matter known to be false (the amounts due, the judgment date, the debtor's address); or a paper offered as genuine, known to be altered | The application text was not read. EJ-130 item 18 gives totals of "$29,237.14", "$10,206.29" and "$7,657.87"; their basis is NOT SHOWN. |
| BPC 6128(a) | Deceit "with intent to deceive the court or any party" in obtaining or serving the writs or the levy | NOT SHOWN. Ally is not a party. |
| Civil (not in LAW/) | A claim of exemption; a motion on the writs; the levying officer's file | Not in LAW/. |

**GAPS (g)**

| # | Missing fact | Who holds it | Lawful way to obtain it |
|---|---|---|---|
| g-1 | The Notices of Levy received on 7/29 and 8/5/2026, who served them, and the levying officer | Ally; LASD | **H**: R-16 (the LASD levy file 2026069969; open since 2026-10-29); R-7 and R-17 (owned by the financial thread; pointers); Q-H7(c) |
| g-2 | Ally's 9/4/2026 secure message: the stated authority for the restriction (the link expires 2026-12-03) | Halsey | **H** (Q-H7(a)) |
| g-3 | Who at Ally named Spiegel's office, and when | Ally (call record; ECR 64504079 / 65504572) | R-7 (pointer); Q-H7(b) |
| g-4 | The writ applications and the 5/12/2025 order | LASC | **CLK** |
| g-5 | Why the EJ-130 says "05/12/2025" where the register's Judgment is dated 10/23/2024 | LASC | **CLK**; **FAM** |

**FORUM NOTE (g).**
- The jurisdiction file's P4 row: "Regulators in the sources' complaint routes (not police): **Federal Reserve** … **CFPB** … **Utah DFI** for state banks … **FDIC** is the insurer". [5.8]: "No source retrieved says whether a bank's restriction of a customer's accounts is, or is not, a matter for the police, and none addresses a bank referring a customer by telephone to an attorney's office."
- Questions about the writs go to the issuing court. The Ally rows are owned by the financial thread.

---

### (h) Other

**Entries:** L-65…L-77. The guardrails for Halsey's own acts are in §5.

**H1 · PC 118 — Spiegel's own declarations**

The declarations: D1 of 12/2x/2025 (SP-0387, read in full); File A of 12/29/2025 (SP-0390, read in full); File B of 12/30/2025 (SP-0395, a copy of SP-0397, read in full); D4 of 2/24/2026 (SP-0532, partial); and D17/D18 of 2/2/2026 (SP-1791/SP-1574, p4 read).

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Actor | SHOWN | SP-0387, SP-0390, SP-0397, SP-0532 | "LANCE S. SPIEGEL" |
| el.2 Penalty of perjury | SHOWN | SP-0390; SP-0397 | "I declare under penalty of perjury of the laws of the State of California that the foregoing is true and correct". SPIEGEL_DECLARATIONS: "each signed by Spiegel under penalty of perjury". |
| el.3 "states as true" | SHOWN | each | The statements in the rows below. |
| el.4 "any material matter" | NOT SHOWN (the dating slips) | SP-0659 | The court relied on ¶12's retention and "Janine" statements: "According to a sworn declaration from counsel Lance Spiegel, the email correspondence did not in fact occur … counsel has declared that he never had any assistant named Janine". No document shows either statement untrue. |
| el.5: the four dating slips in L-75 | PARTLY (each difference sits beside the declaration's own exhibits; knowledge NOT SHOWN) | SP-0390 | (1) ¶7 "Later that same day" (6/17/2024) against Ex. 4 "Sent: Tuesday, June 18, 2024 12:12 PM". (2) ¶11 "Since entry of Judgment, on October 23, 2025" against ¶10 and Ex. 9, "October 23, 2024". (3) ¶11.A "dated February 7, 2025" against the FL-142's "FEBRUARY 24, 2025". (4) ¶11.B "January 1, 2025" against the FL-150 signed 1/7/2025 and filed 1/8/2025. |
| el.5: L-58 (2/24/2026 ¶7) | PARTLY | SP-0532 | The same 6/17 / 6/18 difference. |
| el.5: L-76 ¶2, "links" | PARTLY | SP-0397 | "include direct "links" to webpages", against Ex. 2's "[link]" and "[link to a generic financial literacy website]"; no URL appears. |
| el.5: L-74 ¶3.A, "evading personal service" | NOT SHOWN | SP-0387; SP-0712; SP-0869 (pp.2–7 not read) | The register shows "Request to Continue and Reissue TRO (Form 115)" (Respondent, 7/14/2025) before the 7/16/2025 continuance. Whose request the 8/6 and 8/27 continuances were is not stated. No DVRO POS or non-service return is in the corpus. |
| el.5: L-74 ¶3.B, "criminal extortion" and "admonished by the Court" | NOT SHOWN | SP-0387 | No court finding of extortion and no admonishment appears in any minute order read. The transcripts were not read. See §5 (G-1, G-2). |
| el.5: D1 ¶2 against its execution day | PARTLY (the order of dates is documented; the day digit is uncertain) | SP-0387 | p11 ¶2: "On December 26, 2025, Petitioner served Petitioner's Objections …". p13: "Executed December 2[?], 2025 at Beverly Hills, California." The reader: "The second glyph resembles a "4" … (it could be read as "5")". Either reading is before 12/26. |
| el.5: other year slips | PARTLY | SP-1791 / SP-1574 p4; SP-0532 ¶13 | "Executed February 2, 2025 [sic], at Los Angeles, California." / "on January 5, 2025 [sic]". |
| el.6 "willfully" | NOT SHOWN | — | — |
| el.7 Place | SHOWN | SP-0390; SP-0397; SP-0387 | "Executed December 29, 2025 at Los Angeles, California."; "… at Beverly Hills, California." |
| el.8 Proof limitation | n/a | — | Falsity is not shown. The contrasts are documentary (his own exhibits; the register). |

**H2 · BPC 6068(d)**

| Element | Status | Pointers | Operative words / missing fact |
|---|---|---|---|
| el.1 Attorney | SHOWN | SP-0712 | — |
| el.2 Means "consistent with truth" | NOT SHOWN | — | — |
| el.3 "never to seek to mislead the judge … by an artifice or false statement of fact": (ii) the judge is the target; (iii) the statement differs; (i) "seek to mislead" | PARTLY | SP-0659; H1 rows | The declarations were filed and relied on (SP-0659). The date differences are as in H1. That he sought to mislead is NOT SHOWN. |

**H3 · BPC 6128(a):** el.1 SHOWN (SP-0712); el.2 and el.3 NOT SHOWN.

**H4 · (h) entries with no LAW element on their face:**
- L-65, L-66 and L-70 (advice to retain counsel: SP-0099, SP-0100, SP-0140).
- L-69 (the extension ended: SP-0221, Ex. 14).
- L-71 (privilege waiver and deposition: SP-3030).
- L-72, "Criminal Extortion under California law." (SP-0268, read in full).
- L-73, the continuance replies. The first, SP-0277 (1980aad41bcc7b22), is now quoted at source (ASKS_TO_FIRM_2025_2026 §3a). The second, SP-0278, has not been read at source.
- L-77, "We intend to enforce the court's order" (SP-0702).
- L-67, "$550,000 … used to pay Spiegel" — ACCOUNT. State Bar 7/24/2024 (SP-0147): "does not present sufficient facts to support an investigation".
- L-68, the call to his counsel — ACCOUNT. A billing lead only.

**GAPS (h)**

| # | Missing fact | Who holds it | Lawful way to obtain it |
|---|---|---|---|
| h-1 | Materiality: whether any ruling turned on a misdated item | LASC; the court reporter | **CLK**; **CSR** |
| h-2 | Knowledge: whether the declarant knew the correct dates when signing (the correct date sits in his own exhibits: Ex. 4, Ex. 6, Ex. 9) | The firm (drafts, file) | **SUBP** |
| h-3 | The handwritten execution day on D1 p13 | LASC; the printed original (CCP 1010.6(e)(2)(B)(i)) | **CLK**; a party's request in the case |
| h-4 | The reasons for the DVRO continuances of 7/16, 8/6 and 8/27/2025, and any "admonished" remarks | LASC; the court reporter | **CLK**; **CSR** |
| h-5 | Whether a firm employee was known as "Janine". Halsey, 4/22/2026: "Yes Lance she has 2 names same person" (SP-0672, not re-opened). [F] — EV-003 rests on ¶12. | The firm; Halsey (to say who) | **SUBP**; **H** |
| h-6 | Pp. 2–7 of the 11/14/2025 Declaration re Non-Service (SP-0869) | Halsey's Drive; LASC | **H**; **CLK** |
| h-7 | Spiegel's second 7/14/2025 reply (SP-0278), and items 4–5 of Halsey's 7/14/2025 letter (G-2), read at source | Halsey's mailbox | **H** |

**FORUM NOTE (h).**
- The P3 row: "for a filing at 111 N. Hill St., **LAPD Central Division** [1.5]; for the place where the declaration was signed, the agency serving that address".
- D1 was "Executed … at Beverly Hills, California". If that was at 301 N. Canon, the agency is BHPD [1.1–1.4].
- Files A and B were "Executed … at Los Angeles, California"; no address is stated.
- PEN 118: "This subdivision is applicable whether the statement … is made or subscribed within or without the State of California." [3.2]
- JSID [2.3].
- State Bar (SP-0689): "If that court were to find any impropriety by the lawyer, please forward such written findings to our office for review."
- The §271 amount "is reserved to the time of trial" (SP-0659).

---

## 5. GUARDRAILS — PC 518 / 519 / 523 / 524 × Halsey's documented acts

**These rows protect Halsey.** They record words he sent, verbatim, together with what the record does not show. They are not findings, and nothing here characterizes him.

The guardrail file:
- "§ 519(2) contains no exception for a person who is a crime victim and no qualifier such as "false" or "falsely"."
- "NOT addressed on the official pages … whether a demand tied to the victim's own loss (return of property, repayment, compensation) is "wrongful" or an "intent to extort"."

Spiegel raised the subject in writing on 2025-06-23 (SP-0268): "Criminal Extortion under California law."

**5.1 · The acts** (ledger G-0…G-10, plus items surfaced in this pass)

| G | Date | Reached | Words of a §519 kind (verbatim) | Words of a request (verbatim) | Pointer / read |
|---|---|---|---|---|---|
| G-0 | 2024-01-31 (sent 2024-02-01T02:57:22Z) | AnnaK@, cc lances@ | "I would be obliged to report such unauthorized removal of company property to the authorities under normal circumstances." | "I need a thorough accounting of all funds." | SP-2816 (read in full: ASKS_TO_FIRM_2024); the sentence as quoted in SP-0100 |
| G-1 | 2025-06-23T20:25:58Z | lances@ | "The criminal court is beyond my control, and I am offering nothing more than an opportunity to return what has been taken without threatening prosecution." | "The misappropriated funds for a "college" fund can be given back and should be." | SP-0269 (read in full) |
| G-2 | 2025-07-14 | lances@ | Item 4: "Felony complaints for grand theft, attempted murder, and attempted insurance fraud are actively under investigation. I have no power to influence or discontinue that inquiry, and nothing in this letter is intended—or could be construed—as leverage regarding it." | "Withdraw the current DVRO." / "Please advise by July 21st 2025 whether Ms. Minor will accept this resolution." (read at source: ASKS_TO_FIRM_2025_2026 TSV row 49). Item 5: "If the 529 is not re-titled within 20 days, I will instruct civil counsel…" | SP-3100 (the proposal items read at source); items 4–5 not read at source (via 85_V3/81B) |
| G-3 | 2026-01-05 | lances@ and other firm addresses | Subject: "FORMAL NOTICE: Criminal Spoliation of Evidence, Internal Leakage, and Demand for Preservation" | "Demand for Preservation" (subject) | SP-0433 (not opened) |
| G-4 | 2026-02-25T01:20:51Z | City/BHPD + lances@, AnnaK@ | "Technically, only Alex Kale knows how this is possible…at this moment." | none in the text quoted | SP-0538 (AI-LEAD carrier; body read) |
| G-5 | 2026-02-28T10:20:38Z | 17 To, including lances@, + 4 Bcc | "CRIMINAL COMPLAINT AND REQUEST FOR ARREST WARRANT FOR LANCE SPIEGEL"; "FILING DEADLINE CONTEXT: Pre-emptive filing before March 2, 2026 court ruling"; "Pre-March 2, 2026 Filing Creates Checkmate" | "I need a safe, mutually agreed way to deliver evidence collected meticulously over 365 days." | SP-0549 (read in full) |
| G-6 | 2026-03-01T02:30:34Z | shannonmimor@gmail.com (as shown) | "your situation was creating more and more attention, Federal attention."; "when he had broken so many laws to get it" | "I just needed Lance to not want the TRO"; "He has very likely destroyed your life when offered an off ramp."; "Exactly why I offered it." | SP-0555 (read in full) |
| G-7 | 2026-03-29/30 | DA and federal addresses; Cc/Bcc shannonminor@ | "Preserved Evidence of Premeditated Murder Never Retrieved — Immediate Subpoena Required" | "Marsy's Law Demand — Victim Right to Confer…" (to the DA) | SP-0601, SP-0602 (read in full) |
| G-8 | 2026-04-20T15:52:53Z | DA + federal (not Spiegel, not Shannon) | "A sanctions hearing premised on this evidence destruction is scheduled for April 24, 2026 — four days from today." | — | SP-0649 (register metadata-only) |
| G-9 | 2026-04-22T22:50:29Z | shannonminor@, replying to "You have not paid a dime of support…" | "I alerted them to the fraud that was coming and the da as well." / "Lance will be hearing soon." | none from him; the money demand in the thread is hers | SP-0674 (checked at source per the ledger) |
| G-10 | 2026-08-08T00:36:58Z / 00:47:54Z | lances@ (+ 12 Bcc) | none | "Please confirm immediately whether you, your firm, Shannon Minor, or anyone acting at your or your client's direction requested, procured, transmitted, served, or otherwise caused this restriction." | SP-3429, SP-3430 (read in full) |
| G-x1 | 2024-03-20T15:32:27Z | lances@; shannonminor@ | "I am prepared to waive pressing charges for the funds unlawly taken." | "I am open to and indeed prefer the route of mediation, offering transparency with my financials" | SP-2836 (read in full: FIRST_CONVERSATIONS §2; not in the ledger's G-list) |
| G-x2 | 2024-10-22T15:08:09Z | lances@, cc shannonminor@ and others | None of the five §519 kinds appears in its words. The consequence it names is a subpoena: "I am not forced to issue the upcoming subpoena" | "You now have a choice: waste significant amounts of money to eventually provide what the state already mandates, or comply with the law and allow these funds to address the urgent mental health crisis in the family" | SP-2896 (read in full: ASKS_TO_FIRM_2024) |
| G-x3 | 2026-03-27 | LASC filing, served on the firm | Decl. ¶10: "I have filed a criminal referral regarding the conduct of Petitioner's counsel in connection with this matter." | — (filed in opposition to the §271 RFO) | SP-0590 (pp.1–3 read in full) |
| G-x4 | 2026-01-11 | City officials | A settlement demand addressed to the City. It concerns neither Spiegel nor Shannon, and the ledger does not quote it. | — | Ledger, "Outside this ledger's subject" |

**5.2 · Element by element: what the record shows and does not show**

| Provision / element | The record shows | The record does not show |
|---|---|---|
| PC 518 el.1: "the obtaining of property or other consideration from another, with his or her consent" | No document shows that anything was obtained from Spiegel, his firm or Shannon after any G-item. G-6 speaks of an "off ramp" "offered" and refused: "Twice he answered "no"." | What the "off ramp" was, or when and in what writing it was offered. No such writing is in the record read. |
| PC 518 el.2: "induced by a wrongful use of force or fear" | No response induced by fear is recorded. | "wrongful" is not defined in the text. |
| PC 518 el.3: "consideration" "means anything of value" | The requests on the record are for: an accounting or records (G-0, G-x2); the return or re-titling of the 529 funds (G-1, G-2); withdrawal of the DVRO/TRO (G-2, G-6); a way to deliver evidence (G-5); an explanation of the restriction (G-10). | Whether the withdrawal of a court request is "anything of value" is not addressed on the official pages. |
| PC 519, type 2: "To accuse the individual threatened … of a crime" | Words of accusation reached Spiegel or the firm (G-3, G-4, G-5) and Shannon (G-6, G-7, G-9). | — |
| PC 519, type 3: "To expose, or to impute … a deformity, disgrace, or crime" | G-0 ("report … to the authorities"); G-1 ("prosecution"); G-2 item 4; G-6 ("Federal attention"); G-9 ("Lance will be hearing soon"); G-x1 ("waive pressing charges"); G-x3 (a referral, in a filing). | — |
| PC 519, types 1, 4 and 5 (injury, secret, immigration) | None appears in any G-item quoted. | — |
| PC 523 el.1: "with intent to extort property or other consideration from another" | No document states such an intent. G-2 item 4 states the opposite: "nothing in this letter is intended—or could be construed—as leverage regarding it." | Intent, either way. |
| PC 523 el.2: "sends or delivers to any person any letter or other writing" | Every G-item is a writing that was sent; G-x3 is a filing. | The text does not say whether e-mail is a "letter or other writing"; this is not addressed on the official page. |
| PC 523 el.3: "expressing or implying, or adapted to imply, any threat such as is specified in Section 519" | In G-1, G-2, G-6 and G-x1, words about crime or prosecution and words of a request appear in the same writing (above). | A statement that a report will be made, withdrawn or withheld in exchange for the request. G-2 disclaims it; G-x1 offers to waive charges. |
| PC 524 el.2–4: "attempts, by means of any threat … to extort property or other consideration" | No document records an attempt to obtain property by a threat. | — |

**5.3 · Going forward: never** (the charter's rules, applied to these words)
1. Never send a report, complaint, accusation or referral about a crime, or a copy of one, to Spiegel, his firm, Shannon Minor or her family (G-3, G-4, G-5, G-6, G-7; the Bcc pattern in G-10). The charter: "no communication with Spiegel, his firm, Shannon Minor or her family about any report or behavior".
2. Never put words about police, the DA, the Bar, prosecution, charges, "authorities" or "federal attention" in the same writing as any request for money, property, records, the 529 funds, a TRO/DVRO withdrawal, a settlement term or an "off ramp" (G-0, G-1, G-2, G-6, G-x1).
3. Never offer to waive, withdraw, delay or not press criminal charges for anything (G-x1). Never write that a report could be avoided (G-6).
4. Never tie a report's timing to a family-court date in any writing ("Pre-emptive filing before March 2, 2026 court ruling"; "Checkmate"; G-8 "four days from today").
5. Keep civil asks (disclosure, accounts, levy records) inside the court process and with counsel, with no reference to any report. The charter: "nothing ever links criminal reporting to any demand, settlement or position in the family or civil cases". In a family-court filing, say nothing about a criminal referral (G-x3).
6. Make one report to one agency, the one with jurisdiction; never use mass lists (G-5: 17 To and 4 Bcc; G-7).
7. Never answer a money demand with references to complaints (G-9).

---

## 6. ELEMENT COVERAGE AT A GLANCE

The figures count elements as **SHOWN / total (+PARTLY)**. The SHOWN elements are mostly formal ones (actor, oath, statement, place).

| Behavior | Provision | Shown / total | Single most important missing fact |
|---|---|---|---|
| (a) | PC 502(c) | 0/7 (+2) | Who accessed the account: Google server-side session, IP, device and deletion records (Q-F3); the Workspace create event for the 2025-09-24 document (Q-H2) |
| (a) | PC 134 | 1/4 (+1) | The one SHOWN element is EV-003's finding that Exhibit F was not authentic. Missing: who or what created the document. |
| (a) | PC 135 / PC 182 / PC 132 (L-04) | 0/4 (+1) / 0/5 / 0/6 | Actor; a second person; the email read in court |
| (b) | PC 502(c)(2) | 0/7 | One filing that used a fact then existing only in his private channels (Q-H3) |
| (b) | PC 182 (L-09) | 0/5 | Any record of the mediator's file or a payment |
| (c) | PC 118 (POS) | 4/8 (+1) | Which paper travelled in which envelope, matched to its POS (Q-H4), with the USPS scans |
| (c) | PC 132 | 3/6 (+1) | The two 12/30/2025 POS (D24 Exs. A and B), and any showing that they were ante-dated |
| (c) | PC 134 / PC 127 | 2/4 / 2/5 | Falsity, and any instruction to a declarant |
| (c) | BPC 6128(a) / 6068(d) | 1/3 / 1/3 | Deceit and intent |
| (c) | CCP 415.30 (civil) | 4/7 | el.5 is SHOWN: the summons was completed on 3/8/2024 by Halsey's executed acknowledgment |
| (c) | CCP 1013b (civil) | 3/4 (+1) | The signing procedure behind the script-font names |
| (d) | CRC 2.251 | 2/6 (+2) | Whether any consent exists outside the records read (his provider's terms; the court file) |
| (d) | CCP 1010.6(c) consent | 2/5 | No consent document is in the record read, and no criminal provision applies |
| (d) | CCP 473(d) | 0/4 | Any motion, and a void order |
| (e) | FAM 2104 | 3/8 (+4) | Whether the accounts first listed on 2/24/2025 existed in Petitioner's name on 6/17/2024 |
| (e) | FAM 2105(d) / 2106 | 7/8 (+1) / 1/1 | That the representations on the FL-144 were untrue. They are shown as representations only. |
| (e) | FAM 2107 / 2121 / 2122 | 1/5 (+1) / 3/5 / 0/6 | A set-aside ground and its discovery date |
| (e) | PC 118 (FL-141) | 3/8 (+1) | Materiality and knowledge |
| (e) | BPC 6068(d) / 6128(a) | 1/3 / 1/3 | What Spiegel knew of the PDD's contents |
| (f) | PC 182 | 0/5 | Whom BHPD's withheld item-6 records concern (PRA, R-6); Exhibits 18–19 |
| (f) | BPC 6128(a) | 1/3 | The same |
| (g) | — (no criminal provision fits) | — | The Notices of Levy and who served them (R-16, R-17; Q-H7) |
| (h) | PC 118 (Spiegel's declarations) | 4/8 (+1) | Materiality and knowledge of the date differences |
| (h) | BPC 6068(d) / 6128(a) | 1/3 (+1) / 1/3 | That he sought to mislead |

---

## 7. LEDGER ENTRIES FOUND INTERNALLY INCONSISTENT, OR CONTRADICTED BY NOTES IN THE SAME FOLDER

1. **L-10 and L-12** say no signed acknowledgment is shown ("a signed acknowledgment returned by Halsey"; "who signed the acknowledgment and when"). FIRST_CONVERSATIONS §3, which was in READING_NOTES at 03:47, before the ledger's 03:53 save, shows the opposite:
   - Halsey returned the signed NAR on 2024-03-08T07:32:29Z: "Accepted March 7, 11:31 PM Pacific Time" (SP-2835).
   - The NOAR was filed "3/8/2024 12:24 PM" (attached to SP-0144).
   - FL-180: "The court acquired jurisdiction of the respondent on (date): 3/8/24".
2. **L-01** says "15/17 verified … That is, 15 of its 17 emails are absent from the live account." The JURISDICTION_SPLIT notes (observation 2) record that 85_V3 marks "15 verified absent, 2 verified present, 3 undated" as SUPERSEDED, and gives the current state as "17 listed → 12 verified absent, 2 verified present (false positives, disclosed first), 3 undated/untestable".
3. **L-62's heading**, "issued on the judgment of 5/12/2025", conflicts with the register, which records "10/23/2024 — Judgment" and writ lines "based on Order 5/12/2025". L-75 itself records ¶10 and Ex. 9 giving October 23, 2024. The EJ-130 forms do print "05/12/2025". The difference is real, but the ledger does not flag it.
4. **L-74** quotes "Executed December 24, 2025" as verbatim. Its source (BEHAVIOR_c §2.2, D1 p13) reads "Executed December 2[?], 2025", handwritten, with a second glyph that "resembles a "4" … (it could be read as "5")". The same declaration's ¶2 states service "On December 26, 2025". The ledger does not record that sequence.
5. **EV-108** is listed in "How to read this ledger" as AI material, yet its register primary SP-0397 is the §271 RFO itself (COURT, read in full). L-76 rests on the same filing (drive:1MZDYige…, SP-0395, a copy of SP-0397).
6. **L-73 (DOCUMENTED) and G-2/L-09 (verbatim quotations)** rest on 7/14/2025 messages that no thread reader had opened when the ledger was written. Their text came from 81B (AI-LEAD) and 85_V3 (WORK-PRODUCT).
   - Since then, the first reply (SP-0277) and the letter's proposal items (SP-3100) have been read at source (ASKS_TO_FIRM_2025_2026, 04:11).
   - The second reply (SP-0278) and items 4–5 of the letter are still not read at source. L-23's quotations also come via 85_V3.
7. **L-81 is DOCUMENTED**, but its only record is a reader's transcript of a live page. The ledger itself quotes that note's limit: "a reader's transcript, which is AI work and so not evidence in itself". The register classes SP-3513 as ACCOUNT.
8. **X-04** calls Exhibit C p.14 a Google Legal Support "Delivery Status Notification (Failure)". GOOGLE_NOTICES §2 shows that the DSN header is the thread's first message, a bounce from mayorandcitycouncil@beverlyhills.com; this is the coordinator's correction.
9. **L-29** cites EV-005 as drive:1qWjh1R2…. The register holds that file as SP-0560, an unverified same-size copy (metadata-only). EV-005's primary is SP-0559.

---

## Appendix A — SP-ids whose register status lags a full read, or that are cited but not read at source

| SP-id(s) | Register status | Where the read is recorded |
|---|---|---|
| SP-0029, SP-0074, SP-0075, SP-0078, SP-0079, SP-0080–SP-0083 (EV-049/050/051) | not-read | Read in full: GOOGLE_NOTICES §1 |
| SP-0042–SP-0046 (thread 18461348b9fe0954) | not-read | GOOGLE_NOTICES §4: all 5 returned |
| SP-0337, SP-0338 (EV-052); SP-0379 (EV-053); SP-0472 | not-read / metadata-only | Read in full: GOOGLE_NOTICES §1–§3 |
| SP-0091, SP-0094; and gmail 18cf83d7742fd195, 18d12e3cc70ee998, 18d4096c9993218d (no register rows) | not-read / absent | Read in full: FIRST_CONVERSATIONS §3 |
| SP-0096 (attachments), SP-0097, SP-0099, SP-0100, SP-0102, SP-0144, SP-0157, SP-2816–SP-2822, SP-2830, SP-2835, SP-2836 | partial / metadata-only | Read in full: FIRST_CONVERSATIONS §0–§4; ASKS_TO_FIRM_2024 §2 |
| SP-2896, SP-2905 | metadata-only | Read in full: ASKS_TO_FIRM_2024 |
| SP-3100, SP-3160, SP-0277, SP-0261 | metadata-only | ASKS_TO_FIRM_2025_2026 (TSV row 49; §1a; §3a) |
| SP-0276, SP-0278 | not-read / metadata-only | **Not read at source** |
| SP-0282, SP-0284, SP-0459, SP-0547, SP-0649, SP-0674 | not-read / metadata-only | Quoted by the ledger: SP-0284, SP-0547 and SP-0674 "checked at source"; the others through the index or notes |
| SP-0270, SP-0433, SP-0494, SP-1066, SP-3005, SP-1410 (WP) | metadata-only / not-read | **Not read** |
| SP-2527, SP-2706 (Ally subpoena returns) | DUPLICATE, metadata-only | Read in part: ALLY notes §2a–§2b |
| SP-1426 / SP-1416 (Ally package) | ACCOUNT, provisional, unopened | ALLY notes §1: "This is not an Ally document." The ledger treats it as AI-LEAD. |
| SP-0221, SP-0532, SP-0590, SP-0199, SP-0160 | partial / full (message body only) | The parts relied on were read: ¶7 and Exs. 9–14; ¶¶7–8, ¶13, Exs. 1, 4 and 7; pp. 1–3; pp. 1–4 + POS; attachment pp. 1, 2, 5, 6, 7 and 9 |
| SP-0869, SP-1143, SP-1706, SP-2760, SP-1904, SP-2683, SP-1791, SP-1574, SP-1228, SP-2393, SP-1774, SP-2503, SP-1864, SP-1857, SP-0915, SP-1941, SP-2583 | partial | Each POS page was read in full: BEHAVIOR_c §2.1 |
| SP-3513 (Correos) | ACCOUNT, full | A reader's transcript of a live page; no saved capture |
