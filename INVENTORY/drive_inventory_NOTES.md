# Drive inventory: run notes (locate-only, read-only)

Run date: 2026-11-01. Companion file: `/home/user/spiegel-thread/INVENTORY/drive_inventory.tsv`.

Tools used: `mcp__Google_Drive__search_files` and `mcp__Google_Drive__get_file_metadata` only. No file contents were read, downloaded, created, updated, shared or trashed. Writes were limited to the two files in this folder.

## Counts
- Raw rows returned across all queries: 37,521 (duplicates included).
- Unique file IDs written to the TSV: 17,617 (one row per `drive:<fileId>`).
- Rows flagged `AI?` by title keyword (gemini, analysis, summary, timeline, reconstruction, or "AI" as a standalone word): 529. Flags only, not judgments. Per AGENT_RULES item 6, AI-output material must be classed AI-LEAD before use; no classes are assigned here.
- Newest `createdTime` seen across all rows: 2026-11-01T00:52:18.653Z.

## matched_terms conventions
- A plain term means the search query for that term returned the file (full-text or title query).
- `term(title)` means the file's title contains the term (substring, case-insensitive). For multi-word terms and `FL-141`, the search matches tokens and this tag is approximate.
- `named_id` marks one of the five named IDs.
- `AI?` is the title flag above.

## Queries run (24 terms from the brief)
Full text uses `fullText contains`, which the tool documents as matching title or body. Title uses `title contains`.

**A. Title queries, complete (paged to the end, no nextPageToken):**
- Spiegel 144; Lance 495; ysfamilylaw 182; 24STFL00432 279; "proof of service" 113; "State Bar" 109; "Exhibit F" 134; "minute order" 146; FL-150 363.
- "Young Spiegel" and "postmark": 0 results.

**B. Title queries combined into one OR query with a Spiegel pad (complete, 366 rows):** calbar, 26-O-13820, 24-O-18793, 271, "register of actions", "declaration of disclosure", "income and expense", FL-141, envelope, Ally, 64504079, Janine, Janina, plus the Spiegel pad. Used because the single-term results were small enough to return inline. Attribution is by title substring, so it is approximate for phrase terms and for FL-141.

**C. Full-text queries, complete:** calbar 292; FL-141 704; postmark 224; 64504079 215; Janine 688; Janina 2 (returned inline, transcribed by hand).

**D. Full-text queries derived by subtraction, complete:**
- 24-O-18793: 48 rows.
- 26-O-13820: 12 rows.
- Method: (fullText T OR title 'Spiegel') minus (title 'Spiegel' AND NOT fullText T).

**E. Full-text queries INCOMPLETE.** The last page fetched still returned a nextPageToken for every chain. Page size is capped at 1000 (a request for 5000 returned 1000).

| Term | Pages fetched | Rows fetched | Resume from (saved page file) |
|---|---|---|---|
| Spiegel | 3 | 3,000 | 1793498773301 |
| Lance | 3 | 3,000 | 1793498775064 |
| ysfamilylaw | 2 | 2,000 | 1793498776716 |
| Young Spiegel | 2 | 2,000 | 1793498778937 |
| 24STFL00432 | 2 | 2,000 | 1793498780213 |
| proof of service | 2 | 2,000 | 1793498786285 |
| State Bar | 2 | 2,000 | 1793498787495 |
| Exhibit F | 2 | 2,000 | 1793498791853 |
| 271 | 2 | 2,000 | 1793498838289 |
| minute order | 2 | 2,000 | 1793498838016 |
| register of actions | 2 | 2,000 | 1793498839109 |
| declaration of disclosure | 2 | 2,000 | 1793498838975 |
| income and expense | 2 | 2,000 | 1793498838401 |
| FL-150 | 2 | 2,000 | 1793498838030 |
| envelope | 2 | 2,000 | 1793498838060 |
| Ally | 1 | 1,000 | 1793498886796 |

The full-text rows for these 16 terms are partial. The complete sets are larger. The saved page files are in `/root/.claude/projects/-home-user/9a86eccf-071d-5c97-88ae-ef129ec55f9d/tool-results/` with the file name prefix `mcp-Google_Drive-search_files-`, and each "resume from" file holds the next-page token. Completing them needs many more pages per term; that was not done in this run.

**Reconciliation:** 33,000 (incomplete full-text) + 2,123 (complete full-text) + 60 (derived) + 1,965 (complete title) + 366 (combined title) + 2 (Janina) + 5 (named IDs) = 37,521 raw rows.

## Errors and limitations
- Results above the inline size limit were saved to files and parsed with jq. These are not content reads; only metadata fields were extracted.
- Some title queries are token-based rather than exact phrase matches. For example, "State Bar" returned 109 titles but only 91 contain the exact phrase, and "Exhibit F" returned 134 titles but only 27 contain it. The `matched_terms` entries still reflect which query returned each file.
- Full-text matches were not verified against body text; they are the search tool's matches.
- Titles are copied as returned, including any leading spaces.

## Five named IDs: all found (get_file_metadata)
1. `1zyRwrL_fJQGt1UNLVhf8NS-GbPWxYQZVQKbrjIcMzXs`: "24-O-18793 Minor Closing Letter", Google Doc, created 2024-07-24T20:00:26.824Z, size 21884.
2. `1435_9jNwJYI_MKG-V0vwwan_tibz0-G5`: "2026-05-06__calbar.ca.gov__26-O-13820 Minor Closing Letter.pdf", PDF, created 2026-08-22T03:20:45.839Z, size 255327.
3. `1RUnL4pXOy5KlC48-z7Pg3qpih4FK9A3Q`: "2026-03-04__gmail.com__MO 3-2-2026 Sanctions (Lance).pdf", PDF, created 2026-08-22T12:19:12.218Z, size 97808.
4. `1BPYr5canO7MruSeWbXdwX-D1zs2CU9Vhh9CbdQ6zB1c`: "Register of Actions — KEY DATES LOCKED (24STFL00432)", Google Doc, created 2026-06-10T03:14:49.978Z, size 3135.
5. `1UKOpnbqJtKBVtEvv23XtG2SUXcfgFpvIUPL19n-3qfI`: "MINOR CASE — 24 BHPD CRIMINAL REPORT OUTLINE (2026-07-30)", Google Doc, created 2026-07-30T19:45:16.295Z, size 5376.

All five appear once in the TSV with the `named_id` tag.
