# writs_levy_locate: run log

Locate-only sweep (writ / levy / garnishment / sheriff / Ally / EJ- / WG- / invoice #001406). Read-only tools only: Gmail search_threads (includeTrash true) and Drive search_files. No file, message body or thread was opened, read, sent, labelled, moved or shared. No git. Written: this file and writs_levy_locate.tsv only. No findings are stated here; findings are in the SubagentHandback.

## Output

- writs_levy_locate.tsv: header + 997 rows (Drive 666, Gmail 331). Columns: pointer, date, title_or_subject, from, matched_query.
- Pointer: `drive:<fileId>` for Drive; `gmail:msg:<message ids returned> thread:<threadId>` for Gmail.
- Date: Drive createdTime (UTC, date part). Gmail `n/a` (search_threads returns no date field).
- From: Gmail sender of the first returned message; Drive `n/a`.
- matched_query: every query in this run that returned the item, joined with " | ". Query strings are verbatim.
- Dedup key: Gmail thread id, Drive file id. Checked: 0 duplicate keys, 0 duplicate pointers, 0 rows with a field count other than 5.
- Title/subject text is exactly as returned by the search tool.

## Pagination facts

- Gmail search_threads: no nextPageToken is returned, pageSize max 50. A query whose result count reached 50 was re-run in date windows (after: inclusive, before: exclusive, midnight). A window counts as complete when it returned fewer than 50 threads.
- Gmail resultCountEstimate changes between calls (for example 84 then 94; 180 for the base query, 167 as the sum of its windows). The estimate is treated as approximate.
- Drive search_files: nextPageToken is returned. Paged until the token was absent, or the query is marked PARTIAL.

## Run log (call, rows returned, status)

Drive, title queries (pageSize 50, excludeContentSnippets true):
- title contains 'writ': 62 rows (50 + 12). Complete.
- title contains 'levy': 7. Complete.
- title contains 'EWO': 0. Complete.
- title contains 'withholding': 4. Complete.
- title contains 'Ally': 109 (50 + 50 + 9). Complete.
- title contains 'sheriff': 21. Complete.
- title contains 'garnish': 5. Complete.
- title contains 'EJ-': 30. Complete. Title matching is word/prefix based; unrelated titles are included.

Drive, fullText queries:
- fullText contains 'writ of execution' and createdTime > '2026-05-01T00:00:00Z': pages 1-5 retrieved, 250 rows; nextPageToken still present. PARTIAL.
- fullText contains 'levy' and createdTime > '2026-07-01T00:00:00Z': pages 1-5 retrieved, 250 rows; nextPageToken still present. PARTIAL.
- fullText contains 'writ of execution' and createdTime > '2026-04-20T00:00:00Z': page 1 only, 50 rows; nextPageToken present. PARTIAL.
- fullText contains 'Notice of Levy': page 1 only, 50 rows; nextPageToken present. PARTIAL.
- fullText contains '64504079': 2 rows. Complete.

Gmail, original queries (includeTrash true, pageSize 50):
- writ after:2026/06/01: 50 returned of est 90 (cap). Covered by the three windows below.
- levy after:2026/07/01: 50 returned of est 58 (cap). Covered by the two windows below.
- "earnings withholding": 0. Complete.
- from:ally.com after:2026/07/01: 16. Complete.
- ally.com 64504079: 2. Complete.
- "001406": 32. Complete.
- from:katflds@gmail.com after:2026/08/01: 0. Complete.
- from:messaging.squareup.com after:2026/08/01: 16. Complete.
- subject:writ: 2. Complete.
- from:lasd.org OR sheriff after:2026/04/20: 50 returned of est 84 (cap). Covered by the three windows below.
- ally after:2026/04/20: 50 returned of est 857 (cap). NOT split. PARTIAL (first page only).
- "EJ-150" OR "EJ-130" OR "WG-" after:2026/04/20: 8. Complete.
- from:lasd.org OR sheriff after:2026/04/20 with pageSize 3 (test call): 3 rows, nothing new.

Gmail, extension query (sheriff/levy/garnish), base was 50 of est 180 (cap); windows:
- after:2026/04/20 before:2026/05/15: 25. Complete.
- after:2026/05/15 before:2026/06/01: 29. Complete.
- after:2026/06/01 before:2026/07/15: 27. Complete.
- after:2026/07/15 before:2026/08/31: 40. Complete.
- after:2026/08/31 before:2026/10/15: 36. Complete.
- after:2026/10/15: 10. Complete.
- Window sum 167 (base est 180). Treated as complete.

Gmail, extension query (from:lasd.org OR sheriff), windows:
- (from:lasd.org OR sheriff) after:2026/04/20 before:2026/06/01: 29. Complete.
- (from:lasd.org OR sheriff) after:2026/06/01 before:2026/08/15: 13. Complete.
- (from:lasd.org OR sheriff) after:2026/08/15: 38. Complete.
- Window sum 80 (base est 84 to 94).

Gmail, writ and levy windows:
- writ after:2026/06/01 before:2026/08/15: 24. Complete.
- writ after:2026/08/15 before:2026/10/01: 32. Complete.
- writ after:2026/10/01: 28. Complete.
- levy after:2026/07/01 before:2026/09/01: 37. Complete.
- levy after:2026/09/01: 21. Complete.

Gmail, Ally sender window:
- from:ally.com after:2026/04/20 before:2026/07/01: 45. Complete.
- (from:ally.com after:2026/07/01 is the 16-row query above.)

## Repairs made in this run

- The earlier pass had not written Drive fullText pages 2-5 for 'writ of execution' (created after 2026-05-01) and 'levy' (created after 2026-07-01) into the TSV. Those pages were in the saved transcript and have now been appended: 178 new rows from writ pages 2-5 and 192 from levy pages 1-5 (10 new on page 1, the rest on pages 2-5). Existing rows only had their matched_query extended.
- Drive fullText 'Notice of Levy' page 1 (35 new rows, 15 existing) and 'writ of execution' created after 2026-04-20 page 1 (28 new rows) are now in the TSV.

## AI-LEAD candidates (marked, not verified)

Automated-monitor output, classed AI-LEAD candidate pending review. Identified by title/sender pattern only; none opened.
- Drive titles starting "MINOR CASE —": 37 rows.
- Gmail rows whose subject contains "Court & legal inbox monitor" or whose sender is no-reply-claude@mail.anthropic.com: 51 rows (subject match 51, sender match 50; subjects include "routine completed" and "scheduled task completed").
- Drive chart items (title starts "chart-") with "sheriff" in the title: 19 rows: provenance not checked, not classified.
- Totals: 88 rows carry an AI-LEAD candidate pattern (37 Drive, 51 Gmail).

## Gaps (what was not covered)

1. Drive fullText 'writ of execution' created after 2026-05-01: 250 of an unknown total; continuation token present.
2. Drive fullText 'levy' created after 2026-07-01: 250 of an unknown total; token present.
3. Drive fullText 'writ of execution' created after 2026-04-20: page 1 (50); token present.
4. Drive fullText 'Notice of Levy': page 1 (50); token present.
5. Gmail 'ally after:2026/04/20': 50 of est 857; not split. Only the sender-based Ally windows (from:ally.com) are complete.
6. Gmail search_threads returns up to 5 messages per thread, so message ids and subjects may not cover a whole thread.
7. Drive title matching is word/prefix based (for example 'EJ-' returns unrelated "Ej..." titles). Matches are listed as returned, not filtered.
8. No body text was read, so no row shows whether a document is a writ, levy or withholding order.

