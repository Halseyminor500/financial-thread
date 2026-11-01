# Family Code — disclosure and relief from judgment (§§ 2104, 2107, 2120-2129)

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `FAM_disclosure` · sections: FAM 2104, 2107, 2120, 2121, 2122, 2123, 2124, 2125, 2126, 2127, 2128, 2129

## How this file was produced (read first)

1. **Direct fetch of the leginfo HTML page failed.** On 2026-11-01 curl (through the session proxy) and WebFetch received HTTP 403 with a Cloudflare "Just a moment..." JavaScript challenge for `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118` (01:56:59Z) and the same challenge for two other leginfo paths (`/faces/codes.xhtml`, `/faces/codes_displayText.xhtml`; 01:57:38Z). This is the origin site's bot challenge, not an egress-proxy policy denial (the proxy log was clean). No attempt was made to defeat the challenge. The first Exa connector returned HTTP 402 (credit limit) at 01:57:36Z.
2. **Text source actually used.** The Legislature's own data publication behind the leginfo site: `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` (HTTP Last-Modified Mon, 26 Oct 2026 04:26:08 GMT; entries dated 2026-10-25). Read by HTTP byte-range requests: the ZIP central directory, `LAW_SECTION_TBL.dat` (section metadata incl. the official history note), `LAW_TOC_TBL.dat` (official headings) and one `LAW_SECTION_TBL_<n>.lob` XML record per section. Every entry passed its ZIP CRC-32 check; each section's SHA-256 is listed in its source record.
3. **Independent cross-check against the live page.** A second Exa connector fetched live leginfo pages. Penal Code § 118: text identical to the record (machine-compared). Code of Civil Procedure § 1010.6: identical on visual comparison of subdivisions (a)-(e)(4)(C). Code of Civil Procedure § 473: the live page presents a two-version selection list whose history notes match the record. Other sections were not individually cross-checked against the live page.
4. **Rendering.** The source is Legislative Counsel XML. Only whitespace is normalised (source line-wrap whitespace collapsed to single spaces; the XML en-space/em-space spacing elements shown as one space); no word, number, punctuation or subdivision label is altered. Italic markup is shown with asterisks; the source's underlined signature leader (CCP 415.30 form only) is shown as "[underlined signature line]". Curly quotes and apostrophes are as in the source.
5. **Currency as of 2026-11-01.** The publication was generated 2026-10-25. The Legislature's later incremental update files (pubinfo_Mon/Wed/Thu, last-modified 27, 29 and 30 Oct 2026) contain no law-section tables, i.e. no code-section changes between the snapshot and 30 Oct 2026 (no later incremental file had been published at retrieval). The law tables include 2026-session statutes (latest cited: Stats. 2026, ch. 1036). Every bill chaptered in 2025 (991 bills; 4,663 amendment action lines) and in 2026 (1,263 bills; 5,684 action lines) was scanned for amendments to the sections in the whole LAW/ set: the only hits were AB 747 (Stats. 2025, ch. 563 -> CCP § 473) and AB 540 (Stats. 2026, ch. 263 -> CCP § 1010.6); both are handled in `VERIFIED_AT_SOURCE_2026-11-01_CCP_service.md`.
6. **Limits.** No case law, annotations or secondary sources were consulted; "ELEMENTS" are drawn only from the quoted statutory words (every quoted phrase was machine-checked against the retrieved text). Statutes enacted in 2026 that take effect 1 Jan 2027 are not yet in the code tables except as noted. This is legal research support, not legal advice.


> **Structure:** §§ 2104 and 2107 are in Division 6, Part 1, Chapter 9 ("Disclosure of Assets and Liabilities [2100 - 2113]"); §§ 2120-2129 are in Chapter 10 ("Relief From Judgment [2120 - 2129]"). § 2104(a) refers to "Chapter 10 (commencing with Section 2120)" and § 2120(a) refers to "Chapter 9 (commencing with Section 2100)". All twelve sections are reproduced in full.


## 1. Family Code § 2104 — Preliminary declaration of disclosure

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2104> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19602.lob` (3,393 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:07Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2019, Ch. 115, Sec. 19. (AB 1817) Effective January 1, 2020."
- **Effective-date field:** 2020-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_424eb5b3-0bb2-11ea-912d-915c88c10a14`; SHA-256 of the XML record `07379f8b3e5bfcafc64bb36fdef8868f481142e7f0dd790e63a3eb30aed07aaa`

### (2) Operative text (verbatim)

> (a) Except by court order for good cause, as provided in Section 2107, or when service of the preliminary declaration of disclosure is not required pursuant to Section 2110, in the time period set forth in subdivision (f), each party shall serve on the other party a preliminary declaration of disclosure, executed under penalty of perjury on a form prescribed by the Judicial Council. The commission of perjury on the preliminary declaration of disclosure may be grounds for setting aside the judgment, or any part or parts thereof, pursuant to Chapter 10 (commencing with Section 2120), in addition to any and all other remedies, civil or criminal, that otherwise are available under law for the commission of perjury. The preliminary declaration of disclosure shall include all tax returns filed by the declarant within the two years prior to the date that the party served the declaration.
>
> (b) The preliminary declaration of disclosure shall not be filed with the court, except on court order. However, the parties shall file proof of service of the preliminary declaration of disclosure with the court.
>
> (c) The preliminary declaration of disclosure shall set forth with sufficient particularity, that a person of reasonable and ordinary intelligence can ascertain, all of the following:
>
> (1) The identity of all assets in which the declarant has or may have an interest and all liabilities for which the declarant is or may be liable, regardless of the characterization of the asset or liability as community, quasi-community, or separate.
>
> (2) The declarant’s percentage of ownership in each asset and percentage of obligation for each liability when property is not solely owned by one or both of the parties. The preliminary declaration may also set forth the declarant’s characterization of each asset or liability.
>
> (d) A declarant may amend the preliminary declaration of disclosure without leave of the court. Proof of service of an amendment shall be filed with the court.
>
> (e) Along with the preliminary declaration of disclosure, each party shall provide the other party with a completed income and expense declaration unless an income and expense declaration has already been provided and is current and valid.
>
> (f) The petitioner shall serve the other party with the preliminary declaration of disclosure either concurrently with the petition for dissolution or legal separation, or within 60 days of filing the petition. When a petitioner serves the summons and petition by publication or posting pursuant to court order and the respondent files a response prior to a default judgment being entered, the petitioner shall serve the other party with the preliminary declaration of disclosure within 30 days of the response being filed. The respondent shall serve the other party with the preliminary declaration of disclosure either concurrently with the response to the petition, or within 60 days of filing the response. The time periods specified in this subdivision may be extended by written agreement of the parties or by court order.

### (3) ELEMENTS

1. Who must act: “each party”.
2. Act: “shall serve on the other party a preliminary declaration of disclosure, executed under penalty of perjury on a form prescribed by the Judicial Council”.
3. Exceptions: “Except by court order for good cause, as provided in Section 2107, or when service of the preliminary declaration of disclosure is not required pursuant to Section 2110”.
4. Timing (subd. (f)): petitioner — “either concurrently with the petition for dissolution or legal separation, or within 60 days of filing the petition”; respondent — “either concurrently with the response to the petition, or within 60 days of filing the response”; publication/posting case — “within 30 days of the response being filed”; extension — “by written agreement of the parties or by court order”.
5. Content (subd. (c)): “with sufficient particularity, that a person of reasonable and ordinary intelligence can ascertain” (1) “The identity of all assets in which the declarant has or may have an interest and all liabilities for which the declarant is or may be liable, regardless of the characterization of the asset or liability as community, quasi-community, or separate.” and (2) the declarant's percentage of ownership/obligation.
6. Attachments: “all tax returns filed by the declarant within the two years prior to the date that the party served the declaration” (subd. (a)); “a completed income and expense declaration unless an income and expense declaration has already been provided and is current and valid” (subd. (e)).
7. Filing (subd. (b)): “shall not be filed with the court, except on court order. However, the parties shall file proof of service of the preliminary declaration of disclosure with the court.”
8. Amendment (subd. (d)): “A declarant may amend the preliminary declaration of disclosure without leave of the court. Proof of service of an amendment shall be filed with the court.”

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL (family law disclosure duty)**

CIVIL / PROCEDURAL (Family Code, Division 6, Part 1, Chapter 9, "Disclosure of Assets and Liabilities"). No criminal punishment is stated. The perjury link is in subd. (a): “The commission of perjury on the preliminary declaration of disclosure may be grounds for setting aside the judgment, or any part or parts thereof, pursuant to Chapter 10 (commencing with Section 2120), in addition to any and all other remedies, civil or criminal, that otherwise are available under law for the commission of perjury.”


## 2. Family Code § 2107 — Remedies for non-compliance with disclosure requirements

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2107> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19604.lob` (3,575 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:07Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2015, Ch. 46, Sec. 3. (SB 340) Effective January 1, 2016."
- **Effective-date field:** 2016-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 9. Disclosure of Assets and Liabilities [2100. - 2113.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_0c94b1bd-aa5d-11e5-828e-dfe62b045024`; SHA-256 of the XML record `8066d8b0d922f5b3fcd5226fe92c4be27bb61f579a10d88b1ed09cbf74f06539`

### (2) Operative text (verbatim)

> (a) If one party fails to serve on the other party a preliminary declaration of disclosure under Section 2104, unless that party is not required to serve a preliminary declaration of disclosure pursuant to Section 2110, or a final declaration of disclosure under Section 2105, or fails to provide the information required in the respective declarations with sufficient particularity, and if the other party has served the respective declaration of disclosure on the noncomplying party, the complying party may, within a reasonable time, request preparation of the appropriate declaration of disclosure or further particularity.
>
> (b) If the noncomplying party fails to comply with a request under subdivision (a), the complying party may do one or more of the following:
>
> (1) File a motion to compel a further response.
>
> (2) File a motion for an order preventing the noncomplying party from presenting evidence on issues that should have been covered in the declaration of disclosure.
>
> (3) File a motion showing good cause for the court to grant the complying party’s voluntary waiver of receipt of the noncomplying party’s preliminary declaration of disclosure pursuant to Section 2104 or final declaration of disclosure pursuant to Section 2105. The voluntary waiver does not affect the rights enumerated in subdivision (d).
>
> (c) If a party fails to comply with any provision of this chapter, the court shall, in addition to any other remedy provided by law, impose money sanctions against the noncomplying party. Sanctions shall be in an amount sufficient to deter repetition of the conduct or comparable conduct, and shall include reasonable attorney’s fees, costs incurred, or both, unless the court finds that the noncomplying party acted with substantial justification or that other circumstances make the imposition of the sanction unjust.
>
> (d) Except as otherwise provided in this subdivision, if a court enters a judgment when the parties have failed to comply with all disclosure requirements of this chapter, the court shall set aside the judgment. The failure to comply with the disclosure requirements does not constitute harmless error. If the court granted the complying party’s voluntary waiver of receipt of the noncomplying party’s preliminary declaration of disclosure pursuant to paragraph (3) of subdivision (b), the court shall set aside the judgment only at the request of the complying party, unless the motion to set aside the judgment is based on one of the following:
>
> (1) Actual fraud if the defrauded party was kept in ignorance or in some other manner was fraudulently prevented from fully participating in the proceeding.
>
> (2) Perjury, as defined in Section 118 of the Penal Code, in the preliminary or final declaration of disclosure, in the waiver of the final declaration of disclosure, or in the current income and expense statement.
>
> (e) Upon the motion to set aside judgment, the court may order the parties to provide the preliminary and final declarations of disclosure that were exchanged between them. Absent a court order to the contrary, the disclosure declarations shall not be filed with the court and shall be returned to the parties.

### (3) ELEMENTS

1. Request step (subd. (a)): precondition — one party “fails to serve on the other party a preliminary declaration of disclosure under Section 2104” (unless excused under § 2110), or a final declaration under § 2105, or “fails to provide the information required in the respective declarations with sufficient particularity”, AND “the other party has served the respective declaration of disclosure on the noncomplying party”; the complying party “may, within a reasonable time, request preparation of the appropriate declaration of disclosure or further particularity”.
2. Motions if the request is ignored (subd. (b)): “If the noncomplying party fails to comply with a request under subdivision (a)” the complying party may “File a motion to compel a further response”; “File a motion for an order preventing the noncomplying party from presenting evidence on issues that should have been covered in the declaration of disclosure”; or file a motion for a voluntary waiver of receipt (subd. (b)(3)).
3. Mandatory sanctions (subd. (c)): “If a party fails to comply with any provision of this chapter, the court shall, in addition to any other remedy provided by law, impose money sanctions against the noncomplying party.” Exceptions: “unless the court finds that the noncomplying party acted with substantial justification or that other circumstances make the imposition of the sanction unjust”.
4. Set-aside (subd. (d)): “if a court enters a judgment when the parties have failed to comply with all disclosure requirements of this chapter, the court shall set aside the judgment”; “The failure to comply with the disclosure requirements does not constitute harmless error.” Where a voluntary waiver was granted, the court sets the judgment aside “only at the request of the complying party, unless the motion to set aside the judgment is based on” (1) “Actual fraud if the defrauded party was kept in ignorance or in some other manner was fraudulently prevented from fully participating in the proceeding.” or (2) “Perjury, as defined in Section 118 of the Penal Code, in the preliminary or final declaration of disclosure, in the waiver of the final declaration of disclosure, or in the current income and expense statement.”
5. Court may order exchange of declarations on a set-aside motion (subd. (e)): “Upon the motion to set aside judgment, the court may order the parties to provide the preliminary and final declarations of disclosure that were exchanged between them.”

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL. Family Code, Division 6, Part 1, Chapter 9. No criminal punishment; the money sanctions in subd. (c) are civil. Cross-reference: subd. (d)(2) incorporates the Penal Code § 118 definition of perjury.


## 3. Family Code § 2120 — Legislative findings (relief from judgment)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2120> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23813.lob` (1,569 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:10Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 219, Sec. 108. Effective January 1, 1994."
- **Effective-date field:** 1994-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f677205-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `91e092c9d6bc37e6270b63fd867e9c6b10d08f7216c1257a3f4ff83cac65a9d8`

### (2) Operative text (verbatim)

> The Legislature finds and declares the following:
>
> (a) The State of California has a strong policy of ensuring the division of community and quasi-community property in the dissolution of a marriage as set forth in Division 7 (commencing with Section 2500), and of providing for fair and sufficient child and spousal support awards. These policy goals can only be implemented with full disclosure of community, quasi-community, and separate assets, liabilities, income, and expenses, as provided in Chapter 9 (commencing with Section 2100), and decisions freely and knowingly made.
>
> (b) It occasionally happens that the division of property or the award of support, whether made as a result of agreement or trial, is inequitable when made due to the nondisclosure or other misconduct of one of the parties.
>
> (c) The public policy of assuring finality of judgments must be balanced against the public interest in ensuring proper division of marital property, in ensuring sufficient support awards, and in deterring misconduct.
>
> (d) The law governing the circumstances under which a judgment can be set aside, after the time for relief under Section 473 of the Code of Civil Procedure has passed, has been the subject of considerable confusion which has led to increased litigation and unpredictable and inconsistent decisions at the trial and appellate levels.

### (3) ELEMENTS

1. This section states findings, not elements. It records the policy that “These policy goals can only be implemented with full disclosure of community, quasi-community, and separate assets, liabilities, income, and expenses”, that “It occasionally happens that the division of property or the award of support, whether made as a result of agreement or trial, is inequitable when made due to the nondisclosure or other misconduct of one of the parties”, and that “The public policy of assuring finality of judgments must be balanced against the public interest in ensuring proper division of marital property, in ensuring sufficient support awards, and in deterring misconduct.”

### (4) Nature of the provision / punishment

**Kind: CIVIL (legislative findings; no operative elements)**

CIVIL — legislative findings introducing Chapter 10, "Relief From Judgment" (Family Code §§ 2120–2129). No elements and no punishment.


## 4. Family Code § 2121 — Authority to grant relief; required findings

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2121> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23722.lob` (838 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:10Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 219, Sec. 108. Effective January 1, 1994."
- **Effective-date field:** 1994-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f677207-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `0e0d1726875e3cff1ddd705e74e0091168270be45255f3cccfa9ba7c8184157c`

### (2) Operative text (verbatim)

> (a) In proceedings for dissolution of marriage, for nullity of marriage, or for legal separation of the parties, the court may, on any terms that may be just, relieve a spouse from a judgment, or any part or parts thereof, adjudicating support or division of property, after the six-month time limit of Section 473 of the Code of Civil Procedure has run, based on the grounds, and within the time limits, provided in this chapter.
>
> (b) In all proceedings under this chapter, before granting relief, the court shall find that the facts alleged as the grounds for relief materially affected the original outcome and that the moving party would materially benefit from the granting of the relief.

### (3) ELEMENTS

1. Proceeding type (subd. (a)): “In proceedings for dissolution of marriage, for nullity of marriage, or for legal separation of the parties”.
2. Relief sought: the court “may, on any terms that may be just, relieve a spouse from a judgment, or any part or parts thereof, adjudicating support or division of property”.
3. Timing relative to CCP § 473: “after the six-month time limit of Section 473 of the Code of Civil Procedure has run”.
4. Grounds and time limits: “based on the grounds, and within the time limits, provided in this chapter” (§ 2122).
5. Mandatory findings before relief (subd. (b)): “the court shall find that the facts alleged as the grounds for relief materially affected the original outcome and that the moving party would materially benefit from the granting of the relief”.

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL. No punishment. The power is discretionary (“may”) but conditioned on the subd. (b) findings.


## 5. Family Code § 2122 — Grounds and time limits for a motion to set aside a judgment

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2122> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19608.lob` (1,986 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:08Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2001, Ch. 703, Sec. 7. Effective January 1, 2002."
- **Effective-date field:** 2002-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f677209-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `8571ef40685dca5ece32c91a24d858f92a72e560ffaa2743f45ed41cb97e9bba`

### (2) Operative text (verbatim)

> The grounds and time limits for a motion to set aside a judgment, or any part or parts thereof, are governed by this section and shall be one of the following:
>
> (a) Actual fraud where the defrauded party was kept in ignorance or in some other manner was fraudulently prevented from fully participating in the proceeding. An action or motion based on fraud shall be brought within one year after the date on which the complaining party either did discover, or should have discovered, the fraud.
>
> (b) Perjury. An action or motion based on perjury in the preliminary or final declaration of disclosure, the waiver of the final declaration of disclosure, or in the current income and expense statement shall be brought within one year after the date on which the complaining party either did discover, or should have discovered, the perjury.
>
> (c) Duress. An action or motion based upon duress shall be brought within two years after the date of entry of judgment.
>
> (d) Mental incapacity. An action or motion based on mental incapacity shall be brought within two years after the date of entry of judgment.
>
> (e) As to stipulated or uncontested judgments or that part of a judgment stipulated to by the parties, mistake, either mutual or unilateral, whether mistake of law or mistake of fact. An action or motion based on mistake shall be brought within one year after the date of entry of judgment.
>
> (f) Failure to comply with the disclosure requirements of Chapter 9 (commencing with Section 2100). An action or motion based on failure to comply with the disclosure requirements shall be brought within one year after the date on which the complaining party either discovered, or should have discovered, the failure to comply.

### (3) ELEMENTS

1. Lead-in: “The grounds and time limits for a motion to set aside a judgment, or any part or parts thereof, are governed by this section and shall be one of the following:” — the moving party must establish ONE ground and file within that ground's time limit:
   - (a) FRAUD — ground: “Actual fraud where the defrauded party was kept in ignorance or in some other manner was fraudulently prevented from fully participating in the proceeding.” Time: “within one year after the date on which the complaining party either did discover, or should have discovered, the fraud”.
   - (b) PERJURY — ground: “perjury in the preliminary or final declaration of disclosure, the waiver of the final declaration of disclosure, or in the current income and expense statement”. Time: “within one year after the date on which the complaining party either did discover, or should have discovered, the perjury”.
   - (c) DURESS — “An action or motion based upon duress shall be brought within two years after the date of entry of judgment.”
   - (d) MENTAL INCAPACITY — “An action or motion based on mental incapacity shall be brought within two years after the date of entry of judgment.”
   - (e) MISTAKE — ground: “As to stipulated or uncontested judgments or that part of a judgment stipulated to by the parties, mistake, either mutual or unilateral, whether mistake of law or mistake of fact.” Time: “within one year after the date of entry of judgment”.
   - (f) NON-DISCLOSURE — ground: “Failure to comply with the disclosure requirements of Chapter 9 (commencing with Section 2100).” Time: “within one year after the date on which the complaining party either discovered, or should have discovered, the failure to comply”.

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL. No punishment. The perjury ground in (b) is tied to the Penal Code definition by FAM § 2107(d)(2) (“Perjury, as defined in Section 118 of the Penal Code”).


## 6. Family Code § 2123 — Inequity alone is not a ground

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2123> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23605.lob` (413 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:09Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 219, Sec. 108. Effective January 1, 1994."
- **Effective-date field:** 1994-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f68f8ab-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `63ca20f27d78029bc828657af3478e7f4074444c9b4b4fb16771f4f3d65f4a8d`

### (2) Operative text (verbatim)

> Notwithstanding any other provision of this chapter, or any other law, a judgment may not be set aside simply because the court finds that it was inequitable when made, nor simply because subsequent circumstances caused the division of assets or liabilities to become inequitable, or the support to become inadequate.

### (3) ELEMENTS

1. Limitation: “a judgment may not be set aside simply because the court finds that it was inequitable when made, nor simply because subsequent circumstances caused the division of assets or liabilities to become inequitable, or the support to become inadequate”.
2. Scope: “Notwithstanding any other provision of this chapter, or any other law”.

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL (a limit on relief). No punishment.


## 7. Family Code § 2124 — Attorney negligence not imputed to client

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2124> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19609.lob` (339 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:08Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2019, Ch. 115, Sec. 21. (AB 1817) Effective January 1, 2020."
- **Effective-date field:** 2020-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_52be2b17-0bb2-11ea-912d-915c88c10a14`; SHA-256 of the XML record `17ff4120425be0fc0d95fc710cba21563687b3eeb3f85964df69888d4872ba35`

### (2) Operative text (verbatim)

> The negligence of an attorney shall not be imputed to a client to bar an order setting aside a judgment, unless the court finds that the client knew, or should have known, of the attorney’s negligence and unreasonably failed to self-protect.

### (3) ELEMENTS

1. Rule: “The negligence of an attorney shall not be imputed to a client to bar an order setting aside a judgment”.
2. Exception: “unless the court finds that the client knew, or should have known, of the attorney’s negligence and unreasonably failed to self-protect” — i.e. the opposing party must show (i) the client “knew, or should have known” of the negligence AND (ii) the client “unreasonably failed to self-protect”.

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL. No punishment.


## 8. Family Code § 2125 — Scope of what is set aside

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2125> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23606.lob` (407 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:09Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended (as added by Stats. 1993, Ch. 219) by Stats. 1993, Ch. 1101, Sec. 16. Effective October 11, 1993. Operative January 1, 1994, by Sec. 18 of Ch. 1101."
- **Effective-date field:** 1993-10-11
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f68f8af-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `08b8fa09ec23603199f34a406e8608546bfabd9369df5c5c0e037251ae3bfa0f`

### (2) Operative text (verbatim)

> When ruling on an action or motion to set aside a judgment, the court shall set aside only those provisions materially affected by the circumstances leading to the court’s decision to grant relief. However, the court has discretion to set aside the entire judgment, if necessary, for equitable considerations.

### (3) ELEMENTS

1. General rule: “the court shall set aside only those provisions materially affected by the circumstances leading to the court’s decision to grant relief”.
2. Discretion: “However, the court has discretion to set aside the entire judgment, if necessary, for equitable considerations.”

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL. No punishment.


## 9. Family Code § 2126 — Valuation date and division of re-opened assets

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2126> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23607.lob` (407 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:09Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 219, Sec. 108. Effective January 1, 1994."
- **Effective-date field:** 1994-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f68f8b1-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `4efe24910b0fe6d22500a83b6d3127a0b79b80a74e013197d7a731cb45355de3`

### (2) Operative text (verbatim)

> As to assets or liabilities for which a judgment or part of a judgment is set aside, the date of valuation shall be subject to equitable considerations. The court shall equally divide the asset or liability, unless the court finds upon good cause shown that the interests of justice require an unequal division.

### (3) ELEMENTS

1. Valuation date: “the date of valuation shall be subject to equitable considerations”.
2. Division: “The court shall equally divide the asset or liability, unless the court finds upon good cause shown that the interests of justice require an unequal division.”
3. Scope: applies “As to assets or liabilities for which a judgment or part of a judgment is set aside”.

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL. No punishment.


## 10. Family Code § 2127 — Statement of decision

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2127> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19627.lob` (282 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:08Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended (as added by Stats. 1993, Ch. 219) by Stats. 1993, Ch. 1101, Sec. 17. Effective October 11, 1993. Operative January 1, 1994, by Sec. 18 of Ch. 1101."
- **Effective-date field:** 1993-10-11
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f68f8b3-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `1758fd4547925e58e50a9f99affdef922c2d0869304f77683fd9b9e7d50578c9`

### (2) Operative text (verbatim)

> As to actions or motions filed under this chapter, if a timely request is made, the court shall render a statement of decision where the court has resolved controverted factual evidence.

### (3) ELEMENTS

1. Applies to “actions or motions filed under this chapter”.
2. Trigger: “if a timely request is made”.
3. Duty: “the court shall render a statement of decision where the court has resolved controverted factual evidence”.

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL. No punishment.


## 11. Family Code § 2128 — Savings provisions

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2128> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_23608.lob` (829 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:10Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 219, Sec. 108. Effective January 1, 1994."
- **Effective-date field:** 1994-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f6a7f55-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `430f0b98f1ea10576ee8487f18cafda44044acb9f994ad8b1dc9d9db4d5519ea`

### (2) Operative text (verbatim)

> (a) Nothing in this chapter prohibits a party from seeking relief under Section 2556.
>
> (b) Nothing in this chapter changes existing law with respect to contract remedies where the contract has not been merged or incorporated into a judgment.
>
> (c) Nothing in this chapter is intended to restrict a family law court from acting as a court of equity.
>
> (d) Nothing in this chapter is intended to limit existing law with respect to the modification or enforcement of support orders.
>
> (e) Nothing in this chapter affects the rights of a bona fide lessee, purchaser, or encumbrancer for value of real property.

### (3) ELEMENTS

1. (a) “Nothing in this chapter prohibits a party from seeking relief under Section 2556.”
2. (b) “Nothing in this chapter changes existing law with respect to contract remedies where the contract has not been merged or incorporated into a judgment.”
3. (c) “Nothing in this chapter is intended to restrict a family law court from acting as a court of equity.”
4. (d) “Nothing in this chapter is intended to limit existing law with respect to the modification or enforcement of support orders.”
5. (e) “Nothing in this chapter affects the rights of a bona fide lessee, purchaser, or encumbrancer for value of real property.”

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL (savings clauses; no elements for a moving party). No punishment.


## 12. Family Code § 2129 — Application date of Chapter 10

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=FAM&sectionNum=2129> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_19628.lob` (166 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:09Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1993, Ch. 219, Sec. 108. Effective January 1, 1994."
- **Effective-date field:** 1994-01-01
- **Official location:** Family Code DIVISION 6. NULLITY, DISSOLUTION, AND LEGAL SEPARATION [2000. - 2452.] > PART 1. GENERAL PROVISIONS [2000. - 2129.] > CHAPTER 10. Relief From Judgment [2120. - 2129.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5f6a7f57-291f-11d9-a4bc-e54ef1b82d84`; SHA-256 of the XML record `9cf4b7932e4c39edd5a6b7cea2db50ad600ab1f6fc33afe9c4bd5dfdb76ad1ef`

### (2) Operative text (verbatim)

> This chapter applies to judgments entered on or after January 1, 1993.

### (3) ELEMENTS

1. Temporal scope: “This chapter applies to judgments entered on or after January 1, 1993.”

### (4) Nature of the provision / punishment

**Kind: CIVIL / PROCEDURAL**

CIVIL / PROCEDURAL (applicability). No punishment.

