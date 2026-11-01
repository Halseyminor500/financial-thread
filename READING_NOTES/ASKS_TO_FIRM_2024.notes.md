# Asks to the firm (ysfamilylaw.com), calendar 2024: full-reading count

Request: Halsey Minor, 2026-11-01: "check how many times I asked him for my own information and for the initial financial statements".
Reader: full-reading subagent, 2026-11-01. Rules: /home/user/spiegel-thread/INVENTORY/AGENT_RULES.md, obeyed. Gmail used read-only (search_threads, get_thread, get_message only). No git run. Files written: this file and /home/user/spiegel-thread/INVENTORY/asks_to_firm_2024.tsv. Scratch work: /tmp/claude-0/-home-user/9a86eccf-071d-5c97-88ae-ef129ec55f9d/scratchpad/ (not deliverables).
These notes record what the messages say. Category assignments are this reader's classification under the brief's definitions; borderline calls are listed in section 7 so they can be re-judged.

## 1. Universe

Every message dated 2024 (UTC) whose sender is halsey2005@gmail.com, halsey@minorventures.com or Halsey@realitylab.com and whose To or Cc header holds a ysfamilylaw.com address. Bcc was not used.

Result: **65 messages in 47 threads** (58 from halsey2005@gmail.com, 7 from halsey@minorventures.com, 0 from Halsey@realitylab.com). This equals the 2024 bucket-A rows of gmail_inventory.tsv whose sender is Halsey (65 rows, 47 threads), message for message. The TSV takes date, sender, To and Cc from the inventory headers. For the 47 messages read from inline results, the date, sender, To and Cc I transcribed match the inventory exactly. For the 18 read from saved files, the date in the file matches.

Searches (all includeTrash=true, pageSize 50, none reached the cap):

| Query | Threads |
|---|---|
| `from:halsey2005@gmail.com to:ysfamilylaw.com after:2024/01/01 before:2025/01/01` | 44 |
| `from:halsey@minorventures.com to:ysfamilylaw.com after:2024/01/01 before:2025/01/01` | 5 |
| `from:me cc:ysfamilylaw.com after:2024/01/01 before:2025/01/01` | 0 (empty result). `from:me to:ysfamilylaw.com` (same dates) also returned 0, so the `from:me` operator returned nothing in this API. Replaced by the next four rows. |
| `from:halsey2005@gmail.com cc:ysfamilylaw.com` (same dates) | 19 |
| `from:halsey@minorventures.com cc:ysfamilylaw.com` (same dates) | 4 |
| `from:halsey@realitylab.com ysfamilylaw.com` (same dates) | 0 |
| `in:sent (to:ysfamilylaw.com OR cc:ysfamilylaw.com)` (same dates) | 47 |
| `in:sent (to:ysfamilylaw OR cc:ysfamilylaw OR to:lances OR cc:lances OR to:spiegel OR cc:spiegel OR to:annak OR cc:annak OR to:mvs OR cc:mvs OR to:vivianh OR cc:vivianh)` (same dates) | 47 |
| `(from:halsey2005@gmail.com OR from:halsey@minorventures.com OR from:halsey@realitylab.com) (to:ysfamilylaw OR cc:ysfamilylaw)` (same dates) | 47 |
| `in:sent bcc:ysfamilylaw.com` (same dates) | 0 |

The union of the address queries is the same 47 threads as the inventory. `in:sent ysfamilylaw` (keyword) returned 50 threads (cap; estimate 104). It also catches sent mail that only mentions the firm (forwards, quoted signatures). Those messages are outside the universe and were not reviewed.

## 2. How each message was read

- **Own text read in full** for all 65: every word above the first quote attribution ("On ... wrote:", "From: ... Sent:", "---------- Forwarded message"), plus every non-quoted line after it (checked for inline answers; none found). **Quoted history (">" lines and Outlook-style quoted blocks) was not read word by word** and nothing in it was counted. Exception: in 18d65cc5dbd32aa5 and 18d65eebafa5fea2 (Anna Kralle, "Please see below.") the forwarded Lance Spiegel text was read, because it is the firm's reply.
- **get_thread PLAIN_TEXT** for 36 threads. In 4 threads with 3 or more messages (1914ca5f58011520, 192b1189b802a9e4, 1913940c28b7e70a, 1917bf993cc8b2d8) get_thread FULL_CONTENT was used, so that large results went to a file; only its plaintextBody field (the field PLAIN_TEXT returns) was read. In 8 multi-message threads whose get_thread METADATA_ONLY listing shows no firm-sent message, the Halsey messages were read with get_message PLAIN_TEXT: 191053d68e3f0cb0, 191149c08b90508a, 191b8ed50b3a8d69, 191bb174ef051ceb, 191fb1c00f129802, 1928de22c2ed57ce, 192acad72a6035b6, 192acba36b560229.
- **Firm messages** in these threads: own text read in full (the firm's standard signature and disclaimer lines skipped).
- **Listed fewer than messageCount:** 18d424f91222fab9 (21 total, 17 listed) and 192aba5b76e8cd03 (5 total, 3 listed). The unlisted messages were not seen; get_thread's description says drafts are omitted.
- **Verbatim check:** 28 ask sentences from threads saved to file were checked by script against the message text (all matched); the other 67 were transcribed from results returned inline and were not machine-checked. 6 of the 7 distinct reply excerpts, and the firm quotes in section 5.2, were checked by script against saved files. The exception in both is the text of `18d6598e61e8abf0`, which was transcribed from an inline result.

## 3. Classification applied

- **Ask** = an explicit request, demand or question seeking something. Not counted: closing courtesies ("I look forward to your cooperation"), statements about earlier refusals, offers, threats with no request, and rhetorical questions (each excluded one is named in section 7).
- **A, his own information**: his records, accounts, funds, data, documents or property; copies of what the firm or Shannon hold about him. This includes joint accounts where he frames the request as "my funds" / "my money", his email account's use, and figures he needs for HIS own disclosure.
- **B, initial financial statements**: preliminary declaration of disclosure; FL-140/142/150; income and expense declaration; schedule of assets; "financials"; Shannon's financial statements, accounts or balances; the Vanguard/Wells Fargo statements.
- **C, other**: one-word label.
- **Counting:** a message counts once per category, however many ask sentences it carries (D-77: "A message is counted once, however many asks it carried"). One message can count in A and B. **A (borderline)** = a soft ask with no imperative or question, reported separately. **Days**: Pacific (America/Los_Angeles) dates and UTC dates are both given; they differ for messages sent in the Pacific evening.

## 4. Totals

| Category | Messages | Different days (Pacific) | Different days (UTC) | First | Last |
|---|---|---|---|---|---|
| A, his own information (strict) | 13 | 11 | 10 | 2024-02-01T02:57:22Z `18d62997d6b16748` | 2024-10-28T21:12:24Z `192d4f936e79866d` |
| A including borderline | 15 | 12 | 12 | 2024-02-01T02:57:22Z `18d62997d6b16748` | 2024-10-28T21:12:24Z `192d4f936e79866d` |
| B, initial financial statements | 3 | 3 | 3 | 2024-07-19T15:49:20Z `190cbaf290e12a0f` | 2024-10-28T21:12:24Z `192d4f936e79866d` |
| A or B (strict) | 14 | 12 | 11 | 2024-02-01T02:57:22Z `18d62997d6b16748` | 2024-10-28T21:12:24Z `192d4f936e79866d` |
| C, any other ask | 31 | 25 | 24 | 2024-02-01T02:57:22Z `18d62997d6b16748` | 2024-10-28T22:40:05Z `192d5498888869d9` |
| Any ask | 42 | 31 | 29 | 2024-02-01T02:57:22Z `18d62997d6b16748` | 2024-10-28T22:40:05Z `192d5498888869d9` |
| No ask at all | 23 | 17 | 18 | 2024-02-01T18:43:28Z `18d65fbaa800d558` | 2024-12-16T14:07:30Z `193cfcba96b5c6e9` |

All 65 messages: 42 carry at least one ask, 23 carry none (65 = 42 + 23).

### 4.1 A, his own information (strict)

Asked 13 times, on 11 different days (Pacific dates; 10 by UTC date), from 31 Jan 2024 to 28 Oct 2024 (Pacific). First: `18d62997d6b16748` 2024-02-01T02:57:22Z. Last: `192d4f936e79866d` 2024-10-28T21:12:24Z.

| # | date_utc | Pacific date | message_id |
|---|---|---|---|
| 1 | 2024-02-01T02:57:22Z | 2024-01-31 | `18d62997d6b16748` |
| 2 | 2024-02-01T14:10:08Z | 2024-02-01 | `18d65016abf6add9` |
| 3 | 2024-02-01T17:35:47Z | 2024-02-01 | `18d65bdb44e8f4fe` |
| 4 | 2024-02-01T18:06:19Z | 2024-02-01 | `18d65e5f80e56279` |
| 5 | 2024-02-28T06:40:11Z | 2024-02-27 | `18dee71313ef2164` |
| 6 | 2024-06-24T22:30:53Z | 2024-06-24 | `1904c5f9feddc769` |
| 7 | 2024-07-14T00:01:00Z | 2024-07-13 | `190ae8b6b2ad2499` |
| 8 | 2024-07-19T15:49:20Z | 2024-07-19 | `190cbaf290e12a0f` |
| 9 | 2024-07-23T22:38:30Z | 2024-07-23 | `190e1bf05610cbf3` |
| 10 | 2024-08-13T23:23:59Z | 2024-08-13 | `1914e0e6404edc78` |
| 11 | 2024-08-17T03:13:17Z | 2024-08-16 | `1915e53383cbfb56` |
| 12 | 2024-08-22T15:13:17Z | 2024-08-22 | `1917aa6f57cad088` |
| 13 | 2024-10-28T21:12:24Z | 2024-10-28 | `192d4f936e79866d` |

A (borderline), not in 4.1: `18db34acd305cd09` (2024-02-16) and `1915bc216b362f39` (2024-08-16). With them: asked 15 times, on 12 different days (Pacific; 12 by UTC date).

### 4.2 B, initial financial statements

Asked 3 times, on 3 different days (Pacific dates; 3 by UTC date), from 19 Jul 2024 to 28 Oct 2024 (Pacific). First: `190cbaf290e12a0f` 2024-07-19T15:49:20Z. Last: `192d4f936e79866d` 2024-10-28T21:12:24Z.

| # | date_utc | Pacific date | message_id |
|---|---|---|---|
| 1 | 2024-07-19T15:49:20Z | 2024-07-19 | `190cbaf290e12a0f` |
| 2 | 2024-10-22T15:08:09Z | 2024-10-22 | `192b4c56f932189e` |
| 3 | 2024-10-28T21:12:24Z | 2024-10-28 | `192d4f936e79866d` |

Two of the three B messages also count in A (`190cbaf290e12a0f`, `192d4f936e79866d`). The only B ask that is not also an A ask is `192b4c56f932189e`, which refers to the other side's 'mandatory financial disclosure'.

### 4.3 C, other (by label)

| C subcategory | messages | Pacific days | UTC days | message_ids |
|---|---|---|---|---|
| C:assurance | 1 | 1 | 1 | `18df122430e5e248` |
| C:billing | 1 | 1 | 1 | `190cbaf290e12a0f` |
| C:corporate | 1 | 1 | 1 | `18d62997d6b16748` |
| C:custody | 6 | 4 | 4 | `192831cb2bc68a02`, `192acad72a6035b6`, `192acba36b560229`, `192b46097eb9a2c9`, `192b4c56f932189e`, `192d5498888869d9` |
| C:equipment | 1 | 1 | 1 | `18e621a8349a0268` |
| C:filings | 4 | 3 | 3 | `18da4403caf1c684`, `18da4a915a927293`, `1906f540755b5bfc`, `190e1bf05610cbf3` |
| C:insurance | 5 | 5 | 5 | `191053d68e3f0cb0`, `1917c70374c2b544`, `191809418abf3100`, `191fb1c00f129802`, `192b1841939b70ba` |
| C:mediation | 3 | 3 | 3 | `18e5c7e0b122f810`, `18ea161400dbc944`, `18fca944348d1f02` |
| C:payment | 2 | 2 | 2 | `191b8ed50b3a8d69`, `191f446e06107203` |
| C:procedure | 1 | 1 | 1 | `190ae8b6b2ad2499` |
| C:restitution | 5 | 3 | 3 | `18d9f9dbabcb51a2`, `18da3778195f3e92`, `18da40445a014287`, `190e1bf05610cbf3`, `190e1c2c61ef406a` |
| C:schooling | 1 | 1 | 1 | `18df6063656b1eb7` |
| C:settlement | 2 | 2 | 2 | `19023a0d80a25376`, `190e1bf05610cbf3` |

C:mediation includes one borderline row (`18fca944348d1f02`, 'I have no dial in information.').

## 5. Firm replies (same thread, within 30 days)

Five messages with an ask have a firm-sent message after them in the same thread within 30 days (8 TSV rows, since two of them count in more than one category). Two messages without an ask (`190c7b10f2af0aa2`, `190c83daeeae325e`) also have one (`190cc20282dd83c3`), and the TSV shows it. Every other row says "none found". 41 of the 47 threads contain no firm-sent message at all. The 6 that do are 18d424f91222fab9, 18d64fbeb13f840e, 18ea11c7a1b64cd0, 190c2fad1c4fd49a, 190dcf708ca9607b and 190e0eee763559a9.

| Ask message | Firm reply | Reply date | Attachments on the reply |
|---|---|---|---|
| `18d62997d6b16748` (A; C:corporate) | `18d659c74c96f2f5` Lance Spiegel (to halsey@minorventures.com and Anna Kralle; Anna re-sent it at 17:14:03Z, `18d65a9dad2be7d3`, saying it had bounced) | 2024-02-01T16:58:59Z | none |
| `18d65016abf6add9` (A) | `18d6598e61e8abf0` Lance Spiegel | 2024-02-01T16:55:06Z | none |
| `18d65bdb44e8f4fe` (A) | `18d65cab1560dea3` Lance Spiegel (re-sent by Anna Kralle at 17:51:43Z, `18d65cc5dbd32aa5`) | 2024-02-01T17:49:27Z | none |
| `18d65e5f80e56279` (A) | `18d65eebafa5fea2` Anna Kralle, "Please see below.", forwarding Lance Spiegel's text | 2024-02-01T18:29:14Z | none |
| `190cbaf290e12a0f` (A; B; C:billing) | `190cc20282dd83c3` Matthew Sirriyeh | 2024-07-19T17:52:52Z | four files, each named "Filing Rejected Notification for Case No. 24STFL00432 (Minor, ShannonvsMinor, Halsey),Filing Rejected Notification for Case No. 24STFL00432 (Minor, ShannonvsMinor, Halsey).eml" |

`1906f540755b5bfc` (2024-07-01, C:filings: "Did you file?" / "Can I see what you filed?"): no firm message is listed after it. Its thread has 4 unlisted messages.

### 5.1 Firm replies that produced a document

Only one in-thread reply carried attachments: `190cc20282dd83c3` (2024-07-19). It attached the four court "Filing Rejected Notification" emails named above. **No in-thread firm reply attached any document of category A or B.**

### 5.2 Asks answered with a refusal or a condition (verbatim)

- To `18d62997d6b16748` (A; 2024-02-01T02:57:22Z), Lance Spiegel, `18d659c74c96f2f5`, 2024-02-01T16:58:59Z: "These are issues that can and will be addressed in the dissolution proceedings. Important for you to have independent counsel. If you have not already done so, I strongly encourage you to retain a lawyer."
- To `18d65016abf6add9` (A; 2024-02-01T14:10:08Z), Lance Spiegel, `18d6598e61e8abf0`, 2024-02-01T16:55:06Z: "It is very important for you to retain counsel so that you have a complete understanding of the process, including how to address the issues mentioned in your email. If you have not already done so, please refer the Notice and Acknowledgment of Receipt to your counsel."
- To `18d65bdb44e8f4fe` (A; 2024-02-01T17:35:47Z), Lance Spiegel, `18d65cab1560dea3`, 2024-02-01T17:49:27Z: "It is not possible for me to give you legal advice. Please consult with counsel to confirm my comment that the process includes an opportunity to obtain the information that you are requesting. Both you and Shannon are required to make full and complete disclosure of financial information. Shannon and I both would like to amicably resolve the issues but that preference does not mean that you and she will not be entitled to request and obtain the kind of financial information mentioned below. There is nothing “aggressive” about my urging you to hire a lawyer. The suggestion is intended to assure that your rights are protected and to avoid unnecessary expense and delay."
- To `18d65e5f80e56279` (A; 2024-02-01T18:06:19Z), Lance Spiegel's text forwarded by Anna Kralle, `18d65eebafa5fea2`, 2024-02-01T18:29:14Z: "I am not going to debate how this process works. I’d like to avoid the necessity of personally serving you with the Petition. Please advise whether you intend to sign and return the Notice and Acknowledgment of Receipt that was sent to you last week."
- To `190cbaf290e12a0f` (A and B; 2024-07-19T15:49:20Z), Matthew Sirriyeh, `190cc20282dd83c3`, 2024-07-19T17:52:52Z. This is not a refusal, and the reply does not mention either request. Its full text: "The tax return you filed with the court bears our client’s unredacted social security number on pages 1, 20, 21, 28 and 31. Going forward, please refrain from filing any documents that contain our client’s confidential or sensitive information with the court, including, but not limited to, any document that bears her unredacted social security number. Also, I emailed you yesterday to inform you that all of the documents you filed yesterday were rejected by the Court. The four rejection emails are attached for your review. Lastly, Mr. Jacobson also emailed you yesterday and offered again to have his assistant Debbie file your Response and Declaration Under UCCJEA with the court. We highly suggest you take Mr. Jacobson up on his offer."

### 5.3 Firm messages to him in 2024 in OTHER threads that carried documents

These are not replies under the same-thread rule. They are listed so that nothing the firm sent in 2024 is missed. Only the dates are stated; no link between any of them and an ask is asserted. The 2024 firm-sent messages in the inventory number 21. All 21 were seen with their attachment lists (14 inside the ask threads, 7 outside). Attachment names only: no PDF was opened.

- `18da4c2fe5eb3cd1`, Anna Kralle, 2024-02-13T23:17:29Z, "Case Inititation Documents", body "Please see the attached documents along with the Notice and Acknowledgment for your signature.". Attachments: 2024-01-12 [P] UCCJEA.pdf; 2024-01-12 Fam.Law.Cover.Sheet.pdf; 2024-01-12 Petition.pdf; 2024-01-12 Summons.pdf; 2024-01-12 [C] Order.Share.Financial.Info.pdf; fl120.pdf; fl105.pdf; FL117 NAR.pdf. Dated 28 minutes after `18da4a915a927293` (2024-02-13T22:49:20Z, C:filings), which asked "please resend The Petition (FL-100) and the Summons (FL-110) documents".
- `19157ba8e41220f7`, Anna Kralle, 2024-08-15T20:28:38Z, "Minor RFO", body "The attached documents have been sent to you via mail. We are sending an email as a courtesy copy to you as well.". Attachments: 2024-08-14 [C] Order.FCCRC.pdf; 2024-08-14 [C] Order.Mediation.pdf; **2024-08-14 [P] I&E.pdf**; 2024-08-14 [P] POS.pdf; 2024-08-14 [P] RFO.CC.CS.SS.pdf. This is the only 2024 firm email whose attachment name indicates a category-B document (an income and expense declaration, by its file name). The only other 2024 firm attachment whose name mentions financial information is "2024-01-12 [C] Order.Share.Financial.Info.pdf", named as a court order, in the January service packet.
- `192e4eb48f4671cf`, Matthew Sirriyeh, 2024-10-31T23:30:57Z, "Minor - Petitioner's Subpoenas to Various Entities". Attachments: 16 files named "2024-10-31 [P] Ntc.Cons.Doc.Subp.<entity>.pdf", one for each of: Abramson Saliba & Associates; Vivid Labs Holdings, Inc.; Live Planet, Inc.; Life Lab Ventures, LLC; Uphold, Inc.; Uphold HQ, Inc.; Ally Bank; Ally Financial Inc.; Ally Servicing LLC; Wells Fargo Bank, N.A.; Banc of California; First-Citizens Bank & Trust Company; Goldman Sachs Bank USA; Capital One, N.A.; SoFi Lending Corp.; Truist Bank. `192e4f2f43647e39` (23:39:35Z) re-sent them as a ShareFile link after the halsey@minorventures.com copy bounced (attachment: "Undeliverable: Minor - Petitioner's Subpoenas to Various Entities.eml").
- `19340b0eb2056651`, Anna Kralle, 2024-11-18T19:12:32Z, "Minor", body "Please see the attached correspondence.". Attachment: 2024-11-18 Ltr.LSS.HM.pdf. **Not read** (Drive copy drive:1Sr6fgmUNqhXhplaaBnFOwlwMuwfGRWge, 13,328 bytes, per drive_inventory.tsv). It is dated 21 days after `192d4f936e79866d` (2024-10-28, A and B), which set a 21-day deadline. Whether the letter answers that request is not established here.
- Firm attachments in the ask threads that were not replies to an ask: `18d424f91222fab9` (2024-01-25) and `18d617333d82df9a` (2024-01-31): 2024-01-25 Ltr.LSS.Halsey.pdf; FL117 NAR.pdf; 2024-01-12 Petition.pdf; 2024-01-12 Summons.pdf; 2024-01-12 [P] UCCJEA.pdf; 2024-01-12 Fam.Law.Cover.Sheet.pdf; 2024-01-12 [C] Order.Share.Financial.Info.pdf; fl120.pdf; fl105.pdf. `18ea11c7a1b64cd0` (2024-04-02): 2024-04-02 [P] Fam.Rogs.Set 1.pdf. `190c2fad1c4fd49a` (2024-07-17): 2024-07-01 [R] Resp.Petition [REJECTED].pdf; 2024-07-13 [R] Decl.UCCJEA [REJECTED].pdf. `190dcf708ca9607b` (2024-07-23): 2024-03-08 Ntc.Ack.Receipt.Petition.pdf.
- No 2024 firm email in this mailbox has an attachment whose name indicates a preliminary declaration of disclosure (FL-140/FL-142). Petitioner's PDD dated 6/17/2024 is in Drive (/home/user/spiegel-thread/READING_NOTES/PDD_2024-06-17_content.notes.md). How it reached him is not established by this task.

## 6. His own statements, in these messages, about earlier requests (quoted; not counted as asks)

- `18db34acd305cd09` (2024-02-16): "your deliberate obstruction of my access to my own bank statements"; "your refusal to provide access to the accounts into which my personal property has been diverted for the past 18 years"; "your refusal to disclose my own financial records".
- `18df122430e5e248` (2024-02-28): "Moreover, you have denied me access to my own financial records, citing the control of account passwords by your client as justification."
- `1904c5f9feddc769` (2024-06-24): "I have been asking for this information for months without success Including in mediation until you walked out."
- `190cbaf290e12a0f` (2024-07-19): "I have an ever growing file of your firm denying me access to my own sole, personal asset and financial records."
- `190e1bf05610cbf3` (2024-07-23): "after 6 months of deliberately stone walling me and depriving me of my rights to my own financial information"
- `1915e53383cbfb56` (2024-08-17): "Lance has my financials."
- `1917aa6f57cad088` (2024-08-22, to Shannon): "A 1 year printout is unacceptable to me and the state of California."
- `192d4f936e79866d` (2024-10-28): "I have repeatedly requested this information over the past nine months, but without success."

Non-firm context, thread `1914ca5f58011520`, from the mediator Jeff Jacobson (jjfamilylaw.com, not the firm). Only the first 400 characters of each of these two messages were read. 2024-08-13T16:50:26Z: "I have checked with Shannon regarding the account information that you are looking for. She received information from Wells Fargo regarding the 1074 account below. Shannon also indicated that she has not used any other accounts associated with you for "well over a year"." 2024-08-16T16:14:30Z (`1915bf8213dcf550`): "Shannon has again looked into the Wells Fargo account and it sounds like you can access all the information you need through Wells Fargo."

## 7. Borderline calls and exclusions (for re-judging)

- **A (borderline):** `18db34acd305cd09` (only ask: "I hope for your understanding and prompt action to rectify this situation, allowing us to proceed with the divorce in a fair and just manner." It follows a sentence about records and misappropriation, so it could also be read as restitution). `1915bc216b362f39` ("This is not about getting her financials. It is an issue of getting my financials." This states the object of his request and has no imperative; it also says expressly that he is NOT asking for her financials).
- **A rather than B:** `18d65016abf6add9` (bank and credit card statements "where my funds were utilized"); `18dee71313ef2164` (figures for HIS own disclosure); `1904c5f9feddc769` ("As part of the process of disclosure", but the object is "my financial accounts"); `190ae8b6b2ad2499` ("grant access to my electronic financial records". Its pasted block on the disclosure rules is not a request).
- **Counted in both A and B:** `190cbaf290e12a0f` (one sentence: "financial documents from Shannon" = B; "names and passwords of accounts that hold or held my personal assets" = A; "should have served me with FL150" listed under B). `192d4f936e79866d` (access to all accounts and records = A; "A complete list of all financial accounts Shannon has opened, managed, administered, or used" = B).
- **B only:** `192b4c56f932189e` (the other side's "mandatory financial disclosure").
- **Not B:** `191809418abf3100` ("Where is this money coming from if not from my child support?", a question about the children's insurance, labelled C:insurance).
- **Not counted (implicit or rhetorical):** `1906f64363cf78a5` ("Happy to help work on it but I was to have been given this months ago completed."); `18d9f9dbabcb51a2` ("This not only deprives me of rightful access to my own financial records and resources", a statement); `1917aa6f57cad088` ("How many times have you taken huge amounts of my money and lied to me about our finances?", rhetorical); `192acad72a6035b6` ("Jon where the hell have you been?" / "Jeff, where have you been?", rhetorical, to his own counsel and the mediator); `190ae8b6b2ad2499` ("However, you may want to amend them.", a suggestion).
- **Addressee note:** in 25 of the 65 messages the firm is only in Cc. The To line in those is Shannon, the mediator Jeff Jacobson, his office or others. Their asks are counted because the brief's universe is every message to or copying the firm. The TSV to_cc column shows who each message went to.

## 8. AI material (rule 6)

No AI-LEAD document was opened. Three sent emails contain AI-related text. Their bodies were read as the record of what he sent, and only his own sentences were counted. `18da3778195f3e92` begins with the word "ChatGPT". `190ae8b6b2ad2499` contains a pasted block on California disclosure rules beginning "In California, failing to provide financial information in a divorce violates specific legal obligations". `190c83daeeae325e` discusses ChatGPT form-filling.

## 9. Not done / limits

- Quoted history inside his messages was not read word by word (section 2).
- Unlisted messages in 18d424f91222fab9 (4) and 192aba5b76e8cd03 (2) were not seen.
- No attachment was opened. The 2024-11-18 letter (section 5.3) is unread.
- Sent mail that mentions the firm without being addressed to it was not reviewed (the `in:sent ysfamilylaw` result is 50 threads at the cap, estimate 104).
- Firm replies were taken from the same thread only, as the brief requires. Section 5.3 lists firm documents sent in other threads.
