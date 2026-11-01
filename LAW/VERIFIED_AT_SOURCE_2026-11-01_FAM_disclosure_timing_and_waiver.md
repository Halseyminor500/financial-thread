# California Family Code — disclosure: timing of delivery and waiver (§§ 2100–2113), CRC rule 5.260, form FL-144

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `FAM_disclosure_timing_and_waiver` · **requested:** FAM 2100, 2102, 2103, 2105, 2106, 2110, 2111, 2112; California Rules of Court rule 5.260; Judicial Council form FL-144 · **adjacent (same chapter, or the requested text points to them):** FAM 2101, 2108, 2109, 2113; CRC rules 5.83 and 5.12 · **cited from the earlier file, NOT re-retrieved:** FAM 2104 (including subdivision (f)) and FAM 2107 — see `VERIFIED_AT_SOURCE_2026-11-01_FAM_disclosure.md`.

Class: primary-source retrieval (statute text, rule text, printed form text) — the verbatim blocks and quotations are the evidence. The flags, section captions, "ELEMENTS" (an index to the quoted words, not a legal conclusion), route log and Parts 15–17 are AI-written research aids (class AI-LEAD) and are not evidence. Not legal advice. Research support only. Question put by Halsey Minor, pro se respondent (petition filed 1/16/2024 per the brief).

**Where the answer is:** Part 15 ("WHAT THE WORDS SAY — no opinion") and Part 16 (arithmetic only).

## Read first — flags

1. **Rule 5.260 is not a disclosure rule.** On the Judicial Council page it is titled "Rule 5.260. General provisions regarding support cases"; its text concerns the Income and Expense Declaration (form FL-150), guideline-support deviations and judgments for support. The word "disclosure" does not occur in it and it cites none of Family Code §§ 2100–2113 (machine check; Part 11). A scan of the 124 Family Rules pages (rules 5.1–5.496) found only three whose text refers to the Family Code disclosure requirements or to a declaration of disclosure: rule 5.12(b) (discovery cross-reference), rule 5.77 (summary dissolution; not reproduced) and rule 5.83(c)(4)(C) (a case-management milestone: "should be served within 60 days of the filing of the petition"). Rules 5.83(c)(4) and 5.12(b) are reproduced in Part 14.
2. **FAM 2110 has a chaptered amendment that is not yet in the code table:** AB 2782 (Stats. 2026, ch. 640; chaptered/approved 2026-09-27; no urgency clause) adds a new subdivision (b) on exchange of declarations where "the parties have an existing enforceable judgment of legal separation that adjudicates the division of property". It is **NOT CURRENT LAW** in the code table as of this retrieval (the table row for § 2110 still shows the 2015 amendment): the bill is enacted, but its § 2110 section states no operative date (the general rule for non-urgency statutes would be 1 January 2027 — not in the retrieved text; unverified). Text and source: Part 8. No other section numbered 2100–2119 was touched by any bill chaptered in 2025 or 2026.
3. **FL-144 as printed:** "[Rev. January 1, 2007]" and "Form Approved for Optional Use"; item 2.c prints "Family Law section 2102" (not "Family Code"); the form cites "Family Code, §§ 2102, 2104, 2105(d)". Part 12.
4. **FAM 2104 and 2107 are cited, not re-retrieved** (as instructed). Check result: subdivision (f) of § 2104 is already in the earlier file (its Part 1, line 47) and this session’s metadata rows for both sections carry the same version IDs and history notes as the earlier file. Parts 4 and 7.
5. **Not all words were read by me:** I read every word of every statute, rule subdivision and form text reproduced here. I did NOT read word for word the other 122 Family Rules pages (machine-scanned for "disclos" and for form/section references), the 2,254 chaptered bills (machine-scanned for Family Code action lines), or the other nine sections of AB 2782 (I read its title, history, digest item (3) and the § 2110 section). Part 17 lists what was not retrieved.

## How this file was produced (read first)

1. **Live leginfo pages were tried first and did not answer.** curl (through the session proxy) received HTTP 403 and a 5,765-byte Cloudflare "Just a moment..." JavaScript challenge for `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=N` for N = 2100, 2102, 2103, 2105, 2106, 2110, 2111, 2112 (2026-11-01, 03:29:53Z–03:29:55Z). WebFetch received HTTP 403 for N = 2105 (about 03:48Z). No attempt was made to defeat the challenge. The leginfo pages for the four adjacent sections were not individually attempted.
2. **Text source actually used** (the method in `INDEX.md`): the Legislature’s own data publication `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip`. HEAD at 03:30:08Z: HTTP 200, `accept-ranges: bytes`, `content-length: 1292052065`, `last-modified: Mon, 26 Oct 2026 04:26:08 GMT`, `etag: "4d032661-65eb6ba9a5800"`; a second HEAD at 03:46:54Z showed the same values (the file did not change during this session). Read by HTTP byte-range (`curl -r`): the tail (to find the Zip64 end-of-central-directory record), the central directory (bytes 1272468662–1292051966; 205,148 entries — the same figures the earlier clerk recorded), `LAW_SECTION_TBL.dat` (43,276,148 bytes; ZIP CRC-32 `ae791104`), `LAW_TOC_TBL.dat` (5,329,533 bytes; CRC-32 `19a0d502`) and one `LAW_SECTION_TBL_<n>.lob` XML record per section. Every entry passed its ZIP CRC-32 and length check. The column order of the `.dat` table is taken from the Legislature’s own load script `law_section_tbl.sql` (inside `pubinfo_load.zip`). The ZIP’s entries are dated 2026-10-25.
3. **Independent cross-check against the live pages.** A second Exa connector (`mcp__Exa_a17196c7__web_fetch_exa`; the first connector was not tried this session) returned the live leginfo pages for the eight requested sections between about 03:39Z and 03:41Z (the connector returns no timestamp). The section text and the parenthetical history note on each page were saved and compared with the data-file record after whitespace collapsing: **all eight are identical** (staged script `cmp_live.py`). The four adjacent sections (2101, 2108, 2109, 2113) were not cross-checked.
4. **Rendering.** The source is Legislative Counsel XML. Only whitespace is normalised (source line-wrap whitespace collapsed to single spaces; the XML en-space elements shown as one space); no word, number, punctuation or subdivision label is altered. Curly quotes and apostrophes are as in the source. Rule text is taken from the Judicial Council page’s rule-content container (bold subdivision headings shown in bold, italics in asterisks). Form text is the PDF text layer, checked by eye against a rendering of the page.
5. **Currency as of 2026-11-01.** (a) Every section 2100–2113 has exactly one active row in `LAW_SECTION_TBL.dat` (14 rows). (b) The Legislature’s incremental files `pubinfo_Tue/Wed/Thu/Fri/Sat/Mon.zip` (fetched 03:46:50Z) contain no `LAW_*` table. (c) All 2,254 chaptered bills of the 2025–26 session (991 chaptered in 2025; 1,263 in 2026) were read by byte-range (every entry CRC-32 verified; 03:41:29Z–03:42:19Z) and scanned for Family Code action lines, then scanned again (03:43:46Z–03:44:33Z) using the structured pointers in each bill’s ActionLine elements: **exactly one** pointer falls in Family Code Division 6, Part 1, Chapter 9 — AB 2782 (Stats. 2026, ch. 640) amending § 2110 (Part 8). No chaptered bill amended or added any other section numbered 2100–2119. Caveat: the earlier clerk noted that statutes enacted in 2026 for 1 January 2027 may not yet be in the code tables; AB 2782 is such a case. The history-note dates of the sections reproduced here are all earlier than 2024-01-16 (table in Part 16).
6. **Rules and form.** Rule pages: direct fetch from `courts.ca.gov` (HTTP 200 after a 301), 03:32:50Z–03:32:52Z (rule 5.260) and 03:36:05Z–03:37:23Z (the 124-page Family Rules scan). Form FL-144: direct fetch of the PDF from `courts.ca.gov` (Part 12). The Judicial Council forms-index search page is script/reCAPTCHA-driven (no FL-144 entry in its static HTML) and was not used.
7. **Scope limits.** No case law, annotations or secondary sources were consulted. "ELEMENTS" are drawn only from the quoted words; where the text is silent the file says so. No case-file documents were read; the two record dates in Part 16 are taken from the brief, not verified.

### Route log — this session, in order (all times UTC, 2026-11-01)

| Time | Route | Target | Result |
|---|---|---|---|
| 03:29:53Z–03:29:55Z | curl via session proxy | leginfo `codes_displaySection.xhtml?lawCode=FAM&sectionNum=` 2100, 2102, 2103, 2105, 2106, 2110, 2111, 2112 | HTTP 403 each; Cloudflare "Just a moment..." (5,765 bytes) |
| 03:30:08Z | curl HEAD | `pubinfo_2025.zip` | HTTP 200; accept-ranges bytes; Last-Modified 26 Oct 2026 04:26:08 GMT; 1,292,052,065 bytes |
| 03:30:55Z–03:30:56Z | curl range reads | ZIP tail, Zip64 end record, central directory | HTTP 206; 205,148 entries |
| 03:31:11Z, 03:31:15Z | curl range reads | `LAW_SECTION_TBL.dat`, `LAW_TOC_TBL.dat` | HTTP 206; CRC-32 OK |
| about 03:31Z | curl | `pubinfo_Readme.pdf`, `pubinfo_load.zip` | HTTP 200 (schema) |
| 03:32:05Z–03:32:10Z | curl range reads | eight requested `LAW_SECTION_TBL_<n>.lob` records | HTTP 206; CRC-32 OK |
| 03:32:50Z–03:32:52Z | curl | courts.ca.gov rule 5.260 (three URL forms) | HTTP 200 after 301; three identical captures, SHA-256 `438c4e6f…a1a4` |
| 03:33:26Z | curl | courts.ca.gov Title Five table of contents | HTTP 200 (263 rule links; no rule title mentions "disclosure") |
| 03:33:56Z–03:34:00Z | curl | `courts.ca.gov/documents/fl144.pdf` (and `www.`); forms index `?filter=FL144` | PDF: HTTP 200 after two 301s, identical bytes; forms index: HTTP 200, script-driven, no FL-144 entry in static HTML (not used) |
| 03:35:30Z–03:35:32Z | curl range reads | adjacent records for 2101, 2108, 2109, 2113 | HTTP 206; CRC-32 OK |
| 03:36:05Z–03:37:23Z | curl (4 parallel) | 124 Family Rules pages, rules 5.1–5.496 | HTTP 200 each; one partial transfer (rule 5.330) re-fetched complete; scanned for "disclos" and form/section references |
| 03:38:56Z | curl | Judicial Council "Latest Changes" forms page | HTTP 200; static HTML has no FL-14x mention |
| about 03:39Z–03:41Z | Exa connector 2 | leginfo pages for the eight requested sections | text returned; identical to the data-file text and history notes |
| 03:40:56Z–03:40:57Z | curl range reads | `BILL_TBL.dat`, `BILL_VERSION_TBL.dat` | HTTP 206; CRC-32 OK |
| 03:41:29Z–03:42:19Z | curl range reads (10 parallel) | chaptered text of all 2,254 chaptered bills | all CRC-32 OK; text scan: 30 bills with Family Code action lines; one touches 2100–2119 (AB 2782 → § 2110) |
| 2026-11-01T03:42:48Z | curl range read | AB 2782 chaptered text (`BILL_VERSION_TBL_18865.lob`) | HTTP 206; CRC-32 `ea78287d` OK |
| 03:43:46Z–03:44:33Z | curl range reads (10 parallel) | same 2,254 texts, structured ActionLine pointers | all CRC-32 OK; 70 Family Code pointers; one into Chapter 9 (AB 2782 → § 2110) |
| 03:46:50Z–03:46:54Z | curl | incremental zips Tue/Wed/Thu/Fri/Sat/Mon; second HEAD of `pubinfo_2025.zip` | no `LAW_*` table in any; `pubinfo_2025.zip` unchanged |
| about 03:48Z | WebFetch | leginfo FAM 2105 | HTTP 403 Forbidden |

## 1. Family Code § 2100 — Legislative findings: early disclosure and continuing duty

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). Live-page cross-check: text and history note identical to the leginfo page as returned by a second Exa connector (machine-compared).
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2100> (leginfo host: HTTP 403 Cloudflare challenge to curl, 03:29:53Z–03:29:55Z; see "How this file was produced", item 1)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23603.lob` (1,729 bytes; ZIP CRC-32 `af6be285` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2100.20017032`).
- **Retrieved (UTC):** 2026-11-01T03:32:05Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2001, Ch. 703, Sec. 2. Effective January 1, 2002."
- **Effective-date field:** 2002-01-01 (OP_STATUES/OP_CHAPTER/OP_SECTION: 2001 / 703 / 2)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f615767-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `d481b29ada27d3776b9a2faf013e7b303580efa1fd06e35d729f2d0258066fe4`

### (2) Operative text (verbatim)

> The Legislature finds and declares the following:
>
> (a) It is the policy of the State of California (1) to marshal, preserve, and protect community and quasi-community assets and liabilities that exist at the date of separation so as to avoid dissipation of the community estate before distribution, (2) to ensure fair and sufficient child and spousal support awards, and (3) to achieve a division of community and quasi-community assets and liabilities on the dissolution or nullity of marriage or legal separation of the parties as provided under California law.
>
> (b) Sound public policy further favors the reduction of the adversarial nature of marital dissolution and the attendant costs by fostering full disclosure and cooperative discovery.
>
> (c) In order to promote this public policy, a full and accurate disclosure of all assets and liabilities in which one or both parties have or may have an interest must be made in the early stages of a proceeding for dissolution of marriage or legal separation of the parties, regardless of the characterization as community or separate, together with a disclosure of all income and expenses of the parties. Moreover, each party has a continuing duty to immediately, fully, and accurately update and augment that disclosure to the extent there have been any material changes so that at the time the parties enter into an agreement for the resolution of any of these issues, or at the time of trial on these issues, each party will have a full and complete knowledge of the relevant underlying facts.

### (3) ELEMENTS

1. Nature: findings. Lead-in: “The Legislature finds and declares the following:”
2. Policy (a): “to marshal, preserve, and protect community and quasi-community assets and liabilities that exist at the date of separation so as to avoid dissipation of the community estate before distribution”, “to ensure fair and sufficient child and spousal support awards”, and “to achieve a division of community and quasi-community assets and liabilities on the dissolution or nullity of marriage or legal separation of the parties as provided under California law”.
3. Policy (b): “Sound public policy further favors the reduction of the adversarial nature of marital dissolution and the attendant costs by fostering full disclosure and cooperative discovery.”
4. Timing words in (c): the disclosure “must be made in the early stages of a proceeding for dissolution of marriage or legal separation of the parties, regardless of the characterization as community or separate, together with a disclosure of all income and expenses of the parties.”
5. Continuing duty in (c): “each party has a continuing duty to immediately, fully, and accurately update and augment that disclosure to the extent there have been any material changes” with the stated purpose “so that at the time the parties enter into an agreement for the resolution of any of these issues, or at the time of trial on these issues, each party will have a full and complete knowledge of the relevant underlying facts.”
6. The section states no number of days and contains no word of waiver: the text is silent on both (machine check: no "days" and no "waiv" in the section; the 60-day period is in § 2104(f), Part 4).

## 2. Family Code § 2102 — Duties from the date of separation (standards of Section 721; continuing update)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). Live-page cross-check: text and history note identical to the leginfo page as returned by a second Exa connector (machine-compared).
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2102> (leginfo host: HTTP 403 Cloudflare challenge to curl, 03:29:53Z–03:29:55Z; see "How this file was produced", item 1)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19600.lob` (2,878 bytes; ZIP CRC-32 `0aa229b7` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2102.201911518`).
- **Retrieved (UTC):** 2026-11-01T03:32:06Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2019, Ch. 115, Sec. 18. (AB 1817) Effective January 1, 2020."
- **Effective-date field:** 2020-01-01 (OP_STATUES/OP_CHAPTER/OP_SECTION: 2019 / 115 / 18)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_3a0b8951-0bb2-11ea-912d-915c88c10a14`; SHA-256 of the XML record `eee4d6c44c2fc74283d77301c8b0e4940ce9ee69fc6bff1eb2d2152a417378c7`

### (2) Operative text (verbatim)

> (a) From the date of separation to the date of the distribution of the community or quasi-community asset or liability in question, each party is subject to the standards provided in Section 721, as to all activities that affect the assets and liabilities of the other party, including, but not limited to, the following activities:
>
> (1) The accurate and complete disclosure of all assets and liabilities in which the party has or may have an interest or obligation and all current earnings, accumulations, and expenses, including an immediate, full, and accurate update or augmentation to the extent there have been material changes.
>
> (2) The accurate and complete written disclosure of any investment opportunity, business opportunity, or other income-producing opportunity that presents itself after the date of separation, but that results from any investment, significant business activity outside the ordinary course of business, or other income-producing opportunity of either spouse from the date of marriage to the date of separation, inclusive. The written disclosure shall be made in sufficient time for the other spouse to make an informed decision as to whether the spouse desires to participate in the investment opportunity, business, or other potential income-producing opportunity, and for the court to resolve any dispute regarding the right of the other spouse to participate in the opportunity. In the event of nondisclosure of an investment opportunity, the division of any gain resulting from that opportunity is governed by the standard provided in Section 2556.
>
> (3) The operation or management of a business or an interest in a business in which the community may have an interest.
>
> (b) From the date that a valid, enforceable, and binding resolution of the disposition of the asset or liability in question is reached, until the asset or liability has actually been distributed, each party is subject to the standards provided in Section 721 as to all activities that affect the assets or liabilities of the other party. Once a particular asset or liability has been distributed, the duties and standards set forth in Section 721 shall end as to that asset or liability.
>
> (c) From the date of separation to the date of a valid, enforceable, and binding resolution of all issues relating to child or spousal support and professional fees, each party is subject to the standards provided in Section 721 as to all issues relating to the support and fees, including immediate, full, and accurate disclosure of all material facts and information regarding the income or expenses of the party.

### (3) ELEMENTS

1. Duty period (a): “From the date of separation to the date of the distribution of the community or quasi-community asset or liability in question”
2. Standard (a): “each party is subject to the standards provided in Section 721, as to all activities that affect the assets and liabilities of the other party, including, but not limited to, the following activities:” (Section 721 was not retrieved.)
3. (a)(1): “The accurate and complete disclosure of all assets and liabilities in which the party has or may have an interest or obligation and all current earnings, accumulations, and expenses, including an immediate, full, and accurate update or augmentation to the extent there have been material changes.”
4. (a)(2): “The accurate and complete written disclosure of any investment opportunity, business opportunity, or other income-producing opportunity that presents itself after the date of separation” and the timing words “The written disclosure shall be made in sufficient time for the other spouse to make an informed decision as to whether the spouse desires to participate in the investment opportunity, business, or other potential income-producing opportunity”
5. (a)(3): “The operation or management of a business or an interest in a business in which the community may have an interest.”
6. (b) period after a resolution: “From the date that a valid, enforceable, and binding resolution of the disposition of the asset or liability in question is reached, until the asset or liability has actually been distributed”; end point: “Once a particular asset or liability has been distributed, the duties and standards set forth in Section 721 shall end as to that asset or liability.”
7. (c) support and fees: “From the date of separation to the date of a valid, enforceable, and binding resolution of all issues relating to child or spousal support and professional fees” including “immediate, full, and accurate disclosure of all material facts and information regarding the income or expenses of the party.”
8. Link to the waiver provision: § 2105(d)(3) (Part 5) requires the representation “Both parties have fully complied with Section 2102 and have fully augmented the preliminary declarations of disclosure”.
9. The section contains no word of waiver and no number of days: the text is silent on both (machine check).

## 3. Family Code § 2103 — Duty to serve both declarations; where waiver is mentioned

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). Live-page cross-check: text and history note identical to the leginfo page as returned by a second Exa connector (machine-compared).
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2103> (leginfo host: HTTP 403 Cloudflare challenge to curl, 03:29:53Z–03:29:55Z; see "How this file was produced", item 1)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19601.lob` (772 bytes; ZIP CRC-32 `6e82e460` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2103.20164747`).
- **Retrieved (UTC):** 2026-11-01T03:32:07Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2016, Ch. 474, Sec. 7. (AB 2882) Effective January 1, 2017."
- **Effective-date field:** 2017-01-01 (OP_STATUES/OP_CHAPTER/OP_SECTION: 2016 / 474 / 7)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_9dc23f76-bbd5-11e6-bdd8-d5db002bdb48`; SHA-256 of the XML record `176ea7dc88d8abff8cc35cf362e2780d366a09df062770884a4b70bb7c2d5797`

### (2) Operative text (verbatim)

> In order to provide full and accurate disclosure of all assets and liabilities in which one or both parties may have an interest, each party to a proceeding for dissolution of the marriage or legal separation of the parties shall serve on the other party a preliminary declaration of disclosure under Section 2104, unless service of the preliminary declaration of disclosure is waived as provided in Section 2107 or is not required pursuant to Section 2110, and a final declaration of disclosure under Section 2105, unless service of the final declaration of disclosure is waived pursuant to Section 2105, 2107, or 2110, and shall file proof of service of each with the court.

### (3) ELEMENTS

1. Purpose clause: “In order to provide full and accurate disclosure of all assets and liabilities in which one or both parties may have an interest”
2. Who: “each party to a proceeding for dissolution of the marriage or legal separation of the parties”
3. Duty — preliminary: “shall serve on the other party a preliminary declaration of disclosure under Section 2104”
4. Exceptions — preliminary: “unless service of the preliminary declaration of disclosure is waived as provided in Section 2107 or is not required pursuant to Section 2110”
5. Duty — final: “and a final declaration of disclosure under Section 2105”
6. Exceptions — final: “unless service of the final declaration of disclosure is waived pursuant to Section 2105, 2107, or 2110”
7. Filing: “and shall file proof of service of each with the court.”
8. The section states no number of days: the text is silent on timing (the periods are in § 2104(f) and § 2105(a)).

## 4. Family Code § 2104 — cross-reference only (check result; NOT re-retrieved)

- **Check requested:** "2104 subdivision (f) only if not already in the earlier file". **Result: it is already there.** `VERIFIED_AT_SOURCE_2026-11-01_FAM_disclosure.md`, Part 1 ("Family Code § 2104"), subsection "(2) Operative text (verbatim)", paragraph beginning "(f) The petitioner shall serve the other party" (line 47 of that file; the whole section 2104, subdivisions (a)–(f), is reproduced there with its record identifiers). Not re-retrieved, as instructed.
- **Metadata-only comparison (the XML record was NOT re-read):** this session’s `LAW_SECTION_TBL.dat` row for FAM 2104 (row ID `FAM2104.201911519`) carries LAW_SECTION_VERSION_ID `id_424eb5b3-0bb2-11ea-912d-915c88c10a14` and history note "Amended by Stats. 2019, Ch. 115, Sec. 19. (AB 1817) Effective January 1, 2020." — identical to the earlier file’s record identifiers and history note. The `pubinfo_2025.zip` snapshot is the same file (same Last-Modified date).
- **Where this file uses § 2104:** the timing words of subdivision (f) are quoted in Part 15 (1) and used in Part 16, each marked "[E]" (earlier file).

## 5. Family Code § 2105 — Final declaration of disclosure; the mutual waiver of the FINAL declaration and its required representations

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). Live-page cross-check: text and history note identical to the leginfo page as returned by a second Exa connector (machine-compared).
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2105> (leginfo host: HTTP 403 Cloudflare challenge to curl, 03:29:53Z–03:29:55Z; see "How this file was produced", item 1)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19603.lob` (3,905 bytes; ZIP CRC-32 `55e75ce7` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2105.20017034`).
- **Retrieved (UTC):** 2026-11-01T03:32:07Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2001, Ch. 703, Sec. 4. Effective January 1, 2002."
- **Effective-date field:** 2002-01-01 (OP_STATUES/OP_CHAPTER/OP_SECTION: 2001 / 703 / 4)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f62de11-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `6d41f5153345598b5fcdcff83368d5d9475ad9c2d44e05b954effed0e2d3c0e6`

### (2) Operative text (verbatim)

> (a) Except by court order for good cause, before or at the time the parties enter into an agreement for the resolution of property or support issues other than pendente lite support, or, if the case goes to trial, no later than 45 days before the first assigned trial date, each party, or the attorney for the party in this matter, shall serve on the other party a final declaration of disclosure and a current income and expense declaration, executed under penalty of perjury on a form prescribed by the Judicial Council, unless the parties mutually waive the final declaration of disclosure. The commission of perjury on the final declaration of disclosure by a party may be grounds for setting aside the judgment, or any part or parts thereof, pursuant to Chapter 10 (commencing with Section 2120), in addition to any and all other remedies, civil or criminal, that otherwise are available under law for the commission of perjury.
>
> (b) The final declaration of disclosure shall include all of the following information:
>
> (1) All material facts and information regarding the characterization of all assets and liabilities.
>
> (2) All material facts and information regarding the valuation of all assets that are contended to be community property or in which it is contended the community has an interest.
>
> (3) All material facts and information regarding the amounts of all obligations that are contended to be community obligations or for which it is contended the community has liability.
>
> (4) All material facts and information regarding the earnings, accumulations, and expenses of each party that have been set forth in the income and expense declaration.
>
> (c) In making an order setting aside a judgment for failure to comply with this section, the court may limit the set aside to those portions of the judgment materially affected by the nondisclosure.
>
> (d) The parties may stipulate to a mutual waiver of the requirements of subdivision (a) concerning the final declaration of disclosure, by execution of a waiver under penalty of perjury entered into in open court or by separate stipulation. The waiver shall include all of the following representations:
>
> (1) Both parties have complied with Section 2104 and the preliminary declarations of disclosure have been completed and exchanged.
>
> (2) Both parties have completed and exchanged a current income and expense declaration, that includes all material facts and information regarding that party’s earnings, accumulations, and expenses.
>
> (3) Both parties have fully complied with Section 2102 and have fully augmented the preliminary declarations of disclosure, including disclosure of all material facts and information regarding the characterization of all assets and liabilities, the valuation of all assets that are contended to be community property or in which it is contended the community has an interest, and the amounts of all obligations that are contended to be community obligations or for which it is contended the community has liability.
>
> (4) The waiver is knowingly, intelligently, and voluntarily entered into by each of the parties.
>
> (5) Each party understands that this waiver does not limit the legal disclosure obligations of the parties, but rather is a statement under penalty of perjury that those obligations have been fulfilled. Each party further understands that noncompliance with those obligations will result in the court setting aside the judgment.

### (3) ELEMENTS

1. (a) Exception to the time rule: “Except by court order for good cause”
2. (a) Time — settlement: “before or at the time the parties enter into an agreement for the resolution of property or support issues other than pendente lite support”
3. (a) Time — trial: “if the case goes to trial, no later than 45 days before the first assigned trial date”
4. (a) Who and what: “each party, or the attorney for the party in this matter, shall serve on the other party a final declaration of disclosure and a current income and expense declaration, executed under penalty of perjury on a form prescribed by the Judicial Council”
5. (a) The waiver reference: “unless the parties mutually waive the final declaration of disclosure.”
6. (a) Perjury: “The commission of perjury on the final declaration of disclosure by a party may be grounds for setting aside the judgment, or any part or parts thereof, pursuant to Chapter 10 (commencing with Section 2120)”.
7. (b) Contents — “The final declaration of disclosure shall include all of the following information:” (1) “All material facts and information regarding the characterization of all assets and liabilities.” (2) “All material facts and information regarding the valuation of all assets that are contended to be community property or in which it is contended the community has an interest.” (3) “All material facts and information regarding the amounts of all obligations that are contended to be community obligations or for which it is contended the community has liability.” (4) “All material facts and information regarding the earnings, accumulations, and expenses of each party that have been set forth in the income and expense declaration.”
8. (c) Scope of a set-aside: “In making an order setting aside a judgment for failure to comply with this section, the court may limit the set aside to those portions of the judgment materially affected by the nondisclosure.”
9. (d) Who may waive and what: “The parties may stipulate to a mutual waiver of the requirements of subdivision (a) concerning the final declaration of disclosure”
10. (d) How: “by execution of a waiver under penalty of perjury entered into in open court or by separate stipulation.”
11. (d) Required contents: “The waiver shall include all of the following representations:”
12. (d)(1): “Both parties have complied with Section 2104 and the preliminary declarations of disclosure have been completed and exchanged.”
13. (d)(2): “Both parties have completed and exchanged a current income and expense declaration, that includes all material facts and information regarding that party’s earnings, accumulations, and expenses.”
14. (d)(3): “Both parties have fully complied with Section 2102 and have fully augmented the preliminary declarations of disclosure, including disclosure of all material facts and information regarding the characterization of all assets and liabilities, the valuation of all assets that are contended to be community property or in which it is contended the community has an interest, and the amounts of all obligations that are contended to be community obligations or for which it is contended the community has liability.”
15. (d)(4): “The waiver is knowingly, intelligently, and voluntarily entered into by each of the parties.”
16. (d)(5): “Each party understands that this waiver does not limit the legal disclosure obligations of the parties, but rather is a statement under penalty of perjury that those obligations have been fulfilled. Each party further understands that noncompliance with those obligations will result in the court setting aside the judgment.”
17. What § 2105 says about the preliminary declaration: the words "preliminary declarations of disclosure" occur only in (d)(1) and (d)(3) (machine index, Appendix A): “the preliminary declarations of disclosure have been completed and exchanged”; “have fully augmented the preliminary declarations of disclosure”. No sentence of § 2105 waives, excuses or extends the preliminary declaration: the text is silent.

## 6. Family Code § 2106 — No judgment on property rights without the final declaration (and exceptions)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). Live-page cross-check: text and history note identical to the leginfo page as returned by a second Exa connector (machine-compared).
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2106> (leginfo host: HTTP 403 Cloudflare challenge to curl, 03:29:53Z–03:29:55Z; see "How this file was produced", item 1)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23719.lob` (870 bytes; ZIP CRC-32 `06ea0f18` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2106.201911520`).
- **Retrieved (UTC):** 2026-11-01T03:32:08Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2019, Ch. 115, Sec. 20. (AB 1817) Effective January 1, 2020."
- **Effective-date field:** 2020-01-01 (OP_STATUES/OP_CHAPTER/OP_SECTION: 2019 / 115 / 20)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_4a8cb1f5-0bb2-11ea-912d-915c88c10a14`; SHA-256 of the XML record `8495059fd066c838ae3d1853ca9c0dbe55c7cf2e8b295024904bcb64da28de30`

### (2) Operative text (verbatim)

> Except as provided in subdivision (d) of Section 2105, Section 2110, or absent good cause as provided in Section 2107, judgment shall not be entered with respect to the parties’ property rights without each party, or the attorney for that party in this matter, having executed and served a copy of the final declaration of disclosure and current income and expense declaration. Each party, or the party’s attorney, shall execute and file with the court a declaration signed under penalty of perjury stating that service of the final declaration of disclosure and current income and expense declaration was made on the other party or that service of the final declaration of disclosure has been waived pursuant to subdivision (d) of Section 2105 or in Section 2110.

### (3) ELEMENTS

1. Bar: “judgment shall not be entered with respect to the parties’ property rights without each party, or the attorney for that party in this matter, having executed and served a copy of the final declaration of disclosure and current income and expense declaration.”
2. Exceptions: “Except as provided in subdivision (d) of Section 2105, Section 2110, or absent good cause as provided in Section 2107”
3. Filing: “Each party, or the party’s attorney, shall execute and file with the court a declaration signed under penalty of perjury stating that service of the final declaration of disclosure and current income and expense declaration was made on the other party or that service of the final declaration of disclosure has been waived pursuant to subdivision (d) of Section 2105 or in Section 2110.”
4. The section speaks of the final declaration only; the word "preliminary" does not occur in it: the text is silent on the preliminary declaration (machine check).

## 7. Family Code § 2107 — cross-reference only (already verified in the earlier file; NOT re-retrieved)

- **Where:** `VERIFIED_AT_SOURCE_2026-11-01_FAM_disclosure.md`, Part 2 ("Family Code § 2107 — Remedies for non-compliance with disclosure requirements"), subsection "(2) Operative text (verbatim)" (lines 82–100 of that file); history note there: "Amended by Stats. 2015, Ch. 46, Sec. 3. (SB 340) Effective January 1, 2016."
- **Metadata-only comparison (the XML record was NOT re-read):** this session’s row for FAM 2107 (row ID `FAM2107.2015463`) carries LAW_SECTION_VERSION_ID `id_0c94b1bd-aa5d-11e5-828e-dfe62b045024` and history note "Amended by Stats. 2015, Ch. 46, Sec. 3. (SB 340) Effective January 1, 2016." — identical to the earlier file.
- **Pointers by subdivision (all quoted in Part 15 (3) and (5), marked "[E]"):** (a) the request step; (b)(1) motion to compel; (b)(2) motion to bar evidence; (b)(3) motion for the court to grant a "voluntary waiver of receipt"; (c) money sanctions; (d) set-aside of the judgment and the effect of a granted waiver; (e) court may order the exchanged declarations on a set-aside motion.

## 8. Family Code § 2110 — Default judgments: petitioner’s waiver of the final declaration; the preliminary declaration still required (CURRENT text)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). Live-page cross-check: text and history note identical to the leginfo page as returned by a second Exa connector (machine-compared).
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2110> (leginfo host: HTTP 403 Cloudflare challenge to curl, 03:29:53Z–03:29:55Z; see "How this file was produced", item 1)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23720.lob` (601 bytes; ZIP CRC-32 `474e0d74` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2110.2015464`).
- **Retrieved (UTC):** 2026-11-01T03:32:09Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2015, Ch. 46, Sec. 4. (SB 340) Effective January 1, 2016."
- **Effective-date field:** 2016-01-01 (OP_STATUES/OP_CHAPTER/OP_SECTION: 2015 / 46 / 4)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_0e98980f-aa5d-11e5-828e-dfe62b045024`; SHA-256 of the XML record `ec36db1571c28f77e6e4318d74fe1c9ec26146fae0be2b3c4ad944d9a5f663a9`

### (2) Operative text (verbatim)

> In the case of a default judgment, the petitioner may waive the final declaration of disclosure requirements provided in this chapter, and shall not be required to serve a final declaration of disclosure on the respondent nor receive a final declaration of disclosure from the respondent. However, a preliminary declaration of disclosure by the petitioner is required unless the petitioner served the summons and petition by publication or posting pursuant to court order and the respondent has defaulted.

### (3) ELEMENTS

1. Scope: “In the case of a default judgment”
2. Final declaration: “the petitioner may waive the final declaration of disclosure requirements provided in this chapter, and shall not be required to serve a final declaration of disclosure on the respondent nor receive a final declaration of disclosure from the respondent.”
3. Preliminary declaration: “However, a preliminary declaration of disclosure by the petitioner is required unless the petitioner served the summons and petition by publication or posting pursuant to court order and the respondent has defaulted.”
4. Who holds the waiver: the section names “the petitioner” only; the text is silent on a waiver by a respondent under this section.
5. Definition used (adjacent, Part 13.1): § 2101(b) — “does not include a stipulated judgment or any judgment pursuant to a marital settlement agreement” (applies to the defined term “Default judgment”).

### (4) PENDING — chaptered amendment, NOT CURRENT LAW as of this retrieval: AB 2782 (Stats. 2026, ch. 640), section 6

- **Status:** PENDING (not current law). The code-table row for § 2110 still shows "Amended by Stats. 2015, Ch. 46, Sec. 4. (SB 340) Effective January 1, 2016." and the text above; the amendment below is in a chaptered bill that has not yet been merged into the code table.
- **Source:** bill 202520260AB2782, version `20250AB278294CHP` (Chaptered), ZIP entry `BILL_VERSION_TBL_18865.lob` (86,933 bytes; CRC-32 `ea78287d` verified), retrieved 2026-11-01T03:42:48Z from <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip>; SHA-256 of the XML record `34c7c70d1ee28952b4b193c51ffd00025f7a3d81aa32cc24642ba1d2d8cc3038`.
- **Bill title (from the record):** "An act to amend Sections 2981, 2982, and 2982.2 of the Civil Code, to amend Sections 568.1 and 704.730 of the Code of Civil Procedure, to amend Section 2110 of the Family Code, to amend Section 2699.3 of the Labor Code, and to amend Sections 1063, 9763, and 16350 of the Probate Code, relating to state government."
- **Bill data fields:** GeneralSubject "Judiciary omnibus."; VoteRequired MAJORITY; Urgency NO; ImmediateEffect NO. History actions in the record: INTRODUCED 2026-03-11; AMENDED_ASSEMBLY 2026-04-08; AMENDED_SENATE 2026-05-20 and 2026-06-15; PASSED_SENATE 2026-08-27; PASSED_ASSEMBLY 2026-08-28; ENROLLED 2026-09-02; CHAPTERED, APPROVED and FILED 2026-09-27; ChapterYear 2026, ChapterNum 640.
- **Operative date:** the § 2110 section of the bill states none. The bill has no urgency clause; the general rule for such statutes would make the operative date 1 January 2027 — that rule is not in the retrieved text and is not independently verified here. Confirm on the leginfo bill page.
- **Digest item (3), verbatim from the bill record:**

> Existing law requires each party to a proceeding for dissolution of marriage or legal separation to serve on the other party a preliminary declaration of disclosure of assets, as specified, and a final declaration of disclosure, as specified. In the case of a default judgment, existing law prohibits a petitioner from being required to serve or receive a final declaration of disclosure, but still requires a preliminary declaration of disclosure, except as specified. This bill would provide that both parties are not required to exchange declarations of disclosure in a dissolution of marriage or registered domestic partnership if the parties have an existing enforceable judgment of legal separation that adjudicates the division of property.

- **Text of § 2110 as amended (verbatim from the bill’s section 6; that section of the bill record carries no strike-out or italic markup, so which words are new is not marked in the source — comparison with the current text is by machine below):**

> (a) In the case of a default judgment, the petitioner may waive the final declaration of disclosure requirements provided in this chapter, and shall not be required to serve a final declaration of disclosure on the respondent nor receive a final declaration of disclosure from the respondent. However, a preliminary declaration of disclosure by the petitioner is required unless the petitioner served the summons and petition by publication or posting pursuant to court order and the respondent has defaulted.
>
> (b) The petitioner and respondent shall not be required to exchange declarations of disclosure pursuant to Sections 2104 and 2105 in a dissolution of marriage or registered domestic partnership if the parties have an existing enforceable judgment of legal separation that adjudicates the division of property.

**ELEMENTS of the pending text**

1. Subdivision (a) of the pending text is word-for-word the current § 2110 text (machine-compared: identical).
2. New subdivision (b): “The petitioner and respondent shall not be required to exchange declarations of disclosure pursuant to Sections 2104 and 2105 in a dissolution of marriage or registered domestic partnership if the parties have an existing enforceable judgment of legal separation that adjudicates the division of property.”
3. Condition: “if the parties have an existing enforceable judgment of legal separation that adjudicates the division of property”
4. Digest wording: “This bill would provide that both parties are not required to exchange declarations of disclosure in a dissolution of marriage or registered domestic partnership if the parties have an existing enforceable judgment of legal separation that adjudicates the division of property.”
5. The pending text is silent on any waiver by stipulation or motion and on the timing of the preliminary declaration.

## 9. Family Code § 2111 — Disclosure and the attorney work product privilege / protective orders

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). Live-page cross-check: text and history note identical to the leginfo page as returned by a second Exa connector (machine-compared).
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2111> (leginfo host: HTTP 403 Cloudflare challenge to curl, 03:29:53Z–03:29:55Z; see "How this file was produced", item 1)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23721.lob` (248 bytes; ZIP CRC-32 `45f8706f` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2111.1993110113`).
- **Retrieved (UTC):** 2026-11-01T03:32:09Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 1101, Sec. 13. Effective October 11, 1993. Operative January 1, 1994, by Sec. 18 of Ch. 1101."
- **Effective-date field:** 1993-10-11 (OP_STATUES/OP_CHAPTER/OP_SECTION: 1993 / 1101 / 13)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f65eb5d-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `d6b02330594ba21f5093c66698a1898f0b9f1315eeee28db3518199018281829`

### (2) Operative text (verbatim)

> A disclosure required by this chapter does not abrogate the attorney work product privilege or impede the power of the court to issue protective orders.

### (3) ELEMENTS

1. Rule: “A disclosure required by this chapter does not abrogate the attorney work product privilege or impede the power of the court to issue protective orders.”
2. Two things the section says disclosure does not displace: “the attorney work product privilege” and “the power of the court to issue protective orders”.
3. The section contains no word of waiver and no number of days: the text is silent on both (machine check).

## 10. Family Code § 2112 — Judicial Council to adopt forms

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). Live-page cross-check: text and history note identical to the leginfo page as returned by a second Exa connector (machine-compared).
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2112> (leginfo host: HTTP 403 Cloudflare challenge to curl, 03:29:53Z–03:29:55Z; see "How this file was produced", item 1)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19606.lob` (216 bytes; ZIP CRC-32 `7a1a877f` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2112.1993110114`).
- **Retrieved (UTC):** 2026-11-01T03:32:10Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 1101, Sec. 14. Effective October 11, 1993. Operative January 1, 1994, by Sec. 18 of Ch. 1101."
- **Effective-date field:** 1993-10-11 (OP_STATUES/OP_CHAPTER/OP_SECTION: 1993 / 1101 / 14)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f65eb5f-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `f6de06f571c6d61022a38e92c642ded3c50c8e2a0ab6abb83ea4c9f63282a0e2`

### (2) Operative text (verbatim)

> The Judicial Council shall adopt appropriate forms and modify existing forms to effectuate the purposes of this chapter.

### (3) ELEMENTS

1. Actor and duty: “The Judicial Council shall adopt appropriate forms and modify existing forms”
2. Purpose: “to effectuate the purposes of this chapter.”
3. The section names no form number: the text is silent on which forms (compare § 2104(a) and § 2105(a), which say “on a form prescribed by the Judicial Council”).

## 11. California Rules of Court, rule 5.260 — as published by the Judicial Council (requested; see flag 1)

### (1) Source record

- **Status:** VERIFIED at the official source (direct fetch of the Judicial Council page) — **but the published rule is not about declarations of disclosure** (see ELEMENTS 9–10).
- **URL actually fetched:** <https://courts.ca.gov/cms/rules/index.cfm?title=five&linkid=rule5_260> (final URL <https://courts.ca.gov/cms/rules/index/five/rule5_260>; also fetched as `www.courts.ca.gov/...` and directly at the final URL — three captures, identical bytes).
- **Retrieved (UTC):** 2026-11-01T03:32:50Z to 03:32:52Z. SHA-256 of the HTML received: `438c4e6ff7ad0b6429cb98aafea79668481a5e8e8dbbacb39dd99dd04970a1a4` (275,182 bytes).
- **Page title:** "Rule 5.260. General provisions regarding support cases | Judicial Branch of California"; edition label on the page: **California Rules of Court 2026**.
- **Page’s own history notes:** "Rule 5.260 adopted effective January 1, 2013." and "Title 5, Family and Juvenile Rules-Division 1, Family Rules-Chapter 9, Child, Spousal, and Domestic Partner Support-Article 2, Certification of Statewide Uniform Guideline Support Calculators; amended January 1, 2013; adopted as Chapter 6." (as printed on the page).
- **Text source:** the page’s rule-content container (25 paragraphs); subdivision headings were bold on the page and are shown in bold; italics shown with asterisks; whitespace normalised; no words altered.

### (2) Operative text (verbatim)

> **(a) Financial declarations**
>
> Except as provided below, for all hearings involving child, spousal, or domestic partner support, both parties must complete, file, and serve a current *Income and Expense Declaration* (form FL-150) on all parties.
>
> (1) A party requesting support orders must include a current, completed *Income and Expense Declaration* (form FL-150) with the *Request for Order* (form FL-300) that is filed with the court and served on all parties.
>
> (2) A party responding to a request for support orders must include a current, completed *Income and Expense Declaration* (form FL-150) with the *Responsive Declaration to Request for Order* (form FL-320) that is filed with the court and served on all parties.
>
> (3) "Current" means the form has been completed within the past three months providing no facts have changed. The form must be sufficiently completed to allow the court to make an order.
>
> (4) In child support hearings, a party may complete a current *Financial Statement (Simplified)* (form FL-155) instead of a current *Income and Expense Declaration* (form FL-150) if he or she meets the requirements allowing submission of a *Financial Statement (Simplified)* (form FL-155).
>
> (5) *Financial Statement (Simplified)* (form FL-155) is not appropriate for use in proceedings to determine or modify spousal or domestic partner support, to determine or modify family support, or to determine attorney's fees and costs.
>
> **(b) Deviations from guideline child support in orders and judgments**
>
> (1) If a party contends that the amount of support as calculated under the statewide uniform guideline formula is inappropriate, that party must file a declaration stating the amount of support alleged to be proper and the factual and legal bases justifying a deviation from guideline support under Family Code section 4057.
>
> (2) In its discretion, for good cause shown, the court may deviate from the amount of guideline support resulting from the computer calculation. If the court finds good cause to deviate from the statewide uniform guideline formula for child support, the court must state its findings in writing or on the record as required by Family Code sections 4056, 4057, and 4065.
>
> (3) Stipulated agreements for child support that deviate from the statewide uniform guideline must include either a *Non-Guideline Child Support Findings Attachment* (form FL-342(A)) or language in the agreement or judgment conforming with Family Code sections 4056 and 4065.
>
> **(c) Request to change prior support orders**
>
> The supporting declaration submitted in a request to change a prior child, spousal, or domestic partner support order must include specific facts demonstrating a change of circumstances. No change of circumstances must be shown to change a previously agreed upon child support order that was below the child support guidelines.
>
> **(d) Notification to the local child support agency**
>
> The party requesting court orders must provide the local child support agency timely notice of any request to establish, change, or enforce any child, spousal, or domestic partner support order if the agency is providing support enforcement services or has intervened in the case as described in Family Code section 17400.
>
> **(e) Judgment for support**
>
> (1) If child support is an issue in a judgment:
>
> (A) Each party should file a proposed support calculation with the proposed judgment that sets forth the party's assumptions with regard to gross income, tax filing status, time-share, add-on expenses, and any other factor relevant to the support calculation.
>
> (B) The moving party should file the documents in (A) with the proposed judgment if the judgment is based on respondent's default or a stipulation of the parties.
>
> (C) The court may use and must permit parties or their attorneys to use any software certified by the Judicial Council to present support calculations to the court.
>
> (2) If spousal or domestic partner support is an issue in a judgment:
>
> (A) Use of support calculation software is not appropriate when requesting a judgment or modification of a judgment for spousal or domestic partner support.
>
> (B) Petitioner or the parties may use *Spousal or Partnership Support Declaration Attachment* (form FL-157) to address the issue of spousal or domestic partner support under Family Code section 4320 when relevant to the case.
>
> Rule 5.260 adopted effective January 1, 2013.
>
> Title 5, Family and Juvenile Rules-Division 1, Family Rules-Chapter 9, Child, Spousal, and Domestic Partner Support-Article 2, Certification of Statewide Uniform Guideline Support Calculators; amended January 1, 2013; adopted as Chapter 6.

### (3) ELEMENTS

1. (a) Scope: “for all hearings involving child, spousal, or domestic partner support” (carve-out: “Except as provided below”).
2. (a) Duty: “both parties must complete, file, and serve a current Income and Expense Declaration (form FL-150) on all parties.”
3. (a)(1) Requesting party: “must include a current, completed Income and Expense Declaration (form FL-150) with the Request for Order (form FL-300) that is filed with the court and served on all parties.”
4. (a)(2) Responding party: “must include a current, completed Income and Expense Declaration (form FL-150) with the Responsive Declaration to Request for Order (form FL-320) that is filed with the court and served on all parties.”
5. (a)(3) Meaning of "current": “means the form has been completed within the past three months providing no facts have changed.” “The form must be sufficiently completed to allow the court to make an order.”
6. (a)(4)–(5) Simplified statement: “In child support hearings, a party may complete a current Financial Statement (Simplified) (form FL-155) instead of a current Income and Expense Declaration (form FL-150)”; “is not appropriate for use in proceedings to determine or modify spousal or domestic partner support, to determine or modify family support, or to determine attorney's fees and costs.”
7. (b)(1) Deviations: “If a party contends that the amount of support as calculated under the statewide uniform guideline formula is inappropriate, that party must file a declaration stating the amount of support alleged to be proper and the factual and legal bases justifying a deviation from guideline support under Family Code section 4057.”
8. (c), (d), (e): request to change prior support orders; notice to the local child support agency; judgment for support — see the verbatim text above (headings: “(c) Request to change prior support orders”; “(d) Notification to the local child support agency”; “(e) Judgment for support”).
9. What the rule does NOT contain: the word "disclosure" does not occur in the rule text and none of Family Code §§ 2100–2113 is cited (machine check: no "disclos", no "preliminary", no "2100"–"2113"). The text is silent on declarations of disclosure, on the timing of a preliminary or final declaration of disclosure, on forms for them, and on waiver.
10. Where the Judicial Council text does speak to a declaration of disclosure: not in rule 5.260 — see Part 14 (rules 5.83(c)(4)(C) and 5.12(b)). The Judicial Council’s Title Five table of contents (263 rule links) has no rule whose title contains "disclosure".
11. Cross-reference by words only: § 2104(e) [E] uses “a completed income and expense declaration unless an income and expense declaration has already been provided and is current and valid”; rule 5.260(a)(3) defines "current" (element 5). Neither text refers to the other (rule 5.260 does not cite § 2104); the text is silent on whether the rule 5.260(a)(3) meaning applies to § 2104(e).

## 12. Judicial Council form FL-144 — "Stipulation and Waiver of Final Declaration of Disclosure"

### (1) Source record

- **Status:** VERIFIED at the official source (direct fetch of the form PDF from the Judicial Council site).
- **URL requested:** <https://courts.ca.gov/documents/fl144.pdf> (and `www.courts.ca.gov/documents/fl144.pdf`) → HTTP 301 → **<https://courts.ca.gov/sites/default/files/courts/default/2024-11/fl144.pdf>** (HTTP 200, `application/pdf`; two captures, identical bytes).
- **Retrieved (UTC):** 2026-11-01T03:33:56Z (both captures within that second). Server headers on the PDF: `last-modified: Thu, 28 Nov 2024 07:21:33 GMT`; `etag: "674819fd-a77d"`; 42,877 bytes. SHA-256 `102991083d5e64762afd0161d797ac5329a6891cbf315d1ac59c51ffc021cb6c`.
- **REVISION DATE (printed on the form, lower left): "FL-144 [Rev. January 1, 2007]"**, with "Form Approved for Optional Use" and "Judicial Council of California"; lower right: "Family Code, §§ 2102, 2104, 2105(d)" and "www.courtinfo.ca.gov"; "Page 1 of 1".
- **PDF metadata (not the revision date):** Title "FL-144 STIPULATION AND WAIVER OF FINAL DECLARATION OF DISCLOSURE"; Author "Judicial Council of California"; CreationDate Mon Dec 16 20:39:24 2019 UTC; ModDate Tue Sep 8 18:26:11 2020 UTC; 1 page; XFA form file.
- **Text extraction:** the PDF carries a "copy: no" permission flag; the standard `pdftotext` returned the text layer without error and no permission was altered or bypassed. The rendered page image was also read by eye and matches the text layer (including "Family Law section 2102" in item 2.c).
- **Forms index:** the Judicial Council forms-index search (`courts.ca.gov/forms-rules/court-forms?filter=FL144`) is script/reCAPTCHA-driven; its static HTML has no FL-144 entry and the "Latest Changes" page (static HTML) has no FL-14x mention. Not used. The printed revision date above is therefore the only revision record I have.

### (2) Printed text (verbatim; header boxes, blanks, signature captions and screen-only buttons omitted from the block)

> **STIPULATION AND WAIVER OF FINAL DECLARATION OF DISCLOSURE**
>
> 1. Under Family Code section 2105(d), the parties agree to waive the requirements of Family Code section 2105(a) concerning the final declaration of disclosure.
>
> 2. The parties agree as follows:
>
> a. We have complied with Family Code section 2104, and the preliminary declarations of disclosure have been completed and exchanged.
>
> b. We have completed and exchanged a current *Income and Expense Declaration* (form FL-150) that includes all material facts and information on each party's earnings, accumulations, and expenses.
>
> c. We have fully complied with Family Law section 2102 and have fully augmented the preliminary declarations of disclosure, including disclosure of all material facts and information on
>
> (1) the characterization of all assets and liabilities,
>
> (2) the valuation of all assets that are community property or in which the community has an interest, and
>
> (3) the amounts of all community debts and obligations.
>
> d. Each of the parties enters into this waiver knowingly, intelligently, and voluntarily.
>
> e. Each party understands that this waiver does not limit the legal disclosure obligations of the parties but rather is a statement under penalty of perjury that those obligations have been fulfilled.
>
> f. The parties also understand that if they do not comply with these obligations, the court will set aside the judgment.
>
> The petitioner and respondent declare under penalty of perjury under the laws of the State of California that the foregoing is true and correct.
>
> Date: ________
>
> ________ (TYPE OR PRINT NAME)    ________ (SIGNATURE OF PETITIONER)
>
> ________ (TYPE OR PRINT NAME)    ________ (SIGNATURE OF RESPONDENT)

The form’s caption boxes (attorney or party without attorney; court; PLAINTIFF/PETITIONER; DEFENDANT/RESPONDENT; OTHER; CASE NUMBER) are blank fields. The footer also prints "For your protection and privacy, please press the Clear This Form button after you have printed the form." beside "Print this form / Save this form / Clear this form" (screen-only).

### (3) ELEMENTS

1. Title: “STIPULATION AND WAIVER OF FINAL DECLARATION OF DISCLOSURE”
2. Item 1 (the waiver): “Under Family Code section 2105(d), the parties agree to waive the requirements of Family Code section 2105(a) concerning the final declaration of disclosure.”
3. Item 2 lead-in: “The parties agree as follows:”
4. Item 2.a: “We have complied with Family Code section 2104, and the preliminary declarations of disclosure have been completed and exchanged.” (compare § 2105(d)(1), Part 5).
5. Item 2.b: “We have completed and exchanged a current Income and Expense Declaration (form FL-150) that includes all material facts and information on each party's earnings, accumulations, and expenses.” (compare § 2105(d)(2)).
6. Item 2.c: “We have fully complied with Family Law section 2102 and have fully augmented the preliminary declarations of disclosure, including disclosure of all material facts and information on” (1) “the characterization of all assets and liabilities,” (2) “the valuation of all assets that are community property or in which the community has an interest, and” (3) “the amounts of all community debts and obligations.” (compare § 2105(d)(3); the form prints "Family Law section 2102" as quoted).
7. Item 2.d: “Each of the parties enters into this waiver knowingly, intelligently, and voluntarily.” (compare § 2105(d)(4)).
8. Item 2.e: “Each party understands that this waiver does not limit the legal disclosure obligations of the parties but rather is a statement under penalty of perjury that those obligations have been fulfilled.” (compare the first sentence of § 2105(d)(5)).
9. Item 2.f: “The parties also understand that if they do not comply with these obligations, the court will set aside the judgment.” (compare the second sentence of § 2105(d)(5)).
10. Declaration: “The petitioner and respondent declare under penalty of perjury under the laws of the State of California that the foregoing is true and correct.”
11. Signers: “(SIGNATURE OF PETITIONER)” and “(SIGNATURE OF RESPONDENT)”, with a “Date:” line.
12. Status words printed on the form: “Form Approved for Optional Use”; “FL-144 [Rev. January 1, 2007]”; “Family Code, §§ 2102, 2104, 2105(d)”.
13. The only places the form uses the words "preliminary declarations of disclosure" are items 2.a and 2.c; the only words of waiver are the title, item 1, item 2.d ("this waiver") and item 2.e ("this waiver"). No sentence of the form waives the preliminary declaration: the text is silent (machine index, Appendix B).

## 13. Adjacent sections of Chapter 9 (not requested; retrieved so the whole chapter 2100–2113 has been read)

Sections 2104 and 2107 are in the earlier file (Parts 4 and 7 above). The four below were retrieved by the same method; they are NOT cross-checked against the live page.

### 13.1. Family Code § 2101 — Definitions (adjacent)

#### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). ADJACENT (not requested). Not cross-checked against the live page.
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2101> (leginfo host: HTTP 403 for the eight requested sections; this URL not individually attempted)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23604.lob` (1,388 bytes; ZIP CRC-32 `0c75ffe2` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2101.19985815`).
- **Retrieved (UTC):** 2026-11-01T03:35:30Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 1998, Ch. 581, Sec. 5. Effective January 1, 1999."
- **Effective-date field:** 1999-01-01 (OP_STATUES/OP_CHAPTER/OP_SECTION: 1998 / 581 / 5)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f615769-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `eb703d291c07462b16f1eb4da3c4336aab5becf526b76531f969f837ea51d636`

#### (2) Operative text (verbatim)

> Unless the provision or context otherwise requires, the following definitions apply to this chapter:
>
> (a) “Asset” includes, but is not limited to, any real or personal property of any nature, whether tangible or intangible, and whether currently existing or contingent.
>
> (b) “Default judgment” does not include a stipulated judgment or any judgment pursuant to a marital settlement agreement.
>
> (c) “Earnings and accumulations” includes income from whatever source derived, as provided in Section 4058.
>
> (d) “Expenses” includes, but is not limited to, all personal living expenses, but does not include business related expenses.
>
> (e) “Income and expense declaration” includes the Income and Expense Declaration forms approved for use by the Judicial Council, and any other financial statement that is approved for use by the Judicial Council in lieu of the Income and Expense Declaration, if the financial statement form satisfies all other applicable criteria.
>
> (f) “Liability” includes, but is not limited to, any debt or obligation, whether currently existing or contingent.

#### (3) ELEMENTS

1. Lead-in: “Unless the provision or context otherwise requires, the following definitions apply to this chapter:”
2. (b): the defined term “Default judgment” “does not include a stipulated judgment or any judgment pursuant to a marital settlement agreement.”
3. (e): the defined term “Income and expense declaration” “includes the Income and Expense Declaration forms approved for use by the Judicial Council, and any other financial statement that is approved for use by the Judicial Council in lieu of the Income and Expense Declaration, if the financial statement form satisfies all other applicable criteria.”
4. (a), (c), (d), (f): definitions of “Asset”, “Earnings and accumulations”, “Expenses”, “Liability” — see the verbatim text.
5. The section defines no term “preliminary declaration” or “final declaration” and contains no word of waiver: the text is silent (machine check).

### 13.2. Family Code § 2108 — Liquidation of assets requires service of the appropriate declaration (adjacent)

#### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). ADJACENT (not requested). Not cross-checked against the live page.
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2108> (leginfo host: HTTP 403 for the eight requested sections; this URL not individually attempted)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_7.lob` (570 bytes; ZIP CRC-32 `1cb0f7ad` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2108.1993219107`).
- **Retrieved (UTC):** 2026-11-01T03:35:30Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 219, Sec. 107. Effective January 1, 1994."
- **Effective-date field:** 1994-01-01 (OP_STATUES/OP_CHAPTER/OP_SECTION: 1993 / 219 / 107)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f6464b7-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `09832abbc951f73c6d156ae6408a78adf5666b7265e9732c251ba343c788dfdc`

#### (2) Operative text (verbatim)

> At any time during the proceeding, the court has the authority, on application of a party and for good cause, to order the liquidation of community or quasi-community assets so as to avoid unreasonable market or investment risks, given the relative nature, scope, and extent of the community estate. However, in no event shall the court grant the application unless, as provided in this chapter, the appropriate declaration of disclosure has been served by the moving party.

#### (3) ELEMENTS

1. Authority: “At any time during the proceeding, the court has the authority, on application of a party and for good cause, to order the liquidation of community or quasi-community assets so as to avoid unreasonable market or investment risks, given the relative nature, scope, and extent of the community estate.”
2. Condition: “However, in no event shall the court grant the application unless, as provided in this chapter, the appropriate declaration of disclosure has been served by the moving party.”
3. The text is silent on waiver and on a number of days.

### 13.3. Family Code § 2109 — Summary dissolution (adjacent)

#### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). ADJACENT (not requested). Not cross-checked against the live page.
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2109> (leginfo host: HTTP 403 for the eight requested sections; this URL not individually attempted)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19605.lob` (278 bytes; ZIP CRC-32 `4deb945a` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2109.1993110111`).
- **Retrieved (UTC):** 2026-11-01T03:35:31Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 1101, Sec. 11. Effective October 11, 1993. Operative January 1, 1994, by Sec. 18 of Ch. 1101."
- **Effective-date field:** 1993-10-11 (OP_STATUES/OP_CHAPTER/OP_SECTION: 1993 / 1101 / 11)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f6464b9-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `5bbe136837a4e4a1da4095284a77b74052d0b60132d3eae494c1371ba0803315`

#### (2) Operative text (verbatim)

> The provisions of this chapter requiring a final declaration of disclosure do not apply to a summary dissolution of marriage, but a preliminary declaration of disclosure is required.

#### (3) ELEMENTS

1. Rule: “The provisions of this chapter requiring a final declaration of disclosure do not apply to a summary dissolution of marriage, but a preliminary declaration of disclosure is required.”
2. Words of exclusion: “The provisions of this chapter requiring a final declaration of disclosure do not apply to a summary dissolution of marriage”; words of requirement: “but a preliminary declaration of disclosure is required.”
3. The text is silent on waiver and on a number of days.

### 13.4. Family Code § 2113 — Application date of the chapter (adjacent)

#### (1) Source record

- **Status:** VERIFIED at the official source (Legislature’s own data publication; the leginfo HTML page was unreachable — see "How this file was produced"). ADJACENT (not requested). Not cross-checked against the live page.
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2113> (leginfo host: HTTP 403 for the eight requested sections; this URL not individually attempted)
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19607.lob` (173 bytes; ZIP CRC-32 `990b9aaa` verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat` (row ID `FAM2113.1993110110`).
- **Retrieved (UTC):** 2026-11-01T03:35:32Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by renumbering Section 2109 (as added by Stats. 1993, Ch. 219) by Stats. 1993, Ch. 1101, Sec. 10. Effective October 11, 1993. Operative January 1, 1994, by Sec. 18 of Ch. 1101."
- **Effective-date field:** 1993-10-11 (OP_STATUES/OP_CHAPTER/OP_SECTION: 1993 / 1101 / 10)
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f65eb61-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `d8890c736276422c690f7a64ba3148db1859e38073fcb896960a6c91efcfd37a`

#### (2) Operative text (verbatim)

> This chapter applies to any proceeding commenced on or after January 1, 1993.

#### (3) ELEMENTS

1. Rule: “This chapter applies to any proceeding commenced on or after January 1, 1993.”
2. Date comparison (not an interpretation): the petition filing date in the brief, 1/16/2024, is later than 1/1/1993.

## 14. Adjacent: Family Rules that refer to the Family Code disclosure requirements (found by the Title Five scan; not requested)

**Scan method and result.** I fetched the 124 rule pages of Title Five, Division 1 (Family Rules, rules 5.1–5.496; 03:36:05Z–03:37:23Z) and searched each rule’s text for "disclos" and for FL-14x / FL-150 / FL-160 / § 21xx references. Rules whose text refers to the Family Code disclosure requirements or to a declaration of disclosure: **5.12(b)**, **5.77(a)** (summary dissolution; not reproduced here) and **5.83(c)(4)(C)**. Rule 5.92 cites rule 5.260 only for when an FL-150 is "current". All other hits were unrelated uses of "disclose/disclosure" (mediator and evaluator conflicts, ex parte applications, tribal-court related cases, limited-scope representation, etc.). I did not read the other 122 pages word for word.

### 14.1 Rule 5.83 (Family centered case resolution), subdivision (c)(4)(C)

- **URL actually fetched:** <https://courts.ca.gov/cms/rules/index/five/rule5_83> — retrieved within the 03:36:05Z–03:37:23Z window; SHA-256 of the HTML `788f9745707c8ca599b09654850b873ef96015eb0e1a81a97b236593342fe900` (200,643 bytes). Page’s own history note: "Rule 5.83 amended effective January 1, 2016; adopted effective January 1, 2012."

> (c) Family centered case resolution process
>
> (4) In deciding whether a case is progressing in an effective and timely manner, the court should consider procedural milestones including the following:
>
> (A) A proof of service of summons and petition should be filed within 60 days of case initiation;
>
> (B) If no response has been filed, and the parties have not agreed on an extension of time to respond, a request to enter default should be submitted within 60 days after the date the response was due;
>
> (C) The petitioner's preliminary declaration of disclosure should be served within 60 days of the filing of the petition;
>
> (D) When a default has been entered, a judgment should be submitted within 60 days of the entry of default;

ELEMENTS: (1) the stem: “In deciding whether a case is progressing in an effective and timely manner, the court should consider procedural milestones including the following:”; (2) the milestone: “The petitioner's preliminary declaration of disclosure should be served within 60 days of the filing of the petition;”; (3) the rule’s stated purpose: “This rule establishes processes and procedures for courts to manage cases from initial filing to final disposition in an effective and timely manner.”; (4) the rule names the petitioner’s declaration only; the text is silent on the respondent’s declaration and on waiver (machine check: the rule text contains "disclos" once, in this milestone, and no "waiv").

### 14.2 Rule 5.12 (Request for order regarding discovery), subdivision (b)

- **URL actually fetched:** <https://courts.ca.gov/cms/rules/index/five/rule5_12> — retrieved within the 03:36:05Z–03:37:23Z window; SHA-256 of the HTML `0e90fb139f8826d7a773571782f9e275f4ec00d4f3c9bfd2b3ad43a9ff92c3e0` (271,615 bytes). Page’s own history note: "Rule 5.12 amended effective July 1, 2016; adopted effective January 1, 2013."

> (b) Applicable law
>
> A request for order regarding discovery in family court is subject to the provisions for discovery motions under Code of Civil Procedure sections 2016.010 through 2036.050 and Family Code sections 2100 through 2113 regarding disclosure of assets and liabilities.

ELEMENTS: (1) “A request for order regarding discovery in family court is subject to the provisions for discovery motions under Code of Civil Procedure sections 2016.010 through 2036.050 and Family Code sections 2100 through 2113 regarding disclosure of assets and liabilities.” (2) The rule text is silent on timing and waiver of a declaration of disclosure.

## 15. WHAT THE WORDS SAY — no opinion

Every line below is a quotation with its source, a pointer to one, or the words "the text is silent". "[this file]" = the Part named; "[E]" = `VERIFIED_AT_SOURCE_2026-11-01_FAM_disclosure.md` (FAM 2104 and 2107, not re-retrieved). Every quotation was machine-checked against the retrieved text of the source named.

### (1) Which declaration each party must serve, and when

**Preliminary declaration — who and what**

- § 2103 [Part 3]: “each party to a proceeding for dissolution of the marriage or legal separation of the parties shall serve on the other party a preliminary declaration of disclosure under Section 2104”
- § 2104(a) [E]: “each party shall serve on the other party a preliminary declaration of disclosure, executed under penalty of perjury on a form prescribed by the Judicial Council.”
- § 2104(e) [E]: “Along with the preliminary declaration of disclosure, each party shall provide the other party with a completed income and expense declaration unless an income and expense declaration has already been provided and is current and valid.”

**Preliminary declaration — when (the timing words)**

- § 2104(f) [E], petitioner: “The petitioner shall serve the other party with the preliminary declaration of disclosure either concurrently with the petition for dissolution or legal separation, or within 60 days of filing the petition.”
- § 2104(f) [E], respondent: “The respondent shall serve the other party with the preliminary declaration of disclosure either concurrently with the response to the petition, or within 60 days of filing the response.”
- § 2104(f) [E], publication or posting: “When a petitioner serves the summons and petition by publication or posting pursuant to court order and the respondent files a response prior to a default judgment being entered, the petitioner shall serve the other party with the preliminary declaration of disclosure within 30 days of the response being filed.”
- § 2104(f) [E], extension: “The time periods specified in this subdivision may be extended by written agreement of the parties or by court order.”
- § 2104(a) [E], exception words: “Except by court order for good cause, as provided in Section 2107, or when service of the preliminary declaration of disclosure is not required pursuant to Section 2110, in the time period set forth in subdivision (f)”
- Filing and proof of service: § 2104(b) [E] “The preliminary declaration of disclosure shall not be filed with the court, except on court order. However, the parties shall file proof of service of the preliminary declaration of disclosure with the court.” And § 2103: “and shall file proof of service of each with the court.”
- Pointers for what the preliminary declaration contains and how it may be changed: § 2104(a) last sentence, (c), (d) [E] — see the earlier file, Part 1, subsections (2) and (3).
- Rule 5.83(c)(4) [Part 14.1]: “In deciding whether a case is progressing in an effective and timely manner, the court should consider procedural milestones including the following:” — “The petitioner's preliminary declaration of disclosure should be served within 60 days of the filing of the petition;”
- Rule 5.260 [Part 11]: the text is silent on when a declaration of disclosure is to be served.

**Final declaration — who, what, when**

- § 2105(a) [Part 5]: “Except by court order for good cause, before or at the time the parties enter into an agreement for the resolution of property or support issues other than pendente lite support, or, if the case goes to trial, no later than 45 days before the first assigned trial date, each party, or the attorney for the party in this matter, shall serve on the other party a final declaration of disclosure and a current income and expense declaration, executed under penalty of perjury on a form prescribed by the Judicial Council, unless the parties mutually waive the final declaration of disclosure.”

**Continuing duty (both declarations)**

- § 2100(c) [Part 1]: “each party has a continuing duty to immediately, fully, and accurately update and augment that disclosure to the extent there have been any material changes”
- § 2102(a)(1) [Part 2]: “including an immediate, full, and accurate update or augmentation to the extent there have been material changes.”

### (2) The declaration the statute lets the parties waive by stipulation — the exact words

- § 2105(a): “unless the parties mutually waive the final declaration of disclosure.”
- § 2105(d): “The parties may stipulate to a mutual waiver of the requirements of subdivision (a) concerning the final declaration of disclosure, by execution of a waiver under penalty of perjury entered into in open court or by separate stipulation. The waiver shall include all of the following representations:”
- § 2105(d)(1): “Both parties have complied with Section 2104 and the preliminary declarations of disclosure have been completed and exchanged.”
- § 2105(d)(2): “Both parties have completed and exchanged a current income and expense declaration, that includes all material facts and information regarding that party’s earnings, accumulations, and expenses.”
- § 2105(d)(3): “Both parties have fully complied with Section 2102 and have fully augmented the preliminary declarations of disclosure, including disclosure of all material facts and information regarding the characterization of all assets and liabilities, the valuation of all assets that are contended to be community property or in which it is contended the community has an interest, and the amounts of all obligations that are contended to be community obligations or for which it is contended the community has liability.”
- § 2105(d)(4): “The waiver is knowingly, intelligently, and voluntarily entered into by each of the parties.”
- § 2105(d)(5): “Each party understands that this waiver does not limit the legal disclosure obligations of the parties, but rather is a statement under penalty of perjury that those obligations have been fulfilled. Each party further understands that noncompliance with those obligations will result in the court setting aside the judgment.”
- Pointers: § 2103 “unless service of the final declaration of disclosure is waived pursuant to Section 2105, 2107, or 2110”; § 2106 “Except as provided in subdivision (d) of Section 2105, Section 2110, or absent good cause as provided in Section 2107”; § 2110 “the petitioner may waive the final declaration of disclosure requirements provided in this chapter”

### (3) What the statute says about the PRELIMINARY declaration and waiver

**Words of requirement**

- § 2103 and § 2104(a): quoted in (1).
- § 2109 [Part 13.3]: “but a preliminary declaration of disclosure is required.”
- § 2110 [Part 8]: “However, a preliminary declaration of disclosure by the petitioner is required unless the petitioner served the summons and petition by publication or posting pursuant to court order and the respondent has defaulted.”

**Words of exception or waiver**

- § 2103: “unless service of the preliminary declaration of disclosure is waived as provided in Section 2107 or is not required pursuant to Section 2110”
- § 2104(a) [E]: “Except by court order for good cause, as provided in Section 2107, or when service of the preliminary declaration of disclosure is not required pursuant to Section 2110”

**The court-order route in § 2107 [E, Part 2 of the earlier file]**

- § 2107(a): “If one party fails to serve on the other party a preliminary declaration of disclosure under Section 2104, unless that party is not required to serve a preliminary declaration of disclosure pursuant to Section 2110, or a final declaration of disclosure under Section 2105, or fails to provide the information required in the respective declarations with sufficient particularity, and if the other party has served the respective declaration of disclosure on the noncomplying party, the complying party may, within a reasonable time, request preparation of the appropriate declaration of disclosure or further particularity.”
- § 2107(b): “If the noncomplying party fails to comply with a request under subdivision (a), the complying party may do one or more of the following:”
- § 2107(b)(3): “File a motion showing good cause for the court to grant the complying party’s voluntary waiver of receipt of the noncomplying party’s preliminary declaration of disclosure pursuant to Section 2104 or final declaration of disclosure pursuant to Section 2105. The voluntary waiver does not affect the rights enumerated in subdivision (d).”
- § 2107(d), the sentence on a granted waiver: “If the court granted the complying party’s voluntary waiver of receipt of the noncomplying party’s preliminary declaration of disclosure pursuant to paragraph (3) of subdivision (b), the court shall set aside the judgment only at the request of the complying party, unless the motion to set aside the judgment is based on one of the following:”
- § 2107(d)(1): “Actual fraud if the defrauded party was kept in ignorance or in some other manner was fraudulently prevented from fully participating in the proceeding.”
- § 2107(d)(2): “Perjury, as defined in Section 118 of the Penal Code, in the preliminary or final declaration of disclosure, in the waiver of the final declaration of disclosure, or in the current income and expense statement.”

**Waiver of the preliminary declaration by stipulation**

- A stipulation of the parties to waive the preliminary declaration, as § 2105(d) provides for the final declaration: the text is silent — no sentence of §§ 2100–2113 (as retrieved here and in [E]) provides for it. Appendix A lists every paragraph of the chapter in which "waive", "waiver" or "waived" occurs.
- A sentence forbidding a waiver of the preliminary declaration: the text is silent.
- Words that bear on excusing or waiving the preliminary declaration (pointers, all quoted above): § 2103; § 2104(a) [E]; § 2107(b)(3) [E]; § 2107(d) [E].
- The only agreement words attached to the preliminary declaration: § 2104(f) [E] “The time periods specified in this subdivision may be extended by written agreement of the parties or by court order.” and § 2105(d)(1) “the preliminary declarations of disclosure have been completed and exchanged.”
- Pending, NOT CURRENT LAW (AB 2782, Part 8): “The petitioner and respondent shall not be required to exchange declarations of disclosure pursuant to Sections 2104 and 2105 in a dissolution of marriage or registered domestic partnership if the parties have an existing enforceable judgment of legal separation that adjudicates the division of property.”

### (4) What the FL-144 recitals say the signers are agreeing to; what the form does and does not waive by its own words

- Title [Part 12]: “STIPULATION AND WAIVER OF FINAL DECLARATION OF DISCLOSURE”
- Item 1: “Under Family Code section 2105(d), the parties agree to waive the requirements of Family Code section 2105(a) concerning the final declaration of disclosure.”
- Item 2.a: “We have complied with Family Code section 2104, and the preliminary declarations of disclosure have been completed and exchanged.”
- Item 2.b: “We have completed and exchanged a current Income and Expense Declaration (form FL-150) that includes all material facts and information on each party's earnings, accumulations, and expenses.”
- Item 2.c: “We have fully complied with Family Law section 2102 and have fully augmented the preliminary declarations of disclosure, including disclosure of all material facts and information on (1) the characterization of all assets and liabilities, (2) the valuation of all assets that are community property or in which the community has an interest, and (3) the amounts of all community debts and obligations.”
- Item 2.d: “Each of the parties enters into this waiver knowingly, intelligently, and voluntarily.”
- Item 2.e: “Each party understands that this waiver does not limit the legal disclosure obligations of the parties but rather is a statement under penalty of perjury that those obligations have been fulfilled.”
- Item 2.f: “The parties also understand that if they do not comply with these obligations, the court will set aside the judgment.”
- Declaration: “The petitioner and respondent declare under penalty of perjury under the laws of the State of California that the foregoing is true and correct.”
- What the form waives, by its words: “the requirements of Family Code section 2105(a) concerning the final declaration of disclosure”
- What the form says its waiver does not do, by its words: “this waiver does not limit the legal disclosure obligations of the parties”
- The preliminary declaration in the form: the words appear only in items 2.a and 2.c ("have been completed and exchanged"; "have fully augmented"); the form contains no sentence waiving the preliminary declaration — the text is silent.

Side by side (quotations only): § 2105(d)(1)–(5) and the FL-144 items printed to correspond to them (compare Part 5 and Part 12).

| § 2105(d) | FL-144 |
|---|---|
| (d)(1) “Both parties have complied with Section 2104 and the preliminary declarations of disclosure have been completed and exchanged.” | Item 2.a: “We have complied with Family Code section 2104, and the preliminary declarations of disclosure have been completed and exchanged.” |
| (d)(2) “Both parties have completed and exchanged a current income and expense declaration, that includes all material facts and information regarding that party’s earnings, accumulations, and expenses.” | Item 2.b: “We have completed and exchanged a current Income and Expense Declaration (form FL-150) that includes all material facts and information on each party's earnings, accumulations, and expenses.” |
| (d)(3) “Both parties have fully complied with Section 2102 and have fully augmented the preliminary declarations of disclosure, including disclosure of all material facts and information regarding the characterization of all assets and liabilities, the valuation of all assets that are contended to be community property or in which it is contended the community has an interest, and the amounts of all obligations that are contended to be community obligations or for which it is contended the community has liability.” | Item 2.c: “We have fully complied with Family Law section 2102 and have fully augmented the preliminary declarations of disclosure, including disclosure of all material facts and information on (1) the characterization of all assets and liabilities, (2) the valuation of all assets that are community property or in which the community has an interest, and (3) the amounts of all community debts and obligations.” |
| (d)(4) “The waiver is knowingly, intelligently, and voluntarily entered into by each of the parties.” | Item 2.d: “Each of the parties enters into this waiver knowingly, intelligently, and voluntarily.” |
| (d)(5) “Each party understands that this waiver does not limit the legal disclosure obligations of the parties, but rather is a statement under penalty of perjury that those obligations have been fulfilled. Each party further understands that noncompliance with those obligations will result in the court setting aside the judgment.” | Items 2.e and 2.f: “Each party understands that this waiver does not limit the legal disclosure obligations of the parties but rather is a statement under penalty of perjury that those obligations have been fulfilled.” “The parties also understand that if they do not comply with these obligations, the court will set aside the judgment.” |

### (5) Remedies the statute names for non-service — § 2107(b)–(d) [E, Part 2 of the earlier file]

- § 2107(b)(1): “File a motion to compel a further response.”
- § 2107(b)(2): “File a motion for an order preventing the noncomplying party from presenting evidence on issues that should have been covered in the declaration of disclosure.”
- § 2107(b)(3): “File a motion showing good cause for the court to grant the complying party’s voluntary waiver of receipt of the noncomplying party’s preliminary declaration of disclosure pursuant to Section 2104 or final declaration of disclosure pursuant to Section 2105. The voluntary waiver does not affect the rights enumerated in subdivision (d).”
- § 2107(c): “If a party fails to comply with any provision of this chapter, the court shall, in addition to any other remedy provided by law, impose money sanctions against the noncomplying party. Sanctions shall be in an amount sufficient to deter repetition of the conduct or comparable conduct, and shall include reasonable attorney’s fees, costs incurred, or both, unless the court finds that the noncomplying party acted with substantial justification or that other circumstances make the imposition of the sanction unjust.”
- § 2107(d): “Except as otherwise provided in this subdivision, if a court enters a judgment when the parties have failed to comply with all disclosure requirements of this chapter, the court shall set aside the judgment. The failure to comply with the disclosure requirements does not constitute harmless error. If the court granted the complying party’s voluntary waiver of receipt of the noncomplying party’s preliminary declaration of disclosure pursuant to paragraph (3) of subdivision (b), the court shall set aside the judgment only at the request of the complying party, unless the motion to set aside the judgment is based on one of the following:”
- § 2107(d)(1): “Actual fraud if the defrauded party was kept in ignorance or in some other manner was fraudulently prevented from fully participating in the proceeding.”
- § 2107(d)(2): “Perjury, as defined in Section 118 of the Penal Code, in the preliminary or final declaration of disclosure, in the waiver of the final declaration of disclosure, or in the current income and expense statement.”
- Pointers: § 2107(a) (request step, quoted in (3)); § 2107(e) [E] “Upon the motion to set aside judgment, the court may order the parties to provide the preliminary and final declarations of disclosure that were exchanged between them.”
- Related words in this file: § 2106 [Part 6] “judgment shall not be entered with respect to the parties’ property rights without each party, or the attorney for that party in this matter, having executed and served a copy of the final declaration of disclosure and current income and expense declaration.”; § 2108 [Part 13.2] “in no event shall the court grant the application unless, as provided in this chapter, the appropriate declaration of disclosure has been served by the moving party.”
- Pointer to the earlier file: § 2122(f) ("Failure to comply with the disclosure requirements of Chapter 9") and its one-year period are quoted in `VERIFIED_AT_SOURCE_2026-11-01_FAM_disclosure.md`, Part 5.

## 16. ARITHMETIC ONLY — FAM 2104(f) against the record dates

Record dates are those given in the brief and were not checked against the case file: petition filed **1/16/2024**; Petitioner’s FL-141 declares service **6/18/2024**. Words used: “The petitioner shall serve the other party with the preliminary declaration of disclosure either concurrently with the petition for dissolution or legal separation, or within 60 days of filing the petition.” [E].

| Step | Date | Weekday |
|---|---|---|
| Petition filed (day 0) | 2024-01-16 | Tuesday |
| Day 60 (filing + 60 days; February 2024 has 29 days) | 2024-03-16 | Saturday |
| Service date declared on Petitioner’s FL-141 | 2024-06-18 | Tuesday |

- Days from filing (1/16/2024) to 6/18/2024: **154** (22 weeks exactly).
- Days from day 60 (3/16/2024) to 6/18/2024: **94**.
- Calendar fact only: 3/16/2024 is a Saturday; the next Monday, 3/18/2024, is 92 days before 6/18/2024. The retrieved text of § 2104(f) states no counting convention and no rule for a last day that falls on a weekend: the text is silent. The computation-of-time statutes (Code of Civil Procedure §§ 12 and 12a) were not retrieved.
- Extension words: “The time periods specified in this subdivision may be extended by written agreement of the parties or by court order.” [E]. No written agreement or order was supplied with the brief.
- Respondent’s own period: “within 60 days of filing the response” [E] — the date the response was filed was not supplied; not computed.
- "Concurrently" alternative: “either concurrently with the petition for dissolution or legal separation” [E] — the date the petition was served was not supplied; not computed.
- Other timing words for comparison, not computed: “The petitioner's preliminary declaration of disclosure should be served within 60 days of the filing of the petition;” (rule 5.83(c)(4)(C)).

**Version in force on the record dates.** The history notes of the sections reproduced or cited show their latest amendments took effect before the petition date (comparison of dates only):

| Authority | Latest-amendment effective date (per its history note) | Earlier than 2024-01-16? |
|---|---|---|
| FAM 2100 | 2002-01-01 (Amended by Stats. 2001, Ch. 703, Sec. 2. Effective January 1, 2002.) | yes |
| FAM 2102 | 2020-01-01 (Amended by Stats. 2019, Ch. 115, Sec. 18. (AB 1817) Effective January 1, 2020.) | yes |
| FAM 2103 | 2017-01-01 (Amended by Stats. 2016, Ch. 474, Sec. 7. (AB 2882) Effective January 1, 2017.) | yes |
| FAM 2104 [E] | 2020-01-01 (Amended by Stats. 2019, Ch. 115, Sec. 19. (AB 1817) Effective January 1, 2020.) | yes |
| FAM 2105 | 2002-01-01 (Amended by Stats. 2001, Ch. 703, Sec. 4. Effective January 1, 2002.) | yes |
| FAM 2106 | 2020-01-01 (Amended by Stats. 2019, Ch. 115, Sec. 20. (AB 1817) Effective January 1, 2020.) | yes |
| FAM 2107 [E] | 2016-01-01 (Amended by Stats. 2015, Ch. 46, Sec. 3. (SB 340) Effective January 1, 2016.) | yes |
| FAM 2110 (current text) | 2016-01-01 (Amended by Stats. 2015, Ch. 46, Sec. 4. (SB 340) Effective January 1, 2016.) | yes |
| FAM 2111 | 1993-10-11 (Added by Stats. 1993, Ch. 1101, Sec. 13. Effective October 11, 1993. Operative January 1, 1994, by Sec. 18 of Ch. 1101.) | yes |
| FAM 2112 | 1993-10-11 (Added by Stats. 1993, Ch. 1101, Sec. 14. Effective October 11, 1993. Operative January 1, 1994, by Sec. 18 of Ch. 1101.) | yes |
| Rule 5.260 | "Rule 5.260 adopted effective January 1, 2013." (page note; nothing later on the page) | yes |
| Form FL-144 | "[Rev. January 1, 2007]" (printed) | yes |
| FAM 2110 pending text | AB 2782, approved 2026-09-27 | no — after the record dates; not current law (Part 8) |

## 17. Limits, and what was not retrieved or not read

1. **Not retrieved:** Family Code § 721 (cited by § 2102) and § 4058; Code of Civil Procedure §§ 12 and 12a (counting days); the printed text of forms FL-140, FL-141, FL-142, FL-150 and FL-160 (FL-141 is mentioned only as the brief describes it); the constitutional or statutory source of the general 1 January operative-date rule for non-urgency statutes; rule 5.77 (summary dissolution); local court rules; case law.
2. **Read in full by me:** the twelve statute texts reproduced in Parts 1–3, 5, 6, 8–10 and 13; rule 5.260; rule 5.83 and rule 5.12 (both whole pages’ rule text); the FL-144 printed text and its rendered image; AB 2782’s title, history, digest item (3) and § 2110 section.
3. **Not read word for word:** the other 122 Family Rules pages (machine-scanned only); the 2,254 chaptered bills (machine-scanned only); the other nine sections of AB 2782; the Judicial Council forms-index and "Latest Changes" pages (static HTML searched for "FL-144"/"FL-14x" only).
4. **Cross-check coverage:** eight requested sections were compared with the live leginfo pages (identical); sections 2101, 2108, 2109 and 2113 and the pending AB 2782 text were not.
5. **Currency:** the data-file snapshot is dated 2026-10-25; the Legislature’s incremental files up to 30 Oct 2026 contain no law-section tables; the bill scan covers all bills chaptered in 2025 and 2026 in the data-file snapshot. Statutes chaptered later than the snapshot would not be seen. AB 2782 is the one chaptered change found for §§ 2100–2119 (Part 8).
6. **Rule and form currency:** the rule pages show the edition label "California Rules of Court 2026"; no amendment to rule 5.260 or 5.83 is shown on their pages. The only revision record for FL-144 is the printed "Rev. January 1, 2007" (Part 12). I did not search for Judicial Council proposals effective 1 January 2027.
7. **Record dates** (petition 1/16/2024; FL-141 service 6/18/2024) come from the brief, not from case documents.
8. **Not legal advice.** Research support only.

## Appendix A — machine index of "waive/waiver/waived" and "preliminary" in Family Code §§ 2100–2113

Generated by script from the texts above (FAM 2104 and 2107 from the earlier file). Each row is a paragraph (subdivision) in which the word occurs. Sections not listed contain neither word. This index supports the statements above that the text is silent where it says so.

| Provision | Waiver words in the paragraph | Count of "preliminary" |
|---|---|---|
| FAM 2103 (lead-in) | waived | 2 |
| FAM 2104 [E](a) | — | 4 |
| FAM 2104 [E](b) | — | 2 |
| FAM 2104 [E](c) | — | 1 |
| FAM 2104 [E](c)(2) | — | 1 |
| FAM 2104 [E](d) | — | 1 |
| FAM 2104 [E](e) | — | 1 |
| FAM 2104 [E](f) | — | 3 |
| FAM 2105(a) | waive | — |
| FAM 2105(d) | waiver | — |
| FAM 2105(d)(1) | — | 1 |
| FAM 2105(d)(3) | — | 1 |
| FAM 2105(d)(4) | waiver | — |
| FAM 2105(d)(5) | waiver | — |
| FAM 2106 (lead-in) | waived | — |
| FAM 2107 [E](a) | — | 2 |
| FAM 2107 [E](b)(3) | waiver | 1 |
| FAM 2107 [E](d) | waiver | 1 |
| FAM 2107 [E](d)(2) | waiver | 1 |
| FAM 2107 [E](e) | — | 1 |
| FAM 2109 (lead-in) | — | 1 |
| FAM 2110 (lead-in) | waive | 1 |
| FAM 2110 [pending AB 2782, not current law](a) | waive | 1 |

## Appendix B — machine index of the FL-144 text layer

- Occurrences of "waive/waiver" in the recitals: 4 — in the title, item 1 ("agree to waive"), item 2.d ("this waiver") and item 2.e ("this waiver").
- Occurrences of "preliminary" in the recitals: 2 — item 2.a and item 2.c.

