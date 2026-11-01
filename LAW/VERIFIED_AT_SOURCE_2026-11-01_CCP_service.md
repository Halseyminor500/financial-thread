# Code of Civil Procedure — service and relief (§§ 415.30, 1010.6, 473)

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `CCP_service` · sections: CCP 415.30, 1010.6, 473 (+ adjacent CCP 1013b; + PENDING AB 540 version of 1010.6)

## How this file was produced (read first)

1. **Direct fetch of the leginfo HTML page failed.** On 2026-11-01 curl (through the session proxy) and WebFetch received HTTP 403 with a Cloudflare "Just a moment..." JavaScript challenge for `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118` (01:56:59Z) and the same challenge for two other leginfo paths (`/faces/codes.xhtml`, `/faces/codes_displayText.xhtml`; 01:57:38Z). This is the origin site's bot challenge, not an egress-proxy policy denial (the proxy log was clean). No attempt was made to defeat the challenge. The first Exa connector returned HTTP 402 (credit limit) at 01:57:36Z.
2. **Text source actually used.** The Legislature's own data publication behind the leginfo site: `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` (HTTP Last-Modified Mon, 26 Oct 2026 04:26:08 GMT; entries dated 2026-10-25). Read by HTTP byte-range requests: the ZIP central directory, `LAW_SECTION_TBL.dat` (section metadata incl. the official history note), `LAW_TOC_TBL.dat` (official headings) and one `LAW_SECTION_TBL_<n>.lob` XML record per section. Every entry passed its ZIP CRC-32 check; each section's SHA-256 is listed in its source record.
3. **Independent cross-check against the live page.** A second Exa connector fetched live leginfo pages. Penal Code § 118: text identical to the record (machine-compared). Code of Civil Procedure § 1010.6: identical on visual comparison of subdivisions (a)-(e)(4)(C). Code of Civil Procedure § 473: the live page presents a two-version selection list whose history notes match the record. Other sections were not individually cross-checked against the live page.
4. **Rendering.** The source is Legislative Counsel XML. Only whitespace is normalised (source line-wrap whitespace collapsed to single spaces; the XML en-space/em-space spacing elements shown as one space); no word, number, punctuation or subdivision label is altered. Italic markup is shown with asterisks; the source's underlined signature leader (CCP 415.30 form only) is shown as "[underlined signature line]". Curly quotes and apostrophes are as in the source.
5. **Currency as of 2026-11-01.** The publication was generated 2026-10-25. The Legislature's later incremental update files (pubinfo_Mon/Wed/Thu, last-modified 27, 29 and 30 Oct 2026) contain no law-section tables, i.e. no code-section changes between the snapshot and 30 Oct 2026 (no later incremental file had been published at retrieval). The law tables include 2026-session statutes (latest cited: Stats. 2026, ch. 1036). Every bill chaptered in 2025 (991 bills; 4,663 amendment action lines) and in 2026 (1,263 bills; 5,684 action lines) was scanned for amendments to the sections in the whole LAW/ set: the only hits were AB 747 (Stats. 2025, ch. 563 -> CCP § 473) and AB 540 (Stats. 2026, ch. 263 -> CCP § 1010.6); both are handled in `VERIFIED_AT_SOURCE_2026-11-01_CCP_service.md`.
6. **Limits.** No case law, annotations or secondary sources were consulted; "ELEMENTS" are drawn only from the quoted statutory words (every quoted phrase was machine-checked against the retrieved text). Statutes enacted in 2026 that take effect 1 Jan 2027 are not yet in the code tables except as noted. This is legal research support, not legal advice.


> **Three things to know before relying on this file**
>
> 1. **§ 473 has TWO active versions.** Version A (Stats. 2025, ch. 563, § 12; AB 747) is operative now and is repealed as of 1 Jan 2027; Version B (§ 13) becomes operative 1 Jan 2027 and adds a new subdivision (e). Subdivision (d) — the part you asked for — is word-for-word identical in both.
> 2. **§ 1010.6 contains no proof-of-service subdivision.** Proof of electronic service is in § 1013b (retrieved below as an adjacent section) and rule 2.251(j). Consent (unrepresented person) is § 1010.6(c); mandatory acceptance (represented person) is § 1010.6(b).
> 3. **§ 1010.6 is about to change.** Stats. 2026, ch. 263 (AB 540) amends it (no urgency clause; expected operative date 1 Jan 2027): it removes the two-court-day extension for electronic service in (a)(3) and conforms the last sentence of (d). The PENDING text is reproduced at the end of § 1010.6's section below. It is NOT current law on 2026-11-01.


## 1. Code of Civil Procedure § 415.30 — Service of summons by mail with acknowledgment of receipt

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=CCP&sectionNum=415.30> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_3407.lob` (4,217 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:06Z
- **Official history note (HISTORY field, whitespace collapsed):** "Added by Stats. 1969, Ch. 1610."
- **Effective-date field:** (none recorded in the source table)
- **Official location:** Code of Civil Procedure PART 2. OF CIVIL ACTIONS [307. - 1062.34.] > TITLE 5. JURISDICTION AND SERVICE OF PROCESS [410.10. - 418.11.] > CHAPTER 4. Service of Summons [413.10. - 417.40.] > ARTICLE 3. Manner of Service of Summons [415.10. - 415.95.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_e409d758-c72c-11db-94ae-b20113ea4192`; SHA-256 of the XML record `50979429714d4309f0b87802338f9e17b72873742b6e6f8f8ac13334f1ecd427`

### (2) Operative text (verbatim)

> (a) A summons may be served by mail as provided in this section. A copy of the summons and of the complaint shall be mailed (by first-class mail or airmail, postage prepaid) to the person to be served, together with two copies of the notice and acknowledgment provided for in subdivision (b) and a return envelope, postage prepaid, addressed to the sender.
>
> (b) The notice specified in subdivision (a) shall be in substantially the following form:
>
> (Title of court and cause, with action number, to be inserted by the sender prior to mailing)
>
> NOTICE
>
> To: (Here state the name of the person to be served.)
>
> This summons is served pursuant to Section 415.30 of the California Code of Civil Procedure. Failure to complete this form and return it to the sender within 20 days may subject you (or the party on whose behalf you are being served) to liability for the payment of any expenses incurred in serving a summons upon you in any other manner permitted by law. If you are served on behalf of a corporation, unincorporated association (including a partnership), or other entity, this form must be signed in the name of such entity by you or by a person authorized to receive service of process on behalf of such entity. In all other cases, this form must be signed by you personally or by a person authorized by you to acknowledge receipt of summons. Section 415.30 provides that this summons is deemed served on the date of execution of an acknowledgment of receipt of summons.
>
> Signature of sender
>
> ACKNOWLEDGMENT OF RECEIPT OF SUMMONS
>
> This acknowledges receipt on (insert date) of a copy of the summons and of the complaint at (insert address).
>
> Date: (Date this acknowledgement is executed)
>
> [underlined signature line]
>
> Signature of person acknowledging receipt, with title if  
> acknowledgment is made on behalf of another person
>
> (c) Service of a summons pursuant to this section is deemed complete on the date a written acknowledgement of receipt of summons is executed, if such acknowledgement thereafter is returned to the sender.
>
> (d) If the person to whom a copy of the summons and of the complaint are mailed pursuant to this section fails to complete and return the acknowledgement form set forth in subdivision (b) within 20 days from the date of such mailing, the party to whom the summons was mailed shall be liable for reasonable expenses thereafter incurred in serving or attempting to serve the party by another method permitted by this chapter, and, except for good cause shown, the court in which the action is pending, upon motion, with or without notice, shall award the party such expenses whether or not he is otherwise entitled to recover his costs in the action.
>
> (e) A notice or acknowledgment of receipt in form approved by the Judicial Council is deemed to comply with this section.

### (3) ELEMENTS

1. Method: “A summons may be served by mail as provided in this section.”
2. What is mailed: “A copy of the summons and of the complaint shall be mailed (by first-class mail or airmail, postage prepaid) to the person to be served”.
3. Enclosures: “together with two copies of the notice and acknowledgment provided for in subdivision (b) and a return envelope, postage prepaid, addressed to the sender”.
4. Form of the notice: “shall be in substantially the following form” (the form is in the verbatim text above).
5. Service is complete only on return of the signed acknowledgment: “Service of a summons pursuant to this section is deemed complete on the date a written acknowledgement of receipt of summons is executed, if such acknowledgement thereafter is returned to the sender.” Two conditions: the acknowledgment is “executed” AND “thereafter is returned to the sender”.
6. If the form is not returned: “fails to complete and return the acknowledgement form set forth in subdivision (b) within 20 days from the date of such mailing” — the person is “liable for reasonable expenses thereafter incurred in serving or attempting to serve the party by another method permitted by this chapter”, and “except for good cause shown, the court in which the action is pending, upon motion, with or without notice, shall award the party such expenses”.
7. Judicial Council forms: “A notice or acknowledgment of receipt in form approved by the Judicial Council is deemed to comply with this section.”

### (4) Nature of the provision / punishment

**Kind: PROCEDURAL (civil; service of summons)**

PROCEDURAL / CIVIL. Code of Civil Procedure, Part 2, Title 5, Chapter 4 ("Service of Summons"), Article 3. No punishment. The section governs service of a SUMMONS (and complaint) by mail; it is not the rule for service of later papers (see § 1010.6 and rule 2.251 for electronic service). History note on the page: "Added by Stats. 1969, Ch. 1610." — no amendment recorded.


## 2. Code of Civil Procedure § 473 — Amendments; relief from judgment (subdivision (d)) — TWO ACTIVE VERSIONS

### (1) Source record — Version A (operative on 2026-11-01)

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=CCP&sectionNum=473> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_3376.lob` (5,231 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:05Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2025, Ch. 563, Sec. 12. (AB 747) Effective January 1, 2026. Repealed as of January 1, 2027, by its own provisions. See later operative version added by Sec. 13 of Stats. 2025, Ch. 563."
- **Effective-date field:** 2026-01-01
- **Official location:** Code of Civil Procedure PART 2. OF CIVIL ACTIONS [307. - 1062.34.] > TITLE 6. OF THE PLEADINGS IN CIVIL ACTIONS [420. - 475.] > CHAPTER 8. Variance—Mistakes in Pleadings and Amendments [469. - 475.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_b65b2914-c40a-11f0-975c-e301db986e9c`; SHA-256 of the XML record `d1d340fccdfa2c7db267523206c80e7562a8fa5f5ea1335a17c1459efbcd2f3a`

### (2) Operative text (verbatim) — Version A (Stats. 2025, ch. 563, § 12; effective 1 Jan 2026; repealed as of 1 Jan 2027)

> (a) (1) The court may, in furtherance of justice, and on any terms as may be proper, allow a party to amend any pleading or proceeding by adding or striking out the name of any party, or by correcting a mistake in the name of a party, or a mistake in any other respect; and may, upon like terms, enlarge the time for answer or demurrer. The court may likewise, in its discretion, after notice to the adverse party, allow, upon any terms as may be just, an amendment to any pleading or proceeding in other particulars; and may upon like terms allow an answer to be made after the time limited by this code.
>
> (2) When it appears to the satisfaction of the court that the amendment renders it necessary, the court may postpone the trial, and may, when the postponement will by the amendment be rendered necessary, require, as a condition to the amendment, the payment to the adverse party of any costs as may be just.
>
> (b) The court may, upon any terms as may be just, relieve a party or the party’s legal representative from a judgment, dismissal, order, or other proceeding taken against the party through the party’s mistake, inadvertence, surprise, or excusable neglect. Application for this relief shall be accompanied by a copy of the answer or other pleading proposed to be filed therein, otherwise the application shall not be granted, and shall be made within a reasonable time, in no case exceeding six months, after the judgment, dismissal, order, or proceeding was taken. However, in the case of a judgment, dismissal, order, or other proceeding determining the ownership or right to possession of real or personal property, without extending the six-month period, when a notice in writing is personally served within the State of California both upon the party against whom the judgment, dismissal, order, or other proceeding has been taken, and upon the party’s attorney of record, if any, notifying that party and the party’s attorney of record, if any, that the order, judgment, dismissal, or other proceeding was taken against the party and that any rights the party has to apply for relief under the provisions of Section 473 of the Code of Civil Procedure shall expire 90 days after service of the notice, then the application shall be made within 90 days after service of the notice upon the defaulting party or the party’s attorney of record, if any, whichever service shall be later. No affidavit or declaration of merits shall be required of the moving party. Notwithstanding any other requirements of this section, the court shall, whenever an application for relief is made no more than six months after entry of judgment, is in proper form, and is accompanied by an attorney’s sworn affidavit attesting to the attorney’s mistake, inadvertence, surprise, or neglect, vacate any (1) resulting default entered by the clerk against the attorney’s client, and which will result in entry of a default judgment, or (2) resulting default judgment or dismissal entered against the attorney’s client, unless the court finds that the default or dismissal was not in fact caused by the attorney’s mistake, inadvertence, surprise, or neglect. The court shall, whenever relief is granted based on an attorney’s affidavit of fault, direct the attorney to pay reasonable compensatory legal fees and costs to opposing counsel or parties. However, this section shall not lengthen the time within which an action shall be brought to trial pursuant to Section 583.310.
>
> (c) (1) Whenever the court grants relief from a default, default judgment, or dismissal based on any of the provisions of this section, the court may do any of the following:
>
> (A) Impose a penalty of no greater than one thousand dollars ($1,000) upon an offending attorney or party.
>
> (B) Direct that an offending attorney pay an amount no greater than one thousand dollars ($1,000) to the State Bar Client Security Fund.
>
> (C) Grant other relief as is appropriate.
>
> (2) However, where the court grants relief from a default or default judgment pursuant to this section based upon the affidavit of the defaulting party’s attorney attesting to the attorney’s mistake, inadvertence, surprise, or neglect, the relief shall not be made conditional upon the attorney’s payment of compensatory legal fees or costs or monetary penalties imposed by the court or upon compliance with other sanctions ordered by the court.
>
> (d) The court may, upon motion of the injured party, or its own motion, correct clerical mistakes in its judgment or orders as entered, so as to conform to the judgment or order directed, and may, on motion of either party after notice to the other party, set aside any void judgment or order.
>
> (e) This section shall remain in effect only until January 1, 2027, and as of that date is repealed.

### (1b) Source record — Version B (operative 1 Jan 2027; NOT yet operative on 2026-11-01)

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=CCP&sectionNum=473> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_3377.lob` (5,434 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:06Z
- **Official history note (HISTORY field, whitespace collapsed):** "Repealed (in Sec. 12) and added by Stats. 2025, Ch. 563, Sec. 13. (AB 747) Effective January 1, 2026. Operative January 1, 2027, by its own provisions."
- **Effective-date field:** 2026-01-01
- **Official location:** Code of Civil Procedure PART 2. OF CIVIL ACTIONS [307. - 1062.34.] > TITLE 6. OF THE PLEADINGS IN CIVIL ACTIONS [420. - 475.] > CHAPTER 8. Variance—Mistakes in Pleadings and Amendments [469. - 475.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_88e3c262-c40a-11f0-975c-e301db986e9c`; SHA-256 of the XML record `530143cc2d8c824f6fb08e5fe018a7a180fc658139744d633f1fad00edb08b92`
- **Live-page cross-check (both versions):** Exa fetch of the live leginfo page for § 473 (2026-11-01, approx. 02:10Z-02:14Z; no timestamp returned) showed a selection list of exactly two entries, "(Amended by Stats. 2025, Ch. 563, Sec. 12.)" and "(Repealed (in Sec. 12) and added by Stats. 2025, Ch. 563, Sec. 13.)", matching the two records.

### (2b) Operative text (verbatim) — Version B (operative 1 Jan 2027)

> (a) (1) The court may, in furtherance of justice, and on any terms as may be proper, allow a party to amend any pleading or proceeding by adding or striking out the name of any party, or by correcting a mistake in the name of a party, or a mistake in any other respect; and may, upon like terms, enlarge the time for answer or demurrer. The court may likewise, in its discretion, after notice to the adverse party, allow, upon any terms as may be just, an amendment to any pleading or proceeding in other particulars; and may upon like terms allow an answer to be made after the time limited by this code.
>
> (2) When it appears to the satisfaction of the court that the amendment renders it necessary, the court may postpone the trial, and may, when the postponement will by the amendment be rendered necessary, require, as a condition to the amendment, the payment to the adverse party of any costs as may be just.
>
> (b) The court may, upon any terms as may be just, relieve a party or the party’s legal representative from a judgment, dismissal, order, or other proceeding taken against the party through the party’s mistake, inadvertence, surprise, or excusable neglect. Application for this relief shall be accompanied by a copy of the answer or other pleading proposed to be filed therein, otherwise the application shall not be granted, and shall be made within a reasonable time, in no case exceeding six months, after the judgment, dismissal, order, or proceeding was taken. However, in the case of a judgment, dismissal, order, or other proceeding determining the ownership or right to possession of real or personal property, without extending the six-month period, when a notice in writing is personally served within the State of California both upon the party against whom the judgment, dismissal, order, or other proceeding has been taken, and upon the party’s attorney of record, if any, notifying that party and the party’s attorney of record, if any, that the order, judgment, dismissal, or other proceeding was taken against the party and that any rights the party has to apply for relief under the provisions of Section 473 of the Code of Civil Procedure shall expire 90 days after service of the notice, then the application shall be made within 90 days after service of the notice upon the defaulting party or the party’s attorney of record, if any, whichever service shall be later. No affidavit or declaration of merits shall be required of the moving party. Notwithstanding any other requirements of this section, the court shall, whenever an application for relief is made no more than six months after entry of judgment, is in proper form, and is accompanied by an attorney’s sworn affidavit attesting to the attorney’s mistake, inadvertence, surprise, or neglect, vacate any (1) resulting default entered by the clerk against the attorney’s client, and which will result in entry of a default judgment, or (2) resulting default judgment or dismissal entered against the attorney’s client, unless the court finds that the default or dismissal was not in fact caused by the attorney’s mistake, inadvertence, surprise, or neglect. The court shall, whenever relief is granted based on an attorney’s affidavit of fault, direct the attorney to pay reasonable compensatory legal fees and costs to opposing counsel or parties. However, this section shall not lengthen the time within which an action shall be brought to trial pursuant to Section 583.310.
>
> (c) (1) Whenever the court grants relief from a default, default judgment, or dismissal based on any of the provisions of this section, the court may do any of the following:
>
> (A) Impose a penalty of no greater than one thousand dollars ($1,000) upon an offending attorney or party.
>
> (B) Direct that an offending attorney pay an amount no greater than one thousand dollars ($1,000) to the State Bar Client Security Fund.
>
> (C) Grant other relief as is appropriate.
>
> (2) However, where the court grants relief from a default or default judgment pursuant to this section based upon the affidavit of the defaulting party’s attorney attesting to the attorney’s mistake, inadvertence, surprise, or neglect, the relief shall not be made conditional upon the attorney’s payment of compensatory legal fees or costs or monetary penalties imposed by the court or upon compliance with other sanctions ordered by the court.
>
> (d) The court may, upon motion of the injured party, or its own motion, correct clerical mistakes in its judgment or orders as entered, so as to conform to the judgment or order directed, and may, on motion of either party after notice to the other party, set aside any void judgment or order.
>
> (e) Notwithstanding any other requirements of this section, a party to an action may bring a motion to vacate a default judgment that is void for lack of proper service at any time after entry of the judgment.
>
> (f) This section shall become operative on January 1, 2027.

### Subdivision (d) — verbatim (identical in Version A and Version B)

> (d) The court may, upon motion of the injured party, or its own motion, correct clerical mistakes in its judgment or orders as entered, so as to conform to the judgment or order directed, and may, on motion of either party after notice to the other party, set aside any void judgment or order.

### (3) ELEMENTS

1. Subdivision (d) is IDENTICAL in both active versions (current through 31 Dec 2026, and operative 1 Jan 2027).
2. Clerical-mistake correction: “The court may, upon motion of the injured party, or its own motion, correct clerical mistakes in its judgment or orders as entered, so as to conform to the judgment or order directed”. Elements: (i) initiated “upon motion of the injured party, or its own motion”; (ii) the thing corrected is “clerical mistakes in its judgment or orders as entered”; (iii) the correction is made “so as to conform to the judgment or order directed”; (iv) the power is discretionary (“may”).
3. Void judgment or order: “and may, on motion of either party after notice to the other party, set aside any void judgment or order”. Elements: (i) a motion by “either party”; (ii) “after notice to the other party”; (iii) the judgment or order is “void”; (iv) discretionary (“may”).
4. Textual observation: subdivision (d) states no deadline. The outer time limit in the section appears in subdivision (b), which concerns relief for “mistake, inadvertence, surprise, or excusable neglect” and requires an application made “within a reasonable time, in no case exceeding six months, after the judgment, dismissal, order, or proceeding was taken”.
5. VERSION B ONLY (operative 1 Jan 2027) — new subdivision (e): “Notwithstanding any other requirements of this section, a party to an action may bring a motion to vacate a default judgment that is void for lack of proper service at any time after entry of the judgment.” Version A instead ends with a repeal clause: “This section shall remain in effect only until January 1, 2027, and as of that date is repealed.”

### (4) Nature of the provision / punishment

**Kind: PROCEDURAL / CIVIL**

PROCEDURAL / CIVIL (court's power to correct or set aside). No punishment. Code of Civil Procedure, Part 2, Title 6, Chapter 8 ("Variance—Mistakes in Pleadings and Amendments").

Two active versions exist in the official data and on the official site's own selection page (the live page for § 473 lists "(Amended by Stats. 2025, Ch. 563, Sec. 12.)" and "(Repealed (in Sec. 12) and added by Stats. 2025, Ch. 563, Sec. 13.)"):

- Version A — Stats. 2025, ch. 563, § 12 (AB 747), effective 1 Jan 2026, repealed as of 1 Jan 2027 by its own provisions: THIS is the operative text on 2026-11-01.
- Version B — Stats. 2025, ch. 563, § 13 (AB 747), operative 1 Jan 2027: adds subd. (e) (quoted above) and subd. (f) “This section shall become operative on January 1, 2027.”

## 3. Code of Civil Procedure § 1010.6 — Electronic service and filing (full section, as currently in force)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=CCP&sectionNum=1010.6> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_4218.lob` (22,689 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:06Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2024, Ch. 151, Sec. 1. (AB 2283) Effective July 18, 2024."
- **Effective-date field:** 2024-07-18
- **Official location:** Code of Civil Procedure PART 2. OF CIVIL ACTIONS [307. - 1062.34.] > TITLE 14. OF MISCELLANEOUS PROVISIONS [989. - 1062.34.] > CHAPTER 5. Notices, and Filing and Service of Papers [1010. - 1020.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_ef16a6cb-45de-11ef-b598-a368f6618c34`; SHA-256 of the XML record `f25fe39e7861ccbf1e15bd10a12b57fdb0924e6ed9257ee1330330adfb7e50b2`
- **Live-page cross-check:** Exa fetch of the live leginfo URL for this section (2026-11-01, approx. 02:10Z-02:14Z; the tool returns no timestamp) returned text matching the record for subdivisions (a) through (e)(4)(C) on visual comparison (the tool output was cut off after about 9,000 characters; the remainder was not compared).

### (2) Operative text (verbatim)

> (a) A document may be served electronically in an action filed with the court as provided in this section, in accordance with rules adopted pursuant to subdivision (h).
>
> (1) For purposes of this section:
>
> (A) “Electronic service” means service of a document, on a person, by either electronic transmission or electronic notification. Electronic service may be performed directly by a person, including a party, by a person’s agent, including the person’s attorney, or through an electronic filing service provider, and by a court.
>
> (B) “Electronic transmission” means the transmission of a document by electronic means to the electronic service address at or through which a person receives electronic service.
>
> (C) “Electronic notification” means the notification of the person that a document is served by sending an electronic message to the electronic address at or through which the person receives electronic service, specifying the exact name of the document served, and providing a hyperlink at which the served document may be viewed and downloaded.
>
> (D) “Electronic filing” means the electronic transmission to a court of a document presented for filing in electronic form. For purposes of this section, this definition of electronic filing concerns the activity of filing and does not include the processing and review of the document and its entry into the court’s records, which are necessary for a document to be officially filed.
>
> (2) If a document is required to be served by certified or registered mail, electronic service of the document is not authorized.
>
> (3) (A) If a document may be served by mail, express mail, overnight delivery, or facsimile transmission, electronic service of that document is deemed complete at the time of the electronic transmission of the document or at the time that the electronic notification of service of the document is sent.
>
> (B) Any period of notice, or any right or duty to do any act or make any response within any period or on a date certain after the service of the document, which time period or date is prescribed by statute or rule of court, shall be extended after service by electronic means by two court days, but the extension shall not apply to extend the time for filing any of the following:
>
> (i) A notice of intention to move for new trial.
>
> (ii) A notice of intention to move to vacate judgment under Section 663a.
>
> (iii) A notice of appeal.
>
> (C) This extension applies in the absence of a specific exception provided by any other statute or rule of court.
>
> (4) Any document that is served electronically between 12:00 a.m. and 11:59:59 p.m. on a court day shall be deemed served on that court day. Any document that is served electronically on a noncourt day shall be deemed served on the next court day.
>
> (5) Confidential or sealed records shall be electronically served through encrypted methods to ensure that the documents are not improperly disclosed.
>
> (b) (1) This subdivision applies to mandatory electronic service. The court may order electronic service on a person represented by counsel who has appeared in an action or proceeding.
>
> (2) A person represented by counsel, who has appeared in an action or proceeding, shall accept electronic service of a notice or document that may be served by mail, express mail, overnight delivery, or facsimile transmission.
>
> (3) Before first serving a represented person electronically, the person effecting service shall confirm the appropriate electronic service address for the counsel being served.
>
> (4) A person represented by counsel shall, upon the request of any person who has appeared in an action or proceeding and who provides an electronic service address, electronically serve the requesting person with any notice or document that may be served by mail, express mail, overnight delivery, or facsimile transmission.
>
> (c) (1) This subdivision applies to electronic service by consent of an unrepresented person in a civil action.
>
> (2) An unrepresented party may consent to receive electronic service.
>
> (3) Express consent to electronic service may be given by either of the following:
>
> (i) Serving a notice on all parties and filing the notice with the court.
>
> (ii) Manifesting affirmative consent through electronic means with the court or the court’s electronic filing service provider, and concurrently providing the party’s electronic address with that consent for the purpose of receiving electronic service. The act of electronic filing shall not be construed as express consent.
>
> (4) A person who has provided express consent to accept service electronically may withdraw consent at any time by completing and filing with the court the appropriate Judicial Council form.
>
> (5) Consent, or the withdrawal of consent, to receive electronic service may only be completed by a person entitled to service.
>
> (d) On and after July 1, 2025, in any action in which a party or other person is subject to mandatory electronic service under subdivision (b) or has consented to electronic service under subdivision (c), the court shall electronically serve, to a person subject to mandatory electronic service or who consented to electronic service, any document issued by the court that the court is required to transmit, deliver, or serve. The electronic service of documents by the court shall have the same legal effect as service by mail, except as provided in paragraph (3) of subdivision (a).
>
> (e) A trial court may adopt local rules permitting electronic filing of documents, subject to rules adopted by the Judicial Council pursuant to subdivision (h) and the following conditions:
>
> (1) A document that is filed electronically shall have the same legal effect as an original paper document.
>
> (2) (A) When a document to be filed requires the signature of any person, not under penalty of perjury, the document shall be deemed to have been signed by that person if filed electronically and if either of the following conditions is satisfied:
>
> (i) The filer is the signer.
>
> (ii) The person has signed the document pursuant to the procedure set forth in the California Rules of Court.
>
> (B) When a document to be filed requires the signature, under penalty of perjury, of any person, the document shall be deemed to have been signed by that person if filed electronically and if either of the following conditions is satisfied:
>
> (i) The person has signed a printed form of the document before, or on the same day as, the date of filing. The attorney or other person filing the document represents, by the act of filing, that the declarant has complied with this section. The attorney or other person filing the document shall maintain the printed form of the document bearing the original signature until final disposition of the case, as defined in subdivision (c) of Section 68151 of the Government Code, and make it available for review and copying upon the request of the court or any party to the action or proceeding in which it is filed.
>
> (ii) The person has signed the document using a computer or other technology pursuant to the procedure set forth in a rule of court adopted by the Judicial Council by January 1, 2019.
>
> (3) Any document received electronically by the court between 12:00 a.m. and 11:59:59 p.m. on a court day shall be deemed filed on that court day. Any document that is received electronically on a noncourt day shall be deemed filed on the next court day.
>
> (4) (A) Whichever of a court, an electronic filing service provider, or an electronic filing manager is the first to receive a document submitted for electronic filing shall promptly send a confirmation of receipt of the document indicating the date and time of receipt to the party or person who submitted the document.
>
> (B) If a document received by the court under subparagraph (A) complies with filing requirements and all required filing fees have been paid, the court shall promptly send confirmation that the document has been filed to the party or person who submitted the document.
>
> (C) If the clerk of the court does not file a document received by the court under subparagraph (A) because the document does not comply with applicable filing requirements or the required filing fee has not been paid, the court shall promptly send notice of the rejection of the document for filing to the party or person who submitted the document. The notice of rejection shall state the reasons that the document was rejected for filing and include the date the clerk of the court sent the notice.
>
> (D) If the court utilizes an electronic filing service provider or electronic filing manager to send the notice of rejection described in subparagraph (C), the electronic filing service provider or electronic filing manager shall promptly send the notice of rejection to the party or person who submitted the document. A notice of rejection sent pursuant to this subparagraph shall include the date the electronic filing service provider or electronic filing manager sent the notice.
>
> (E) If the clerk of the court does not file a complaint or cross complaint because the complaint or cross complaint does not comply with applicable filing requirements or the required filing fee has not been paid, any statute of limitations applicable to the causes of action alleged in the complaint or cross complaint shall be tolled for the period beginning on the date on which the court received the document and as shown on the confirmation of receipt described in subparagraph (A), through the later of either the date on which the clerk of the court sent the notice of rejection described in subparagraph (C) or the date on which the electronic filing service provider or electronic filing manager sent the notice of rejection as described in subparagraph (D), plus one additional day if the complaint or cross complaint is subsequently submitted in a form that corrects the errors which caused the document to be rejected. The party filing the complaint or cross complaint shall not make any change to the complaint or cross complaint other than those required to correct the errors which caused the document to be rejected.
>
> (5) Upon electronic filing of a complaint, petition, or other document that must be served with a summons, a trial court, upon request of the party filing the action, shall issue a summons with the court seal and the case number. The court shall keep the summons in its records and shall electronically transmit a copy of the summons to the requesting party. Personal service of a printed form of the electronic summons shall have the same legal effect as personal service of an original summons.
>
> (6) The court shall permit a party or attorney to file an application for waiver of court fees and costs, in lieu of requiring the payment of the filing fee, as part of the process involving the electronic filing of a document. The court shall consider and determine the application in accordance with Article 6 (commencing with Section 68630) of Chapter 2 of Title 8 of the Government Code and shall not require the party or attorney to submit any documentation other than that set forth in Article 6 (commencing with Section 68630) of Chapter 2 of Title 8 of the Government Code. The court, an electronic filing service provider, or an electronic filing manager shall waive any fees charged to a party or the party’s attorney if the party has been granted a waiver of court fees pursuant to Section 68631 of the Government Code or if the party is indigent or being represented by the public defender or court-appointed counsel. The electronic filing manager or electronic filing service provider shall not seek payment from the court of any fee waived by the court. This section does not require the court to waive a filing fee that is not otherwise waivable.
>
> (7) If a party electronically files a filing that is exempt from the payment of filing fees under any other law, including a filing described in Section 212 of the Welfare and Institutions Code or Section 6103.9, subdivision (b) of Section 70617, or Section 70672 of the Government Code, the party shall not be required to pay any court fees associated with the electronic filing. An electronic filing service provider or an electronic filing manager shall not seek payment of these fees from the court.
>
> (8) A fee, if any, charged by the court, an electronic filing service provider, or an electronic filing manager to process a payment for filing fees and other court fees shall not exceed the costs incurred in processing the payment.
>
> (9) The court shall not charge fees for electronic filing and service of documents that are more than the court’s actual cost of electronic filing and service of the documents.
>
> (f) (1) Except as provided in paragraph (2), if a trial court adopts rules conforming to subdivision (e), it may provide by order, subject to the requirements and conditions stated in paragraphs (2) to (4), inclusive, of subdivision (g), and the rules adopted by the Judicial Council under subdivision (i), that all parties to an action file documents electronically in a class action, a consolidated action, a group of actions, a coordinated action, or an action that is deemed complex under Judicial Council rules, provided that the trial court’s order does not cause undue hardship or significant prejudice to any party in the action.
>
> (2) Unrepresented persons are exempt from any mandatory electronic filing imposed pursuant to this subdivision.
>
> (g) A trial court may, by local rule, require electronic filing in civil actions, subject to the requirements and conditions stated in subdivision (e), the rules adopted by the Judicial Council under subdivision (i), and the following conditions:
>
> (1) The court shall have the ability to maintain the official court record in electronic format for all cases where electronic filing is required.
>
> (2) The court and the parties shall have access to more than one electronic filing service provider capable of electronically filing documents with the court or to electronic filing access directly through the court. Any fees charged by an electronic filing service provider shall be reasonable. An electronic filing manager or an electronic filing service provider shall waive any fees charged if the court deems a waiver appropriate, including in instances where a party has received a fee waiver.
>
> (3) The court shall have a procedure for the filing of nonelectronic documents in order to prevent the program from causing undue hardship or significant prejudice to any party in an action, including, but not limited to, unrepresented parties. The Judicial Council shall make a form available to allow a party to seek an exemption from mandatory electronic filing and service on the grounds provided in this paragraph.
>
> (4) Unrepresented persons are exempt from mandatory electronic filing imposed pursuant to this subdivision.
>
> (5) Until January 1, 2021, a local child support agency, as defined in subdivision (h) of Section 17000 of the Family Code, is exempt from a trial court’s mandatory electronic filing and service requirements, unless the Department of Child Support Services and the local child support agency determine it has the capacity and functionality to comply with the trial court’s mandatory electronic filing and service requirements.
>
> (h) The Judicial Council shall adopt uniform rules for the electronic filing and service of documents in the trial courts of the state, which shall include statewide policies on vendor contracts, privacy, and access to public records, and rules relating to the integrity of electronic service. These rules shall conform to the conditions set forth in this section, as amended from time to time.
>
> (i) The Judicial Council shall adopt uniform rules to permit the mandatory electronic filing and service of documents for specified civil actions in the trial courts of the state, which shall include statewide policies on vendor contracts, privacy, access to public records, unrepresented parties, parties with fee waivers, hardships, reasonable exceptions to electronic filing, and rules relating to the integrity of electronic service. These rules shall conform to the conditions set forth in this section, as amended from time to time.
>
> (j) (1) Any system for the electronic filing and service of documents, including any information technology applications, internet websites and web-based applications, used by an electronic service provider or any other vendor or contractor that provides an electronic filing and service system to a trial court, regardless of the case management system used by the trial court, shall satisfy both of the following requirements:
>
> (A) The system shall be accessible to individuals with disabilities, including parties and attorneys with disabilities, in accordance with Section 508 of the federal Rehabilitation Act of 1973 (29 U.S.C. Sec. 794d), as amended, the regulations implementing that act set forth in Part 1194 of Title 36 of the Code of Federal Regulations and Appendices A, C, and D of that part, and the federal Americans with Disabilities Act of 1990 (42 U.S.C. Sec. 12101 et seq.).
>
> (B) The system shall comply with the Web Content Accessibility Guidelines 2.0 at a Level AA success criteria.
>
> (2) Commencing on June 27, 2017, the vendor or contractor shall provide an accommodation to an individual with a disability in accordance with subparagraph (D) of paragraph (3).
>
> (3) A trial court that contracts with an entity for the provision of a system for electronic filing and service of documents shall require the entity, in the trial court’s contract with the entity, to do all of the following:
>
> (A) Test and verify that the entity’s system complies with this subdivision and provide the verification to the Judicial Council no later than June 30, 2019.
>
> (B) Respond to, and resolve, any complaints regarding the accessibility of the system that are brought to the attention of the entity.
>
> (C) Designate a lead individual to whom any complaints concerning accessibility may be addressed and post the individual’s name and contact information on the entity’s internet website.
>
> (D) Provide to an individual with a disability, upon request, an accommodation to enable the individual to file and serve documents electronically at no additional charge for any time period that the entity is not compliant with paragraph (1). Exempting an individual with a disability from mandatory electronic filing and service of documents shall not be deemed an accommodation unless the person chooses that as an accommodation. The vendor or contractor shall clearly state on its internet website that an individual with a disability may request an accommodation and the process for submitting a request for an accommodation.
>
> (4) A trial court that provides electronic filing and service of documents directly to the public shall comply with this subdivision to the same extent as a vendor or contractor that provides electronic filing and services to a trial court.
>
> (5) (A) The Judicial Council shall submit four reports to the appropriate committees of the Legislature relating to the trial courts that have implemented a system of electronic filing and service of documents. The first report is due by June 30, 2018; the second report is due by December 31, 2019; the third report is due by December 31, 2021; and the fourth report is due by December 31, 2023.
>
> (B) The Judicial Council’s reports shall include all of the following information:
>
> (i) The name of each court that has implemented a system of electronic filing and service of documents.
>
> (ii) A description of the system of electronic filing and service.
>
> (iii) The name of the entity or entities providing the system.
>
> (iv) A statement as to whether the system complies with this subdivision and, if the system is not fully compliant, a description of the actions that have been taken to make the system compliant.
>
> (6) An entity that contracts with a trial court to provide a system for electronic filing and service of documents shall cooperate with the Judicial Council by providing all information, and by permitting all testing, necessary for the Judicial Council to prepare its reports to the Legislature in a complete and timely manner.

### (3) ELEMENTS

1. SCOPE (subd. (a)): “A document may be served electronically in an action filed with the court as provided in this section, in accordance with rules adopted pursuant to subdivision (h).” Excluded: “If a document is required to be served by certified or registered mail, electronic service of the document is not authorized.”
2. WHAT COUNTS AS ELECTRONIC SERVICE (subd. (a)(1)(A)–(C)): ““Electronic service” means service of a document, on a person, by either electronic transmission or electronic notification.” Notification requires “specifying the exact name of the document served, and providing a hyperlink at which the served document may be viewed and downloaded”.
3. A. REPRESENTED PERSON — MANDATORY SERVICE (subd. (b)): “This subdivision applies to mandatory electronic service.” Elements: (i) the person served is “represented by counsel”; (ii) counsel “has appeared in an action or proceeding”; (iii) the document is “a notice or document that may be served by mail, express mail, overnight delivery, or facsimile transmission”; (iv) the represented person “shall accept electronic service”; (v) the server has complied with “Before first serving a represented person electronically, the person effecting service shall confirm the appropriate electronic service address for the counsel being served.” No consent step appears in subdivision (b).
4. B. UNREPRESENTED PERSON — CONSENT (subd. (c)): “This subdivision applies to electronic service by consent of an unrepresented person in a civil action.” Elements: (i) “An unrepresented party may consent to receive electronic service.” (ii) Express consent is given by ONE of: “Serving a notice on all parties and filing the notice with the court.” OR “Manifesting affirmative consent through electronic means with the court or the court’s electronic filing service provider, and concurrently providing the party’s electronic address with that consent for the purpose of receiving electronic service.” (iii) “The act of electronic filing shall not be construed as express consent.” (iv) Withdrawal: “may withdraw consent at any time by completing and filing with the court the appropriate Judicial Council form”. (v) Who may consent or withdraw: “Consent, or the withdrawal of consent, to receive electronic service may only be completed by a person entitled to service.”
5. TEXTUAL OBSERVATION on represented vs. unrepresented: the compulsory acceptance duty in subd. (b) is imposed on “A person represented by counsel”; for an “unrepresented person” the statute supplies the consent mechanism in subd. (c). The section contains no sentence stating the converse (that service on an unrepresented person without consent is ineffective). Compare the wording of rule 2.251(c)(3)(B): “those parties or other persons are to be served by non-electronic methods unless they affirmatively consent to electronic service”.
6. WHEN SERVICE IS COMPLETE (subd. (a)(3)–(4), current text): “electronic service of that document is deemed complete at the time of the electronic transmission of the document or at the time that the electronic notification of service of the document is sent”; extension: “shall be extended after service by electronic means by two court days” (not for the three filings listed in (a)(3)(B)(i)–(iii)); court-day rule: “Any document that is served electronically between 12:00 a.m. and 11:59:59 p.m. on a court day shall be deemed served on that court day.” (See the PENDING AB 540 version below: the two-court-day extension is removed from 1 Jan 2027.)
7. PROOF OF ELECTRONIC SERVICE: this section contains NO proof-of-service subdivision (the word "proof" does not appear in § 1010.6). Proof of electronic service is governed by Code of Civil Procedure § 1013b (retrieved below as an adjacent section) — “Proof of electronic service may be made by any of the following methods:” — and by rule 2.251(j)(1) (“Proof of electronic service shall be made as provided in Code of Civil Procedure section 1013b.”). The only signature rule in § 1010.6 that § 1013b incorporates is subd. (e)(2)(B): “When a document to be filed requires the signature, under penalty of perjury, of any person, the document shall be deemed to have been signed by that person if filed electronically and if either of the following conditions is satisfied:”
8. COURT'S OWN ELECTRONIC SERVICE (subd. (d)): “On and after July 1, 2025, in any action in which a party or other person is subject to mandatory electronic service under subdivision (b) or has consented to electronic service under subdivision (c), the court shall electronically serve”.

### (4) Nature of the provision / punishment

**Kind: PROCEDURAL (civil)**

PROCEDURAL / CIVIL (Code of Civil Procedure, Part 2, Title 14, Chapter 5, "Notices, and Filing and Service of Papers"). No punishment.

Relevance map of the subdivisions you asked about: consent of an unrepresented person = subd. (c); mandatory acceptance by a represented person = subd. (b); proof of electronic service = NOT in this section (see § 1013b and rule 2.251(j)).

PENDING CHANGE (not yet operative on 2026-11-01): Stats. 2026, ch. 263 (AB 540) amends § 1010.6 — see the separate PENDING subsection below. Only subd. (a)(3) and the last sentence of subd. (d) change; the consent subdivisions (b) and (c) are unchanged.


### PENDING (not yet operative) — § 1010.6 as amended by Stats. 2026, ch. 263 (AB 540), SEC. 4

- **Source:** bill-version record `20250AB54096CHP` (chaptered), ZIP entry `BILL_VERSION_TBL_18543.lob` inside <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip>; bill record `202520260AB540`: Chaptered, Statutes of 2026, chapter 263; bill-version action date 2026-09-18 (history in the XML: ENROLLED 2026-09-03, CHAPTERED / APPROVED / FILED 2026-09-18); `<Urgency>NO</Urgency>`; five bill sections, none an operative-date section. Title of the act: "to amend Section 6155 of the Business and Professions Code, to amend Sections 437c, 1005, and 1010.6 of, and to add Section 2016.100 to, the Code of Civil Procedure, relating to civil actions." Retrieved (UTC): 2026-11-01T02:07:09Z.
- **Method:** the amended § 1010.6 text in the chaptered bill was converted with the same rules as the code record and compared paragraph-by-paragraph with the current text above; exactly two places differ, shown below. Every other paragraph of the current text — including all of subdivisions (b) and (c) on consent — is word-for-word unchanged.
- **Expected operative date:** see the nature note below (no urgency clause; general rule stated from general knowledge, to be confirmed on the leginfo bill-status page).

**Current paragraphs that the amendment removes or replaces (verbatim, from the current text above):**

> (3) (A) If a document may be served by mail, express mail, overnight delivery, or facsimile transmission, electronic service of that document is deemed complete at the time of the electronic transmission of the document or at the time that the electronic notification of service of the document is sent.
>
> (B) Any period of notice, or any right or duty to do any act or make any response within any period or on a date certain after the service of the document, which time period or date is prescribed by statute or rule of court, shall be extended after service by electronic means by two court days, but the extension shall not apply to extend the time for filing any of the following:
>
> (i) A notice of intention to move for new trial.
>
> (ii) A notice of intention to move to vacate judgment under Section 663a.
>
> (iii) A notice of appeal.
>
> (C) This extension applies in the absence of a specific exception provided by any other statute or rule of court.
>
> (d) On and after July 1, 2025, in any action in which a party or other person is subject to mandatory electronic service under subdivision (b) or has consented to electronic service under subdivision (c), the court shall electronically serve, to a person subject to mandatory electronic service or who consented to electronic service, any document issued by the court that the court is required to transmit, deliver, or serve. The electronic service of documents by the court shall have the same legal effect as service by mail, except as provided in paragraph (3) of subdivision (a).

**Replacement text in AB 540 (verbatim):**

> (3) If a document may be served by mail, express mail, overnight delivery, or facsimile transmission, electronic service of that document is deemed complete at the time of the electronic transmission of the document or at the time that the electronic notification of service of the document is sent.
>
> (d) On and after July 1, 2025, in any action in which a party or other person is subject to mandatory electronic service under subdivision (b) or has consented to electronic service under subdivision (c), the court shall electronically serve, to a person subject to mandatory electronic service or who consented to electronic service, any document issued by the court that the court is required to transmit, deliver, or serve. The electronic service of documents by the court shall have the same legal effect as service by mail.

**Effect, by the words:** the current two-court-day extension after "service by electronic means" in (a)(3)(B), its three exceptions (a)(3)(B)(i)-(iii) and (a)(3)(C) do not appear in the amended text; the sentence in (d) no longer carries the clause "except as provided in paragraph (3) of subdivision (a)". The Legislative Counsel's digest in the chaptered bill describes the change as one that "would clarify that service of a notice of motion described above by electronic service is not among the methods of service requiring an increase to the period of notice" and "would also make conforming changes".

#### Elements / nature of the pending text

1. Subd. (a)(3) as amended reads in full: “If a document may be served by mail, express mail, overnight delivery, or facsimile transmission, electronic service of that document is deemed complete at the time of the electronic transmission of the document or at the time that the electronic notification of service of the document is sent.” — the current subparagraphs (a)(3)(B) (two-court-day extension and its three exceptions) and (a)(3)(C) are not present in the amended text.
2. Subd. (d), last sentence as amended: “The electronic service of documents by the court shall have the same legal effect as service by mail.” — the current clause “except as provided in paragraph (3) of subdivision (a)” is dropped.

**Kind: PROCEDURAL (civil) — NOT CURRENT LAW on 2026-11-01**

Not current law. The chaptered bill carries <Urgency>NO</Urgency> (bill-version record: URGENCY "No") and contains five bill sections with no separate operative-date section. A statute enacted at a regular session without an urgency clause ordinarily takes effect on January 1 of the following year (Cal. Const., art. IV, § 8(c)) — that general rule is stated from general knowledge, NOT from a retrieved page; the expected operative date is therefore January 1, 2027 and should be confirmed on the leginfo bill-status page for AB 540 (2025–26), Statutes of 2026, chapter 263.

---

# ADJACENT SECTION (retrieved because § 1010.6 has no proof-of-service provision and rule 2.251(j)(1) points here; not on the requested list)


## 4. Code of Civil Procedure § 1013b — Proof of electronic service (ADJACENT section; not on the requested list)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=CCP&sectionNum=1013b> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_4223.lob` (2,678 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:05:32Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2022, Ch. 215, Sec. 2. (AB 2961) Effective January 1, 2023."
- **Effective-date field:** 2023-01-01
- **Official location:** Code of Civil Procedure PART 2. OF CIVIL ACTIONS [307. - 1062.34.] > TITLE 14. OF MISCELLANEOUS PROVISIONS [989. - 1062.34.] > CHAPTER 5. Notices, and Filing and Service of Papers [1010. - 1020.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_42c76ad9-6a95-11ed-823c-e74f056edb17`; SHA-256 of the XML record `e42f281677f85f6cd38e4595c616961ad34bf8466619be9aed418dc85e7913e7`

### (2) Operative text (verbatim)

> (a) Proof of electronic service may be made by any of the following methods:
>
> (1) An affidavit setting forth the exact title of the document served and filed in the cause, showing the name and residence or business address of the person making the service, showing that the person is a resident of or employed in the county where the electronic service occurs, and that the person is over 18 years of age.
>
> (2) A certificate setting forth the exact title of the document served and filed in the cause, showing the name and business address of the person making the service, and showing that the person is an active member of the State Bar of California.
>
> (3) An affidavit setting forth the exact title of the document served and filed in the cause, showing all of the following:
>
> (A) The name and residence or business address of the person making the service.
>
> (B) That the person is a resident of, or employed in, the county where the electronic service occurs.
>
> (C) That the person is over 18 years of age.
>
> (D) That the person is readily familiar with the business’ practice for filing electronically.
>
> (E) That the document would be electronically served that same day in the ordinary course of business following ordinary business practices.
>
> (4) In case of service by the clerk of a court of record, a certificate by that clerk setting forth the exact title of the document served and filed in the cause, showing the name of the clerk and the name of the court of which they are the clerk.
>
> (b) Proof of electronic service shall include all of the following:
>
> (1) The electronic service address and the residence or business address of the person making the electronic service.
>
> (2) The date of electronic service.
>
> (3) The name and electronic service address of the person served.
>
> (4) A statement that the document was served electronically.
>
> (c) Proof of electronic service shall be signed as provided in subparagraph (B) of paragraph (2) of subdivision (e) of Section 1010.6.
>
> (d) Proof of electronic service may be in electronic form and may be filed electronically with the court.

### (3) ELEMENTS

1. Method — ONE of (a)(1)–(a)(4): (1) “An affidavit setting forth the exact title of the document served and filed in the cause, showing the name and residence or business address of the person making the service, showing that the person is a resident of or employed in the county where the electronic service occurs, and that the person is over 18 years of age.” (2) a certificate showing the person “is an active member of the State Bar of California”; (3) an affidavit with the five showings (A)–(E) quoted above; (4) “In case of service by the clerk of a court of record, a certificate by that clerk”.
2. Contents — ALL of (subd. (b)): “The electronic service address and the residence or business address of the person making the electronic service.” “The date of electronic service.” “The name and electronic service address of the person served.” “A statement that the document was served electronically.”
3. Signature (subd. (c)): “Proof of electronic service shall be signed as provided in subparagraph (B) of paragraph (2) of subdivision (e) of Section 1010.6.”
4. Form (subd. (d)): “Proof of electronic service may be in electronic form and may be filed electronically with the court.”

### (4) Nature of the provision / punishment

**Kind: PROCEDURAL (civil)**

PROCEDURAL / CIVIL. Included because § 1010.6 contains no proof-of-service provision and rule 2.251(j)(1) points here. Note that § 1013b(c) incorporates § 1010.6(e)(2)(B), which addresses signatures “under penalty of perjury” (see the Penal Code § 118 file for the perjury definition; no inference about any particular proof of service is drawn here).

