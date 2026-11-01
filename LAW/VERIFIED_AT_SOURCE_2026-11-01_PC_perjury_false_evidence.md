# Penal Code — perjury and false evidence (§§ 118, 127, 132, 134, 135)

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `PC_perjury_false_evidence` · sections: PEN 118, 127, 132, 134, 135 (+ adjacent PEN 126)

## How this file was produced (read first)

1. **Direct fetch of the leginfo HTML page failed.** On 2026-11-01 curl (through the session proxy) and WebFetch received HTTP 403 with a Cloudflare "Just a moment..." JavaScript challenge for `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118` (01:56:59Z) and the same challenge for two other leginfo paths (`/faces/codes.xhtml`, `/faces/codes_displayText.xhtml`; 01:57:38Z). This is the origin site's bot challenge, not an egress-proxy policy denial (the proxy log was clean). No attempt was made to defeat the challenge. The first Exa connector returned HTTP 402 (credit limit) at 01:57:36Z.
2. **Text source actually used.** The Legislature's own data publication behind the leginfo site: `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` (HTTP Last-Modified Mon, 26 Oct 2026 04:26:08 GMT; entries dated 2026-10-25). Read by HTTP byte-range requests: the ZIP central directory, `LAW_SECTION_TBL.dat` (section metadata incl. the official history note), `LAW_TOC_TBL.dat` (official headings) and one `LAW_SECTION_TBL_<n>.lob` XML record per section. Every entry passed its ZIP CRC-32 check; each section's SHA-256 is listed in its source record.
3. **Independent cross-check against the live page.** A second Exa connector fetched live leginfo pages. Penal Code § 118: text identical to the record (machine-compared). Code of Civil Procedure § 1010.6: identical on visual comparison of subdivisions (a)-(e)(4)(C). Code of Civil Procedure § 473: the live page presents a two-version selection list whose history notes match the record. Other sections were not individually cross-checked against the live page.
4. **Rendering.** The source is Legislative Counsel XML. Only whitespace is normalised (source line-wrap whitespace collapsed to single spaces; the XML en-space/em-space spacing elements shown as one space); no word, number, punctuation or subdivision label is altered. Italic markup is shown with asterisks; the source's underlined signature leader (CCP 415.30 form only) is shown as "[underlined signature line]". Curly quotes and apostrophes are as in the source.
5. **Currency as of 2026-11-01.** The publication was generated 2026-10-25. The Legislature's later incremental update files (pubinfo_Mon/Wed/Thu, last-modified 27, 29 and 30 Oct 2026) contain no law-section tables, i.e. no code-section changes between the snapshot and 30 Oct 2026 (no later incremental file had been published at retrieval). The law tables include 2026-session statutes (latest cited: Stats. 2026, ch. 1036). Every bill chaptered in 2025 (991 bills; 4,663 amendment action lines) and in 2026 (1,263 bills; 5,684 action lines) was scanned for amendments to the sections in the whole LAW/ set: the only hits were AB 747 (Stats. 2025, ch. 563 -> CCP § 473) and AB 540 (Stats. 2026, ch. 263 -> CCP § 1010.6); both are handled in `VERIFIED_AT_SOURCE_2026-11-01_CCP_service.md`.
6. **Limits.** No case law, annotations or secondary sources were consulted; "ELEMENTS" are drawn only from the quoted statutory words (every quoted phrase was machine-checked against the retrieved text). Statutes enacted in 2026 that take effect 1 Jan 2027 are not yet in the code tables except as noted. This is legal research support, not legal advice.


## 1. Penal Code § 118 — Perjury

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118> — direct fetch returned HTTP 403 (Cloudflare challenge) at 2026-11-01T01:56:59Z; WebFetch likewise.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_69289.lob` (1,273 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:12Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 1990, Ch. 950, Sec. 2."
- **Effective-date field:** (none recorded in the source table)
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 7. OF CRIMES AGAINST PUBLIC JUSTICE [92. - 186.36.] > CHAPTER 5. Perjury and Subornation of Perjury [118. - 131.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_6530331d-2920-11d9-9844-b32bb8dfae52`; SHA-256 of the XML record `14cada31a67a532c5ec84e487188b81c3b2166dc7340b56c2f72718d795b78cb`
- **Live-page cross-check:** Exa fetch of the live leginfo URL for this section (2026-11-01, approx. 01:58Z; the tool returns no timestamp) returned text identical to the record for subdivisions (a) and (b) (machine-compared by the generating script).

### (2) Operative text (verbatim)

> (a) Every person who, having taken an oath that he or she will testify, declare, depose, or certify truly before any competent tribunal, officer, or person, in any of the cases in which the oath may by law of the State of California be administered, willfully and contrary to the oath, states as true any material matter which he or she knows to be false, and every person who testifies, declares, deposes, or certifies under penalty of perjury in any of the cases in which the testimony, declarations, depositions, or certification is permitted by law of the State of California under penalty of perjury and willfully states as true any material matter which he or she knows to be false, is guilty of perjury.
>
> This subdivision is applicable whether the statement, or the testimony, declaration, deposition, or certification is made or subscribed within or without the State of California.
>
> (b) No person shall be convicted of perjury where proof of falsity rests solely upon contradiction by testimony of a single person other than the defendant. Proof of falsity may be established by direct or indirect evidence.

### (3) ELEMENTS

1. Actor: “Every person who” (alternative A) / “every person who testifies, declares, deposes, or certifies” (alternative B).
2. Qualifying setting — ONE of two alternatives. (A) OATH: “having taken an oath that he or she will testify, declare, depose, or certify truly before any competent tribunal, officer, or person, in any of the cases in which the oath may by law of the State of California be administered”. (B) PENALTY OF PERJURY: “every person who testifies, declares, deposes, or certifies under penalty of perjury in any of the cases in which the testimony, declarations, depositions, or certification is permitted by law of the State of California under penalty of perjury”.
3. Act: the person “states as true” a matter.
4. Materiality: the matter is “any material matter”.
5. Falsity and knowledge: the matter is one “which he or she knows to be false” (the text expresses falsity and the speaker's knowledge of it in the same words).
6. Willfulness: “willfully” (alternative A adds “willfully and contrary to the oath”).
7. Place of the statement does not limit the offense: “This subdivision is applicable whether the statement, or the testimony, declaration, deposition, or certification is made or subscribed within or without the State of California.”
8. Proof limitation on conviction (subd. (b)): “No person shall be convicted of perjury where proof of falsity rests solely upon contradiction by testimony of a single person other than the defendant.” Manner of proof: “Proof of falsity may be established by direct or indirect evidence.”

### (4) Nature of the provision / punishment

**Kind: CRIMINAL**

CRIMINAL offense (Penal Code, Part 1, Title 7, Chapter 5, "Perjury and Subornation of Perjury"). Section 118 names the offense (“is guilty of perjury”) but states NO punishment. The punishment is in § 126 (retrieved below as an adjacent, unrequested section): “Perjury is punishable by imprisonment pursuant to subdivision (h) of Section 1170 for two, three or four years.”

Cross-reference elsewhere in this retrieval: Family Code § 2107(d)(2) uses the phrase “Perjury, as defined in Section 118 of the Penal Code”.


## 2. Penal Code § 127 — Subornation of perjury

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=127> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_69367.lob` (302 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:12Z
- **Official history note (HISTORY field, whitespace collapsed):** "Enacted 1872."
- **Effective-date field:** (none recorded in the source table)
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 7. OF CRIMES AGAINST PUBLIC JUSTICE [92. - 186.36.] > CHAPTER 5. Perjury and Subornation of Perjury [118. - 131.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_65334073-2920-11d9-9844-b32bb8dfae52`; SHA-256 of the XML record `005c147a110db614b22de374f12a66b7ccb9693c2a638236bfc4d4725f9713d2`

### (2) Operative text (verbatim)

> Every person who willfully procures another person to commit perjury is guilty of subornation of perjury, and is punishable in the same manner as he would be if personally guilty of the perjury so procured.

### (3) ELEMENTS

1. Actor: “Every person who”.
2. Act and state of mind: “willfully procures”.
3. Target: “another person” (a person other than the actor).
4. Procured conduct: “to commit perjury”. "Perjury" is the offense that § 118(a) describes with the words “is guilty of perjury”.
5. Result of the elements: “is guilty of subornation of perjury”.

### (4) Nature of the provision / punishment

**Kind: CRIMINAL**

CRIMINAL. Punishment is stated by reference: “is punishable in the same manner as he would be if personally guilty of the perjury so procured” — i.e. the § 126 punishment (“two, three or four years” under § 1170(h)).

What the text does not say: it speaks of procuring another “to commit perjury” and punishes “the perjury so procured”; it contains no sentence stating whether the procured perjury must actually be committed. That question is not addressed on the official page (no case law retrieved).


## 3. Penal Code § 132 — Offering forged or altered documentary evidence

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=132> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_61362.lob` (412 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:11Z
- **Official history note (HISTORY field, whitespace collapsed):** "Enacted 1872."
- **Effective-date field:** (none recorded in the source table)
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 7. OF CRIMES AGAINST PUBLIC JUSTICE [92. - 186.36.] > CHAPTER 6. Falsifying Evidence, and Bribing, Influencing, Intimidating or Threatening Witnesses [132. - 141.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_6534c71d-2920-11d9-9844-b32bb8dfae52`; SHA-256 of the XML record `b52a1fbf465f6ca17652841a89a08b17e656c8a5795c29e6b95c5c9e2ef65e02`

### (2) Operative text (verbatim)

> Every person who upon any trial, proceeding, inquiry, or investigation whatever, authorized or permitted by law, offers in evidence, as genuine or true, any book, paper, document, record, or other instrument in writing, knowing the same to have been forged or fraudulently altered or ante-dated, is guilty of felony.

### (3) ELEMENTS

1. Actor: “Every person who”.
2. Setting: “upon any trial, proceeding, inquiry, or investigation whatever, authorized or permitted by law”.
3. Act: “offers in evidence, as genuine or true”.
4. Object: “any book, paper, document, record, or other instrument in writing”.
5. The object is “forged or fraudulently altered or ante-dated”.
6. Knowledge: “knowing the same to have been forged or fraudulently altered or ante-dated”.

### (4) Nature of the provision / punishment

**Kind: CRIMINAL**

CRIMINAL. Class stated in the text: “is guilty of felony”. The section states no term of imprisonment or fine.


## 4. Penal Code § 134 — Preparing false documentary evidence

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=134> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_69411.lob` (426 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:12Z
- **Official history note (HISTORY field, whitespace collapsed):** "Enacted 1872."
- **Effective-date field:** (none recorded in the source table)
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 7. OF CRIMES AGAINST PUBLIC JUSTICE [92. - 186.36.] > CHAPTER 6. Falsifying Evidence, and Bribing, Influencing, Intimidating or Threatening Witnesses [132. - 141.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_6537d465-2920-11d9-9844-b32bb8dfae52`; SHA-256 of the XML record `69dd3b1b5b67c941b01aa5354203b462192267ead885edc55d05c00a8922434c`

### (2) Operative text (verbatim)

> Every person guilty of preparing any false or ante-dated book, paper, record, instrument in writing, or other matter or thing, with intent to produce it, or allow it to be produced for any fraudulent or deceitful purpose, as genuine or true, upon any trial, proceeding, or inquiry whatever, authorized by law, is guilty of felony.

### (3) ELEMENTS

1. Act: “preparing” (the text opens “Every person guilty of preparing”).
2. Object: “any false or ante-dated book, paper, record, instrument in writing, or other matter or thing”.
3. Intent: “with intent to produce it, or allow it to be produced for any fraudulent or deceitful purpose, as genuine or true”.
4. Intended setting of the production: “upon any trial, proceeding, or inquiry whatever, authorized by law”.

### (4) Nature of the provision / punishment

**Kind: CRIMINAL**

CRIMINAL. Class stated in the text: “is guilty of felony”. The section states no term of imprisonment or fine.

Textual observation: the mental element is an intent (“with intent to produce it, or allow it to be produced”); the text contains no words requiring that the item actually be produced.


## 5. Penal Code § 135 — Destroying or concealing evidence

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=135> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_69412.lob` (491 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:12Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2015, Ch. 463, Sec. 1. (AB 256) Effective January 1, 2016."
- **Effective-date field:** 2016-01-01
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 7. OF CRIMES AGAINST PUBLIC JUSTICE [92. - 186.36.] > CHAPTER 6. Falsifying Evidence, and Bribing, Influencing, Intimidating or Threatening Witnesses [132. - 141.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_c110c829-a358-11e5-b6cb-8d365f46d37f`; SHA-256 of the XML record `5fabe668f573372147a74c84479b0b2695d829ff18b1ee4a91b5153f9900177a`

### (2) Operative text (verbatim)

> A person who, knowing that any book, paper, record, instrument in writing, digital image, video recording owned by another, or other matter or thing, is about to be produced in evidence upon a trial, inquiry, or investigation, authorized by law, willfully destroys, erases, or conceals the same, with the intent to prevent it or its content from being produced, is guilty of a misdemeanor.

### (3) ELEMENTS

1. Actor: “A person who”.
2. Knowledge of imminent evidentiary use: “knowing that any book, paper, record, instrument in writing, digital image, video recording owned by another, or other matter or thing, is about to be produced in evidence upon a trial, inquiry, or investigation, authorized by law”.
3. Act: “willfully destroys, erases, or conceals the same”.
4. Intent: “with the intent to prevent it or its content from being produced”.

### (4) Nature of the provision / punishment

**Kind: CRIMINAL**

CRIMINAL. Class stated in the text: “is guilty of a misdemeanor”. The section states no term of imprisonment or fine.

Textual observation on scope: the words “owned by another” appear after “video recording” in a series of items; the text does not say whether they limit only "video recording" or the whole series. The question is not addressed on the official page.


---

# ADJACENT SECTION (retrieved for the punishment cross-reference; not on the requested list)


## 6. Penal Code § 126 — Punishment for perjury (ADJACENT section; not on the requested list)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=126> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_61361.lob` (207 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:11Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2011, Ch. 15, Sec. 249. (AB 109) Effective April 4, 2011. Operative October 1, 2011, by Sec. 636 of Ch. 15, as amended by Stats. 2011, Ch. 39, Sec. 68."
- **Effective-date field:** 2011-04-04
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 7. OF CRIMES AGAINST PUBLIC JUSTICE [92. - 186.36.] > CHAPTER 5. Perjury and Subornation of Perjury [118. - 131.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_d78f5e8d-660d-11e0-8fc7-8d05c2a88098`; SHA-256 of the XML record `b204882fa16b966cc93ecd6c90d8c09626ec78e9871578007978320ff5e036f6`

### (2) Operative text (verbatim)

> Perjury is punishable by imprisonment pursuant to subdivision (h) of Section 1170 for two, three or four years.

### (3) ELEMENTS

1. This section creates no separate elements; it supplies the punishment for the offense defined in § 118: “Perjury is punishable by imprisonment pursuant to subdivision (h) of Section 1170 for two, three or four years.”

### (4) Nature of the provision / punishment

**Kind: CRIMINAL (punishment provision)**

CRIMINAL — punishment provision. Included only because §§ 118 and 127 do not themselves state a term. Stated punishment: imprisonment pursuant to subdivision (h) of Section 1170 for two, three or four years (the text of § 1170(h) was not retrieved).

