# Gmail inventory: notes

Run date: 2026-11-01. Status: **partial**. The TSV covers threads that sit in complete search result sets, plus the three named-ID checks. The large buckets were not exhausted (see Coverage), so this is not a complete register.

## Files

- `gmail_inventory.tsv`: 211 message rows across 63 threads. Header: `pointer date_utc from to cc subject attachments search_bucket`. Sorted by date.
- `gmail_work_rows.psv`: source rows, pipe-delimited, from which the TSV was built. The work file writes `D,C` where the TSV writes `C,D`.
- Backups and scratch copies: `/tmp/claude-0/-home-user/9a86eccf-071d-5c97-88ae-ef129ec55f9d/scratchpad/` (not deliverables).
- Raw get_thread results (PLAIN_TEXT, which include message bodies) are saved under `/root/.claude/projects/-home-user/9a86eccf-071d-5c97-88ae-ef129ec55f9d/tool-results/`. They were read with jq for header fields only, and nothing from them was copied into INVENTORY.

## Method

- Tools: Gmail `search_threads` (includeTrash=true, pageSize 50; IDS_ONLY and MINIMAL views) and `get_thread` (PLAIN_TEXT). No send, draft, label, trash, spam or modify calls were made.
- No message body text appears in any output file. Each row holds the message ID, thread ID, date, sender, to, cc, subject and attachment filenames.
- Dates, senders, recipients and subjects come from get_thread. Search output has no date field, and its per-message subject can differ from the message's own (for example, a missing "Re:" prefix), so search subjects were not used.
- BCC: get_thread returns bccRecipients, but the TSV schema has no bcc column, so BCC is not recorded.
- Attachments: names come only from PLAIN_TEXT fetches. An attachment part with no filename is written as `(unnamed)`. One message has four such parts: `gmail:msg:19cfe9056c46687a`.

## Search behaviour that limits completeness

- No search returned a nextPageToken, so none could be followed. A full page of 50 is treated as truncated.
- resultCountEstimate is approximate and changes between windows.
- Search previews show only up to five of each thread's oldest messages. messageCount is the thread total.
- The in:spam probe returned no results. Spam coverage is unverified.
- No query returned an error.

## Query log

All queries used includeTrash=true and pageSize 50.

| ID | Query | Returned | Estimate | Status |
|---|---|---|---|---|
| A1 | from:ysfamilylaw.com | 50 | 71-74 | truncated |
| A2 | to:ysfamilylaw.com | 50 | 384 | truncated |
| A3 | cc:ysfamilylaw.com | 50 | 232 | truncated |
| A4 | ysfamilylaw | 50 | 896 | truncated |
| B1 | Spiegel | 50 | 2096 | truncated. Windows: before 2024/01/01 50 (est. 232); 2024 50 (233); 2025 50 (866); 2026 onward 50 (667); June 2025 31 (complete for that window); Jan 2026 50 (133, truncated) |
| B2 | "Lance Spiegel" | 50 | 1116 | truncated |
| C1 | "24STFL00432" | 50 | 1819 | truncated |
| C2 | "proof of service" | 50 | 502 | truncated |
| C3 | "eService" OR "e-service" OR "electronic service" | 50 | 288 | truncated |
| C4 | "Notice of Electronic Service" | 11 | 11 | complete. Re-run this pass: 11 IDs, all labelled C |
| C5 | "preliminary declaration of disclosure" | 50 | 140 | truncated |
| C6 | "income and expense declaration" | 50 | 182 | truncated |
| C7 | "FL-141" OR "FL-150" OR "FL-142" OR "FL-335" OR "POS-050" | 50 | 214 | truncated |
| D1 | calbar.ca.gov | 37 | 37 | complete. Re-run this pass: 37 IDs, all labelled D |
| D2 | "State Bar" Spiegel | 50 | 224 | truncated |
| D3 | "24-O-18793" | 10 | 10 | complete. Re-run this pass: 10 IDs, all labelled D |
| D4 | "26-O-13820" | 10 | 10 | complete. Re-run this pass: 10 IDs, all labelled D |
| E | after:2026/02/01 before:2026/06/01 (Spiegel OR ysfamilylaw OR "Lance") | 50 | 439 | truncated |
| F1 | ally.com Spiegel | 50 | 101 | truncated |
| F2 | "64504079" | 2 | 2 | complete. Re-run this pass: 2 IDs, both labelled F |
| G1 | postmark | 50 | 287 | truncated; most results unrelated to the matter |
| G2 | "envelope 24STFL00432" | 0 | 0 | complete (zero) |
| G3 | "certified mail" Spiegel | 18 | 18 | complete. Re-run this pass: 18 IDs, all labelled G |
| probe | in:spam Spiegel | 0 | - | no results; spam not searchable here |

Calibration (run record): ysfamilylaw in January 2026 returned 26; to:ysfamilylaw.com in January 2025 returned 5.

## Coverage

- Labelled from complete sets: C4, D1, D3, D4, F2, G3 and G2 (G2 returned zero). Every member of these sets is in the TSV with its letter.
- Not exhausted, so no rows from them: A1-A4, B1 (except the June 2025 window), B2, C1, C2, C3, C5, C6, C7, D2, E, F1 and G1.
- The June 2025 window of B1 returned 31 results and is complete for that window. It was not fetched or labelled, because B as a whole is not complete.
- Threads seen only in truncated results have no rows, except the two fetched-but-unlabelled threads listed next.
- Two fetched threads carry no letter and are excluded: `18d424f91222fab9` (21 messages, 17 listed) and `190c2fad1c4fd49a` (7 messages). Neither is in any complete set checked in this run.

## Bucket labels

- A letter comes only from a complete set (C4, D1, D3, D4, F2, G3, G2). It is applied to every listed message in the thread.
- ID marks the named message only: `19cafa12df3a5ca4` and `1979e5eb9bbac178`.
- Truncated-set memberships are never labelled. Threads `19ca398af605f23a` and `198fcf44b5f0e72a` also appeared in partial B and E results; that added no letter. Their letters come from complete sets.
- Combined letters are in alphabetical order (C,D; D,G; D,G,ID).
- Correction made in this pass: on the first pass, three C4 threads (`19b883533165b9af`, `19b881b5c3bf7402`, `19b87fe2892d0c64`) carried D but not C. They now carry C. The re-run found no other gaps. Every member of C4, D1, D3, D4, F2 and G3 carries its letter, and no thread carries a letter without being a member of its set.

## Named-ID checks

- Thread `19ca398af605f23a`: FOUND. get_thread messageCount 9; 7 messages listed, and all 7 are in the TSV. Two messages were not listed.
- Message `19cafa12df3a5ca4`: FOUND. 2026-03-02T17:38:09Z; from info@da.lacounty.gov; to halsey@minorventures.com; subject "Re: CRIMINAL COMPLAINT AND REQUEST FOR ARREST WARRANT FOR LANCE SPIEGEL"; no attachment parts. Bucket D,G,ID.
- Message `1979e5eb9bbac178`: FOUND. 2025-06-23T19:58:07Z; from lances@ysfamilylaw.com; to halsey@minorventures.com; cc mvs@ysfamilylaw.com; thread `1979db6b2125390b`; subject "RE: In Re Marriage of Minor - LASC Case No. 24STFL00432 - EX PARTE NOTICE"; no attachment parts. Bucket ID.
  - Thread `1979db6b2125390b` has 11 messages. Only `1979e5eb9bbac178` is in the TSV. The other ten carry no letter and are listed here as thread context, not as inventory rows: `1979db6b2125390b`, `1979e246622738f5`, `1979e2946a3346f0`, `1979e2cd049f87a2`, `1979e2dcb382217d`, `1979e30e22e4ae99`, `1979e7813a178045`, `197ef5895435e31b`, `197ef5eeb73a5be8`, `1983aeaaaf2f91a4`.

## Totals

- Rows: 211 messages, 211 unique message IDs, 63 threads.
- Exact labels: D 93; G 66; C,D 25; C 12; D,G 10; F 3; ID 1; D,G,ID 1.
- Rows carrying each letter: C 37; D 129; F 3; G 77; ID 2.
- Threads per letter: C 11; D 40; F 2; G 18; ID 2.
- Earliest date_utc: 2010-08-10T01:11:41Z (`gmail:msg:12a598dab8b9972c`). Latest: 2026-10-31T04:29:54Z (`gmail:msg:1a19038a7b1f6fa6`).

## messageCount above listed messages

get_thread lists fewer messages than messageCount for these threads. The cause is not established. get_thread's own description says drafts are omitted, which may explain some of the gap.

- `18d424f91222fab9`: 21 total, 17 listed (not inventoried).
- `19ca398af605f23a`: 9 total, 7 listed.
- `196a6faebfb2aefa`: 20 total, 19 listed.
- `19b9f7b82104dd6f`: 18 total, 17 listed.
- `19c59a367a2e5a11`: 7 total, 5 listed.
- `19c8768a3814f78f`: 7 total, 6 listed.
- Recorded earlier in this run, not re-checked in this pass: `19b881b5c3bf7402` (5 total, 4 listed); `19ceaeeaf689ff5c` (2, 1); `19b752501ec26c61` (8, 7); `19877883724ab380` (5, 4); `19cc3a0728287e4c` (4, 3).

## Verification items

- Attachment-to-message mapping for identical filenames within a thread is not independently checked. Thread `19b9e4e25bc5663b` (8 messages) was read from one inline get_thread result; check with get_message. Thread `19b9e2435572b38e` has FORENSIC EVIDENCE.pdf on more than one message, plus bounces. Thread `1a14a971610082f4` (15 rows) has bounces.
- `19b8b52017ce229e` was flagged earlier for the same name-mapping check. It is in no complete set, so it has no rows here and was not verified.
- Thread `19ff78c508bffa74` has no attachment parts in its metadata.
- Thread `1979db6b2125390b`: ten messages are not inventoried (see Named-ID checks).

## Not done and decisions for the caller

- The register is incomplete. Result estimates for the unexhausted buckets: C1 about 1,819 threads; B1 about 2,096; E about 439.
- A full pass needs date-partitioned searches (`after:` / `before:`) until each window returns fewer than 50 results, then one get_thread per thread. A PLAIN_TEXT fetch costs roughly 3-10k tokens. METADATA_ONLY and MINIMAL views omit attachment names.
- Decision needed: narrow the scope, or authorize a multi-pass continuation by date window.
- No AI-LEAD file was opened. The flags below are name-based only.

## Appendix: AI-LEAD candidates (name-based; not reviewed)

One line per message. Flagged attachment names follow the colon. Format: pointer (date | bucket): names.

- `gmail:msg:19b9f636a1ef17f8 thread:19b9e4e25bc5663b` (2026-01-08T20:54:10Z | G): Google Realization.jpg; FORENSIC EVIDENCE.pdf
- `gmail:msg:19b9f90d62b85db7 thread:19b9f7b82104dd6f` (2026-01-08T21:43:47Z | G): FORENSIC EVIDENCE.pdf
- `gmail:msg:19b9fc157f5152c8 thread:19b9f7b82104dd6f` (2026-01-08T22:36:46Z | G): FORENSIC EVIDENCE.pdf
- `gmail:msg:19ba0331e15a53ff thread:19b9e2435572b38e` (2026-01-09T00:41:02Z | G): FORENSIC EVIDENCE.pdf; Google Realization.jpg; Google Busts Lance.jpg
- `gmail:msg:19ba03405774f1c8 thread:19b9e2435572b38e` (2026-01-09T00:41:56Z | G): FORENSIC EVIDENCE.pdf; Google Realization.jpg; Google Busts Lance.jpg
- `gmail:msg:19baf9dcd5a99455 thread:19b9f7b82104dd6f` (2026-01-12T00:31:52Z | G): FORENSIC EVIDENCE.pdf
- `gmail:msg:19bb44ffb3cfb52d thread:19b9f7b82104dd6f` (2026-01-12T22:24:24Z | G): Forensic Evidence.docx
- `gmail:msg:19bb5420c794797e thread:19bb5420c794797e` (2026-01-13T02:49:00Z | C): Google Realization.jpg; Google Busts Lance.jpg; Forensic Evidence.docx
- `gmail:msg:19bba22940d44fba thread:19b9f7b82104dd6f` (2026-01-14T01:32:27Z | G): FORENSIC EVIDENCE.pdf; Google Busts Lance.jpg; Google Realization.jpg; POLICE REPORT_Revised Analysis of Evidence Supporting Allegations in the Minor Case (Updated with August 2025 Evidence).docx
- `gmail:msg:19bba4c06df0c280 thread:19b9f7b82104dd6f` (2026-01-14T02:17:50Z | G): Executive Summary_AI_Analysis_of_All_Evidence_Kale.pdf
- `gmail:msg:19bba5cc9a6a37ae thread:19b9f7b82104dd6f` (2026-01-14T02:36:40Z | G): FORENSIC EVIDENCE.pdf
- `gmail:msg:19bc3ce414c43f56 thread:19bc34acacd98e29` (2026-01-15T22:36:21Z | G): Google Realization.jpg; Google Busts Lance.jpg; Empirical Analysis of Evidence Spoliation.pdf; POLICE REPORT_Revised Analysis of Evidence Supporting Allegations in the Minor Case (Updated with August 2025 Evidence).docx; ppl-ai-code-interpreter-files.s3.amazonaws.com_web_direct-files_df0167c0a611ff40eff6b8c736b42fa9_70acc24a-5467-4dc5-addc-0fa8ff6c71f9_index.html.png
- `gmail:msg:19be5ceb7f6c5533 thread:19bb5420c794797e` (2026-01-22T13:04:47Z | C): Officer_Kale_Report_Footnoted_v2.docx
- `gmail:msg:19c2bc0838971569 thread:19b9e4e25bc5663b` (2026-02-05T03:02:42Z | G): Google Realization.jpg; FORENSIC EVIDENCE.pdf
- `gmail:msg:19c2bd0ba9679d66 thread:19b9e4e25bc5663b` (2026-02-05T03:20:25Z | G): Google Realization.jpg; FORENSIC EVIDENCE.pdf
- `gmail:msg:19c2bd150757301f thread:19b9e4e25bc5663b` (2026-02-05T03:21:03Z | G): Google Realization.jpg; FORENSIC EVIDENCE.pdf
- `gmail:msg:19c8768a3814f78f thread:19c8768a3814f78f` (2026-02-22T22:11:30Z | G): POLICE REPORT_Revised Analysis of Evidence Supporting Allegations in the Minor Case (Updated with August 2025 Evidence).docx
- `gmail:msg:19ceaeeaf689ff5c thread:19ceaeeaf689ff5c` (2026-03-14T06:00:20Z | C): Officer_Kale_Report_Footnoted_v2.pdf
- `gmail:msg:19d7abd58ca942ae thread:19d74ea3f2d3cbb2` (2026-04-11T04:12:01Z | D): Marsys Officer_Kale_Report_Footnoted_v2 2.pdf; Forensic Audit of False Service Abuse 2.docx; Officer_Kale_Report_Footnoted_v2.pdf; GOOGLE GEMINI LEADING LANCES MOTION AND ALL OFFICER KALES REJECTIONS TO RECOVER EMAILS AND SEE 100 PERCENT MATCH PLUS HACKING OF EVIDENCE 2.pdf
- `gmail:msg:19dcd8aa4640181d thread:19dcd8aa4640181d` (2026-04-27T06:05:07Z | D): Forensic Audit of False Service Abuse.pdf
- `gmail:msg:19de9aa1b7293869 thread:19de9aa1b7293869` (2026-05-02T17:08:51Z | D): bar_evidence_correlation_package.html
- `gmail:msg:19de9c7499d43619 thread:19de9c7499d43619` (2026-05-02T17:40:41Z | D): officer_kale_report_footnoted_v2.pdf; bar_evidence_correlation_package.html
- `gmail:msg:19dea32df5dbea33 thread:19dea32df5dbea33` (2026-05-02T19:38:14Z | D): Lance_Criminal_Evidence_App.html
- `gmail:msg:19dea47680f034f7 thread:19dea47680f034f7` (2026-05-02T20:00:41Z | D): Exhibit_1_Officer_Kale_Forensic_Report.pdf; Exhibit_4_Lance_Criminal_Evidence_Analysis.html; Exhibit_7a_Gemini_Collusion_Analysis.jpg; Exhibit_7b_Gemini_Analysis_2.jpg; Exhibit_7c_Gemini_Analysis_3.jpg
- `gmail:msg:19dff13fd9dd8b9b thread:19dff13fd9dd8b9b` (2026-05-06T20:56:00Z | D): Digital_Forensic_Dossier Older I think.pdf
- `gmail:msg:19dff2cfa242d6ac thread:19dff18b2aa86646` (2026-05-06T21:23:50Z | D): Officer_Kale_Report_Footnoted_v2 2.pdf

## Continuation: bucket A (message-level, all windows) and bucket E (Feb-May 2026)

Scope as narrowed by the coordinator: bucket A only, and bucket E as `in:sent after:2026/02/01 before:2026/06/01 (Spiegel OR ysfamilylaw OR "Lance")`. Gmail use was read-only (search_threads, get_thread METADATA_ONLY). No body text was read or written. Writes went only to this folder.

### Method

- A query: `(from:ysfamilylaw.com OR to:ysfamilylaw.com OR cc:ysfamilylaw.com)`, calendar-month windows from 2024/01/01 through before:2026/11/02, includeTrash true, pageSize 50. Any window at the 50 cap was split into 1st-15th and 16th-end.
- E query: the query above, monthly windows (Feb, Mar, Apr, May 2026). March hit the 50 cap (estimate 64) and was split into 03/01-03/15 and 03/16-03/31; both halves are complete.
- Thread membership for 2025-12 through 2026-05 and all E windows was re-listed with THREAD_VIEW_IDS_ONLY. The query and window were unchanged, and the counts matched the METADATA_ONLY counts logged earlier.
- METADATA_ONLY previews carry no date or label fields, so every returned thread was fetched with get_thread METADATA_ONLY. 210 threads in total: 39 A-only, 159 E-only, 12 in both.
- A rule (message level): a message is an A row when its sender, To or Cc header contains ysfamilylaw.com and its date falls between 2024-01-01 and 2026-11-01. Bcc is not used. Gmail returned some threads only because a firm address appears in Bcc; those messages are not A rows and are listed in the flags below.
- E rule: a message with the SENT label, dated inside a window, in a thread that the same window's query returned. A SENT message in a thread returned only by a different window is not included.
- E superset caveat: body-term matches (Spiegel, Lance) cannot be checked from metadata. E rows are therefore every SENT message in the returned threads within the window, which is a superset of the query's hits.
- Dates are the UTC dates from Gmail. One February E message (19c171a6e277bd30, 2026-02-01T02:48:52Z) is January 31 in US Pacific time; it is kept as February because its thread was returned by the February query.
- A windows: rows keep the message's own header values. For METADATA_ONLY-sourced rows, subject and attachments are "(not fetched)".
- Existing rows already in the TSV keep their values; only the bucket letters were merged (alphabetical, comma-joined). New rows were added for message IDs not already present.

### Per-window table: bucket A

| Window | Query range | Threads returned | Complete |
|---|---|---|---|
| 2024-01 | 2024/01/01-2024/02/01 | 1 | yes |
| 2024-02 | 2024/02/01-2024/03/01 | 14 | yes |
| 2024-03 | 2024/03/01-2024/04/01 | 3 | yes |
| 2024-04 | 2024/04/01-2024/05/01 | 1 | yes |
| 2024-05 | 2024/05/01-2024/06/01 | 3 | yes |
| 2024-06 | 2024/06/01-2024/07/01 | 3 | yes |
| 2024-07 | 2024/07/01-2024/08/01 | 11 | yes |
| 2024-08 | 2024/08/01-2024/09/01 | 6 | yes |
| 2024-09 | 2024/09/01-2024/10/01 | 5 | yes |
| 2024-10 | 2024/10/01-2024/11/01 | 13 | yes |
| 2024-11 | 2024/11/01-2024/12/01 | 1 | yes |
| 2024-12 | 2024/12/01-2025/01/01 | 3 | yes |
| 2025-01 | 2025/01/01-2025/02/01 | 5 | yes |
| 2025-02 | 2025/02/01-2025/03/01 | 11 | yes |
| 2025-03 | 2025/03/01-2025/04/01 | 12 | yes |
| 2025-04 | 2025/04/01-2025/05/01 | 3 | yes |
| 2025-05 | 2025/05/01-2025/06/01 | 0 | yes |
| 2025-06 | 2025/06/01-2025/07/01 | 18 | yes |
| 2025-07 | 2025/07/01-2025/08/01 | 6 | yes |
| 2025-08 | 2025/08/01-2025/09/01 | 15 | yes |
| 2025-09 | 2025/09/01-2025/10/01 | 1 | yes |
| 2025-10 | 2025/10/01-2025/11/01 | 11 | yes |
| 2025-11 | 2025/11/01-2025/12/01 | 12 | yes |
| 2025-12 | 2025/12/01-2026/01/01 | 9 | yes |
| 2026-01 | 2026/01/01-2026/02/01 | 13 | yes |
| 2026-02 | 2026/02/01-2026/03/01 | 13 | yes |
| 2026-03 | 2026/03/01-2026/04/01 | 3 | yes |
| 2026-04 | 2026/04/01-2026/05/01 | 4 | yes |
| 2026-05 | 2026/05/01-2026/06/01 | 3 | yes |
| 2026-06 | 2026/06/01-2026/07/01 | 1 | yes |
| 2026-07 | 2026/07/01-2026/08/01 | 4 | yes |
| 2026-08 | 2026/08/01-2026/09/01 | 4 | yes |
| 2026-09 | 2026/09/01-2026/10/01 | 0 | yes |
| 2026-10 | 2026/10/01-2026/11/01 | 0 | yes |
| 2026-11-01 | 2026/11/01-2026/11/02 | 0 | yes |

A windows total (sum of per-window counts; a thread can appear in two months): 212. Distinct A-window threads: 51 in the 2025-12 to 2026-08 range fetched in this continuation; earlier windows were transcribed previously.

### Per-window table: bucket E

| Window | Query range | Threads returned | Complete |
|---|---|---|---|
| E-2026-02 | 2026/02/01-2026/03/01 | 47 | yes |
| E-2026-03 | 2026/03/01-2026/04/01 (full month, first call) | 50 | no (cap; split below) |
| E-2026-03a | 2026/03/01-2026/03/16 | 21 | yes |
| E-2026-03b | 2026/03/16-2026/04/01 | 43 | yes |
| E-2026-04 | 2026/04/01-2026/05/01 | 37 | yes |
| E-2026-05 | 2026/05/01-2026/06/01 | 32 | yes |

March halves: 21 + 43 = 64 returned, 63 distinct threads (19c66cb256ed6d7d is in both halves).

### Totals

- TSV rows: 211 before, 874 after (663 new rows added; no duplicate pointers or message IDs).
- A letter: 420 rows total, 405 new rows and 15 existing rows that gained A. By year: 2024 = 123, 2025 = 227, 2026 = 70.
- E letter: 304 rows total, 269 new rows (258 E only, 11 A and E) and 35 existing rows that gained E. By month: 2026-02 = 101, 2026-03 = 97, 2026-04 = 61, 2026-05 = 45.
- Existing rows that gained letters: 49 (A only 14, E only 34, both 1).
- Windows that could not be completed: none. Every window above is complete.

### Caveats and exceptions

- messageCount above returned messages: 35 threads returned fewer messages from get_thread than messageCount reported. The missing messages cannot be listed with METADATA_ONLY (possibly drafts or trashed messages). Threads and counts (messageCount, returned):
  - 19b5c4e233f60118 (4, 3): A:2025-12;E:-
  - 19b6cc55639bdc93 (8, 7): A:2025-12;E:-
  - 19b5d526bad05170 (7, 6): A:2025-12;E:-
  - 19ae64fb3079084e (2, 1): A:2025-12;E:-
  - 19b8f1dd4d7a670c (18, 10): A:2026-01;E:2026-02
  - 19b9ec48515756ba (7, 6): A:2026-01;E:-
  - 19ca398af605f23a (9, 7): A:2026-02;E:2026-02,2026-03a
  - 19c9262bb219c577 (8, 7): A:2026-02;E:2026-02
  - 19c4f9dc9d26b93f (5, 4): A:2026-02;E:2026-02
  - 19c59a367a2e5a11 (7, 5): E:2026-02;A:-
  - 19b9f7b82104dd6f (18, 17): E:2026-02;A:-
  - 19c21703604c62e5 (11, 9): E:2026-02;A:-
  - 19c40473d0746dfb (11, 8): E:2026-02
  - 19be37485b19f067 (14, 13): E:2026-02,2026-03a
  - 19c30cfc5f20dddb (7, 6): E:2026-02
  - 19c66d015a085e3d (6, 5): E:2026-02
  - 19c23d3150784831 (3, 2): E:2026-02
  - 19c7219c24bd03c3 (9, 5): E:2026-02
  - 19c6e8c40f8e9c2e (12, 11): E:2026-02
  - 19cb22151685fd7a (4, 3): E:2026-03a
  - 19ceaeeaf689ff5c (2, 1): E:2026-03a
  - 19cce78c216e7912 (6, 5): E:2026-03a
  - 19cbb8c9201890b4 (4, 3): E:2026-03a
  - 19cc3d5a07ae99b1 (8, 6): E:2026-03a
  - 19cf8d7719277a3a (6, 4): E:2026-03b
  - 19d17f84a4c27f0a (7, 6): E:2026-03b
  - 19d204a3bbefd6d3 (9, 7): E:2026-03b
  - 19d3fe84a1dc818e (19, 15): E:2026-03b
  - 19d2d270351e162b (4, 3): E:2026-03b
  - 19cf9153215efa4c (3, 2): E:2026-03b
  - 19a93c44e4f8f6e1 (14, 12): E:2026-03b
  - 19cf91f427c2d88b (6, 4): E:2026-03b
  - 19c85c8367323de8 (10, 9): E:2026-03b
  - 19d4fc9c20fac011 (13, 12): E:2026-04
  - 19e1783453b65f2e (17, 14): E:2026-05
- Bcc-only hits (not A rows, not added to the TSV; flags for the caller to decide): 3.
  - 19b9e2435572b38e | 19ba0331e15a53ff | 2026-01-09T00:41:02Z | halsey2005@gmail.com | LosAngeles@fbi.gov | bcc only: VivianH@ysfamilylaw.com;AnnaK@ysfamilylaw.com;lances@ysfamilylaw.com (not an A row under the sender/to/cc rule)
  - 19b9e4e25bc5663b | 19b9f636a1ef17f8 | 2026-01-08T20:54:10Z | halsey2005@gmail.com | info@da.lacounty.gov | bcc only: VivianH@ysfamilylaw.com;AnnaK@ysfamilylaw.com;lances@ysfamilylaw.com;mvs@ysfamilylaw.com;keny@ysfamilylaw.co (not an A row under the sender/to/cc rule)
  - 19b9e2e602fb5f38 | 19b9f2e529d79fbc | 2026-01-08T19:56:11Z | halsey2005@gmail.com | akale@beverlyhills.org;mstainbrook@beverlyhills.org;MayorandCityCouncil@beverlyhills.org;Sharona@sharonanazarian.com;ddimond@beverlyhills.org;lwiener@beverlyhills.org;shannonminor@gmail.com | bcc only: lances@ysfamilylaw.com;AnnaK@ysfamilylaw.com;VivianH@ysfamilylaw.com (not an A row under the sender/to/cc rule)
- Excluded under the E window rule: 19c85c89ad7860f5 (2026-02-22) and 19c8b941e639157d (2026-02-23), both SENT, in thread 19c85c8367323de8, which the February query did not return.
- Address forms seen in headers, recorded as received: keny@ysfamilylaw.co (To, 19b8f1dd4d7a670c, 2026-01-05; the .co domain is not ysfamilylaw.com, but the message has other firm addresses), ances@ysfamilylaw.com (To, 19fb9141436502ce, 2026-07-31), and Halsey@realitylab.com (sender of SENT messages 19e336e7fed5eea7 and 19e1783453b65f2e).
- Earlier thread 1979db6b2125390b: the thread-level exclusion was replaced by the message-level A rule, as recorded above.
- Quota: earlier in this continuation Gmail returned "Resource has been exhausted" on about 7 of 16 rapid get_thread calls. Retries after a pause succeeded; later batches were kept to about 10 calls.

