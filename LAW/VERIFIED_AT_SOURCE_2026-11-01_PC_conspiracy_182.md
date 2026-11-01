# Penal Code § 182 — Conspiracy

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `PC_conspiracy_182` · sections: PEN 182

## How this file was produced (read first)

1. **Direct fetch of the leginfo HTML page failed.** On 2026-11-01 curl (through the session proxy) and WebFetch received HTTP 403 with a Cloudflare "Just a moment..." JavaScript challenge for `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118` (01:56:59Z) and the same challenge for two other leginfo paths (`/faces/codes.xhtml`, `/faces/codes_displayText.xhtml`; 01:57:38Z). This is the origin site's bot challenge, not an egress-proxy policy denial (the proxy log was clean). No attempt was made to defeat the challenge. The first Exa connector returned HTTP 402 (credit limit) at 01:57:36Z.
2. **Text source actually used.** The Legislature's own data publication behind the leginfo site: `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` (HTTP Last-Modified Mon, 26 Oct 2026 04:26:08 GMT; entries dated 2026-10-25). Read by HTTP byte-range requests: the ZIP central directory, `LAW_SECTION_TBL.dat` (section metadata incl. the official history note), `LAW_TOC_TBL.dat` (official headings) and one `LAW_SECTION_TBL_<n>.lob` XML record per section. Every entry passed its ZIP CRC-32 check; each section's SHA-256 is listed in its source record.
3. **Independent cross-check against the live page.** A second Exa connector fetched live leginfo pages. Penal Code § 118: text identical to the record (machine-compared). Code of Civil Procedure § 1010.6: identical on visual comparison of subdivisions (a)-(e)(4)(C). Code of Civil Procedure § 473: the live page presents a two-version selection list whose history notes match the record. Other sections were not individually cross-checked against the live page.
4. **Rendering.** The source is Legislative Counsel XML. Only whitespace is normalised (source line-wrap whitespace collapsed to single spaces; the XML en-space/em-space spacing elements shown as one space); no word, number, punctuation or subdivision label is altered. Italic markup is shown with asterisks; the source's underlined signature leader (CCP 415.30 form only) is shown as "[underlined signature line]". Curly quotes and apostrophes are as in the source.
5. **Currency as of 2026-11-01.** The publication was generated 2026-10-25. The Legislature's later incremental update files (pubinfo_Mon/Wed/Thu, last-modified 27, 29 and 30 Oct 2026) contain no law-section tables, i.e. no code-section changes between the snapshot and 30 Oct 2026 (no later incremental file had been published at retrieval). The law tables include 2026-session statutes (latest cited: Stats. 2026, ch. 1036). Every bill chaptered in 2025 (991 bills; 4,663 amendment action lines) and in 2026 (1,263 bills; 5,684 action lines) was scanned for amendments to the sections in the whole LAW/ set: the only hits were AB 747 (Stats. 2025, ch. 563 -> CCP § 473) and AB 540 (Stats. 2026, ch. 263 -> CCP § 1010.6); both are handled in `VERIFIED_AT_SOURCE_2026-11-01_CCP_service.md`.
6. **Limits.** No case law, annotations or secondary sources were consulted; "ELEMENTS" are drawn only from the quoted statutory words (every quoted phrase was machine-checked against the retrieved text). Statutes enacted in 2026 that take effect 1 Jan 2027 are not yet in the code tables except as noted. This is legal research support, not legal advice.


## 1. Penal Code § 182 — Conspiracy

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=182> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_60931.lob` (3,725 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:11Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2011, Ch. 15, Sec. 272. (AB 109) Effective April 4, 2011. Operative October 1, 2011, by Sec. 636 of Ch. 15, as amended by Stats. 2011, Ch. 39, Sec. 68."
- **Effective-date field:** 2011-04-04
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 7. OF CRIMES AGAINST PUBLIC JUSTICE [92. - 186.36.] > CHAPTER 8. Conspiracy [182. - 185.5.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_0144b52b-660e-11e0-8fc7-8d05c2a88098`; SHA-256 of the XML record `c4f1130c7d9d5f25e387e52f8b0ccff70b7c3477783fa1adec41e8f216077278`

### (2) Operative text (verbatim)

> (a) If two or more persons conspire:
>
> (1) To commit any crime.
>
> (2) Falsely and maliciously to indict another for any crime, or to procure another to be charged or arrested for any crime.
>
> (3) Falsely to move or maintain any suit, action, or proceeding.
>
> (4) To cheat and defraud any person of any property, by any means which are in themselves criminal, or to obtain money or property by false pretenses or by false promises with fraudulent intent not to perform those promises.
>
> (5) To commit any act injurious to the public health, to public morals, or to pervert or obstruct justice, or the due administration of the laws.
>
> (6) To commit any crime against the person of the President or Vice President of the United States, the Governor of any state or territory, any United States justice or judge, or the secretary of any of the executive departments of the United States.
>
> They are punishable as follows:
>
> When they conspire to commit any crime against the person of any official specified in paragraph (6), they are guilty of a felony and are punishable by imprisonment pursuant to subdivision (h) of Section 1170 for five, seven, or nine years.
>
> When they conspire to commit any other felony, they shall be punishable in the same manner and to the same extent as is provided for the punishment of that felony. If the felony is one for which different punishments are prescribed for different degrees, the jury or court which finds the defendant guilty thereof shall determine the degree of the felony the defendant conspired to commit. If the degree is not so determined, the punishment for conspiracy to commit the felony shall be that prescribed for the lesser degree, except in the case of conspiracy to commit murder, in which case the punishment shall be that prescribed for murder in the first degree.
>
> If the felony is conspiracy to commit two or more felonies which have different punishments and the commission of those felonies constitute but one offense of conspiracy, the penalty shall be that prescribed for the felony which has the greater maximum term.
>
> When they conspire to do an act described in paragraph (4), they shall be punishable by imprisonment in a county jail for not more than one year, or by imprisonment pursuant to subdivision (h) of Section 1170, or by a fine not exceeding ten thousand dollars ($10,000), or by both that imprisonment and fine.
>
> When they conspire to do any of the other acts described in this section, they shall be punishable by imprisonment in a county jail for not more than one year, or pursuant to subdivision (h) of Section 1170, or by a fine not exceeding ten thousand dollars ($10,000), or by both that imprisonment and fine. When they receive a felony conviction for conspiring to commit identity theft, as defined in Section 530.5, the court may impose a fine of up to twenty-five thousand dollars ($25,000).
>
> All cases of conspiracy may be prosecuted and tried in the superior court of any county in which any overt act tending to effect the conspiracy shall be done.
>
> (b) Upon a trial for conspiracy, in a case where an overt act is necessary to constitute the offense, the defendant cannot be convicted unless one or more overt acts are expressly alleged in the indictment or information, nor unless one of the acts alleged is proved; but other overt acts not alleged may be given in evidence.

### (3) ELEMENTS

1. Parties: “If two or more persons conspire”.
2. The agreement: “conspire” — the section does not define the word.
3. Object of the conspiracy — at least ONE of paragraphs (a)(1)–(a)(6):
   - (a)(1) “To commit any crime.”
   - (a)(2) “Falsely and maliciously to indict another for any crime, or to procure another to be charged or arrested for any crime.”
   - (a)(3) “Falsely to move or maintain any suit, action, or proceeding.”
   - (a)(4) “To cheat and defraud any person of any property, by any means which are in themselves criminal, or to obtain money or property by false pretenses or by false promises with fraudulent intent not to perform those promises.”
   - (a)(5) “To commit any act injurious to the public health, to public morals, or to pervert or obstruct justice, or the due administration of the laws.”
   - (a)(6) “To commit any crime against the person of the President or Vice President of the United States, the Governor of any state or territory, any United States justice or judge, or the secretary of any of the executive departments of the United States.”
4. Overt act (subd. (b)): “Upon a trial for conspiracy, in a case where an overt act is necessary to constitute the offense, the defendant cannot be convicted unless one or more overt acts are expressly alleged in the indictment or information, nor unless one of the acts alleged is proved; but other overt acts not alleged may be given in evidence.” The text does not itself identify which conspiracies are "a case where an overt act is necessary".
5. Venue: “All cases of conspiracy may be prosecuted and tried in the superior court of any county in which any overt act tending to effect the conspiracy shall be done.”

### (4) Nature of the provision / punishment

**Kind: CRIMINAL**

CRIMINAL. Punishment as stated in the text (graded by the object of the conspiracy):

- Conspiracy under (a)(6): “they are guilty of a felony and are punishable by imprisonment pursuant to subdivision (h) of Section 1170 for five, seven, or nine years”.
- Conspiracy to commit any other felony: “they shall be punishable in the same manner and to the same extent as is provided for the punishment of that felony” (with the degree rules in the same paragraph).
- Conspiracy under (a)(4): “they shall be punishable by imprisonment in a county jail for not more than one year, or by imprisonment pursuant to subdivision (h) of Section 1170, or by a fine not exceeding ten thousand dollars ($10,000), or by both that imprisonment and fine”.
- “When they conspire to do any of the other acts described in this section, they shall be punishable by imprisonment in a county jail for not more than one year, or pursuant to subdivision (h) of Section 1170, or by a fine not exceeding ten thousand dollars ($10,000), or by both that imprisonment and fine.”

Apart from (a)(6), the text does not label the offense "felony" or "misdemeanor"; it states the alternative punishments quoted above.

