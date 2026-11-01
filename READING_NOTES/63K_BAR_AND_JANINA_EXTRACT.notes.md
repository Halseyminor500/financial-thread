# READING NOTES · 63K_BAR_AND_JANINA_EXTRACT.md

| field | value |
|---|---|
| Path @ commit | `/home/user/minor-v-minor-legal-tracker/governance/matters/04_criminal_bhpd_2025-14983/report_2026-08/63K_BAR_AND_JANINA_EXTRACT.md` @ `6f5d8b0` (6f5d8b0479c15614799a4cf371fcc6c52add0e34 = tracker HEAD) |
| sha256 | `2e1d51ec0bab4ae28578c1adf6116cde304fb1fc63412fa03cc00c9514fc763b` (working copy; identical to `git show 6f5d8b0:<path> \| sha256sum`) |
| Bytes / lines | 260,008 bytes · 6,283 lines |
| Read in full | **yes**. Lines 1–6283 were read in order with the Read tool. The only line over 2,000 characters (L4380, 2,236 chars) was re-read with `sed` to confirm it was complete. |
| Reader | Opus subagent (claude-opus-5-5), 2026-11-01 |
| File history | `git log --follow` shows one commit touching this file: `6f5d8b0` (2026-10-31 23:50:47 +0000). The file's own footer says "NOT committed (per tasking)" (L6273). |
| Evidence class | **AI-LEAD** (AGENT_RULES rule 6). Lead sheet only. Nothing in it is evidence; it points to Gmail records. |

**Repeated text, checked by diff.** The 2026-02-28 criminal complaint appears four times: L185–1510 (sent copy); L1599–2924 (2/28 forward to tw@waitt.com); L2956–4281 (3/01 forward to shannonmimor@gmail.com); L4303–5418 (as quoted inside the LA DA's 3/02 reply). Each copy was compared to copy 1 with an in-memory `diff`:
- Copy 2 is byte-identical.
- Copy 3 differs only at L3078, "evidence hold email below. **During", where L307 reads "evidence hold email. During".
- The DA-quoted copy is word-identical apart from formatting, except one word: L5283 reads "arrest warrant = custody loss" where L1369 reads "arrest warrant custody loss".

Line references below cite copy 1 unless stated otherwise.

**Interpretation of the brief's class (b).** Class (b) is "material from his accounts appearing in filings". "His" is ambiguous, so both readings were applied:
- (b1): material from Halsey's accounts appearing in Spiegel-side filings or court use.
- (b2): material from Spiegel's accounts appearing in any filing.

---

## 1. WHAT IT IS

**Its stated purpose and method (verbatim):**
- L1: "# 63K · STATE BAR CORRESPONDENCE + JANINA/JANINE IDENTITY EXTRACT"
- L3–6: "**Session:** mailbox reader, 2026-09-01. Gmail MCP, live mailbox `halsey2005@gmail.com`, read-only; every query `in:anywhere` (spam/trash included); no attachments downloaded (inventory by filename only, per tasking). Ruling D-13 governs: capture everything, grade specificity, filter nothing. Written for verbatim read-back to the client."
- L8–11, grading key: "**A** = full body captured verbatim from live mail · **B** = live-mail metadata + snippet captured, body not pulled · **C** = content sits inside an attachment this session was barred from downloading (match known only from Gmail full-text search, which indexes attachments) · **D** = inference." No item in the file is graded [D] (checked with grep).
- L13–22, caveats:
  - "(1) Gmail `search_threads` previews show only the ~5 oldest messages of a thread — every thread quoted below was re-pulled in full with `get_thread`."
  - "(2) Gmail name search is fuzzy: a search for "Janine" also returns "Janina" threads and vice-versa, and matches text inside attachments. Every occurrence claimed below was verified against a fetched body, or is explicitly graded C (attachment-level)."
  - "(3) Per the client (via coordinator, 2026-09-01): Jan/Janina's mail lives **primarily in his VIVIDLABS workspace account, which is NOT connected to this session** — plenty is nonetheless present in halsey2005@gmail.com, and this report covers only what this mailbox holds. A gap here is absence-of-access, not absence."
- L6271–6273: "*Read-only session: nothing in Gmail was sent, modified, labeled, or deleted. No attachments downloaded. Working files: session scratchpad `…/scratchpad/bar/` (thread JSONs, search pages, jq renderer). NOT committed (per tasking).*"

**Its sources:**
1. The live Gmail mailbox halsey2005@gmail.com, read through the Gmail MCP. Message and thread ids are given throughout.
2. Cross-references to tracker work product:
   - 63C / T-43: L5598, L5628, L5883, L5912
   - 63H N-12: L6178, L6180, L6182, L6189, L6190
   - 61_KALE_STATEMENT_LEDGER §7.6: L6078, L6109
   - v3_parts/qa_Q61_exhibit_F_provenance.md: L6276
   - repo T-08: L171
   - ruling D-13: L5, L6118, L6264
3. A session scratchpad `bar/`, cited for material omitted from the file (L5472, L5567, L5874, L6272). The scratchpad is not in the repository.

**Is it AI work product?** Yes. A "mailbox reader" session wrote it through the Gmail MCP (L3), using a session scratchpad and a "jq renderer" (L6272). It is a lead sheet only. Its email reproductions point to Gmail message ids, which are the primary records. No attachment was opened (L4, L6271), so every letter, PDF, filing and court order it names is unread here.

**Content the file, or its source, describes as AI-made:**
- The 2/28/26 complaint: "*This document prepared by Halsey Minor with AI assistance for legal research and document organization. All facts, timeline, and evidence assertions are my sworn statements.*" (L1507–1509)
- The 5/02/26 Bar supplementals:
  - "This report, generated by Google Gemini AI using the complete case file as input" (L5650)
  - "GEMINI AI COLLUSION ANALYSIS (graphic) Generated independently by Google Gemini AI when analyzing the case data." (L5658–5659)
  - "Generated by Google Gemini AI from raw case data." (L5748)
  - "Independently generated by Google Gemini from raw case data." (L5766)
- The 5/06/26 email: "The coloring book version created by AI and the 6-page summary created for the initial police report included, summarized over 600 pages processed by AI down to 6 pages" (L5808)
- The "Max" persona and related items:
  - "— Max (Halsey's AI assistant)" (L5928)
  - "attachment (AI-drafted declaration)" (L6081)
  - "Perplexity Prompt — Add Vocabulary Timeline to Slider HTML" (L6080)
- The Janine log:
  - "the "Janine"-named correspondence log in the client's Drive is a generated reconstruction artifact" (L6109–6110)
  - ""phantom assistant, Janine" is the language of the AI-generated log" (L6277–6278)

**The extractor's own characterizations.** These are not graded D, but they are inferential on their face:
- "Halsey concedes-and-defers to Esther Fallas 7/24/24" (L38)
- "Her reply reached Halsey as the attached closing letter (1.3, same day) or off-mailbox." (L107–108)
- "their communications reached Halsey as attached letters/phone only" (L47–48). No pointer is given for "phone".
- "The subject reads as a reply to the closing decision" … "her determination evidently arrived as the 1.15 closing-letter PDF" (L5833–5837)
- "i.e., the client himself identifies the day-before-the-motion event as **his Bar complaint filing of 4/20**" (L5917–5918). "[hearing]" in the quote at L5916 is an insertion.
- "consistent with her leaving Vivid" (L5985)
- "the client's "only other employee" description is consistent with what this mailbox holds" (L5997–5998)

**Dangling reference.** The file cites "§0" (L5947, L6129, L6229), but no heading by that name exists. The only caveat block is L13–22.

---

## 2. STATE BAR

### 2.1 The file's own summary (verbatim, L36–50)

| Bar case | filed | outcome visible in mailbox |
|---|---|---|
| **24-O-18793** (ref 224000) | 2024-06-25 online | Acknowledged 6/26/24; **closing letter 7/24/24**; Halsey concedes-and-defers to Esther Fallas 7/24/24 |
| **26-O-13820** | opened from the 2/28/26 emailed criminal complaint | Acknowledged 3/02/26; case number given 3/19/26; **closing letter 5/06/26** |
| ref **268155** | 2026-04-20 online portal | Successful-submission ack 4/20/26; supplementals 5/02 and 5/06/26 filed to complaint@ under all three numbers; no reply to any supplemental |

L42–50: "**Did the Bar ever reply?** Yes — but only: (a) automated acks (complaint@ portal receipts 6/25/24 and 4/20/26; Intake auto-reply 3/01/26), (b) OCTC do-not-reply letters as PDF attachments (ack 6/26/24; closing 7/24/24; ack 3/02/26; closing 5/06/26), and (c) **one live human exchange: Intake Dept., two replies on 2026-03-19** (quoted in full at 1.9). No inbound email exists from Esther Fallas or Lakshmi Jagannath (searched `from:` both; their communications reached Halsey as attached letters/phone only). Nothing from the Bar after 5/06/26. No reply ever to the three 5/02/26 supplemental-evidence emails, the 5/06/26 "Coloring Book" email, or the 5/06/26 email to investigator/attorney Lakshmi Jagannath."

L29: "→ **16 threads / 33 messages**"

### 2.2 Complaint 1: 24-O-18793 (portal ref 224000)

- **Filed:** 2024-06-25, online. The receipt [A], 2024-06-25 15:32Z, complaint@calbar.ca.gov, id 190503e0ad8885f5 (L52–61), says: "You have successfully submitted your Attorney Misconduct Complaint to the State Bar of California. Please keep a record of your reference number: 224000 […] While the complaint is being processed, you may sign in […] with your reference number to print and download the complaint or add additional documents to your complaint."
- **What was alleged:** the complaint's text is **not in this file**. The only description is Halsey's own 7/24/24 email, quoted below. On the subject of the complaint, it says Spiegel was compensated from property Halsey says was his sole property, "when he knew she had no known source of income".
- **What the Bar replied (verbatim):**
  - Acknowledgment, 2024-06-26 17:37Z, octcdonotreply@calbar.ca.gov, id 19055a01bc508ed6, attachment `24-O-18793 Lance Stephen Spiegel.pdf` (not downloaded): "Please see the attached Acknowledgment letter regarding your State Bar complaint." (L75)
  - Closing, 2024-07-24 15:24Z, id 190e5588b28b881b, attachment **`24-O-18793 Minor Closing Letter.pdf`** ("not downloaded — this is the 2024 CLOSING letter", L88): "Please see the attached letter regarding the above referenced State Bar matter. Thank you." (L94)
  - Survey, 2024-08-14, no.reply@calbar.ca.gov, id 191520d1b41ce456: "The State Bar of California recently sent you a closing letter regarding a complaint that you filed." (L144–145)
- **Halsey's reply to the closing.** Halsey → esther.fallas@calbar.ca.gov, 2024-07-24 20:21Z, id 190e6683ba52e8f5 (thread 190e656108df1d8f). Full body (L111–127):
  > "Esther, thank you for your detailed reply. I appreciate your position. We will first leave it to the courts to decide if my sole property was taken and then used to compensate a lawyer when he knew she had no known source of income, and full access to her financials, but all of my personal sole assets were now gone, assets which she had access to but not the right to control. I think it prudent to wait for the facts rather than the Bar adjudicate. I can always better address the matter with a ruling from the courts that determines whether the money was embezzled. When that is determined, and if it is shown to be true, then I will refile. A society where a separate legal entity can embezzle all sole assets of another person and use those funds to hire a lawyer to sue the victim is not one any of us want. I respect your determination to let the courts decide the crime, and then you can decide whether the actions meet the guidelines of the California Bar and are designed to stop these kinds of acts upon which civil society rests. / Thank you."
- **The extract's note on Fallas** (L105–108): "this thanks Esther Fallas for "your detailed reply", but **no inbound email from esther.fallas@ exists anywhere in the mailbox** (`from:esther.fallas@calbar.ca.gov` → 0)."
- L169: "*(No calbar traffic between 2024-08-14 and 2026-02-28 — an 18½-month gap.)*"

### 2.3 Complaint 2: 26-O-13820

**Origin (L172–174):** "The 2/28/26 send that put Intake@calbar.ca.gov on notice (one of 17 To: recipients) and from which Bar case 26-O-13820 was opened."
- The send is id 19ca3c3b9151b03c, 2026-02-28T10:20:38Z, thread 19ca398af605f23a ("= repo T-08").
- Subject: "CRIMINAL COMPLAINT AND REQUEST FOR ARREST WARRANT FOR LANCE SPIEGEL".
- The To: list includes `lances@ysfamilylaw.com` and `Intake@calbar.ca.gov` (L178). Bcc: "jswearingen.elliot@gmail.com, davidfife@gmail.com, isnow@snowphipps.com, kat.flds@gmail.com" (L179).
- Attachments: "index.html · Spiegel, The Beverly Hills Police Department, and City Administration- FORMAL NO.pdf · index.html" (L182). None were opened.

**What was alleged (verbatim):**
- "*RE:* Computer Crimes, Evidence Tampering, Perjury, and Conspiracy" (L219)
- "*PRIMARY SUSPECT:* Lance Spiegel, Esq. (California State Bar Member)" (L221)
- Statutes listed under "CRIMINAL CHARGES SUPPORTED BY EVIDENCE" (L674–941): Cal. PC § 502.7, § 502(c)(1), § 135; 18 U.S.C. § 2701, § 1030; PC § 134, § 132, § 118(a); 18 U.S.C. § 1623; PC § 528.5(a), § 529(3), § 182(a)(1).
- The request addressed to the Bar (L1040–1053): "*CALIFORNIA STATE BAR:* Forward all evidence to: - Office of Chief Trial Counsel - Request immediate suspension pending investigation - Disbarment proceedings for: - Computer crimes - Evidence tampering - Perjury (7 false declarations) - Fraud on the court - Violation of professional conduct rules"
- Halsey's own summary of the allegations to Intake, 3/19/26 (L5484): "alleging attorney misconduct including false proofs of service (Hague Convention violations), computer crimes coordination, and discovery abuse in connection with BHPD Case No. 2025-14983 / 24STFL00432."

**What the Bar replied (verbatim):**
- **1.8a, Intake auto-reply.** 2026-03-01 00:02Z, id 19ca6b437528a8d3 (L5429–5439): "Thank you for your email. This is a monitored inbox for submissions related to attorney misconduct complaints. / The Intake unit of the Office of Chief Trial Counsel confirms receipt of your email. We review all email submissions. If you have previously made an attorney misconduct complaint and your email is related to your complaint and provides a case number and/or name that allows us to identify your complaint, we will forward the email to the staff handling your complaint. The initial review of attorney misconduct complaints can take up to 60 days. / If you have not filed an attorney misconduct complaint and you wish to pursue discipline against an attorney licensed in California, you may file an attorney misconduct complaint online. […] Thank you for contacting the State Bar of California."
- **1.8b, OCTC acknowledgment.** 2026-03-02 18:22Z, id 19cafc93aee2594b, attachment **`26-O-13820 Lance Stephen Spiegel.pdf`** (not downloaded) (L5447–5452): "Please see the attached acknowledgement letter regarding your complaint. / Thank you. / OFFICE OF THE CHIEF TRIAL COUNSEL / LG"
- **1.8c / 1.8d, Halsey's reply and the bounce.** Halsey replied on 3/07, id 19cca584e0a1b847: "I see it's do not reply meaning if I have evidence as suggested in the complaint it would not be evaluated." (L5459). It bounced, id 19cca586d5d5d393: "`550 5.7.129 RESOLVER.RST.RestrictedToRecipientsPermission; not authorized to send to recipient because the sender isn't on the recipient's list of senders to accept mail from`" (L5470–5472).
- **1.9, "the ONLY live human Bar exchange" (L5475), 2026-03-19, thread 19d0437bd9408458:**
  - Halsey's follow-up, id 19d0437bd9408458 (L5477–5499). He asks: "1. Confirm receipt of February 28 submission. 2. Provide case number and assigned investigator. 3. Advise on review timeline for misconduct allegations."
  - Intake reply #1, 04:08:42Z, id 19d04482043a4a07 (L5504): "You'll need to provide more information. Do you have a State Bar case number? If not, please identify the attorney about whom you complained. If you have not received an acknowledgement letter from us, it's likely we haven't opened a case. Also note that once a case is opened it will take 60-90 days to complete an initial review, and an investigator is only assigned if your case isn't closed in Intake."
  - Halsey, 14:59:18Z, id 19d069bd9786bb5a (L5521): "I have not received an acknowledgement letter from the State Bar and do not have a State Bar case number."
  - Intake reply #2, 20:31:17Z, id 19d07cba88589d86 (L5540): "The case number is 26-O-13820. We sent you an acknowledgment letter, via email to this address, on March 2, 2026. The email came from 'octcdonotreply@calbar.ca.gov" and provides the current status of the case. Please check your email."
  - Halsey, 21:01:36Z, id 19d07e75de594652 (L5552–5553): "I think I will let the criminal process play out. Then it will be much cleaner. Thank you. I need my time dedicated to ensuring that happens."
- **1.15, closing.** 2026-05-06 15:56Z, id 19dfe00fc8abea03, attachment **`26-O-13820 Minor Closing Letter.pdf`** ("not downloaded — the 2026 CLOSING letter, arriving four days after the supplementals were sent", L5780): "Please see the attached letter regarding the above referenced State Bar matter. Thank you." (L5785)
- **After the closing.** Two sends drew no reply:
  - 1.16, from halsey@minorventures.com, id 19dff13fd9dd8b9b (L5796–5830)
  - 1.17, to Lakshmi.Jagannath@calbar.ca.gov, id 19dff2cfa242d6ac, subject "No. Not unless you actually investigate." (L5832–5868). The extract notes: "addressed to a named Bar staffer, **Lakshmi Jagannath**, from whom no inbound email exists (`from:Lakshmi.Jagannath@calbar.ca.gov` → 0" (L5835–5836).

### 2.4 Ref 268155: online portal filing, 2026-04-20

- **Receipt:** 2026-04-20 15:43Z, complaint@calbar.ca.gov, id 19dab900c339a76b (L5563–5596): "You have successfully submitted your Attorney Misconduct Complaint to the State Bar of California. Please keep a record of your reference number: / 268155".
- **What was alleged:** the complaint's text is **not in this file**. Halsey describes it in his 4/20 notice to the DA: id 19dab983ae3aa08a, 15:52:53Z, attachment **`State_Bar_Complaint_Spiegel_2026-04-20.pdf`** (not downloaded), cc LA_OPCA@fbi.gov, CRM.CivilRights@usdoj.gov, oig.hotline@usdoj.gov, piu@doj.ca.gov, and two others (L5598–5625):
  - "Today I electronically filed a complaint with the California State Bar against opposing counsel Lance Stephen Spiegel, Bar No. 51625, in connection with BHPD Case No. 2025-14983 and the family court proceedings in Minor v. Minor, LASC Case No. 24STFL00432." (L5609)
  - "The complaint is attached. It comprises 72 paragraphs and 9 counts. I direct your attention to Counts 5 and 9, which cite criminal conduct under Cal. Penal Code sections 135 (destroying or concealing evidence), 141 (tampering with evidence), and 182 (criminal conspiracy)." (L5611)
  - "The factual allegations detail the coordinated sequence — leak, delete, demand, sanction — that forms the basis for both the Bar complaint and the criminal referral already under review by your office. The complaint includes the statistical analysis (approximately 1 in 10 billion probability of random selection), the .EML demand for evidence in a format known to be impossible to produce, the four false email service representations to the court, and the pattern of conduct by Mr. Spiegel's firm during the evidence destruction period." (L5613)
  - "A sanctions hearing premised on this evidence destruction is scheduled for April 24, 2026 — four days from today." (L5615)
- **A second copy.** Another copy went to the LDA as `State_Bar_Complaint_Spiegel.pdf` (id 19dab6b5b2ffcf5f, sent by "Max", L5909).
- **What the Bar replied:** only the automated receipt. The file records no acknowledgment letter, case number or closing for ref 268155.
- **Supplementals filed under all three numbers.** None drew a reply:
  - 1.12, id 19de9c7499d43619 (L5630–5685)
  - 1.13, id 19dea32df5dbea33 (L5687–5726)
  - 1.14, id 19dea47680f034f7 (L5728–5777)
  - 1.16, id 19dff13fd9dd8b9b (L5796–5830)

### 2.5 Closing reasons, "specific facts", and court-first language

- **The Bar's reasons for closing either case are NOT in this file.** Both closing letters are PDF attachments that were not downloaded (L88, L5780), and the file holds no text from them. The phrase "specific facts" appears nowhere in the file (grep). The file contains no Bar-authored court-first language.
- The only court-first language in the Bar correspondence is **Halsey's own**, in his 7/24/24 email. It paraphrases a reply that is not in the file:
  - "We will first leave it to the courts to decide if my sole property was taken…" (L111–112)
  - "I think it prudent to wait for the facts rather than the Bar adjudicate." (L116–117)
  - "I respect your determination to let the courts decide the crime, and then you can decide whether the actions meet the guidelines of the California Bar" (L122–124)
- Halsey's 2026 equivalent: "I think I will let the criminal process play out. Then it will be much cleaner." (L5552–5553)
- **Police-first language, from the LA DA, not the Bar.** info@da.lacounty.gov → halsey@minorventures.com, 2026-03-02 17:38:09Z, id 19cafa12df3a5ca4 (L4291): "Please be advised that all crimes must be reported to the police for a proper investigation. Absent such an investigation and a criminal finding, this office is unable to act. Please report the crime to the appropriate law enforcement agency in the jurisdiction where the crime occurred. If the crime has been reported, please contact the law enforcement agency and request to speak to a commanding officer to obtain status of the case. Thank you."
- **Pointers to the primary letters** (see §5): P-02 (2024 acknowledgment), **P-03 (2024 closing)**, P-13 (2026 acknowledgment), **P-24 (2026 closing)**. The complaint texts are at P-01 (portal 224000), **P-17** (`State_Bar_Complaint_Spiegel_2026-04-20.pdf`), P-19 (`State_Bar_Complaint_Spiegel.pdf`), P-16 (portal 268155), and P-07 (the 2/28/26 email and its PDF).

---

## 3. JANINE / JANINA

### 3.1 Who she is, per this file (verbatim, L5966–6005)

- L5966: "### 3.1 · (a) Janina is REAL — a fully documented, multi-year correspondent"
- L5968: "**Full name: JANINA DONG.** Role: HR professional."
- L5972–5976: "`janina@liveplanet.net` — earliest correspondent traffic **2021-01-12** (thread 176f77bf10ac898f); also 9/08/21, 11/17/21, 9/26-28/22, 2/06/23, 4/26/23, 5/04/23. Signature block 1/12/2021: "**Director of Human Resources, Live Planet, Inc., (415) 858-0934, janina@liveplanet.net**"; display name in quoted headers: "**Janina Dong** <janina@liveplanet.net>"."
- L5977–5983: "`janina@vividlabs.com` — from at latest 4/26/2023 (she answers a janina@liveplanet.net email from this address) through **1/13-14/2026** (Workspace-control/final-invoice exchange). Heavy traffic: Halsey↔Janina threads run continuously through 2024–2025 (payroll, benefits, SVB/First Citizens banking, Relation Insurance, Empower 401(k), Accountalent taxes, subpoena logistics, investor emails; she is cc'd on family-case service emails as early as 3/04/25 and receives Shannon's all-hands emails)." No message id is given for the 3/04/25 service-email cc.
- L5984–5988: "`jan@jdhrsolutions.com` — appears **1/04/2026** (Halsey re-forwards a series of December emails to it, consistent with her leaving Vivid); active through **4/16/2026**. Same person: her 1/14/26 email from this address gives the same invoice amount and the bank account name "**Janina Dong**" as the 1/14/26 janina@vividlabs.com email, and signs "**Jan**"."
- L5989–5992: "**Independent identity anchor:** LinkedIn invitation notice, 2019-02-09 (id 168d01b29ecf5f6b) [A]: "**Janina Dong, PHR — HR and Talent Acquisition Professional, San Francisco**". ("PHR" = Professional in Human Resources; "JD HR Solutions" = her initials.)"
- L5993: "**Date range as correspondent in THIS mailbox: 2021-01-12 → 2026-04-16.**"
- L6000–6005: "**Departure arc matching the client statement (U: employees/investors quit):** 12/28/25 she sends account-transition notices to Accountalent, Relation Insurance, Empower ("Checks"/benefits wind-down); 1/13/26 Halsey asks her to hand over control of the Vivid Google Workspace; 1/14/26 she requests final payment of **$7,459.65** and continues limited help ("Important Mail" 3/25/26, "Additional IRS Check" 4/02/26, "John and Vivid Back." 4/16/26 — her last)."
- L5940–5942: "Janina's **last email in this mailbox is 2026-04-16 15:40Z** (jan@jdhrsolutions.com, "Re: John and Vivid Back.", thread 19d9674a44e360f1) — five days before the hearing, and it is Vivid-investor/HR subject matter, not case material."
- §5 summary (L6252–6255): "**Identity:** Janina ("Jan") Dong, PHR — Director of HR at Live Planet, then Vivid Labs; janina@liveplanet.net / janina@vividlabs.com / jan@jdhrsolutions.com; correspondent 1/12/2021 → 4/16/2026; departure and final $7,459.65 invoice Jan 2026. REAL beyond question."

### 3.2 Every document in this file that mentions Janina / Jan, with pointer

| # | line | date | pointer | what the file says |
|---|---|---|---|---|
| N-1 | L5972 | 2021-01-12 | thread 176f77bf10ac898f | earliest janina@liveplanet.net traffic |
| N-2 | L6009–6030 | 2021-01-12 16:55Z | id 176f7864666df364 (janina@liveplanet.net → kellam@liveplanet.net, cc seth@, halsey2005) | HR offer-letter/NDA email signed "Jan … Director of Human Resources, Live Planet, Inc." |
| N-3 | L6032–6035 | 2021-01-12 19:18Z | id 176f809da80fb8be | "Halsey, I've just sent you the agreement via Docusign. Please sign at your earliest convenience." / "Halsey, it should be in your Live Planet inbox..." |
| N-4 | L5989–5991 | 2019-02-09 | id 168d01b29ecf5f6b | LinkedIn: "Janina Dong, PHR — HR and Talent Acquisition Professional, San Francisco" |
| N-5 | L6037–6041 | 2024-11-01 00:40Z | id 192e52ae0b36ccc4 (janina@vividlabs.com → halsey@minorventures.com), thread 192e4eb48f4671cf | "These appear to be official subpoenas. They've stated that they have also sent copies by mail. You should defer to your current lawyer/mediator, Jeff, about how to move forward here. I can help to [snippet truncates — full body in thread 192e4eb48f4671cf]". **The body is truncated, so this is not a full [A] capture.** The same id 192e4eb48f4671cf is listed at L6150 as the firm's 2024-10-31 "Petitioner's Subpoenas to Various Entities" email. |
| N-6 | L6043–6065 | 2026-01-14 17:07Z | id 19bbd7a38e011667 (jan@jdhrsolutions.com → halsey2005, halsey@vividlabs, halsey@minorventures) | final invoice "$7,459.65", signed "Jan". **Bank routing and account numbers appear verbatim at L6059–6060 and are deliberately not reproduced here.** |
| N-7 | L5940–5942 | 2026-04-16 15:40Z | thread 19d9674a44e360f1 | her last email, "Re: John and Vivid Back." |
| N-8 | L5956 | 2026-03-01→03-04 | id 19c9daf655f3002e | "Janina's 3/01–3/04/26 traffic is Vivid checks/QuickBooks (19c9daf655f3002e), not case mail" |
| N-9 | L5933 | query | `{from:jan@jdhrsolutions.com to:jan@jdhrsolutions.com from:janina@vividlabs.com to:janina@vividlabs.com} after:2026/04/17 before:2026/04/26` | "→ **0 results.**" |
| N-10 | L6079 | 2026-04-22 17:06Z | id 19db6286e0fd8857 | J-4; Halsey writes "Janine and Jan" (see 3.3) |

### 3.3 Every "Janine" occurrence the file verifies (verbatim, L6074–6082)

> "| J-1 | 2025-12-29/30 | attachments to mvs@ service emails (threads 19b6cc55639bdc93, 19b70bba0694f1d9: `2025-12-29 [P] Resp.RFO.$400,000.Vanguard….pdf` etc.) | **Opposing counsel's filings (Sirriyeh)** | C | the "phantom assistant Janine" / "falsified" allegation — the earliest "Janine" family in the mailbox is INSIDE Spiegel-firm court filings; the transmitting email bodies themselves do not contain the name |"

> "| J-2 | 2026-01-06 → 2/18 | kat.flds service thread 19b90cfd5117ff74 and Katherine formatting threads (19c6e8c40f8e9c2e, 19c6e667b7ba8a4a, 19c6e65078799f95, 19c11524cb39dfe1 …) | **attachments (Halsey's own draft declarations/responses being formatted for filing)** | C | Gmail matches these threads on "Janine"; no occurrence in any fetched body — the spelling lives in the attached response papers that answer J-1's allegation |"

> "| J-3 | 2026-04-21 | six `2026-04-21 [C] MO.*.pdf` minute orders (threads 19db2dc31208f02d, 19e0415c7756eb39) | **the court's orders** | C | the 4/21 fabrication finding re: emails referencing assistant "Janine" (matches 61_KALE_STATEMENT_LEDGER §7.6-gate context) |"

> "| **J-4** | **2026-04-22 17:06Z** | **id 19db6286e0fd8857, halsey2005 → kat.flds** | **HALSEY'S OWN SENT TEXT** | **A** | "Of course I did not Lance played games with **Janine and Jan** and I had 1 hour to respond… there are **2 forms of her name** before someone looked but my date precedes the judges horrible conclusion… **Yes Lance she has 2 names same person.**" |"

The J-4 quote contains elisions ("…"). The full body is at id 19db6286e0fd8857.

> "| J-5 | 2026-05-02 19:20Z | id 19dea223e125b9fe, halsey2005 → self ("Perplexity Prompt — Add Vocabulary Timeline to Slider HTML") | **Halsey's own sent text, quoting the opposing allegation** | A | "'Falsified' — Dec 30, 2025 — Matt Sirriyeh — **'Phantom assistant Janine' allegation**" |"

> "| J-6 | 2026-05-02 | `declaration_of_nonparticipation_v2.md` attached to id 19de99b4d95ec81b ("— Max (Halsey's AI assistant)") | attachment (AI-drafted declaration) | C | thread matches "Janine"; body does not contain it |"

> "| J-7 | 2025-05-22 | id 196f8888b82a1183, notification@service.tiktok.com | third-party noise | A | TikTok caption "Janine: I mean you can stay friends but like still #breakup…" — an unrelated TikTok creator; not the assistant |"

Further verbatim:
- L6084–6088: "**Not found anywhere, all time:** any email FROM a "Janine"; any address containing "janine"; any message signed "Janine". The name exists in this mailbox only as (i) opposing counsel's characterization (J-1), (ii) the litigation papers responding to it (J-2, J-6), (iii) the court's adoption of it (J-3), and (iv) Halsey's own two 2026 sent messages discussing that fight (J-4, J-5)."
- L6096: "**Janine** | **2 body-text occurrences, both 2026, both authored by Halsey** (J-4 direct use: "Janine and Jan… 2 forms of her name"; J-5 quoting Sirriyeh's "Phantom assistant Janine") | Halsey (2) · opposing counsel/court/litigation papers (attachment level, J-1/J-2/J-3/J-6) · unrelated TikTok (1) | 10+ threads match at attachment level | **no "Janine" ever appears as a sender, address, or signature**"
- L6100–6104: "Within halsey2005@gmail.com **body text**, the client wrote the spelling "Janine" **twice, both AFTER the 12/29-30/2025 sanctions motion made the name an issue** (4/22/2026 and 5/02/2026, J-4/J-5) — and in J-4 he is describing the two spellings as "2 forms of her name… same person," not addressing her. **No pre-December-2025 email was found in which the client calls Janina "Janine."**"

### 3.4 How "Janine" relates to Exhibit F: everything this file says (verbatim)

- **Halsey's account of the court's finding** (5/02/26 supplemental to the Bar, L5664): "- Made a finding that Complainant submitted Exhibit F "knowing that it was not authentic" — WITHOUT evidentiary hearing, in violation of Family Code section 217 and the Elkins reforms"
- **The same, in the corrected supplemental** (L5770): "The next day, the Court made a fabrication finding without evidentiary hearing (FC §217 violation), stripped all work product, reserved sanctions against complainant, imposed zero sanctions on Mr. Spiegel, and conducted the hearing on 90 minutes' email notice — 39 days short of CCP §1005(b)."
- **J-3** (L6078): "the 4/21 fabrication finding re: emails referencing assistant "Janine" (matches 61_KALE_STATEMENT_LEDGER §7.6-gate context)". Graded C, because the minute-order PDFs were not opened.
- **The limits on the negative** (L6104–6108): "Two limits on that negative: (1) occurrences inside attachments (his own drafted declarations, the Exhibit F emails themselves) could not be checked because attachments were off-limits this session — and Exhibit F, where the court located the "Janine" reference, is an attachment-level artifact; (2) the unconnected VIVIDLABS mailbox was not searchable."
- **The §7.6 gate** (L6109–6113): "Per the §7.6 gate (61_KALE_STATEMENT_LEDGER), the "Janine"-named correspondence log in the client's Drive is a generated reconstruction artifact and remains NOT citable; nothing found today changes that holding — but the census above adds one hard fact to it: **the real assistant is Janina ("Jan") Dong, and no genuine "Janine" correspondent has ever existed in this mailbox.**"
- **The addendum** (L6275–6283): "## ADDENDUM 2026-09-03 (append-only; controls) — "phantom assistant" attribution / Per v3_parts/qa_Q61_exhibit_F_provenance.md (Spiegel's re-attached Exhibit "2" and the 4/21/2026 order read at source): "phantom assistant, Janine" is the language of the AI-generated log and of Halsey's own declaration, not of Judge Sirriyeh's order. The order's operative words are quoted verbatim in qa_Q61 §4 ("submitted Exhibit F… as if it were an authentic set of email communications, knowing that it was not…"). Any line in this file attributing "phantom assistant" to the court is corrected accordingly."
- **Halsey's own position** (J-4, L6079): "there are 2 forms of her name before someone looked but my date precedes the judges horrible conclusion… Yes Lance she has 2 names same person."

**What this file does NOT say about Exhibit F:**
- It does not give the number of emails in Exhibit F. The words "six emails" do not appear. The only "six" near the hearing is "Six court order PDFs" (L5889).
- It does not say Exhibit F's emails are signed "Lance", or give their dates or authors.
- It gives no locator for Exhibit F itself.
- It does not compare Exhibit F with any PDF export or control set.

**Conflicts within the file:**
- **Who the addendum names as judge.** The addendum's "Judge Sirriyeh's order" (L6279) conflicts with the file's own §4 key (L6130–6131): "mvs = Matthew Sirriyeh, paralegal/notary".
- **Who coined "phantom assistant".** The addendum corrects only attributions "to the court". It does not address J-1's attribution of the "phantom assistant Janine" allegation to "Opposing counsel's filings (Sirriyeh)" (graded C, attachments not opened), or J-5's "'Falsified' — Dec 30, 2025 — Matt Sirriyeh — 'Phantom assistant Janine' allegation". It also leaves L6087 standing: "(iii) the court's adoption of it (J-3)".

### 3.5 "The email Janine sent the day before the motion was heard": the file's verdict

- **The hearing date.** L5883–5887: "The repo (63C T-43) knows the sanctions hearing as **scheduled for 4/24/2026**. The live mailbox shows the motions were actually **heard 2026-04-21**: - Katherine Schwenke, 4/22/26 01:44Z (id 19db2dc31208f02d) [A]: "See attached Minute Orders from the hearing today 4-21-2026…"". Also at L5891–5892: "**"The hearings were always on the 21st"**" (Katherine via Google Voice, id 19db5b25bb020ddc).
- **The verdict.** L5944–5949: "**Verdict: the email the client remembers — "the email that Janine sent the day before the motion was heard" — does not exist in halsey2005@gmail.com.** What exists the day before the motion was heard is the 4/20 Bar-filing cluster written by "Max" from Halsey's own account. (Caveat per §0: the unconnected VIVIDLABS mailbox could not be checked; but a case-related email to Katherine/the Bar/the court would be expected HERE, and is not.)"
- **Other hearings.** The table at L5953–5960 shows no Jan/Janina/Janine mail in the day-before window of any of six hearing dates.

### 3.6 "Max" (the assistant persona in Halsey's own account)

- L5900–5904: "the sender persona on those emails is **"Max"**, writing from Halsey's own account (halsey2005@gmail.com) to the legal-document assistant **Katherine Schwenke, LDA (kat.flds@gmail.com — Family Law Document Services, Riverside CA)**"
- L5925–5928: "On 4/22 17:27Z (id 19db63bd0a662f4c) Halsey writes, in his own voice: **"Max I think died and with him a massive amount of knowledge but I need this."** — "Max" is on the face of these emails an assistant persona operating out of Halsey's own mailbox, later named explicitly: 5/02/26 id 19de99b4d95ec81b signs "**— Max (Halsey's AI assistant)**" [A]."

---

## 4. ACTS ATTRIBUTED TO SPIEGEL, HIS FIRM (ysfamilylaw.com), OR STAFF

Classes:
- (a) unauthorized access, alteration or creation of content in Halsey's accounts
- (b) material appearing in filings: (b1) from Halsey's accounts, (b2) from Spiegel's accounts
- (c) service date or method discrepancies
- (d) electronic service without consent
- (e) Shannon Minor's preliminary declaration of disclosure, income & expense declaration, or 6/18/2024 email-only proof of service
- (f) concert with court or police
- (g) Ally restriction or bank referral to the firm
- (h) other

The last column of each table answers: is the underlying primary document identified in THIS file?

### 4.1 Acts alleged in Halsey's own documents, as reproduced in the file

Every row is Halsey's allegation, unproven in this file. The 2/28/26 complaint describes itself as AI-assisted (L1507–1508).

| ID | line(s) | act date (as stated) | verbatim | class | primary doc identified? |
|---|---|---|---|---|---|
| A-01 | L285–287 | "March 29, 2024 - June 19, 2025" | "*March 29, 2024 - June 19, 2025:* Lance knew my computer was compromised (7 systematic Hague Convention violations exploiting my defensive blindness)" | (h) knowledge claim; (c) | No |
| A-02 | L288–290 | "March 29, 2024 - January 12, 2026 (654 days)" | "Lance knew Google had no preservation order (demanded native .EML files impossible without preservation)" | (h) | No |
| A-03 | L291–292; L1067 | "March 29, 2025 - August 4, 2025" | "Lance obtained my confidential 567-page police report (only Detective Kale should have this)"; "But *Lance Spiegel obtained this confidential police document.*" | (f) (via the alleged BHPD leak, A-14); (h) | No. "Exhibit N: March 29, 2025 confidential police report to Detective Kale (redacted version…)" is named at L1291–1292, with no locator |
| A-04 | L242–244; L293–294; L497–528 | "August 4, 2025" | "On August 4, 2025, an intruder executed surgical deletion of emails from my Google account. The deleted emails matched my confidential March 29, 2025 police report to Detective Kale *with exact 1-to-1 precision*." … "*Conclusion:* Lance accessed Detective Kale's confidential files, identified the indexed emails, and executed (or directed) precision deletion that preserved email timeline continuity." | (a) | No. Exhibits J and O are named (L1282, L1302) with no locator; Google deletion logs are *requested* (L983–992) |
| A-05 | L373–377; L399–401 | (undated) | "The hack only targeted HER emails - wiping clean all recent correspondence with Shannon Minor like she'd ghosted me." … "Lance exploited complete access to both destroy real evidence AND create false evidence." | (a) | No |
| A-06 | L295–297; L563–575; L786 | "December 29, 2025" | "Lance filed "Code Red" CCP 271 sanctions motion ($250,000) demanding: 1. *November 11, 2022 "smoking gun" tax refund email* - DELETED August 4, 2025 2. *Native .EML file format with metadata* - IMPOSSIBLE without Google preservation order 3. *Authentication of emails I could no longer produce*"; "*Lance's own motion claims $250,000+ damages*" | (h) litigation demand; (b1) as framed; (c): served "U.S. mail (prohibited)" per L541–542 | **Partial.** The transmittal is identified: 2025-12-30 mvs, id 19b70bba0694f1d9, "Minor - RFO for Family Code §271 Sanctions (the $250k motion)" (L6179); see also id 19b6cc55639bdc93 (L6178). The motion text is not quoted or opened |
| A-07 | L592–599 | "January 10, 2026" | "*The "Terrible Documents" Email Read in Court* Lance or his counsel read a "terrible documents" email in court, claiming I sent it. *I DENY SENDING ANY SUCH EMAIL.*" | (a) creation (alleged forgery); (b1) | No. Forensic authentication is *requested* (L994–1001) |
| A-08 | L534–544 | "June 19, 2025 - February 2026" | "Lance filed *7 motions* using prohibited service methods […] 1. *June 19, 2025:* TRO via email (Hague violation #1) 2. *Income Declaration:* U.S. mail to Mexico (prohibited) 3. *Deposition Objections:* U.S. mail (prohibited) 4. *Non-Service Declaration:* U.S. mail (prohibited) 5. *December 29, 2025:* "Code Red" CCP 271 sanctions motion ($250,000) - U.S. mail (prohibited) 6. *Motion to Strike:* U.S. mail (prohibited) 7. *Vexatious Litigant RFO:* U.S. mail (prohibited)" | (c); item 1 (d); item 2 possibly (e), though the file does not say whose Income Declaration | No. "Exhibit K: Service violation table" is named (L1283). §4.2 has rows with matching subject words (L6177, L6182, L6189) but the file does not link them |
| A-09 | L555–561 | "February 24, 2026" | "*February 24, 2026: Physical Proof (Mail Dump)* - All mail Lance claimed to have "served" over 8 months arrived in one batch - Many envelopes never opened before this date" | (c) | No. "Exhibits B-G: February 24, 2026 mail dump photographs (files 191-196)" are named (L1275), with no locator |
| A-10 | L304–316 | (undated; TRO period) | "When responding to a TRO, Lance had used false service multiple times to be heard. He immediately withdrew the TRO when I filed an ex parte motion outlining some of the evidence and promptly delivered the evidence hold email. […] It was the fifth such incident of false email service when I and then through my response informed the judge of Lance's lack of email service rights, which were confirmed by Lance's inability to produce the necessary documentation." | (c); (d) | No |
| A-11 | L323–327 | (undated) | "When the TRO was quickly pulled following notification, I offered to waive service publicly on the record […] Lance, when questioned twice by the judge, stated that he had no interest in the TRO anymore" | (h) | No. "Exhibit R: Lance's employee TRO withdrawal court transcripts" is named (L1308–1309). §4.2 row L6183 (2026-01-21 "Notice of Taking Hearing on Petitioner's Request for DVRO Off-Calendar") exists; the file makes no link |
| A-12 | L2933–2940 (3/01/26 to Shannon, id 19ca73bbab906e02) | (undated) | "I asked Lance Why? Twice. […] He tried to prove no pre se would have control. He has very likely destroyed your life when offered an off ramp. […] I just needed Lance to not want the TRO when he had broken so many laws to get it. Twice he answered "no". Exactly why I offered it." | (h) | No |
| A-13 | L828–830; L848–851 | (undated) | "7 false service declarations filed under penalty of perjury - Claimed proper Hague Convention service (false) - Mail dump proves service dates fabricated"; "7 sworn declarations claiming valid service to Mexico" | (c) | No |
| A-14 | L356; L935; L1019–1022; L1076–1081 | (undated) | "Possible conspiracy or information leak to Lance Spiegel"; "Possible coordination with BHPD leak (how did Lance get police report?)"; "Were there communications between Kale and Lance? - Did Kale coordinate with Lance or provide access?"; "*Scenario 1: BHPD Information Leak* - Detective Kale or BHPD employee leaked report to Lance" | (f), framed as a possibility or question | No |
| A-15 | L199–201 | (undated) | "it's possible that Lance recruited public officials in positions of power across the criminal, judicial, and administrative sectors." | (f), possibility | No |
| A-16 | L937 | (undated) | "Possible coordination with Shannon Minor (strategic timing of TRO)" | (h) | No |
| A-17 | L645–646 | "February 27, 2026" (discovery date) | "*Explains the "how":* Lance could remotely control my closed Mac over network" | (a) capability claim | No. "Exhibit H … (file 509)" is named (L1276–1277) |
| A-18 | L111–115 (7/24/24 email) | (undated) | "if my sole property was taken and then used to compensate a lawyer when he knew she had no known source of income, and full access to her financials" | (h): the subject of the 2024 Bar complaint, per Halsey | No. The complaint text is not in the file (portal ref 224000, P-01) |
| A-19 | L5484 (3/19/26) | (undated) | "alleging attorney misconduct including false proofs of service (Hague Convention violations), computer crimes coordination, and discovery abuse" | (c); (a); (h) | Pointer P-07 (the 2/28 submission); content not opened |
| A-20 | L5611–5613 (4/20/26 to DA) | (undated) | "the coordinated sequence — leak, delete, demand, sanction — […] the .EML demand for evidence in a format known to be impossible to produce, the four false email service representations to the court, and the pattern of conduct by Mr. Spiegel's firm during the evidence destruction period." | (a); (c)/(d); (f); (h) | **Filename only.** `State_Bar_Complaint_Spiegel_2026-04-20.pdf` on id 19dab983ae3aa08a (P-17), not opened |
| A-21 | L5654–5655; L5704 (5/02/26; Gemini-generated material) | "Dec 29-30, 2025" | "Correlation 7: Mr. Spiegel's personal violation rate of 92% (11 of 12 personal actions) vs. staff rates of 25-57%"; "Correlation 3: Zero fabrication language in 18 months of litigation, then all four terms ("fabricated," "fake," "falsified," "perjury") deployed in a 48-hour burst after the evidence was destroyed"; "deployed in a 48-hour burst on Dec 29-30, 2025 — exactly 147 days after the Aug 4, 2025 scalpel hack." | (c); (h) | No primary document. The source is AI-LEAD attachments (P-21–P-23) |
| A-22 | L5664–5669 (5/02/26; court acts) | "April 21, 2026" | "Imposed zero sanctions on Mr. Spiegel despite 12 instances of defective service"; "Conducted the hearing on approximately 90 minutes' email notice to a pro se party in Mexico — 39 days short of the minimum required by CCP section 1005(b)"; "Authorized Mr. Spiegel to serve by email going forward — the method he had been using illegally for two years" | (c); (d); (f) | **Partial.** The 4/21/2026 order files are identified (P-27, P-28) but not opened. The file does not say who sent the 90-minute notice |
| A-23 | L5675 | (undated) | "separate sworn depositions of Matt Sirriyeh and Anna Kralle Vanmali. Neither is a partner. Neither designed the strategy. Neither has reason to protect Mr. Spiegel at the cost of their own career." | (h) | No |
| A-24 | L5819 (5/06/26) | (undated) | "Meanwhile I'm being "mailed" as proper service to Mexico or emailed 5 times without my consent as pro se, ignored, a perfect 12 for 12." | (c); (d) | No |
| A-25 | L5812 (5/06/26) | n/a | "How much is orchestrated by Lance, that's up to you to decide. I am just feeding you statistical certainty." | (h) | No |
| A-26 | L5840–5850 (5/06/26 to Jagannath) | (undated) | "You don't find it odd that Lance would bring a 10 billion:1 to motion forward, or 1:1 if he colluded with the police officer, who did not investigate for 14 months […] It was a motion that fined me $250,000 and freed his client from all criminal and civil liabilities related to $1.5 mm in theft, by him identify out of 600 pages of emails—several thousand —1 of the 12 in the police report summary, that was hacked as "if by a scalpel", removing those 12 emails from the Gmail server (one of which he just happened to claim "fake")." | (a); (b1); (f) | No |
| A-27 | L6079 (4/22/26, J-4) | (undated) | "Lance played games with **Janine and Jan** and I had 1 hour to respond…" | (h) | The email is identified (id 19db6286e0fd8857). No primary document for the act itself |
| A-28 | L6080 (5/02/26, J-5; AI prompt) | "Dec 30, 2025" | "'Falsified' — Dec 30, 2025 — Matt Sirriyeh — **'Phantom assistant Janine' allegation**" | (h) | **Partial.** J-1 points to threads 19b6cc55639bdc93 / 19b70bba0694f1d9 at attachment level (C), not opened. See the conflict with the addendum in §3.4 |

Not attributed to Spiegel: L5806, "The original submitted complaint document I have attached, which became the template of the first cyber attack". That sentence names no actor.

### 4.2 Acts recorded by the extractor from the mailbox

These are attributed to the firm or its staff on the face of Gmail records.

| ID | line(s) | date | verbatim | class | primary doc identified? |
|---|---|---|---|---|---|
| M-01 | L5888–5890 | 2026-05-07 | "Six court order PDFs all dated 04/21/2026, served 5/07/26 by Sirriyeh (id 19e0415c7756eb39, filenames `2026-04-21 [C] MO.*.pdf`)." | (c) | Yes: P-28 (attachments not opened) |
| M-02 | L6076 (J-1) | 2025-12-29/30 | "the earliest "Janine" family in the mailbox is INSIDE Spiegel-firm court filings; the transmitting email bodies themselves do not contain the name" | (h) | Yes, attachment-level only: P-37 (graded C, not opened) |
| M-03 | L6276–6277 | undated | "Spiegel's re-attached Exhibit "2"" | (b2)/(b1). The file does not say what Exhibit "2" contains, beyond its tie to Exhibit F via qa_Q61 | No locator in this file; reached only through the work product qa_Q61 (P-44) |
| M-04 | L5982 | "as early as 3/04/25" | "she is cc'd on family-case service emails as early as 3/04/25" | (d)? | No (no id given) |

**The firm transmission table (verbatim rows L6137–6201).**

Scope, verbatim (L6125–6131): "every message from a Young, Spiegel & Hosp sender (`{from:AnnaK@ from:mvs@ from:lances@ from:VivianH@ysfamilylaw.com}` in:anywhere, both result pages, 65-thread estimate, all threads' previewed messages tabulated; thread-preview limitation noted in §0) […] AnnaK = Anna Kralle (Vanmali), paralegal; mvs = Matthew Sirriyeh, paralegal/notary; lances = Lance Spiegel personally." No VivianH row appears.

Class legend for the table:
- **(d)?** The row records an email transmission of litigation papers by the firm. The file records nothing about consent, and makes no finding on service versus courtesy copy except where the row text says so.
- **(c)?** The row text itself states a service method or date.
- **(e)?** The row names an income & expense declaration; the file does not say whose.
- **(h)** Correspondence, auto-reply, or other.
- **"subject only"** The subject line reveals nothing more.

"Matching words" notes only that the subject shares words with an allegation in §4.1. The file makes no such link itself.

| src line | date (Z) | sender | id | subject (verbatim row) | class | primary doc identified? |
|---|---|---|---|---|---|---|
| L6137 | 2024-01-25 | AnnaK | 18d424f91222fab9 | Minor (correspondence + docs; N&A for signature) | (d)? — N&A sent for signature | yes — Gmail id; attachments not opened |
| L6138 | 2024-01-31 | AnnaK | 18d617333d82df9a | FW: Minor (follow-up, signed N&A) | (d)? — signed N&A follow-up | yes — Gmail id; attachments not opened |
| L6139 | 2024-02-01 | lances | 18d6598e61e8abf0 | RE: Minor Divorce | (h) — Spiegel personally | yes — Gmail id; attachments not opened |
| L6140 | 2024-02-01 | lances | 18d659c74c96f2f5 | RE: Minor | (h) — Spiegel personally | yes — Gmail id; attachments not opened |
| L6141 | 2024-02-01 | AnnaK | 18d65a9dad2be7d3 | FW: Minor (relaying Lance's bounced reply) | (h) — relays Spiegel's bounced reply | yes — Gmail id; attachments not opened |
| L6142 | 2024-02-13 | AnnaK | 18da4c2fe5eb3cd1 | Case Inititation Documents (+ Notice & Acknowledgment) | (d)? — case initiation docs + N&A | yes — Gmail id; attachments not opened |
| L6143 | 2024-04-02 | AnnaK | 18ea11c7a1b64cd0 | Minor | (h)? subject only | yes — Gmail id; attachments not opened |
| L6144 | 2024-06-03 | AnnaK | 18fdf4915ea20042 | RE: Minor Mediation | (h) | yes — Gmail id; attachments not opened |
| L6145 | 2024-07-17 | mvs | 190c2fad1c4fd49a · 190c322ff4021189 | Rejected Response and Declaration Re UCCJEA (x2) | (h) | yes — Gmail id; attachments not opened |
| L6146 | 2024-07-18 | AnnaK | 190c83dfe9cb7fd1 | Automatic reply (out of office until 8/1) | (h) auto-reply | yes — Gmail id; attachments not opened |
| L6147 | 2024-07-23 | mvs | 190dcf708ca9607b | Minor - Response Deadline | (h) | yes — Gmail id; attachments not opened |
| L6148 | 2024-07-23 | mvs | 190e0eee763559a9 | Minor - Response to Proposal (mediation) | (h) | yes — Gmail id; attachments not opened |
| L6149 | 2024-08-15 | AnnaK | 19157ba8e41220f7 | Minor RFO — "The attached documents have been sent to you via mail. We are sending an email as a courtesy copy" | (c)? (d)? — row text: mail + email "courtesy copy" | yes — Gmail id; attachments not opened |
| L6150 | 2024-10-31 | mvs | 192e4eb48f4671cf · 192e4f2f43647e39 | Petitioner's Subpoenas to Various Entities (x2, incl. bounce-remedy resend) | (h) subpoenas; (d)? — same thread id as Janina's 11/01/24 reply (L6040) | yes — Gmail id; attachments not opened |
| L6151 | 2024-11-18 | AnnaK | 19340b0eb2056651 | Minor (correspondence) | (h) | yes — Gmail id; attachments not opened |
| L6152 | 2025-01-08 | AnnaK | 194482330a95baa0 | Minor RFO — "conformed RFO documents… A physical copy of these documents is being mailed to you as well" | (c)? (d)? — row text: physical copy "being mailed" | yes — Gmail id; attachments not opened |
| L6153 | 2025-06-23 | mvs | 1979db6b2125390b | EX PARTE NOTICE (after phone attempts; "(415) 531-2080 – No Answer and Voicemail was Full…") | (c)? (d)? — ex parte notice by email after phone attempts | yes — Gmail id; attachments not opened |
| L6154 | 2025-06-23 | lances | 1979e2cd049f87a2 | RE: EX PARTE NOTICE ("Encouraging you to consult with counsel…") | (h) — Spiegel personally | yes — Gmail id; attachments not opened |
| L6155 | 2025-06-24 | mvs | 197a2dc47ddd607c | COURTESY COPIES OF PLEADINGS (DVRO request package, 16.8 MB) | (d)? — "COURTESY COPIES" | yes — Gmail id; attachments not opened |
| L6156 | 2025-06-24 | mvs | 197a3724d248ab44 | RE: COURTESY COPY OF TRO AND NOTICE OF HEARING | (d)? — "COURTESY COPY OF TRO" | yes — Gmail id; attachments not opened |
| L6157 | 2025-07-09 | mvs | 197f0190d0a820ec | DVRO Pleadings | (d)? | yes — Gmail id; attachments not opened |
| L6158 | 2025-07-14 | lances | 1980aad41bcc7b22 · 1980ab73fbfe94e7 | RE: TRO Strategy, Continuance, and Proposed Resolution (x2) | (h) — Spiegel personally | yes — Gmail id; attachments not opened |
| L6159 | 2025-07-16 | mvs | 19814f71e34d448e | Continuance of Hearing on Petitioner's Request… | (d)? | yes — Gmail id; attachments not opened |
| L6160 | 2025-07-24 | AnnaK | 1983aec0ff36fac3 | Automatic reply | (h) auto-reply | yes — Gmail id; attachments not opened |
| L6161 | 2025-08-06 | AnnaK | 19881ad39b42a700 · 19881b493805982e | **Minor - Service of Documents** (x2) | (d)? — "Service of Documents" | yes — Gmail id; attachments not opened |
| L6162 | 2025-08-07 | AnnaK | 198858d3a85cd7ea | Halsey - Trial Setting Conference Documents | (d)? | yes — Gmail id; attachments not opened |
| L6163 | 2025-08-11 | AnnaK | 1989a0b964394e79 | Minor - Declaration of LSS | (d)? | yes — Gmail id; attachments not opened |
| L6164 | 2025-08-22 | AnnaK | 198d2853d2dd6410 | Minor - Ex Parte Responsive Declaration | (d)? | yes — Gmail id; attachments not opened |
| L6165 | 2025-08-26 | AnnaK | 198e7213c97e482c | Minor - Ex Parte Response | (d)? | yes — Gmail id; attachments not opened |
| L6166 | 2025-08-28 | AnnaK | 198f1708b4eb9340 | Minor - Ex Parte Response | (d)? | yes — Gmail id; attachments not opened |
| L6167 | 2025-08-29 | mvs | 198f6f253f2a7e0a | Petitioner's Request for Production of Documents, Set 1 | (d)? | yes — Gmail id; attachments not opened |
| L6168 | 2025-10-08 | lances | 199c5dc7db16c037 | This morning's discussion | (h) — Spiegel personally | yes — Gmail id; attachments not opened |
| L6169 | 2025-10-14 | AnnaK | 199e40b0c7a5927e · 199e45d488541702 | Minor - Responsive Declaration (x2) | (d)? | yes — Gmail id; attachments not opened |
| L6170 | 2025-10-20 | AnnaK | 19a0369c2de9fe45 | Minor | (h)? subject only | yes — Gmail id; attachments not opened |
| L6171 | 2025-10-22 | AnnaK | 19a0d16829b0084f | Minor | (h)? subject only | yes — Gmail id; attachments not opened |
| L6172 | 2025-10-27 | AnnaK | 19a275d457ec3591 · 19a276eb2382abe7 | Minor - Correspondence · Minor - Notice | (d)? | yes — Gmail id; attachments not opened |
| L6173 | 2025-10-28 | AnnaK | 19a2b9aee561a4c4 · 19a2ba87ce5e12d9 | Minor - Ex Parte Notice · Minor - Ex Parte | (d)? | yes — Gmail id; attachments not opened |
| L6174 | 2025-11-15 | AnnaK | 19a84d3d95de6534 | Minor | (h)? subject only | yes — Gmail id; attachments not opened |
| L6175 | **2025-11-24** | **mvs** | **19ab753ad35b7d52 · 19ab8474aa899682** | **Minor - Stipulation Re PERSONAL SERVICE of Pending Requests for DVRO (x2)** | (c)? — "PERSONAL SERVICE" stipulation; attachments not opened (L6222–6224) | yes — Gmail id; attachments not opened |
| L6176 | 2025-12-03 | mvs | 19ae64fb3079084e | Minor - 12/01/2025 Support Payment | (h) | yes — Gmail id; attachments not opened |
| L6177 | 2025-12-26 | mvs | 19b5cbba04495f7b | Petitioner's Objections to Respondent's Notice of Deposition | (d)? — matching words: A-08 item 3 | yes — Gmail id; attachments not opened |
| L6178 | 2025-12-29→30 | mvs | 19b6cc55639bdc93 | Response to RFO / Motion for Protective Order (the 12/29 Sirriyeh declaration package; = 63H N-12) | (d)? · J-1 attachment-level "Janine" | yes — Gmail id; attachments not opened |
| L6179 | 2025-12-30 | mvs | 19b70bba0694f1d9 | **Minor - RFO for Family Code §271 Sanctions** (the $250k motion) | (d)? · J-1 · A-06 (the §271 motion) | yes — Gmail id; attachments not opened |
| L6180 | 2026-01-05 | AnnaK | 19b8fc6fabdac16f | Minor (service email; = 63H N-12's 1/05 Kralle) | (d)? | yes — Gmail id; attachments not opened |
| L6181 | 2026-01-06 | AnnaK | 19b90daa5f6a5300 | Minor - Discovery Responses | (d)? | yes — Gmail id; attachments not opened |
| L6182 | 2026-01-08 | AnnaK | 19b9ed5b3f686f69 | Minor - Motion to Strike (= 63H N-12's 1/08 Kralle) | (d)? — matching words: A-08 item 6 | yes — Gmail id; attachments not opened |
| L6183 | 2026-01-21 | mvs | 19be2c2fa4b8f5b3 | Notice of Taking Hearing on Petitioner's Request for DVRO Off-Calendar | (d)? — matching words: A-11 | yes — Gmail id; attachments not opened |
| L6184 | 2026-01-28 | mvs | 19c0338466026974 · 19c036b7d786e9b7 | Petitioner's Responsive Declaration (x2) | (d)? | yes — Gmail id; attachments not opened |
| L6185 | 2026-02-02 | AnnaK | 19c20c6b957e80c5 | Minor - Ex Parte Responses | (d)? | yes — Gmail id; attachments not opened |
| L6186 | 2026-02-09 | AnnaK | 19c43efcecf77097 | Minor - Minute Order | (d)? | yes — Gmail id; attachments not opened |
| L6187 | 2026-02-10 | AnnaK | 19c498713648d147 | RE: | (h)? subject only | yes — Gmail id; attachments not opened |
| L6188 | 2026-02-12 | mvs | 19c4f9dc9d26b93f | Minor - Calculation of Support and Fee Payments Due | (h) | yes — Gmail id; attachments not opened |
| L6189 | 2026-02-23 | AnnaK | 19c8c7743a00925a · 19c8ca6230be2d9a · 19c8ce40d7913f4b | Reply Declaration · Income & Expense Declaration · Minor (= 63H N-12's 2/23 declarations) | (d)? (e)? — whose I&E not stated; matching words: A-08 item 2 | yes — Gmail id; attachments not opened |
| L6190 | 2026-02-24 | AnnaK | 19c90cf4d4c1f5ae | Minor - Responsive Declarations (= N-12's 2/24) | (d)? | yes — Gmail id; attachments not opened |
| L6191 | 2026-03-02 | AnnaK | 19cb05b6a5ac0151 | Minor | (h)? subject only | yes — Gmail id; attachments not opened |
| L6192 | 2026-03-27 | mvs | 19d30e829fbc2838 | **Minor - Petitioner's Brief Re Service Issues** | (c)? — "Brief Re Service Issues" | yes — Gmail id; attachments not opened |
| L6193 | 2026-04-08 | AnnaK | 19d6ded69e5461e2 | Minor - Responsive Declaration | (d)? | yes — Gmail id; attachments not opened |
| L6194 | 2026-04-14 | AnnaK | 19d8d4651b42e71a | Minor | (h)? subject only | yes — Gmail id; attachments not opened |
| L6195 | 2026-04-15 | AnnaK | 19d92ff93fc8b4f0 | Minor | (h)? subject only | yes — Gmail id; attachments not opened |
| L6196 | 2026-05-07 | mvs | 19e0415c7756eb39 | Minute Orders (All Remaining RFOs) — "Hard copies… will follow by U.S. Mail w/ USPS Tracking Number: EH045932903US" | (c)? (d)? — row text: USPS tracking; = M-01 | yes — Gmail id; attachments not opened |
| L6197 | 2026-05-08 | mvs | 19e04f7c4026ee5d | Order After Hearing on Respondent's Motion to Quash | (d)? | yes — Gmail id; attachments not opened |
| L6198 | 2026-05-18 | mvs | 19e3d773b931aaea | RE: Order After Hearing… | (h) | yes — Gmail id; attachments not opened |
| L6199 | 2026-07-07 | mvs | 19f3d7ad12f99c51 | Petitioner's Responsive Declaration | (d)? | yes — Gmail id; attachments not opened |
| L6200 | 2026-07-14 | mvs | 19f621d4a50fd4af | Petitioner's Case Management Statement | (d)? | yes — Gmail id; attachments not opened |
| L6201 | 2026-07-21 | mvs | 19f870bf19d5f34f | Minor - Court's Minute Order | (d)? | yes — Gmail id; attachments not opened |

**§4.3 findings, verbatim (L6214–6230):**
- "Email-transmitted service from the firm in **late 2025 runs Kralle (Aug–Nov 15) then Sirriyeh (Nov 24–Dec 30)**; Kralle resumes 1/05–1/08/26 and dominates Feb–Apr 2026 declaration service; Sirriyeh carries the court-order service (May–Jul 2026)."
- "**No email exists in which Lance Spiegel personally transmits service documents.** His personal emails in the whole sweep: 2/01/24 (x2), 6/23/25, 7/14/25 (x2), 10/08/25 — all correspondence/argument, none a document-service email. If Spiegel "served personally" in late 2025, it was not by email visible in this mailbox; the mailbox artifact closest to the client's claim is Sirriyeh's **11/24/2025 "Stipulation Re Personal Service of Pending Requests for DVRO"** (two sends), whose attachments were not opened this session."
- "Late-2025 volume by sender (firm emails above): Aug 2025: Kralle 6, Sirriyeh 1 · Sep: 0 · Oct: Kralle 8, Spiegel 1 · Nov: Kralle 1, Sirriyeh 2 · Dec: Sirriyeh 4. A late-2025 surge exists, but on the face of the email record it is a **Kralle-then-Sirriyeh** surge."
- "Thread-preview limitation (§0) means messages deep in long threads could be undercounted; the ids above are each individually verified."

Halsey-side transmissions to the firm (L6203–6210) are not acts of the firm. They are listed as pointer P-42.

### 4.3 Roll-up by class

- **(a)** A-04, A-05, A-07, A-17, A-20, A-26 (and A-19). All are Halsey's allegations. **None has a primary document identified** in this file.
- **(b)** (b1): A-06, A-07, A-26. (b2) or (b1): M-03 (Spiegel's re-attached Exhibit "2", no locator). Exhibit F itself is never located in this file.
- **(c)** A-01, A-06, A-08, A-09, A-10, A-13, A-19, A-20, A-21, A-22, A-24; M-01; firm rows marked (c)?. The only identified primaries are the firm transmittal ids, whose attachments were not opened.
- **(d)** A-08 item 1, A-10, A-20, A-22, A-24; M-04; firm rows marked (d)?. **The file contains no consent or non-consent document.**
- **(e)** **Preliminary declaration of disclosure: not mentioned anywhere in the file.** Income & expense declaration: only A-08 item 2 ("*Income Declaration:* U.S. mail to Mexico (prohibited)", L538; undated, party not stated) and the firm row at L6189 (2026-02-23, AnnaK, id 19c8ca6230be2d9a, "Income & Expense Declaration"; party not stated). **6/18/2024 email-only proof of service: not mentioned.** The firm table has no 2024-06-18 row (rows run 2024-06-03 at L6144 to 2024-07-17 at L6145), subject to the thread-preview limitation (L6229–6230).
- **(f)** A-03, A-14, A-15, A-20, A-22, A-26. All are possibilities, questions or allegations. **No primary document** apart from the unopened 4/21/2026 order files.
- **(g)** **Nothing in this file.** "Ally" does not occur (case-sensitive grep). Banks named are: "Silicon Valley Bank" (L301), "SVB/First Citizens banking" (L5981), and "Capital One - Savings" (L6057, Janina's own account). None is linked to the firm.
- **(h)** A-01, A-02, A-06, A-11, A-12, A-16, A-18, A-21, A-23, A-25, A-27, A-28; M-02; Spiegel's personal emails (L6139, L6140, L6154, L6158, L6168).

---

## 5. PRIMARY DOCUMENT POINTERS (deduped)

Class key:
- **PRIMARY**: a Gmail record.
- **PRIMARY–ATT**: a Gmail record whose key content is in an attachment not opened by 63K.
- **HALSEY-STMT**: primary as a record of what Halsey said, not of the facts he asserts.
- **AI-AUTHORED**: written by the "Max" persona.
- **AI-LEAD**: AI-generated content.
- **WP**: tracker work product.
- **NAMED-ONLY**: no locator given.

| P-ID | pointer | date | what it is | claim attached | class |
|---|---|---|---|---|---|
| P-01 | id 190503e0ad8885f5 + Bar portal ref 224000 (apps.calbar.ca.gov/complaint/Account) | 2024-06-25 | Bar portal receipt; portal holds the filed complaint ("print and download the complaint") | 24-O-18793 filed; complaint text | PRIMARY (complaint text in portal, not in file) |
| P-02 | id 19055a01bc508ed6 · `24-O-18793 Lance Stephen Spiegel.pdf` | 2024-06-26 | OCTC acknowledgment letter | 24-O-18793 opened | PRIMARY–ATT |
| **P-03** | id 190e5588b28b881b · **`24-O-18793 Minor Closing Letter.pdf`** | 2024-07-24 | **OCTC closing letter, 2024** | Bar's 2024 closing reasons (absent from file) | **PRIMARY–ATT (must open)** |
| P-04 | id 190e6683ba52e8f5 (thread 190e656108df1d8f) | 2024-07-24 | Halsey → esther.fallas@calbar.ca.gov | 2024 allegation substance (A-18); Halsey's court-first deferral | HALSEY-STMT |
| P-05 | id 191520d1b41ce456 | 2024-08-14 | Bar survey ("recently sent you a closing letter") | 2024 closing occurred | PRIMARY |
| P-06 | id 190f163d774c91ba | 2024-07-26 | Bar newsletter [B] | none (not case correspondence) | PRIMARY (irrelevant) |
| **P-07** | thread 19ca398af605f23a · id 19ca3c3b9151b03c · atts `index.html` (x2), **`Spiegel, The Beverly Hills Police Department, and City Administration- FORMAL NO.pdf`** | 2026-02-28 | Halsey's criminal complaint email to 17 recipients incl. Intake@calbar and lances@ysfamilylaw.com | All of A-01–A-17; origin of 26-O-13820 | HALSEY-STMT (self-described as AI-assisted); attachments unread |
| P-08 | ids 19ca3c3ef08606e0 · 19ca3c3ef0ad9987 · 19ca3c3ef8560bd4 | 2026-02-28 | DSN bounces: cityatty@ / citymgr@ / citycouncil@beverlyhills.org "Invalid-Recipient" | delivery failure | PRIMARY |
| P-09 | id 19ca3c7958e0baf8 | 2026-02-28 | forward to tw@waitt.com ("one of the top 3 divorce attorneys in LA") | none new | HALSEY-STMT |
| P-10 | id 19ca73bbab906e02 · atts IMG_1242.jpeg, IMG_1245.jpeg, IMG_1243.jpeg + complaint atts | 2026-03-01 | forward to shannonmimor@gmail.com | A-12 | HALSEY-STMT |
| P-11 | id 19cafa12df3a5ca4 | 2026-03-02 | LA DA reply: report to police first | police-first language | PRIMARY |
| P-12 | id 19ca6b437528a8d3 | 2026-03-01 | Bar Intake auto-reply | receipt of 2/28 email | PRIMARY |
| **P-13** | id 19cafc93aee2594b · **`26-O-13820 Lance Stephen Spiegel.pdf`** | 2026-03-02 | OCTC acknowledgment letter, 26-O-13820 | case opened; "current status" (per L5540) | **PRIMARY–ATT (must open)** |
| P-14 | id 19cca584e0a1b847 · DSN id 19cca586d5d5d393 | 2026-03-07 | Halsey reply to do-not-reply; bounce | none | PRIMARY |
| P-15 | thread 19d0437bd9408458: ids 19d0437bd9408458, 19d04482043a4a07, 19d069bd9786bb5a, 19d07cba88589d86, 19d07e75de594652 | 2026-03-19 | the only live human Intake exchange | case number; process; Halsey stands down | PRIMARY |
| P-16 | id 19dab900c339a76b + portal ref 268155 | 2026-04-20 | portal receipt | 268155 filed; complaint text in portal | PRIMARY |
| **P-17** | id 19dab983ae3aa08a · **`State_Bar_Complaint_Spiegel_2026-04-20.pdf`** | 2026-04-20 | Halsey → DA (cc FBI/DOJ/CA-AG and others) attaching the Bar complaint | A-20 (72 paras / 9 counts) | HALSEY-STMT; **attachment = filed complaint text (must open)** |
| P-18 | DSN id 19dab9842852b961 | 2026-04-20 | CRM.CivilRights@usdoj.gov "550 5.1.1 … User Unknown" | delivery failure | PRIMARY |
| P-19 | ids 19dab6b396f48a12 · 19dab6b5b2ffcf5f (att `State_Bar_Complaint_Spiegel.pdf`) · 19dab6f4f0e2c0be | 2026-04-20 | "Max" → kat.flds re mailing a hard copy | 4/20 day-before cluster | PRIMARY record, AI-AUTHORED; attachment unread |
| P-20 | ids 19dac2031903beab · 19dac20c1ea0c4dc | 2026-04-20 | Katherine: "Halsey I cannot open this PDF." | none | PRIMARY |
| P-21 | id 19de9c7499d43619 · `officer_kale_report_footnoted_v2.pdf`, `bar_evidence_correlation_package.html`, `file_80---d49f37cb-78d9-41a4-b682-e88c4cbf42df.jpg` | 2026-05-02 | Supplemental 1 to complaint@ | A-21, A-22, A-23 | email HALSEY-STMT; attachments **AI-LEAD** ("generated by Google Gemini AI") |
| P-22 | id 19dea32df5dbea33 · `evidence_exposure_timeline_slider.html`, `Lance_Criminal_Evidence_App.html`, `BHPD_Marsys_IA_Presentation.html`, `Criminal_Complaint_Spiegel_v1.html`, `file_81---3aeb99e9….jpg`, `file_82---8136e612….jpg` | 2026-05-02 | Supplemental 2 | A-21 | AI-LEAD |
| P-23 | id 19dea47680f034f7 · Exhibits 1–7c (`Exhibit_1_Officer_Kale_Forensic_Report.pdf` … `Exhibit_7c_Gemini_Analysis_3.jpg`) | 2026-05-02 | Supplemental (corrected) | A-21, A-22 | AI-LEAD |
| **P-24** | id 19dfe00fc8abea03 · **`26-O-13820 Minor Closing Letter.pdf`** | 2026-05-06 | **OCTC closing letter, 2026** | Bar's 2026 closing reasons (absent from file) | **PRIMARY–ATT (must open)** |
| P-25 | id 19dff13fd9dd8b9b (from halsey@minorventures.com) · `Digital_Forensic_Dossier Older I think.pdf`, `Short version.pdf`, `2154004252-…-d.png`, image0–2.jpeg | 2026-05-06 | "Coloring Book" email to complaint@, cc DA | A-24, A-25 | HALSEY-STMT; attachments AI-LEAD ("coloring book version created by AI") |
| P-26 | id 19dff2cfa242d6ac (thread 19dff18b2aa86646) · `Officer_Kale_Report_Footnoted_v2 2.pdf` | 2026-05-06 | Halsey → Lakshmi.Jagannath@calbar.ca.gov | A-26 | HALSEY-STMT; attachment AI-LEAD (same report family as P-21) |
| **P-27** | id 19db2dc31208f02d | 2026-04-22 | Katherine Schwenke: "See attached Minute Orders from the hearing today 4-21-2026…" | 4/21 orders (J-3) | **PRIMARY–ATT (must open; court orders)** |
| **P-28** | id 19e0415c7756eb39 · six `2026-04-21 [C] MO.*.pdf`; "USPS Tracking Number: EH045932903US" | 2026-05-07 | Sirriyeh service of the six 4/21/2026 minute orders | M-01; the Exhibit F finding (J-3); A-22 | **PRIMARY–ATT (must open)** |
| P-29 | id 19db5b25bb020ddc | 2026-04-22 | Katherine via Google Voice: "The hearings were always on the 21st" | hearing date 4/21 | PRIMARY |
| P-30 | id 19db7634412cf151 | 2026-04-22 | Halsey → Shannon: "a day before the one hour" | day-before = Bar filing | HALSEY-STMT |
| P-31 | id 19db1d411f18b570 (+ Katherine 4/21 23:13Z reply, no id given) | 2026-04-21 | "Max here on behalf of Halsey" → kat.flds | Max persona | PRIMARY, AI-AUTHORED |
| P-32 | id 19db63bd0a662f4c | 2026-04-22 | Halsey: "Max I think died…" | Max persona | HALSEY-STMT |
| P-33 | id 19de99b4d95ec81b · `declaration_of_nonparticipation_v2.md` | 2026-05-02 | email signed "— Max (Halsey's AI assistant)" (J-6) | Janine at attachment level | AI-AUTHORED; attachment AI-LEAD |
| P-34 | id 19db6286e0fd8857 | 2026-04-22 | J-4 Halsey → kat.flds | "Janine and Jan… same person"; A-27 | HALSEY-STMT |
| P-35 | id 19dea223e125b9fe | 2026-05-02 | J-5 "Perplexity Prompt — Add Vocabulary Timeline to Slider HTML" | A-28 | HALSEY-STMT (an AI prompt) |
| P-36 | id 196f8888b82a1183 | 2025-05-22 | J-7 TikTok notification | none | PRIMARY (irrelevant) |
| **P-37** | threads 19b6cc55639bdc93 (2025-12-29→30, "Response to RFO / Motion for Protective Order") and 19b70bba0694f1d9 (2025-12-30, "Minor - RFO for Family Code §271 Sanctions"); att `2025-12-29 [P] Resp.RFO.$400,000.Vanguard….pdf` "etc." | 2025-12-29/30 | Spiegel-firm filings (Sirriyeh transmittals) | J-1 "Janine" family; A-06; A-28; M-02 | **PRIMARY–ATT (must open)** |
| P-38 | thread 19b90cfd5117ff74; threads 19c6e8c40f8e9c2e, 19c6e667b7ba8a4a, 19c6e65078799f95, 19c11524cb39dfe1 "…" | 2026-01-06→02-18 | Halsey-side draft papers formatted by the LDA (J-2) | Janine at attachment level | HALSEY-STMT; attachments unread |
| P-39 | Janina corpus: thread 176f77bf10ac898f; ids 176f7864666df364, 176f809da80fb8be, 168d01b29ecf5f6b, 192e52ae0b36ccc4 (thread 192e4eb48f4671cf), 19bbd7a38e011667, 19c9daf655f3002e; thread 19d9674a44e360f1 | 2019-02-09 → 2026-04-16 | Janina Dong's own emails, LinkedIn, last email | identity (§3) | PRIMARY |
| P-40 | ids 1979db6b2125390b, 19e17f7fe0f01875, 19f82164c88d86aa, 19f870bf19d5f34f | 2025-06-23; 2026-05-11/12; 2026-07-21 | hearing-date anchors (table L5953–5960) | day-before windows | PRIMARY |
| P-41 | firm transmittal ids in the table under §4.2 (L6137–6201) | 2024-01-25 → 2026-07-21 | Young, Spiegel & Hosp emails (AnnaK / mvs / lances) | classes (c)/(d)/(e)/(h) | PRIMARY–ATT (attachments unread) |
| P-42 | ids 198e338062a3bb85; 1992ff3853ff8100 · 1992fffec95f776b; 19b90cfd5117ff74; 19c725f84fcd4a29 | 2025-08-25 → 2026-02-18 | kat.flds (Halsey's LDA) → firm "Marriage of Minor" | Halsey-side service | PRIMARY |
| P-43 | **NAMED-ONLY, no locator in this file:** "Exhibit F" (L5664, L6106–6107, L6280); Spiegel's "re-attached Exhibit "2"" (L6276–6277); 2/28/26 complaint Exhibits B–V incl. "files 191-196" (L1275) and "file 509" (L1277); "the "Janine"-named correspondence log in the client's Drive" (L6109–6110); "Declaration of Non-Participation and Preservation of Rights" (L5671); the "terrible documents" email (L596); the 3/29/2025 "567-Page Report" / "Analysis of Evidence" (L451–455); the Silicon Valley Bank "new account application" (L301–304); "the evidence hold email" (L307); the 6/19/2025 TRO (L405–407); the "ex parte motion" (L305–306); "DVRO defense response" (L319); Halsey's 4/17/2026 "formal demand letter" to the DA (L5607) | various | items cited but not located | various | NAMED-ONLY |
| P-44 | **WP cross-refs:** `governance/matters/04_criminal_bhpd_2025-14983/report_2026-08/v3_parts/qa_Q61_exhibit_F_provenance.md` (claims Spiegel's re-attached Exhibit "2" and the 4/21/2026 order were "read at source"; quotes the order at its §4); `…/report_2026-08/61_KALE_STATEMENT_LEDGER.md` §7.6; `…/report_2026-08/63C_DOJ_MAIL_EXTRACT.md` (T-43); `…/report_2026-08/63H_EVIDENCE_TRANSFER_EXTRACT.md` (N-12); session scratchpad `bar/` (not in repo) | 2026-09 | tracker work product | Exhibit F provenance; §7.6 gate | WP / AI-LEAD (paths located by `git ls-files`; not read for these notes) |

---

## 6. FLAGGED INSIDE THE FILE AS FALSE, UNVERIFIED, INVENTED, WITHDRAWN OR CORRECTED (verbatim)

1. L5944–5946: "**Verdict: the email the client remembers — "the email that Janine sent the day before the motion was heard" — does not exist in halsey2005@gmail.com.**"
2. L6084–6085: "**Not found anywhere, all time:** any email FROM a "Janine"; any address containing "janine"; any message signed "Janine"."
3. L6103–6104: "**No pre-December-2025 email was found in which the client calls Janina "Janine."**"
4. L6109–6111: "the "Janine"-named correspondence log in the client's Drive is a generated reconstruction artifact and remains NOT citable"
5. L6275–6283, the ADDENDUM: ""phantom assistant, Janine" is the language of the AI-generated log and of Halsey's own declaration, not of Judge Sirriyeh's order. […] Any line in this file attributing "phantom assistant" to the court is corrected accordingly."
6. L5883–5884, the hearing date corrected: "The repo (63C T-43) knows the sanctions hearing as **scheduled for 4/24/2026**. The live mailbox shows the motions were actually **heard 2026-04-21**". This contradicts Halsey's own L5615: "scheduled for April 24, 2026 — four days from today."
7. L106–108: "**no inbound email from esther.fallas@ exists anywhere in the mailbox** (`from:esther.fallas@calbar.ca.gov` → 0)."
8. L5835–5836: "from whom no inbound email exists (`from:Lakshmi.Jagannath@calbar.ca.gov` → 0"
9. L6218–6222: "**No email exists in which Lance Spiegel personally transmits service documents.** […] If Spiegel "served personally" in late 2025, it was not by email visible in this mailbox"
10. L6227–6228: "A late-2025 surge exists, but on the face of the email record it is a **Kralle-then-Sirriyeh** surge."
11. Delivery failures:
    - L1521–1524, L1542–1545, L1563–1566: "Your message wasn't delivered to cityatty@beverlyhills.org / citymgr@beverlyhills.org / citycouncil@beverlyhills.org […] Recipient address rejected: Invalid-Recipient."
    - L5627–5628: "**CRM.CivilRights@usdoj.gov bounced — "550 5.1.1 … User Unknown"** (matches 63C's finding)."
    - L5469–5470: "**Halsey's 1.8c reply bounced**".
12. Graded C, unverified at attachment level: J-1, J-2, J-3, J-6 (L6076–6081). L6040: "[snippet truncates — full body in thread 192e4eb48f4671cf]". L130–135, 1.5: "[B] … Captured as metadata + snippet".
13. Corrections by the senders themselves:
    - L5736: "(Corrected — prior emails were missing attachments)"
    - L5910: "Quick correction — the State Bar mailing address has changed… 845 S. Figueroa Street… (Not the 1149 S. Hill Street address from my earlier email — that's outdated.) — Max"
14. Hedges inside the 2/28/26 complaint:
    - "⸻G. Possible Email Forgery (January 10, 2026)" (L592)
    - "*Evidence suggests possible forgery:*" (L601)
    - "*Requires forensic authentication. If forged:*" (L620)
    - "Possible scenarios: (a) BHPD information leak to Lance, (b) Lance hacked BHPD systems, (c) Lance already had emails and directed Kale's classification" (L695–697)
    - "*NOTE: There may be other methods involved.*" (L301)
15. L5677 (Halsey to the Bar): "The question is not whether these correlations have innocent explanations. The question is whether the Bar will ask the people who know."

Figures that differ across the documents reproduced in this file. These are placed side by side verbatim; **the file does not flag them**:
- **Number of deleted or targeted emails:**
  - "My police report indexed ~30 specific evidentiary emails - August 4 deletion targeted those exact 30 emails" (L250–251)
  - "fewer than 10 targeted for deletion matching the confidential police report index exactly" (L5650)
  - "fewer than 10 targeted" (L5748)
  - "1 of the 12 in the police report summary […] removing those 12 emails from the Gmail server" (L5847–5849)
- **Probability:** "*~10,000,000,000 to 1*" (L252) vs "(30/116,000)^30 ≈ 10^-138" (L523)
- **Service-violation counts:**
  - "*7 motions*" (L534)
  - "the fifth such incident of false email service" (L312)
  - "the four false email service representations to the court" (L5613)
  - "12 instances of defective service" (L5667)
  - "emailed 5 times without my consent as pro se, ignored, a perfect 12 for 12" (L5819)
  - "11 of 12 personal actions" (L5654)
- **Google preservation refusals:**
  - "Refused 4 explicit requests for Google preservation orders" (L346)
  - "5 evidence preservation calls to Google, ignored" (L5802)
  - "5 times refused a 30-minute call to Google to preserve evidence five times" (L5852–5853)
- **Duration:** "654 days" (e.g., L278, L399) vs "647 days" (L5710, L5760) vs "did not investigate for 14 months" (L5842)
- **Date of the BHPD report:** "*March 29, 2024: Bank-Originated Hack Reported*" (L367) vs "*March 29, 2025: 567-Page Report Submitted to BHPD*" (L451)
- **Theft figures within one email:** "$1.5 mm in theft" (L5846) vs "$2.5 mm in theft" (L5851)
- **The 2026 acknowledgment letter:** Halsey replied to the 3/02/26 acknowledgment email on 3/07/26 (L5455–5466). On 3/19/26 he wrote "I have not received an acknowledgement letter from the State Bar and do not have a State Bar case number." (L5521)
- **Spiegel's personal service:** "Mr. Spiegel's personal violation rate of 92% (11 of 12 personal actions)" (L5654) vs "**No email exists in which Lance Spiegel personally transmits service documents.**" (L6218)
- **Sirriyeh's role:** "Judge Sirriyeh's order" (L6279) vs "mvs = Matthew Sirriyeh, paralegal/notary" (L6130–6131)

---

## 7. OPEN QUESTIONS THE FILE NAMES (verbatim)

1. L6264–6269: "**Tests still owed (D-13 form):** the four OCTC letter PDFs (ack + closing, both cases) and `State_Bar_Complaint_Spiegel_2026-04-20.pdf` — read at source by an attachment-capable session; the J-1/J-2/J-3/J-6 attachment-level "Janine" occurrences — same; the VIVIDLABS workspace mailbox for the primary Janina corpus; page-2+ of the fuzzy "Janina"/"Janine" searches (metadata captured in scratchpad, occurrences beyond the verified set unenumerated)."
2. L6104–6108: "Two limits on that negative: (1) occurrences inside attachments (his own drafted declarations, the Exhibit F emails themselves) could not be checked because attachments were off-limits this session — and Exhibit F, where the court located the "Janine" reference, is an attachment-level artifact; (2) the unconnected VIVIDLABS mailbox was not searchable."
3. L6222–6224: "the mailbox artifact closest to the client's claim is Sirriyeh's **11/24/2025 "Stipulation Re Personal Service of Pending Requests for DVRO"** (two sends), whose attachments were not opened this session."
4. L6229–6230: "Thread-preview limitation (§0) means messages deep in long threads could be undercounted; the ids above are each individually verified."
5. L5947–5949: "(Caveat per §0: the unconnected VIVIDLABS mailbox could not be checked; but a case-related email to Katherine/the Bar/the court would be expected HERE, and is not.)"
6. L21–22: "A gap here is absence-of-access, not absence."
7. L5895–5896: "So the candidate "day before" windows are **4/20/2026** (day before the actual hearing) and **4/23/2026** (day before the originally-noticed 4/24 date)."
8. L5873–5875: "~150 threads where "State Bar" appears only in passing (case chatter, newsletters, signature blocks). Those are captured at metadata level in session scratchpad `bar/search_*.json`; none is a message to or from the Bar."
9. Questions inside Halsey's 2/28/26 complaint:
   - "*How did Lance know which emails were deleted unless he executed or directed the hack?*" (L583–584)
   - "How did Lance obtain 567-page March 2025 report? - Was there information leak to Lance or representatives? - Were there communications between Kale and Lance? - Did Kale coordinate with Lance or provide access?" (L1019–1022)
   - "(how did Lance get police report?)" (L935)
10. Questions in Halsey's Bar emails:
    - "1. Confirm whether my February 28, 2026 submission ("CRIMINAL COMPLAINT AND REQUEST FOR ARREST WARRANT FOR LANCE SPIEGEL") reached Intake and, if so, whether a case has been opened. 2. If no case has been opened, advise on the best way to re-submit this complaint" (L5526–5527). Answered at L5540.
    - "The question is whether the Bar will ask the people who know." (L5677)

---

*Notes written read-only. Nothing in the tracker or in Gmail was modified. The only files written are this one, and a transient table file in this folder that was removed.*
