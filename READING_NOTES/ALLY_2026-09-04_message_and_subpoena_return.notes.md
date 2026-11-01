# Reading notes — Ally 2026-09-04 secure message; Ally subpoena returns (behavior g)

Reader: subagent, 2026-11-01. Read-only. Halsey Minor = victim / reporting party.
Rules: INVENTORY/AGENT_RULES.md. Quotes are verbatim. Nothing inferred. Coverage gaps are stated per item.

---

## 1. Ally secure message of 2026-09-04

### 1a. drive:1k2YTcHZ_ILuf7bg5hYwjPgiiqjac1RIT — "2026-09-04__ally.com__SecureMessageAtt.html"
- Metadata: text/html, 879,530 bytes, created 2026-09-04T18:16:36Z, parent 19_XO6BzLQD4gsbh6f_uo9DzlLYiatQQ9.
- Downloaded in full (base64 decoded to 879,530 bytes) and parsed in full.
- **What the file is:** a Proofpoint Encryption envelope (`<title>Proofpoint Encryption</title>`). The form posts to `https://securemail.ally.com/formpostdir/safeformpost.aspx`. It holds hidden fields `rcptData`, `rcptLocale` ("enus") and `msg0`–`msg438`.
- **All visible text in the file, verbatim (after the HTML is stripped):**
  > Proofpoint Encryption If you do not see a button or clicking the button yields no action, please click the link in the message. More Info Disclaimer : This email and its content are confidential and intended solely for the use of the addressee. Please notify the sender if you have received this email in error or simply delete it. Secured by Proofpoint Encryption, Copyright © 2009-2026 Proofpoint, Inc. All rights reserved.
  The button label reads "Click to read message". The "More Info" link goes to `https://securemail.ally.com/securereader/help.jsf?lang=enus`.
- **The message body is encrypted.** The `msg*` fields join into a 624,956-byte `secure-doc` (sigaba namespace, `ty="SSMAIL"`, `id="db800955-7a23-4442-92fc-4021fa22c797"`, `len="915286"`). Its `<encrypted-data en="Base64" ci="AES-256" co="Gzip"/>`. It can be opened only through Ally's securemail server, which means logging in, which counts as outbound contact under the rules. It was NOT decrypted.
  **Result: the text of Ally's 2026-09-04 message (what it says about the restriction, any writ, levy, court order, levying officer, case number, amount, attorney or firm, and any request or offer) is not in this export. None of it can be transcribed from this file.**
- Readable envelope metadata (not message content):
  - rcptData (decoded): `reply-to` = depositsecr@ally.com; `reply-from` = halsey2005@gmail.com; `subject` = "FLFNCAEBGMGMHJCAECGBGOGL" (encoded); `forward-enabled` false; `reply-enabled` true.
  - identity-data (decoded): Issuer "mechanism/Proofpoint Filter CryptoAPI@CBAE8CC4-…"; `<Date>2026-09-04T10:42:032-07:00</Date>`; `<EncryptionDomain>ally.com</EncryptionDomain>`.
  - signature-data: ECDSA-SHA256 signature over `SSMAIL:db800955-7a23-4442-92fc-4021fa22c797`.
- No case number, ECR number, amount, writ, levy, levying officer, attorney or law firm appears anywhere in the readable parts of the file.

### 1b. Gmail message carrying the attachment — thread/msg 1a06da1478a8cadd (read in full)
- From "DepositsECR@ally.com" to halsey2005@gmail.com. Date 2026-09-04T18:14:08Z. Subject "[] Ally Bank". Attachments: logo.jpeg, lock.gif, SecureMessageAtt.html.
- Body, verbatim (complete):
  > This is a secure message. Click here https://securemail.ally.com/formpostdir/securereader?id=UhWi3Ko-i-SU6nmbl1Ps13HuZGS7oWo1&brand=39c74d84 by 2026-12-03 10:14 PST to read your message. After that, open the attachment.
- The same thread has a second message, 1a19038a7b1f6fa6 (2026-10-31T04:29:54Z, SENT). It is from Halsey@realitylab.com to DepositsECR@ally.com, subject "Follow-up: missing levy notice and funds-disposition records — ECR 64504079 / 65504572". These are HALSEY's words, not Ally's. Relevant parts, verbatim:
  > Please provide the outstanding records explaining the $4,156.66 restrained on August 6, 2026 across my accounts ending 0942 and 9376, associated with LASD file 2026069969 and court case 24STFL00432:
  > 1. Both notices Ally says it received on July 29 and August 5, and every accompanying writ, instruction, and service record.
  > 2. … Please explain the Kingsburg, California address in your correspondence when the execution writ lists Cancún, Mexico.
  > … Referring me to opposing counsel does not answer these questions about Ally's own actions and records.
  It quotes the 9/4 Ally email only as the "This is a secure message. Click here…" text above.
- Related: 1a071d3d2b47c0a0 (2026-09-05T13:48:21Z, SecureMail@ally.com, subject "Proofpoint Encryption Registration") contains a registration validation code. The code is not reproduced here.

### 1c. Gmail notices "You have a secure message from Ally" (each read in full)
| msg id | date (UTC) | to | content |
|---|---|---|---|
| 1a0feba4158e29e6 | 2026-10-02T22:26:49Z | halsey@minorventures.com | "You have a message waiting in your Ally Secure Email." / "Halsey, to view your message at ally.com, log in and select Profile and Settings and choose Secure Messages. If you're using our app, log in and select the envelope-shaped icon." Email ID: deposits-secure-message-reminder 1.2.1 v1 |
| 1a14cebc9178c607 | 2026-10-18T02:51:17Z | halsey@minorventures.com | Same template. Label UNREAD. |
Neither notice includes any message content, case number, amount or authority.

### 1d. Drive searches
- `title contains 'SecureMessage'` returned 1 file (1a above).
- `title contains 'ally.com'` returned 14 files. None is another Ally secure-message export. Files dated 2026-07-01 or later:
  - 1a (above).
  - drive:1IZFMiVDCoIwMlratDV4XxoQdwRMeqPrC "2026-10-29__gmail.com__Ally_Regulatory_Complaint_Package_2026-10-29.pdf". 12 pages, Producer "ReportLab PDF Library". **This is not an Ally document.** It was prepared for Halsey. Its text says Exhibit A was "supplied as photographed documents in this conversation", which indicates AI drafting. → class **AI-LEAD** for its narrative pages. It describes the 9/4 item as "Ally's September 4 written direction to contact that firm for additional information". That is the package's characterization, NOT Ally's words, and the 9/4 letter is not attached to it. All 12 pages were read: the text layer plus the 10 screenshots (Exhibit B-1 to B-10). None of the screenshots is the 9/4 message.
    - B-6 (Halsey's portal message dated October 02, 2026) asks for: "8. A copy of Ally?s September 4 secure response if that message constitutes ECR?s substantive determination." (verbatim, "?" as rendered)
    - B-1/B-2 (thread item dated "October 17, 2026", screenshot IMG_0512/0513 taken "Thu Oct 29"): under "-----Original Message-----" it quotes an ALLY reply. Ally's words, verbatim:
      > As referenced in our previous response, On July 29 and August 5, 2026, Ally Bank received a Notice of Levy from Young, Spiegel and Hosp LLP. In order to comply with their instructions, on August 6, 2026, a hold was put on the funds in your Spending Accounts ending in 0942 and 9376 in the total amount of $4,156.66, along with a restriction on the account to ensure that there were enough funds available. The above-referenced restriction was removed from your accounts on August 19, 2026. A copy of our prior response has been included.
      (The original date of this Ally reply is not shown in the screenshot.)
    - B-3 (October 15, 2026) Ally reply signed "Daniel, Customer Service": "…an Executive Customer Relations (ECR) under reference number 65504572…"
  - The other 12 hits are copies of the "2024-10-31 [P] Ntc.Cons.Doc.Subp.Ally.{Bank,Financial.Inc,Servicing.LLC}.pdf" files (Drive-created 2026-08-24). Not opened for this task.

---

## 2. Ally subpoena returns

### 2a. "ALLY FINANCIAL INC. - 0001.pdf" — drive:1qENnLIJg_5YpO81KCcE8Qd_pixn24n6x (created 2026-05-31; 2,240,168 bytes)
- 13 Drive copies of the same size (e.g. 1gRZ06A04bD8irKB4frCzkDLGzL0i3wm3, created 2025-06-09). Only 1qENn… was opened.
- Downloaded. PDF: 7 pages. Author "MaxPrinters". CreationDate 2024-12-11, ModDate 2025-02-13.
- Read: pages 1, 2, 3, 5, 6, 7. **Page 4 was NOT read.**
- p.1, Litbros cover, verbatim: "SUBPOENA RECORDS 02/13/25 / CASE NAME: SHANNON MINOR v. HALSEY MINOR / CASE NUMBER: 24STFL00432 / RECORDS FROM: ALLY FINANCIAL INC. / RECORDS RECEIVED FROM ENTITY: 12/05/24 / BATES RANGE: 0001 / WORK ORDER NUMBER: 0225_004 / RECORDS DELIVERED TO: SAMANTHA ALVAREZ PROVINZIANO & ASSOCIATES 8888 W. Olympic Blvd., Suite 100 Beverly Hills, CA. 90211 / Litbros Discovery 1010 Wilshire Blvd., Suite 711 Los Angeles, CA. 90017 (213) 785-5636 / www.litbros.com".
- p.2: SUBP-010 "DEPOSITION SUBPOENA FOR PRODUCTION OF BUSINESS RECORDS", 24STFL00432. Attorney: "LANCE S. SPIEGEL [SBN 51625] / KATHERINE C. ALDIN [SBN 229130] YOUNG, SPIEGEL & HOSP, LLP. 301 NORTH CANON DRIVE, SUITE 300 BEVERLY HILLS, CA 90210", "ATTORNEY FOR (Name): PETITIONER, SHANNON MINOR". To: "ALLY FINANCIAL INC. c/o CT CORPORATION SYSTEM 330 North Brand Boulevard, Suite 700, Glendale, CA 91203". Deposition officer: "Tony Astorga; Litbros Discovery". Production date: "December 5, 2024", "10:00 a.m.". Records: "See Attachment 3." "Date issued: October 31, 2024 LANCE S. SPIEGEL", signed "Attorneys for Petitioner SHANNON MINOR".
- p.3: Proof of service (SUBP-010 p.2). Served on "DAISY MONTENEGRO", CT Corporation System, Glendale. "November 11, 2024", "8:28 a.m.". Server "ZELALEM FESSEHA A&F MESSENGER SERVICE". Docusign Envelope A6137DBD-….
- p.5: SUBP-025 "NOTICE TO CONSUMER OR EMPLOYEE AND OBJECTION". "TO (name): HALSEY MINOR". Witness: "ALLY FINANCIAL INC. c/o CT CORPORATION SYSTEM". Date set: "December 5, 2024". "Date: October 31, 2024 LANCE S. SPIEGEL" (box checked: ATTORNEY).
- p.6: SUBP-025 proof of service by mail. Served on "HALSEY MINOR", "210 Woodland Circle Bristol, TN 37620", "Date of mailing: October 31, 2024", "Place of mailing: Beverly Hills, CA", "MATTHEW SIRRIYEH". The objection proof-of-service section is blank.
- p.7 (Bates "ALLY FINANCIAL INC. 0001"): Ally letter, verbatim:
  > ally / P.O. Box 380901 Bloomington, MN 55438 / November 18, 2024 / Litbros Discovery Attention: Tony Astorga 1010 Wilshire Blvd, Ste 711 Los Angeles, CA 90025 / Re: SUBPOENA (DUCES TECUM) Halsey Minor, INO Live Plants INC, INO Vivid Labs Holdings Inc / Dear Tony Astorga: / Ally Financial acknowledges receipt of the enclosed SUBPOENA (DUCES TECUM) regarding the above referenced individual(s). / Ally Financial is unable to locate any open or closed accounts at Ally Financial associated with the individual(s) identified in the request. Thus, Ally Financial has no responsive documents to provide at this time. / Sincerely, Ally Financial
- This file contains no custodian declaration.

### 2b. "ALLY BANK - 0001-0238.pdf" — drive:1wgEzPYyYiKoxMslycWuH9Qytnb46ZgT5 (created 2026-05-31; 19,555,399 bytes)
- 17 Drive copies of the same size, e.g. 1cEGwWdJEG1GR82Mkurs5RUyCFrEiWyBi (created 2025-06-09). Only 1wgEz… was opened.
- download_file_content refused it: "File too large for download, over limit of 10 MB". The pages could not be rendered.
- read_file_content returned 228,994 characters with page markers. **The returned text ends at "Page 114"**, in the middle of statement boilerplate ("For recurring transactions and other inquiries, please call the phone number above."). **The last 3 pages of the file were NOT read; they are not in the returned text and the file is too large to download.** PDF pages 2, 3, 5 and 6 returned no text (image-only) and were NOT read. Statement pages (PDF p.9 onward) were not read, as instructed.
- PDF p.1, Litbros cover, verbatim: "SUBPOENA RECORDS / 02/13/25 / CASE NAME: SHANNON MINOR v. HALSEY MINOR / CASE NUMBER: 24STFL00432 / RECORDS FROM: ALLY BANK / RECORDS RECEIVED FROM ENTITY: 12/05/24 / BATES RANGE: 0001 - 0238 / WORK ORDER NUMBER: 0225_004 / RECORDS DELIVERED TO: SAMANTHA ALVAREZ PROVINZIANO & ASSOCIATES 8888 W. Olympic Blvd., Suite 100 Beverly Hills, CA. 90211 / Litbros Discovery 1010 Wilshire Blvd., Suite 711 Los Angeles, CA. 90017 (213) 785-5636 / www.litbros.com".
- PDF p.4 "ATTACHMENT 3", verbatim:
  > 1. For the time period of January 1, 2021, through and including the date of production, any and all account statements, wire transfer records, cancelled checks, check registers or stubs, certificates of deposit, cashier's or traveler's check acquisition records, and all other documents reflecting deposits, withdrawals and exchanges of funds at ALLY BANK for all CHECKING and SAVINGS accounts in the name of HALSEY MINOR, Social Security no. [blank in text], and/or accounts on which HALSEY MINOR is an authorized signatory, whether held individually, jointly with any other person or entity, and/or trust, including, but not limited to, the following: a. Spending account no. 1113860942 held INO HALSEY MINOR; b. Account no. 7053856273 held INO HALSEY MINOR; c. Any and all accounts held INO LIVE PLANET, INC. (Federal Employer Identification no. 95-4785385; CA Entity no. C3921168; DE File no. 5943613); d. Any and all accounts held INO LIFE LAB VENTURES LLC (Federal Employer Identification no. 47-4362293; CA Entity no. 201517610281; DE File no. 5760677); and, e. Any and all accounts held INO VIVID LABS HOLDINGS INC. (Federal Employer Identification no. 88-4404441; CA Entity no. C5378402; DE File no. 7188602).
- PDF p.7 (Bates ALLY BANK 0001), custodian declaration, verbatim:
  > DECLARATION OF RECORDS CUSTODIAN
  > My name is Abigail R. Gruver I am over 21 years of age, of sound mind, capable of making this Declaration and personally acquainted with the facts herein stated.
  > I am an authorized agent of Ally Bank ("Ally"). There is no one person who is the custodian of records related to the accounts relate to or in the accounts in the name of Halsey Minor.
  > However, since receiving this Subpoena on behalf of Ally, I coordinated the collection and temporarily have custody of the responsive documents for purposes of responding to the Subpoena.
  > The documents produced by Ally in response to the Subpoena and are true and correct copies of original servicing records within its custody or control and are maintained in the usual and regular course of its business. There are a total of 226 pages produced in response to this subpoena. All memoranda, reports, and records of data compilations were made at or near the time by, or from information transmitted by, a person with knowledge of the events, acts, conditions, opinions, or facts described. These records are kept in the course of Ally's regularly conducted business activity, and it is the regular practice of Ally to make or keep such records.
  > I declare under penalty of perjury under the laws of the state of California that the above information is true and correct, and that this Declaration was executed on November 27, 2024, in Riverton, NJ.
  > By: ____ Digitally signed by Abigail R. Gruver DN: cn=Abigail R. Gruver, c=US, o=Ally Bank, email=legaldocumentprocessing@ally.com Date: 2024.11.29 11:29:23 -05'00'
- PDF p.8 (Bates ALLY BANK 0002), Ally cover letter, verbatim:
  > Ally | Deposit Operations / Contact No. 855-290-2559 ext. 5692 / Document Processing Fax No. 267-983-5885 / Email: legaldocumentprocessing@ally.com / November 27, 2024 / Tony Astorga Litbros Discovery Tony@litbros.com / RE: Subpoena in the Matter of: Halsey Minor / Records Subpoenaed from Ally Bank Account No.: xxxxxx0942, xxxxxx9376, xxxxxx0931 / Case No.: 24STFL00432 / Dear Tony Astorga, / Enclosed please find the submission of documents responsive to the above-referenced request. These documents are copies of the Ally Bank customer account files and are those that we determined to be responsive to the subpoena following a good faith, reasonable search for responsive documents. If additional documents are located, we will supplement our response. / These documents consist of those found in the Ally Bank files concerning the following: / A bank account referenced at No. xxxxxx0942 in the name of Halsey Minor is a Spending Account which opened on March 7, 2023 and remains open. / A bank account referenced at No. xxxxxx9376 in the name of Halsey Minor is a Spending Account which opened on September 4, 2024 and remains open. / A bank account reference at No. xxxxxx0931 in the name of Halsey Minor was a Savings Account which opened on March 7, 2023 and was closed on April 6, 2023. / We did not locate deposit accounts for the remaining businesses or accounts listed on the subpoena. / This response is being issued by the Deposit Operations line of business only. If an account is located in another line of business, you will be receiving a separate response. / To ensure a timely response from this office, comments or additional information regarding your subpoena must be communicated in writing by fax or mail to my attention. / Sincerely, Aleisha Thompson Associate Analyst, Document Processing ANT/Enclosure(s)
- Note on forms: the subpoena form in the Ally Financial file is SUBP-010, dated 10/31/2024. The SUBP-025 there is the Notice to Consumer. The image-only pages 2, 3, 5 and 6 of the Ally Bank file were not read, so which forms they contain is not documented here.
- Page counts as stated by the documents: Litbros cover "0001 - 0238"; custodian declaration "a total of 226 pages".

---

## 3. Table

| document | date | what it establishes (DOCUMENTED) | pointer |
|---|---|---|---|
| Ally secure message (Proofpoint envelope) | 2026-09-04 (Proofpoint Date 10:42 -07:00) | Sent by DepositsECR@ally.com to halsey2005@gmail.com. The body is AES-256 encrypted and was not read. No text about authority is readable. | drive:1k2YTcHZ_ILuf7bg5hYwjPgiiqjac1RIT; gmail 1a06da1478a8cadd |
| Halsey follow-up | 2026-10-31 | Halsey asks for the notices, writ, reconciliation and exemption basis behind "$4,156.66 restrained on August 6, 2026" (Halsey's words) | gmail 1a19038a7b1f6fa6 |
| Ally secure-message reminders | 2026-10-02; 2026-10-18 | Generic notices that a message is waiting; no content | gmail 1a0feba4158e29e6; 1a14cebc9178c607 |
| Ally reply quoted in portal screenshot | shown under item dated 2026-10-17 | Ally: "Ally Bank received a Notice of Levy from Young, Spiegel and Hosp LLP" on July 29 and August 5, 2026; hold of $4,156.66 on 0942/9376 on August 6; restriction "removed … on August 19, 2026" | drive:1IZFMiVDCoIwMlratDV4XxoQdwRMeqPrC p.3 (Exh. B-1; package itself AI-LEAD) |
| Ally Financial subpoena return | Litbros 02/13/25; Ally letter 11/18/2024 | SUBP-010 issued 10/31/2024 by Lance S. Spiegel for Shannon Minor, 24STFL00432. Ally Financial: "no responsive documents" | drive:1qENnLIJg_5YpO81KCcE8Qd_pixn24n6x pp.1–3, 5–7 |
| Ally Bank subpoena return | Litbros 02/13/25; declaration 11/27/2024; cover letter 11/27/2024 | Production to Litbros (deposition officer Tony Astorga) for case 24STFL00432, delivered to Provinziano & Associates. Accounts xxxxxx0942, xxxxxx9376, xxxxxx0931. Request period from January 1, 2021 through production. Declaration says 226 pages; cover says Bates 0001-0238 | drive:1wgEzPYyYiKoxMslycWuH9Qytnb46ZgT5 PDF pp.1, 4, 7, 8 (text only; last 3 pages not read) |
