# FORENSIC BRIEF v1 — Exhibit F and the email record (2026-11-01)

**Status: a specification only. Nothing is commissioned, requested, or sent.** Who engages an
examiner, when, and through which forum are Halsey's decisions (ADJUDICATION_WORKSHEET W-F1..W-F4).
Charter step 7: the 4/21/2026 §271 finding stands in front of every email-based behavior.

## 1. Why this brief exists — the finding that stands in front

Minute order 4/21/2026, LASC 24STFL00432, Dept. 23 (EV-003; read in full,
READING_NOTES/COURT_ORDERS_and_FL141.notes.md):

> "In Exhibit F itself, six of the emails are signed "Lance," purportedly written by Petitioner's
> counsel, Lance Spiegel. At least one email also references Mr. Spiegel's assistant, Janine."

> "The Court finds that Respondent submitted Exhibit F to the Court and analyzed it as if it were an
> authentic set of email communications, knowing that it was not. The Court further finds that
> Respondent's misrepresentation to the Court was intentional and was designed to mislead the Court
> into granting his RFO based on fictitious evidence."

The amount of any §271 sanction is "reserved to the time of trial". The finding itself stands.

What the record shows about the exhibit. All of this is from the existing system's own provenance
work, `qa_Q61_exhibit_F_provenance.md`. That file is AI-graded work product, used here only as a
map to the documents it names. Its notes are at READING_NOTES/qa_Q61_exhibit_F_provenance.md.notes.md.
- **Origin of the document:**
  - It existed in Halsey's Drive as "Email Financial Records Chronological Index" from 2025-09-24.
  - Times that day: Google Doc created 06:19:45Z, exported to .docx 06:20:08Z, emailed to self 06:23:43Z.
  - It carried template placeholders ("[User's Name]", "[Last Name]", "[link]").
- **Transmission:** on 2025-10-28 it went to the document preparer with the words "I need to check on the 28 emails to Lance. The
  computer searched what you needed named it and I have attached it."
- **Tests run against real mail:**
  - Of four Exhibit F entries and one "Log B" entry tested, none exists in the live mailbox or in the March 30, 2025 export.
  - The query `(to:lances@ysfamilylaw.com OR from:lances@ysfamilylaw.com OR to:ysfamilylaw.com OR from:ysfamilylaw.com) before:2024/01/25` returns 0 threads.
- **Halsey's two sworn accounts.** Both are his, and reconciling them is his to do (D-5, D-14):
  - 2/18/2026: "draft log/summary … I do not have a basis to represent that those timeline-style entries are authentic emails".
  - 5/11/2026: "prepared from memory after the original emails were destroyed by the hack".
- **Tests NOT run:**
  - no byte or hash comparison of the 9/24/2025 .docx against the 10/28 attachment;
  - the 11/15/2025 service PDF was not opened;
  - no prompt or session record of the generating tool was found.

## 2. The questions a neutral examiner would answer

| # | Question | Why it matters to this thread |
|---|---|---|
| Q-F1 | Was any email between Halsey and Lance Spiegel or his firm sent or received before 2024-01-25, in any account Halsey used? | Decides whether any 2021–2023 "Lance" communication existed to be deleted or altered (behaviors a, b) |
| Q-F2 | What created "Email Financial Records Chronological Index" (2025-09-24): which application, which account, from what inputs? Is the 10/28/2025 attachment byte-identical to it? Is the filed Exhibit F that document? | Decides whether Exhibit F's "Lance" content came from any mailbox, or was generated |
| Q-F3 | Were messages deleted from Halsey's Google accounts (Halsey@realitylab.com = halsey2005@gmail.com, one account per D-67; halsey@minorventures.com) on or about 2025-08-04, or at other dates? If so, which messages, by which session, from which IP address or device? | The only route by which behavior (a) could ever be attributed to a person |
| Q-F4 | Were documents "created and inserted into my files that I had never authored" (Decl. 3/27/2026 ¶8) on Halsey's computer(s)? If so, when, under which user account, by local or remote process? | Behavior (a) "creation of content" — Decl. ¶8 names no actor |
| Q-F5 | Is the March 30, 2025 "Vivid" export genuine and complete? Who generated it, from which mailbox, with which tool, and on what date range? Does it match the live account message by message? | It is the control set that shows zero Spiegel items for 2022–2023 |

## 3. What would be examined (the items, and who holds them)

| Item | Holder | How it is lawfully obtained |
|---|---|---|
| Exhibit F as filed with the 11/12/2025 RFO; the 11/2/2025 signed declaration; Spiegel's sworn declaration (12/29 or 12/30/2025) | LASC clerk (24STFL00432) | Certified copies from the court file (any member of the public may request) |
| The 2025-09-24 Google Doc and its version history; the .docx export; the 06:23:43Z self-email and the 10/28/2025 email to the preparer, as original .eml with full headers | Halsey (Drive and Gmail) | Halsey's own export, made by the examiner's procedure (§4). No AI tool touches it |
| The March 30, 2025 export: the native export file(s), not the 793-page PDF or the rebuilt text | Halsey; the tool or vendor that produced it | Halsey's own copy; the vendor's job logs if any |
| The 29_ control set (EV-087) | Halsey | Halsey's own copies |
| Google Workspace records for realitylab.com: Admin-console audit logs (login, Gmail log events, Drive audit), Vault holds and exports (Halsey reports he has "done the vault", D-67) | Google; the Workspace admin (Halsey) | The admin's own console exports, for what retention still holds. Google's server-side records only by "valid legal process" (Google Legal's written requirement, EV-053) — a police warrant or a court subpoena |
| Account security history: sign-ins and IPs, devices, OAuth grants, password changes (e.g. the 2022-09-14 change, attributed to no one in KNOWN_FALSE) | Google | Same as above |
| Halsey's computer(s) | Halsey | Forensic imaging by the examiner, with Halsey's consent |

## 4. Custody procedure (so that a result can be used by a court or a police agency)

1. **Engagement.** The examiner is neutral and qualified (e.g. certified, with court testimony
   experience). The examiner is engaged in one of three ways: by a law-enforcement agency, under a
   court order (a stipulated neutral, or one appointed on motion), or by Halsey's counsel. The
   engagement letter states the five questions in §2 and nothing else. No AI tool is used to
   generate, summarize or "reconstruct" any part of the evidence or the report.
2. **Acquisition by the examiner, not by Halsey.** The examiner images devices with a hardware
   write-blocker. Cloud data is exported by the examiner on a screen-recorded session using the
   account holder's credentials, or obtained from Google by legal process. Certified copies come
   from the clerk.
3. **Hashing at acquisition.** SHA-256 of every image and file is recorded at the moment of
   acquisition, on a chain-of-custody form signed at each transfer.
4. **Working copies only.** Analysis is done on verified copies. Originals are sealed.
5. **Reproducible report.** The report states method, tools and versions, hashes, and every finding
   with the artifact that supports it, under a recognised standard (e.g. ISO/IEC 27037; NIST SP
   800-86). Findings are written as "consistent / inconsistent / cannot determine".
6. **Privilege.** If counsel engages the examiner, the work stays privileged until Halsey decides to
   use it (W-F3).

## 5. What each possible outcome would mean (no outcome is presumed)

| Outcome | What it would mean for this thread |
|---|---|
| **A.** No Halsey–Spiegel or firm email before 2024-01-25 exists in any source (Q-F1 "none"). Log A was generated from a template without mailbox input (Q-F2) | Every behavior that depends on 2021–2023 "Lance" emails stays DROP. The §271 finding is untouched. How Halsey reconciles his two sworn accounts is for him and his counsel (privileged) |
| **B.** Server-side records show deletions or other access from a session, IP or device not Halsey's (Q-F3) | Behavior (a) becomes an intrusion by a person not yet identified. That is reportable to the agency with jurisdiction over the access (§6 of ASSESSMENT), with the records as the predicate. Naming Spiegel or his firm would further need records that link the session or IP to them, which only legal process can reach |
| **C.** Genuine pre-2024 correspondence with a "Lance" is recovered (Q-F1 "yes") | This bears on the 4/21/2026 finding. The route is the family court: the §271 amount is reserved to trial, where the evidence can be offered, or a motion with new evidence under CCP 1008 or 473(d) on counsel's advice. It is not a police matter until a court acts |
| **D.** Device examination shows documents created by a remote process or another user (Q-F4) | Supports behavior (a) as an intrusion by a person not yet identified, the same as B |
| **E.** Inconclusive | Nothing changes. Email-based behaviors stay WAITING ON EXHIBIT F or INSUFFICIENT |

## 6. Limits

- Retention: Workspace audit logs and Google's server records have retention limits. What still
  exists for 2025-08-04 is unknown. Time works against Q-F3.
- The existing system's D-66 assigns everything about the §271 order and Exhibit F to the civil
  process (Front 1, resolved at exhibit level). This brief does not act on that front; it only
  specifies what a neutral examination would be.
