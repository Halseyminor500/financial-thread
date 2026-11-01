# Penal Code — extortion guardrails (§§ 518, 519, 523, 524)

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `PC_guardrails_extortion` · sections: PEN 518, 519, 523, 524

## How this file was produced (read first)

1. **Direct fetch of the leginfo HTML page failed.** On 2026-11-01 curl (through the session proxy) and WebFetch received HTTP 403 with a Cloudflare "Just a moment..." JavaScript challenge for `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118` (01:56:59Z) and the same challenge for two other leginfo paths (`/faces/codes.xhtml`, `/faces/codes_displayText.xhtml`; 01:57:38Z). This is the origin site's bot challenge, not an egress-proxy policy denial (the proxy log was clean). No attempt was made to defeat the challenge. The first Exa connector returned HTTP 402 (credit limit) at 01:57:36Z.
2. **Text source actually used.** The Legislature's own data publication behind the leginfo site: `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` (HTTP Last-Modified Mon, 26 Oct 2026 04:26:08 GMT; entries dated 2026-10-25). Read by HTTP byte-range requests: the ZIP central directory, `LAW_SECTION_TBL.dat` (section metadata incl. the official history note), `LAW_TOC_TBL.dat` (official headings) and one `LAW_SECTION_TBL_<n>.lob` XML record per section. Every entry passed its ZIP CRC-32 check; each section's SHA-256 is listed in its source record.
3. **Independent cross-check against the live page.** A second Exa connector fetched live leginfo pages. Penal Code § 118: text identical to the record (machine-compared). Code of Civil Procedure § 1010.6: identical on visual comparison of subdivisions (a)-(e)(4)(C). Code of Civil Procedure § 473: the live page presents a two-version selection list whose history notes match the record. Other sections were not individually cross-checked against the live page.
4. **Rendering.** The source is Legislative Counsel XML. Only whitespace is normalised (source line-wrap whitespace collapsed to single spaces; the XML en-space/em-space spacing elements shown as one space); no word, number, punctuation or subdivision label is altered. Italic markup is shown with asterisks; the source's underlined signature leader (CCP 415.30 form only) is shown as "[underlined signature line]". Curly quotes and apostrophes are as in the source.
5. **Currency as of 2026-11-01.** The publication was generated 2026-10-25. The Legislature's later incremental update files (pubinfo_Mon/Wed/Thu, last-modified 27, 29 and 30 Oct 2026) contain no law-section tables, i.e. no code-section changes between the snapshot and 30 Oct 2026 (no later incremental file had been published at retrieval). The law tables include 2026-session statutes (latest cited: Stats. 2026, ch. 1036). Every bill chaptered in 2025 (991 bills; 4,663 amendment action lines) and in 2026 (1,263 bills; 5,684 action lines) was scanned for amendments to the sections in the whole LAW/ set: the only hits were AB 747 (Stats. 2025, ch. 563 -> CCP § 473) and AB 540 (Stats. 2026, ch. 263 -> CCP § 1010.6); both are handled in `VERIFIED_AT_SOURCE_2026-11-01_CCP_service.md`.
6. **Limits.** No case law, annotations or secondary sources were consulted; "ELEMENTS" are drawn only from the quoted statutory words (every quoted phrase was machine-checked against the retrieved text). Statutes enacted in 2026 that take effect 1 Jan 2027 are not yet in the code tables except as noted. This is legal research support, not legal advice.


> **Purpose of this file:** these sections are collected as GUARDRAILS — a statement of what conduct the text would reach, so that a person who is a victim and is reporting or seeking redress can see where demands or threats could be characterised as extortion. Each section carries a plain note, quoting the words, of what conduct by a reporting victim the text would reach. The notes describe the statutory words only; no case law was retrieved.


## 1. Penal Code § 518 — Extortion defined (GUARDRAIL)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=518> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_75773.lob` (888 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:13Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2017, Ch. 518, Sec. 1. (SB 500) Effective January 1, 2018."
- **Effective-date field:** 2018-01-01
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 13. OF CRIMES AGAINST PROPERTY [450. - 593g.] > CHAPTER 7. Extortion [518. - 527.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_4a4a6b2b-df53-11e7-967b-c7bde29c26e0`; SHA-256 of the XML record `4dcab3baefd7d2d83f14f0f5a4125d9a807b990293d9187be49d55deed505d2f`

### (2) Operative text (verbatim)

> (a) Extortion is the obtaining of property or other consideration from another, with his or her consent, or the obtaining of an official act of a public officer, induced by a wrongful use of force or fear, or under color of official right.
>
> (b) For purposes of this chapter, “consideration” means anything of value, including sexual conduct as defined in subdivision (b) of Section 311.3, or an image of an intimate body part as defined in subparagraph (C) of paragraph (4) of subdivision (j) of Section 647.
>
> (c) Notwithstanding subdivision (a), this section does not apply to a person under 18 years of age who has obtained consideration consisting of sexual conduct or an image of an intimate body part.

### (3) ELEMENTS

1. Obtaining — ONE of: “the obtaining of property or other consideration from another, with his or her consent”, OR “the obtaining of an official act of a public officer”.
2. Inducement: “induced by a wrongful use of force or fear, or under color of official right”. (The kinds of threat by which fear may be induced are listed in § 519.)
3. "Consideration" (subd. (b)): “means anything of value, including sexual conduct as defined in subdivision (b) of Section 311.3, or an image of an intimate body part as defined in subparagraph (C) of paragraph (4) of subdivision (j) of Section 647”.
4. Exception (subd. (c)): “this section does not apply to a person under 18 years of age who has obtained consideration consisting of sexual conduct or an image of an intimate body part” — the exception is limited to those two kinds of consideration.

### (4) Nature of the provision / punishment

**Kind: CRIMINAL (definition; no punishment stated in this section)**

CRIMINAL (definitional). Section 518 defines extortion; it states no punishment (the extortion punishment section, § 520, was not retrieved). Related punishments retrieved here: § 523 (writings) and § 524 (attempts).

### GUARDRAIL note — what conduct by a reporting victim the text would reach

What a reporting victim's conduct could fall within on the face of this text: obtaining anything of value — “property or other consideration”, where "consideration" “means anything of value” — from another person who consents because of fear induced by a threat of the kinds listed in § 519 (e.g. a threat "To accuse the individual threatened ... of a crime"). The word that qualifies the inducement is “wrongful” (“induced by a wrongful use of force or fear”); the section does not define "wrongful". The only exception stated (subd. (c)) concerns a person under 18 who “has obtained consideration consisting of sexual conduct or an image of an intimate body part”; it says nothing about a person who is a crime victim, and it does not reach other kinds of consideration.


## 2. Penal Code § 519 — Kinds of threat that constitute extortionate "fear" (GUARDRAIL)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=519> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_75727.lob` (770 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:13Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2014, Ch. 71, Sec. 123. (SB 1304) Effective January 1, 2015."
- **Effective-date field:** 2015-01-01
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 13. OF CRIMES AGAINST PROPERTY [450. - 593g.] > CHAPTER 7. Extortion [518. - 527.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_588f5f79-8664-11e4-9fd7-cecd375806d8`; SHA-256 of the XML record `02e6b3bfaeb0abcd3dec7b1eb7bc28823263e59d7768b14e718d1458461ade38`

### (2) Operative text (verbatim)

> Fear, such as will constitute extortion, may be induced by a threat of any of the following:
>
> 1. To do an unlawful injury to the person or property of the individual threatened or of a third person.
>
> 2. To accuse the individual threatened, or a relative of his or her, or a member of his or her family, of a crime.
>
> 3. To expose, or to impute to him, her, or them a deformity, disgrace, or crime.
>
> 4. To expose a secret affecting him, her, or them.
>
> 5. To report his, her, or their immigration status or suspected immigration status.

### (3) ELEMENTS

1. Lead-in: “Fear, such as will constitute extortion, may be induced by a threat of any of the following:”
2. Threat type 1: “To do an unlawful injury to the person or property of the individual threatened or of a third person.”
3. Threat type 2: “To accuse the individual threatened, or a relative of his or her, or a member of his or her family, of a crime.”
4. Threat type 3: “To expose, or to impute to him, her, or them a deformity, disgrace, or crime.”
5. Threat type 4: “To expose a secret affecting him, her, or them.”
6. Threat type 5: “To report his, her, or their immigration status or suspected immigration status.”
7. Section 519 supplies the "fear" element only; the remaining elements of extortion are in § 518(a) (obtaining “property or other consideration” “induced by a wrongful use of force or fear”). For the writing and attempt offenses see §§ 523(a) and 524.

### (4) Nature of the provision / punishment

**Kind: CRIMINAL (definition; no punishment stated in this section)**

CRIMINAL (definitional). Section 519 creates no offense and states no punishment by itself; §§ 523 and 524 incorporate it by reference (“any threat such as is specified in Section 519”).

### GUARDRAIL note — what conduct by a reporting victim the text would reach

Conduct by a reporting victim that the text would reach on its face:

- Threatening to report someone to law enforcement or to accuse them of a crime in order to obtain something: § 519(2) “To accuse the individual threatened, or a relative of his or her, or a member of his or her family, of a crime.”
- Threatening to expose a crime, disgrace or deformity, or to impute one: § 519(3) “To expose, or to impute to him, her, or them a deformity, disgrace, or crime.”
- Threatening to reveal a secret: § 519(4) “To expose a secret affecting him, her, or them.”
- Threatening to report immigration status: § 519(5) “To report his, her, or their immigration status or suspected immigration status.”
- Threatening unlawful injury: § 519(1) “To do an unlawful injury to the person or property of the individual threatened or of a third person.”

Points about the words: § 519(2) contains no exception for a person who is a crime victim and no qualifier such as "false" or "falsely". Section 519 only lists threats; the offense additionally requires the purpose/result in § 518(a) (“obtaining of property or other consideration”), the intent in § 523(a) (“with intent to extort property or other consideration from another”) or the attempt in § 524. The statutory text does not define “wrongful” (§ 518(a)) or "extort". NOT addressed on the official pages (case law was not retrieved): whether a demand tied to the victim's own loss (return of property, repayment, compensation) is "wrongful" or an "intent to extort".


## 3. Penal Code § 523 — Extortionate letters; ransomware (GUARDRAIL)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=523> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_60828.lob` (2,122 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:10Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2017, Ch. 518, Sec. 3. (SB 500) Effective January 1, 2018."
- **Effective-date field:** 2018-01-01
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 13. OF CRIMES AGAINST PROPERTY [450. - 593g.] > CHAPTER 7. Extortion [518. - 527.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_55f2bb8f-df53-11e7-967b-c7bde29c26e0`; SHA-256 of the XML record `2903fec66a529376d8a9ab7a7d6c77e4d9cbe7c56d5da587c882af8866b4da85`

### (2) Operative text (verbatim)

> (a) Every person who, with intent to extort property or other consideration from another, sends or delivers to any person any letter or other writing, whether subscribed or not, expressing or implying, or adapted to imply, any threat such as is specified in Section 519 is punishable in the same manner as if such property or other consideration were actually obtained by means of such threat.
>
> (b) (1) Every person who, with intent to extort property or other consideration from another, introduces ransomware into any computer, computer system, or computer network is punishable pursuant to Section 520 in the same manner as if such property or other consideration were actually obtained by means of the ransomware.
>
> (2) Prosecution pursuant to this subdivision does not prohibit or limit prosecution under any other law.
>
> (c) (1) “Ransomware” means a computer contaminant, as defined in Section 502, or lock placed or introduced without authorization into a computer, computer system, or computer network that restricts access by an authorized person to the computer, computer system, computer network, or any data therein under circumstances in which the person responsible for the placement or introduction of the ransomware demands payment of money or other consideration to remove the computer contaminant, restore access to the computer, computer system, computer network, or data, or otherwise remediate the impact of the computer contaminant or lock.
>
> (2) A person is responsible for placing or introducing ransomware into a computer, computer system, or computer network if the person directly places or introduces the ransomware or directs or induces another person to do so, with the intent of demanding payment or other consideration to remove the ransomware, restore access, or otherwise remediate the impact of the ransomware.

### (3) ELEMENTS

1. Subd. (a) — Intent: “with intent to extort property or other consideration from another”.
2. Subd. (a) — Act: “sends or delivers to any person any letter or other writing, whether subscribed or not”.
3. Subd. (a) — Content: “expressing or implying, or adapted to imply, any threat such as is specified in Section 519”.
4. Subd. (a) — Result of the elements: “is punishable in the same manner as if such property or other consideration were actually obtained by means of such threat”.
5. Subd. (b)(1) (ransomware) — Intent: “with intent to extort property or other consideration from another”; Act: “introduces ransomware into any computer, computer system, or computer network”.
6. Subd. (c) defines "ransomware" (quoted in full above); subd. (b)(2): “Prosecution pursuant to this subdivision does not prohibit or limit prosecution under any other law.”

### (4) Nature of the provision / punishment

**Kind: CRIMINAL**

CRIMINAL. Punishment is stated by reference: “punishable in the same manner as if such property or other consideration were actually obtained by means of such threat” (subd. (a)); “punishable pursuant to Section 520” (subd. (b)(1)). Section 520 was not retrieved, so no term or class is stated on the pages retrieved.

### GUARDRAIL note — what conduct by a reporting victim the text would reach

Conduct by a reporting victim that the text would reach: sending or delivering “any letter or other writing, whether subscribed or not” “expressing or implying, or adapted to imply, any threat such as is specified in Section 519” (for example a threat to report a crime or expose a secret unless the recipient gives something of value), “with intent to extort property or other consideration”. By its words the offense is the sending or delivery with that intent; the text does not use words requiring that anything actually be obtained (the punishment clause speaks of the property “were actually obtained” as a hypothetical). The text does not say whether electronic messages (text messages, e-mail, social-media messages) are a "letter or other writing"; that question is not addressed on the official page.


## 4. Penal Code § 524 — Attempted extortion (GUARDRAIL)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=524> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_75730.lob` (444 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:13Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2017, Ch. 518, Sec. 4. (SB 500) Effective January 1, 2018."
- **Effective-date field:** 2018-01-01
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 13. OF CRIMES AGAINST PROPERTY [450. - 593g.] > CHAPTER 7. Extortion [518. - 527.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_5bc66e91-df53-11e7-967b-c7bde29c26e0`; SHA-256 of the XML record `4e9cc9267f2d2da894fa6fb21c0b1d570d1650725f2db5bd8eed168d0836d0d0`

### (2) Operative text (verbatim)

> Every person who attempts, by means of any threat, such as is specified in Section 519 of this code, to extort property or other consideration from another is punishable by imprisonment in the county jail not longer than one year or in the state prison or by fine not exceeding ten thousand dollars ($10,000), or by both such fine and imprisonment.

### (3) ELEMENTS

1. Actor: “Every person who”.
2. Act: “attempts”.
3. Means: “by means of any threat, such as is specified in Section 519 of this code”.
4. Object: “to extort property or other consideration from another”.

### (4) Nature of the provision / punishment

**Kind: CRIMINAL**

CRIMINAL. Stated punishment: “is punishable by imprisonment in the county jail not longer than one year or in the state prison or by fine not exceeding ten thousand dollars ($10,000), or by both such fine and imprisonment”. The text does not label the offense "felony" or "misdemeanor"; it states the alternatives quoted.

### GUARDRAIL note — what conduct by a reporting victim the text would reach

Conduct by a reporting victim that the text would reach: an unsuccessful demand is enough — the section covers one who “attempts, by means of any threat, such as is specified in Section 519 of this code, to extort property or other consideration from another”. A threat to accuse the other person of a crime (§ 519(2)), made in an attempt to obtain property or anything of value, is within these words on their face; the section contains no exception for a person who is a crime victim. What "attempts" and "extort" require is not defined in the text and no case law was retrieved.

