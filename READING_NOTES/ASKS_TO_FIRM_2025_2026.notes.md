# Asks to the firm, 2025-01-01 to 2026-11-01: reading notes

- **Request:** Halsey Minor, 2026-11-01: "check how many times I asked him for my own information and for the initial financial statements".
- **Data file:** `INVENTORY/asks_to_firm_2025_2026.tsv`. It has 82 rows, one row per message per category.
- **Source:** the Gmail mailbox signed in as Halsey@realitylab.com. Access was read-only: search_threads, get_thread and get_message only.
- **Attachments:** none was opened, so no PDF was read.
- **Date written:** 2026-11-01.

---

## 1. Totals

**Universe.** The universe is every message Halsey sent that meets all three conditions:
- it was sent from halsey2005@gmail.com, halsey@minorventures.com or Halsey@realitylab.com;
- an `@ysfamilylaw.com` address is in To or Cc;
- it is dated 2025-01-01 to 2026-11-01. The last such message is dated 2026-08-08.

That gives 130 messages. 77 contain at least one ask and 53 contain none. A message counts once per category. Five messages count in both B and C: 1987804f00adef63, 198fcf44b5f0e72a, 19a2d40a9a509a74, 19ab9218ce36c50a and 19b6b024126d3ccd.

| Category | Messages | Different days (UTC) | Different days (Pacific) | First | Last |
|---|---|---|---|---|---|
| A — his own information | **0** | 0 | 0 | — | — |
| B — initial financial statements | **10** | 9 | 9 | 2025-06-17T05:16:54Z `1977c51ddad08b0a` (2025-06-16 Pacific) | 2025-12-29T16:47:16Z `19b6b024126d3ccd` |
| C — other | **72** | 54 | 53 | 2025-01-16T04:13:00Z `1946d50b277915a3` | 2026-08-08T00:47:54Z `19fded7384ca4b84` |

The same totals in D-77 form:
- **B:** asked 10 times, on 9 different days.
- **A:** asked 0 times in this window.
- **C:** asked 72 times, on 54 different days (53 in Pacific time).

### 1a. The ten B messages

| # | date_utc | Pacific day | message_id | thread_id | Addressed to | What the email's own text asks for |
|---|---|---|---|---|---|---|
| 1 | 2025-06-17T05:16:54Z | 06-16 | 1977c51ddad08b0a | 18da4c2fe5eb3cd1 | AnnaK@, lances@ | "I would like to see the documents you failed to file." The same message names FL-140, FL-141, FL-142, FL-150 and FL-160. |
| 2 | 2025-06-20T04:56:45Z | 06-19 | 1978bb2792558e91 | 1978bb2792558e91 | lances@, AnnaK@ | The body says only "Please see attached. Please respond by 5 PM PST." **The category comes from the attachment title** "Demand for Immediate Financial Disclosure and Compliance with Legal Obligations.pdf". The PDF was not read. |
| 3 | 2025-06-23T19:08:12Z | 06-23 | 1979e30e22e4ae99 | 1979db6b2125390b | lances@ | "WHY DONT YOU JUST PROVIDE THE DOCUMENTS YOU OWE ME." **The documents are not named** in this message. |
| 4 | 2025-07-09T13:27:44Z | 07-09 | 197ef5eeb73a5be8 | 1979db6b2125390b | mvs@ cc lances@, VivianH@, AnnaK@ | "Are you going to once again as pro se fail to file deliver the documents?" It is preceded by "I have not received the initial financial document disclosure which apparently don't exist since I have asked twice and you have admitted to never delivering to me." |
| 5 | 2025-08-05T02:17:26Z | 08-04 | 1987804f00adef63 | 19877f1fad1c4529 | lances@, AnnaK@, mvs@, VivianH@, Jeff@jjfamilylaw.com | "I insist that you immediately serve all required preliminary disclosure forms and financial documents that have been missing. This includes a properly completed FL-140, FL-150, FL-160 (or FL-142), and any other mandatory attachments (such as tax returns)." |
| 6 | 2025-08-30T21:48:31Z | 08-30 | 198fcf44b5f0e72a | 198fcf44b5f0e72a | lances@, shannonminor@ cc AnnaK@, mvs@, paulf@, VivianH@, kat.flds@ | "(b) produce the required financial disclosures and responsive documents without further delay (as you should have years ago)" |
| 7 | 2025-10-28T23:56:43Z | 10-28 | 19a2d40a9a509a74 | 19a2d3e5809cfe0a | lances@, AnnaK@, lasuperior2025-14983@lovesndlaw.ai | "this includes serving the complete initial financial disclosures and any other outstanding documents forthwith." |
| 8 | 2025-11-25T00:57:02Z | 11-24 | 19ab8839844998ec | 19ab8474aa899682 | mvs@ (Bcc kat.flds@) | "I am just having to tell you again to provide the information you asked for." **The disclosures are not named.** The same message also says "your information obligations" and "the courts' own mandate for information". |
| 9 | 2025-11-25T03:49:24Z | 11-24 | 19ab9218ce36c50a | 19ab9218ce36c50a | lances@ | "Confirm in writing that there are no other undisclosed accounts funded with my separate property." |
| 10 | 2025-12-29T16:47:16Z | 12-29 | 19b6b024126d3ccd | 19b6b024126d3ccd | lances@ | "Please confirm in writing by Monday, January 5, 2026 that Petitioner will serve a complete, verified Preliminary Declaration of Disclosure with required supporting documents (including but not limited to account statements and tax returns as applicable), and file proof of service." |

**The days.**
- UTC (9 days): 2025-06-17, 06-20, 06-23, 07-09, 08-05, 08-30, 10-28, 11-25, 12-29.
- Pacific (9 days): 2025-06-16, 06-19, 06-23, 07-09, 08-04, 08-30, 10-28, 11-24, 12-29.
- There is no B ask after 2025-12-29. Every B message had a firm address in To.

**Narrower reading.** In three B messages the email's own text does not name the disclosures:
- #2 relies on the attachment title only;
- #3 says "the documents you owe me";
- #8 says "the information".

Without those three, B is **7 messages on 7 different days**, in both UTC and Pacific time.

### 1b. Category A: no explicit ask in this window

None of the 130 messages contains an ask I classed as A. Category A covers:
- his own records, accounts, data or documents;
- copies of what the firm or Shannon hold about him;
- his tax and financial records in their possession;
- his personal information.

What the mail does contain is listed in §5:
- statements about earlier asks (§5a);
- five borderline asks, classed C and listed for the reader to weigh (§5b);
- similar wording in mail that went to no firm address (§5c).

### 1c. Category C labels

A message can carry two labels, so these counts add up to more than 72:
- payments 22, service 11;
- property 5, funds 5, preservation 5;
- deposition 4;
- contact 3, children 3, mediation 3;
- conduct 2, process 2;
- 1 each: asset, reply, storage, fees, tax, emails, filings, settlement, discovery, evidence, strategy, meeting, calendar, resend, investigation.

In 29 of the 72 C messages, someone else was the To addressee and the firm was copied. These addressees were mostly Shannon, plus Janina, M. Gurvitz, Jeff Jacobson, CourtCall and Det. Kale.

---

## 2. Firm replies that produced a document

**How the TSV's reply columns are filled.** A reply is a message from `@ysfamilylaw.com` in the same thread within 30 days. There is one exception, marked in the TSV: `197f0190d0a820ec` is in a separate thread, but it quotes the ask and begins "Per your request".

**Category B: no firm reply to a B ask produced a document.** The only firm reply to a B ask is `1979e5eb9bbac178` (quoted in §3). It has no attachment.

### 2a. The three documents named in the brief, checked at source

- **2025-06-04, `1973c9cdeeb8a442`: this email is not from the firm.**
  - From: bill@provinziano.com, signed "William W. Oxley, Esq. / Senior Certified Family Law Specialist Associate" of Provinziano & Associates.
  - To: halsey2005@gmail.com, at 2025-06-04T20:23:07Z. Subject: "provinziano - 06-17-24 PDD (shannon)".
  - Body: "see attached". Attachment: "2024.06.17, P's PDD.pdf".
  - It is a single-message thread and answers no message in this universe.
  - READING_NOTES/BEHAVIOR_b_e_primary.notes.md line 62 says "The firm emailed it". That firm is Provinziano, not Young, Spiegel & Hosp.

- **2025-12-30, `19b70bba0694f1d9`: the "12/30/2025 I&E".**
  - From: mvs@ysfamilylaw.com (Matthew Sirriyeh), at 2025-12-30T19:28:12Z.
  - To: halsey2005@, halsey@minorventures.com, halsey@vividlabs.com and halsey@liveplanet.net. Cc: kat.flds@gmail.com, VivianH@, AnnaK@ and lances@.
  - It is a new single-message thread. Subject: "Minor - RFO for Family Code §271 Sanctions".
  - Body: "Please see attached the following: 1. Petitioner's RFO for Family Code §271 Sanctions filed 12/30/2025; 1. Petitioner's Income and Expense Declaration filed 10/22/2025; 1. Court Order for Post-Judgment Request for Orders dated 12/30/2025; 1. Blank Responsive Declaration to Request for Order (FL-320); 1. Blank Income and Expense Declaration (FL-150); and, 1. Blank Post-Judgment Request for Order Case Management Statement (LASC FAM 119). Hard copies of all of the above have also been served by U.S. Mail."
  - Attachments: 2025-12-30 [P] RFO.Sanctions.pdf; 2025-10-22 [P] I&E.pdf; 2025-12-30 [C] Order.PJ.RFO.pdf; fl320.pdf; fl150.pdf; LASC FAM 119.pdf.
  - It does not quote or mention any request from Halsey. It was sent 1 day 2 h 41 min after B ask #10 (`19b6b024126d3ccd`). That ask is in a different thread and got no firm reply in its own thread.

- **2026-02-23, `19c8ca6230be2d9a`: the "2/23/2026 I&E".**
  - From: AnnaK@ysfamilylaw.com, at 2026-02-23T22:37:00Z.
  - It is a new thread. Subject: "Minor - Income & Expense Declaration".
  - Body: "Please see the attached document." Attachment: "2026-02-23 [P] I&E.pdf".
  - It is not a reply to anything. The only later message in the thread is Halsey's `19c950ecec081c5a`, sent from vividlabs, which contains no ask.
  - The last B ask before it was 56 days earlier (`19b6b024126d3ccd`).

### 2b. Other firm emails carrying B-type documents

None of these replies to an ask.

- **`19a0d16829b0084f`**
  - From AnnaK@, 2025-10-22T18:02:39Z, first message of its thread.
  - Body: "Please see the attached documents. Hard copies of these documents are being mailed to you as well."
  - Attachments: "2025-10-22 [P] I&E.pdf" and "2025-10-22 [P] Resp.Decl.pdf".
  - This is the I&E that the 12/30 email re-sent. The nearest earlier B ask was 53 days before (#6, 2025-08-30).
- **`19b90daa5f6a5300`**
  - From AnnaK@, 2026-01-06T01:10:02Z. Subject: "Minor - Discovery Responses".
  - Body: "Please see attached Petitioner's Discovery Responses. A hard copy is being sent to you as well."
  - Attachment: "2026-01-05 [P] Resp.RFPs.pdf". Not read, so its contents are unknown.
  - It is not in the thread of any ask.
- **`19e0415c7756eb39`**
  - From mvs@, 2026-05-07T20:16:27Z. Subject: "Minor - Minute Orders (All Remaining RFOs)".
  - Among six orders it lists "Order After Hearing on Respondent's Motion to Compel Declarations of Disclosure and Request for Sanctions dated 04/21/2026".
  - Attachment: "2026-04-21 [C] MO.OAH.MTC.DODs.Sanctions.pdf". Not read.

### 2c. Firm replies with a document, in other categories

- **`197f0190d0a820ec`**
  - From mvs@, 2025-07-09T16:49:49Z. It is in a separate thread and quotes C:service ask `197ef5895435e31b`: "Matt why have you not served me the case? Do you have any proof as pro se I have been served your case?"
  - Text: "Halsey, Per your request, I am enclosing the following pleadings in connection with the hearing scheduled for July 16, 2025 at 8:30 a.m. in Dept. 23 of the Stanley Mosk Courthouse".
  - Attachments: 2025-06-24 [C] Ntc.Hearing.Req.DVRO.pdf; 2025-06-24 [P] Req.DVRO.pdf; 2025-06-24 [C] TRO.pdf; dv120.pdf; dv120info.pdf.
  - Halsey's only later message in that thread is `1983aec90893bcf4` (2025-07-24). Its whole text is "All documents." It is not counted as an ask: it has no verb and does not say what it wants.
- **`19c498713648d147`**
  - From AnnaK@, 2026-02-10T21:48:23Z, in thread.
  - It answers C:resend ask `19c4983f08010bfa`: "Can you try again since I cannot read that."
  - Text: "Please see attached. A hard copy was mailed to you as well."
  - Attachment: "2026-02-09 [C] MO.RFO.Mod.CS.CS".
- **`19c4f9dc9d26b93f`**
  - From mvs@, 2026-02-12T01:55:50Z.
  - Text: "Per your request, please see attached schedule of all CS, SS and Attorney Fee charges together with your payments to date."
  - Attachment: "2026-02-11 Pmnts.Halsey.pdf".
  - It quotes a Halsey request of 2026-02-10 to Shannon: "Please send me the most recent statement or calculation you have for the arrears...". That request does not appear in this mailbox as a message to or copying the firm, so it is outside the universe and not in the TSV.

**Not from the firm.**
- **Jeff Jacobson (mediator, jjfamilylaw.com), `197f53231734a97a`**, 2025-07-10T16:35:57Z.
  - Text: "Halsey: Attached is the Agreement to Mediate executed by you and Shannon in May 2024. Jeff"
  - Attachments: "Mediation Retainer Agr_signed by Halsey.PDF" and "Mediation Retainer Agr_signed by Shannon.pdf".
  - It answers `197f2046dcf71650` (§5b).
- **AnnaK `199e45d488541702`**, 2025-10-14T20:15:37Z: "No, that was the complete document."
  - It answers a question sent from vividlabs (§5e). No document was attached.

---

## 3. Refusals and conditions, quoted

### 3a. Firm replies in the same thread as the ask

- **`1979e5eb9bbac178`** — lances@ to halsey@minorventures.com, cc mvs@, 2025-06-23T19:58:07Z.
  - It came 50 minutes after B ask #3 (`1979e30e22e4ae99`: "WHY DONT YOU JUST PROVIDE THE DOCUMENTS YOU OWE ME.").
  - Reply: "Suggest you consult with counsel and research the following subjects: 1. The ex parte process and procedure in California. 1. The California Domestic Violence Protection Act, including acts constituting abuse and consequences of a finding of domestic violence. 1. Criminal Extortion under California law."
  - No attachment.
- **`1979e2cd049f87a2`** — lances@ to halsey@minorventures.com, 2025-06-23T19:03:35Z.
  - It follows C:filings ask `1979e2946a3346f0`: "SINCE YOU DONT HAVE THE RIGHT TO SERVE BY EMAIL, I WOULD LIKE TO SEE WHAT YOU HAVE PRESENTED TO THE COURT. || PLEASE SEND THE ORDER, TIME, AND PLACE."
  - Reply: "Response: Encouraging you to consult with counsel so that you understand how the ex parte process works."
- **`1980aad41bcc7b22`** — Lance Spiegel, 2025-07-14T20:42:53Z.
  - It follows C:settlement ask `1980a9fa8e91ccd2`, which asked him to withdraw the DVRO, stipulate and mediate, and ended "Please advise by July 21st 2025 whether Ms. Minor will accept this resolution."
  - Reply: "If you request the continuance on Wednesday, there will be no opposition. You are entitled to the continuance pursuant to the statute."
  - The reply text speaks only of a continuance.

### 3b. Firm refusal outside the ask's thread

- **`19b5cbba04495f7b`** — mvs@, 2025-12-26T22:15:50Z. Subject: "Minor - Petitioner's Objections to Respondent's Notice of Deposition".
  - Text: "Please see attached Petitioner's Objections to Respondent's Notice of Deposition. Per the attached, the deposition will not be proceeding as neither the deponent or her counsel are available."
  - Attachment: "2025-12-26 [P] Obj.Ntc.Depo.pdf".
  - It answers a formal deposition notice. It carries the same title as the "Petitioner's Objections" that Halsey's `19b8bc2c23730087` (2026-01-05) refers to.
  - His later asks for deposition dates got no firm reply in their threads: `19b5d526bad05170` (12/27), `19b6b024126d3ccd` (12/29) and `19b8bc2c23730087` (1/5).

### 3c. Firm conditions that answer no ask in this universe

- **`197a3724d248ab44`** — mvs@, 2025-06-24, sending the TRO and Notice of Hearing: "We encourage you to have the attached reviewed by legal counsel as soon as possible."
- **`19ab8474aa899682`** — mvs@, 2025-11-24T23:51:04Z.
  - It answers Halsey's 11/24 message "I have not been served". That message was sent from halsey@vividlabs.com to lances@ and AnnaK@, and appears here only as quoted text.
  - Text: "The document I sent you in the email attached is an unsigned, proposed stipulation, not a proof of service. [...] If you agree, I can send you the document via Docusign for signature. If you do not agree, you need only state you do not agree, and all parties will continue to proceed as required to by the Court."

### 3d. Not from the firm

- **Jeff Jacobson `197f1b0480aa5009`**, 2025-07-10T00:15:36Z: "Halsey: As the mediation was terminated on 12/6/24, I cannot respond to your correspondence. Jeff". He then sent the agreement (§2c).

---

## 4. Method

**Rules.** I followed INVENTORY/AGENT_RULES.md. Gmail access was read-only, and git was never run. The tracker files I consulted (DECISIONS D-77, build_report.py) were treated as data.

### 4a. Searches

All searches used includeTrash.

- **Q1:** `from:halsey2005@gmail.com to:ysfamilylaw.com after:2025/01/01`
  - Run one month at a time, because the whole window returns more than 50 threads.
  - Threads per month: 2025-01 3; 02 10; 03 9; 04 3; 05 0; 06 15; 07 5; 08 6; 09 0; 10 5; 11 9; 12 3; 2026-01 7; 02 6; 03 0; 04 1; 05 1; 2026-06-01 to 11-01 2.
  - Total: 85 hits, 80 distinct threads.
- **Q2:** `from:halsey@minorventures.com to:ysfamilylaw.com after:2025/01/01`
  - 7 threads, 6 of them not in Q1.
- **Q3:** `from:me cc:ysfamilylaw.com after:2025/01/01`
  - 0 threads.
  - In this mailbox `from:me` means the signed-in account Halsey@realitylab.com; every viewUrl carries authuser=Halsey@realitylab.com.
  - A control search, `from:me to:ysfamilylaw.com after:2025/01/01`, also returned 0.
- **Supplementary searches** for Cc and the other addresses:

  | Search | Threads | Notes |
  |---|---|---|
  | halsey2005@gmail.com with the firm in Cc | 35 | All already in Q1 |
  | halsey@minorventures.com with the firm in Cc | 7 | The same 7 as Q2 |
  | Halsey@realitylab.com with the firm in To/Cc | 0 | |
  | Halsey@realitylab.com, free text | 2 | 19fc5d7683f13539 and 19fd72e2b1b4651c. Their metadata shows every Halsey message went to kat.flds@gmail.com only. Bodies not read. |
  | halsey@vividlabs.com | 5 | 3 of them new |

- **Firm-sent searches,** used to check documents and replies:

  | Search | Threads |
  |---|---|
  | `from:ysfamilylaw.com after:2025/12/28 before:2026/01/03` | 2 |
  | `from:ysfamilylaw.com after:2026/02/21 before:2026/02/27` | 4 |
  | `from:ysfamilylaw.com objections after:2025/10/01 before:2026/01/10` | 7 |
  | `from:ysfamilylaw.com after:2026/04/09` | 7 |

  The last search shows that the latest firm-sent message in the mailbox dates from about 2026-07-21. So there is nothing from the firm after Halsey's 2026-08-08 asks.

### 4b. Inventory cross-check

- INVENTORY/gmail_inventory.tsv has 297 bucket-A rows dated 2025–2026. Of these, 135 were sent by Halsey: 130 from the brief's three addresses and 5 from halsey@vividlabs.com. They fall in 87 threads.
- The union of searches and inventory is 92 threads. One thread, `1955e97fcd9b65ee`, came from the inventory only.
- All 135 inventory rows were read. The searches found no in-universe message that is missing from the inventory.

### 4c. Reading

- All 92 threads were fetched with get_thread PLAIN_TEXT, with two exceptions:
  - The two realitylab threads were read METADATA_ONLY only. No firm address appears in any of their headers, and their bodies were not read.
  - The three Bcc threads were read METADATA_ONLY first. get_message was then used for the Halsey messages that Bcc'd the firm.
- Every Halsey message's own text was read in full, except `19ca3c3b9151b03c` (see §6).
- Quoted history was excluded: ">" lines, "On … wrote:" blocks, unprefixed iPhone-style quotes, forwarded blocks and Outlook-style headers. Other senders' text was read only to find replies.

### 4d. Counting rules

- **Universe:** a message is in if an `@ysfamilylaw.com` address appears in To or Cc. That includes paulf@ and aliciat@, not only the five addresses the brief named. Bcc-only and vividlabs messages are listed in §5d–5e and are not in the totals.
- **What counts as an ask:** a sentence that requests, demands, or asks a question seeking something.
- **What does not count:**
  - rhetorical questions;
  - statements about earlier asks (§5a);
  - conditional statements, for example "If you say you sent an email with initial financials, I will check it against Google logs." in `19ba01486b68901c`;
  - offers.
- **Asks addressed to someone else** are counted when the message copies the firm, because the brief's universe is every message to or copying the firm. This covers asks to Shannon, Jeff Jacobson, CourtCall, Det. Kale, "Perplexity" and the authorities. The to_cc column shows who each message was addressed to.
- **Days:** the UTC calendar date of the message timestamp, and the date in America/Los_Angeles. D-77's build_report.py shows Pacific dates.

### 4e. TSV conventions

- `||` separates the ask sentences of one message.
- `[...]` marks text I left out. Any other square brackets are my notes, not quotation.
- The `*` bold markers of the plain-text rendering are dropped in 19fdecd35a44d2ec and 19fded7384ca4b84.
- `none found` means no firm message in the same thread within 30 days.
- Reply excerpts are 200 characters or fewer. The excerpt for 1979e5eb9bbac178 is cut and ends `[...]`.

---

## 5. Lists not in the totals

### 5a. Statements about earlier asks

These are not counted as asks. All are quoted verbatim.

- **2025-02-21T17:03:27Z, `1952976d3b7935c4`** (to Shannon, cc firm):
  - "I am not advising you as your attorney as you appropriately suggested to me Lance while refusing to give me access to my own personal financial information counter to state law—the first of 28 times—"
  - "I am sure you will address all this in the information provided in the request for documents you have owed me by California state law for 18 months"
- **2025-02-24T22:32:10Z, `1953a17078d3a481`:** "given Lance’s behavior the last 28 times I have asked, likely a California record for ignoring a lawful standard disclosure request, I am disappointingly unlikely to receive what I have been owed by law for 18 months."
- **2025-02-27T00:21:18Z, `19544c77bf90eec8`:** "You have still not provided me with financial documents owed to me over a year ago by California Law,"
- **2025-02-28T16:54:27Z, `1954d7b19574d2b5`:** "Like Lance not giving me MY information after 28 polite and recorded requests — information he was legally obligated to provide."
- **2025-06-17T05:16:54Z, `1977c51ddad08b0a`:** "beyond the 44 requests denied for access to my own financial documents I could not see because Shannon set up exclusive account control [...] and the 28 emails sent by me askng for my information Shannon controlled exclusively that was denied or ignored"
- **2025-06-18T21:31:24Z, `19784f4960d89d36`:** "the consequences of your yet again potentially denying me my own money and information to enrich yourself."
  - The same message also says "These disclosures were never served on me by your side, in violation of these statutes." and "If you discover these documents in their original form with proper metadata, that will be considered." Both are statements, not asks.
- **2025-06-23T20:25:58Z, `1979e7813a178045`:** "You have failed to produce documents that I was owed 18 months ago, and that's the issue."
- **2025-06-24T19:14:36Z, `197a35d49eab7993`:** "18 months and you still can't prove you ever provided proper service. Blank forms in disclosures? No preliminary financials."
- **2025-08-30T21:48:31Z, `198fcf44b5f0e72a`:**
  - "Over the course of this litigation, I have made 28 separate, documented requests for the financial disclosures that California Family Code §§ 2100–2107 require each party to exchange."
  - "nor has she produced numerous financial records I've requested."
- **2025-10-09T01:15:22Z, `199c6897b4271990`:** "I am shocked that you claimed the Vanguard money is Shannon's and did not return it to me upon my request."
- **2025-11-21T01:47:35Z, `19aa4186c7fd4cf3`:** "I thoroughly documented your >10% compliance with my prior law firm's financial requests from the file directory they sent me"
- **2026-01-05T01:25:55Z, `19b8bc2c23730087`:** "your client's ongoing failure to provide mandatory preliminary financial disclosures after twenty (20) months"

### 5b. Borderline A asks, classed C

These are listed so the reader can reclassify them. If all five counted as A, A would be 5 messages on 4 UTC days (2025-03-24, 2025-07-09, 2025-07-10, 2026-08-08) or 3 Pacific days (2025-03-24, 2025-07-09, 2026-08-07).

- **2025-03-24T21:23:01Z, `195ca099809464eb`** (to shannonminor@, lances@, qijing@provinziano.com): "Hey Shannon, I need to get the social security numbers for Dan to complete my taxes." Classed C:tax.
- **2025-07-09T19:31:55Z, `197f0ac54f278a03`** (to Jeff@jjfamilylaw.com and the firm): "I demand that you and Lance immediately: [...] 2. Disclose to me exactly what you transmitted, to whom, and when;" Classed C:mediation.
- **2025-07-10T01:47:45Z, `197f2046dcf71650`** (to Jeff, cc the firm): "Please immediately send me your copy of the agreement I signed governing your conduct as a mediator." Classed C:mediation. Jeff, who is not the firm, sent it (§2c).
- **2026-08-08T00:36:58Z, `19fdecd35a44d2ec`** (to lances@):
  - "Please confirm immediately whether you, your firm, Shannon Minor, or anyone acting at your or your client’s direction requested, procured, transmitted, served, or otherwise caused this restriction."
  - "If so, please provide immediately a complete conformed copy of every document upon which the restriction is based".
  - The restriction is on his own bank accounts. Classed C:process because it asks for legal process, not for his records.
- **2026-08-08T00:47:54Z, `19fded7384ca4b84`:** the same text re-sent 11 minutes later to lances@, with Bcc to 12 non-firm addresses.
  - The only replies in the thread are a bounce and Craig Walker (craig@dialpad.com): "Yeah.Paulsy, I think you sent this to the wrong email. This is Craig Walker, not Lance."
  - The firm sent nothing after these two messages.

### 5c. A or B wording in mail that went to no firm address

These are outside the universe.

- **2025-03-09T20:07:43Z, `1957c854b51348fa`** (cc Provinziano addresses only):
  - "Lance and Shannon I'm upset about your decision to force me to spend significant sums to obtain my own financial records."
  - "I also haven't received my financial information, which the law requires, despite 28 polite requests."
- **2025-07-24T05:31:54Z, `1983aeaaaf2f91a4`** (to Brmlaw10@gmail.com): "It started over asking for initial financial disclosures still not served."
- **2025-11-25T01:01:00Z, `19ab887364253d48`** (to kat.flds@gmail.com only): "Katherine, do you have my motion to compel Lance to provide initial financial statements and the 95% of information requested by my prior law firm that has yet to be delivered?"

### 5d. Firm only in Bcc

Three messages, not counted. None contains an A or B ask.

- **`19b9f2e529d79fbc`**, 2026-01-08T19:56:11Z, to BHPD/City: no ask.
- **`19b9f636a1ef17f8`**, 2026-01-08T20:54:10Z, to info@da.lacounty.gov: "I request an immediate independent investigation into this leak and the compromise of the Chain of Custody."
- **`19ba0331e15a53ff`**, 2026-01-09T00:41:02Z, to LosAngeles@fbi.gov: "I request that the federal government preserve the Google logs for my account immediately before they are overwritten."

### 5e. Sent from halsey@vividlabs.com with the firm in To or Cc

Five messages. This address is outside the brief's set, so they are not counted.

- **`197a363a1527b7c2`**, 2025-06-24T19:21:30Z: "Please review the attachment as well as your client." The attachment, "Final Formal Demand Letter.pdf", was not read.
- **`199e45bc07381dc6`**, 2025-10-14T20:13:50Z: "Are you missing a page or a document?" AnnaK answered in `199e45d488541702`: "No, that was the complete document."
- **`19c950ecec081c5a`** (2026-02-25T13:48:09Z), **`19c951a59335a917`** (2026-02-25T14:00:40Z) and **`19d6e912802d6022`** (2026-04-08T19:28:07Z): no ask.

**This list is incomplete.** halsey@vividlabs.com is a separate account; its messages here carry no SENT label. Its mail appears in this mailbox only when it copied an address delivered here. For example, the 2025-11-24 message "I have not been served" (halsey@vividlabs.com to lances@ and AnnaK@) exists here only as quoted text inside `19ab8474aa899682` and `19ab8839844998ec`.

---

## 6. Limits

- **Attachments were not read.** The only category decision taken from an attachment is #2, `1978bb2792558e91`, and that relies on the title alone. Attachments Halsey sent that may contain asks include:
  - "Demand for Immediate Financial Disclosure and Compliance with Legal Obligations.pdf" (1978bb2792558e91);
  - "June_18_Demand_Letter.pdf", the prenup and "The Plan" (19784f4960d89d36);
  - "Motion_to_be_filed_2025-08-30T213612Z.pdf" (198fcf44b5f0e72a);
  - "Harassment_Unsolicited_Advise_Malintended.pdf" (198fd63ce12bceeb, whose body is empty);
  - "Final Formal Demand Letter.pdf" (vividlabs 197a363a1527b7c2);
  - "BHPD Case #24STFL00432 — Marsy_s Law Compliance Analysis & IA Referral copy.pdf" (19c5192768d57a0b);
  - index.html (19aa4186c7fd4cf3).

  None of the firm's attachments was read either: the I&Es, the RFP responses and the orders.
- **Partial read: `19ca3c3b9151b03c`.** This is the 2026-02-28 "CRIMINAL COMPLAINT AND REQUEST FOR ARREST WARRANT FOR LANCE ...", sent to the authorities with cc lances@.
  - Read in full: the opening, section III and section X.
  - The remaining ~1,000 lines were only keyword-searched, for: request, demand, please, provide, produce, ?, disclos, financial, records, statement, FL-1, PDD, preliminary, my own, my information, copies, send me.
  - **Not every line was read.** No A or B ask was found.
  - Its asks are addressed to the authorities and counted as C:investigation.
- **Missing messages.** In 15 threads the messageCount is higher than the number of messages get_thread returned. get_thread omits drafts. The gaps are 1946b867c6b86d86 16/15, 19539e547dd499aa 30/27, 195491711bcd93ab 5/4, 195499fb69cbd995 16/15, 1974ca73931de1bd 3/2, 19751efd03ef9f8a 11/10, 18da4c2fe5eb3cd1 3/2, 1978bb2792558e91 3/2, 199c5dc7db16c037 3/2, 19a8103710fd50a6 3/2, 19b5c4e233f60118 4/3, 19b8f1dd4d7a670c 18/10, 19c4f9dc9d26b93f 5/4, 19c9262bb219c577 8/7 and 19ca398af605f23a 9/7. No inventory row points to a message that was not returned.
- **AI-LEAD (rule 6): AI-written text pasted into messages Halsey sent.** It is not evidence. An ask in such a message is counted only because Halsey sent it.
  - `19ab9218ce36c50a` opens "Absolutely — here is the same hybrid letter, fully preserved in content, but now cleanly formatted for Apple Mail...". Its B ask (#9) is counted.
  - `19b8f1dd4d7a670c` embeds a report headed "FROM: Forensic Data Analysis Unit". The requests inside that report are not counted.
  - `19a7a9b6420826c5` contains a service-of-process guide with web sources [1]–[102]. Only the ask in the preamble is counted.
  - `19b9fffde8c412a1` and `19c9262bb219c577` cite "Gemini" opinions. Neither has an ask.
  - `1979e2dcb382217d` contains a legal explainer on e-service. It has no ask.
- **Scope.** Only this mailbox was searched. Anything before 2025-01-01 is outside this window.
- **Halsey's own count of 28.** It appears in his messages dated 2025-02-21, 02-24, 02-28, 2025-03-09 (outside the universe), 2025-06-17 ("28 emails") and 2025-08-30 ("28 separate, documented requests for the financial disclosures").
