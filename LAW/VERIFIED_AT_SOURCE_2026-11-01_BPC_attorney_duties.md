# Business and Professions Code — attorney duties (§§ 6068, 6128)

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `BPC_attorney_duties` · sections: BPC 6068 (complete; subd. (d) is the candor duty), BPC 6128 (complete; subd. (a) is the deceit offense)

## How this file was produced (read first)

1. **Direct fetch of the leginfo HTML page failed.** On 2026-11-01 curl (through the session proxy) and WebFetch received HTTP 403 with a Cloudflare "Just a moment..." JavaScript challenge for `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118` (01:56:59Z) and the same challenge for two other leginfo paths (`/faces/codes.xhtml`, `/faces/codes_displayText.xhtml`; 01:57:38Z). This is the origin site's bot challenge, not an egress-proxy policy denial (the proxy log was clean). No attempt was made to defeat the challenge. The first Exa connector returned HTTP 402 (credit limit) at 01:57:36Z.
2. **Text source actually used.** The Legislature's own data publication behind the leginfo site: `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` (HTTP Last-Modified Mon, 26 Oct 2026 04:26:08 GMT; entries dated 2026-10-25). Read by HTTP byte-range requests: the ZIP central directory, `LAW_SECTION_TBL.dat` (section metadata incl. the official history note), `LAW_TOC_TBL.dat` (official headings) and one `LAW_SECTION_TBL_<n>.lob` XML record per section. Every entry passed its ZIP CRC-32 check; each section's SHA-256 is listed in its source record.
3. **Independent cross-check against the live page.** A second Exa connector fetched live leginfo pages. Penal Code § 118: text identical to the record (machine-compared). Code of Civil Procedure § 1010.6: identical on visual comparison of subdivisions (a)-(e)(4)(C). Code of Civil Procedure § 473: the live page presents a two-version selection list whose history notes match the record. Other sections were not individually cross-checked against the live page.
4. **Rendering.** The source is Legislative Counsel XML. Only whitespace is normalised (source line-wrap whitespace collapsed to single spaces; the XML en-space/em-space spacing elements shown as one space); no word, number, punctuation or subdivision label is altered. Italic markup is shown with asterisks; the source's underlined signature leader (CCP 415.30 form only) is shown as "[underlined signature line]". Curly quotes and apostrophes are as in the source.
5. **Currency as of 2026-11-01.** The publication was generated 2026-10-25. The Legislature's later incremental update files (pubinfo_Mon/Wed/Thu, last-modified 27, 29 and 30 Oct 2026) contain no law-section tables, i.e. no code-section changes between the snapshot and 30 Oct 2026 (no later incremental file had been published at retrieval). The law tables include 2026-session statutes (latest cited: Stats. 2026, ch. 1036). Every bill chaptered in 2025 (991 bills; 4,663 amendment action lines) and in 2026 (1,263 bills; 5,684 action lines) was scanned for amendments to the sections in the whole LAW/ set: the only hits were AB 747 (Stats. 2025, ch. 563 -> CCP § 473) and AB 540 (Stats. 2026, ch. 263 -> CCP § 1010.6); both are handled in `VERIFIED_AT_SOURCE_2026-11-01_CCP_service.md`.
6. **Limits.** No case law, annotations or secondary sources were consulted; "ELEMENTS" are drawn only from the quoted statutory words (every quoted phrase was machine-checked against the retrieved text). Statutes enacted in 2026 that take effect 1 Jan 2027 are not yet in the code tables except as noted. This is legal research support, not legal advice.


> **Subdivisions requested:** § 6068(d) and § 6128(a). Both sections are reproduced in full (no omissions) so that the section introductions are in front of you: § 6068 opens “It is the duty of an attorney to do all of the following:”; § 6128 opens “Every attorney is guilty of a misdemeanor who either:”.


## 1. Business and Professions Code § 6068 — Duties of an attorney (subdivision (d) is the operative provision for candor)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=BPC&sectionNum=6068> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_74462.lob` (6,307 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:13Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2018, Ch. 659, Sec. 50. (AB 3249) Effective January 1, 2019."
- **Effective-date field:** 2019-01-01
- **Official location:** Business and Professions Code DIVISION 3. PROFESSIONS AND VOCATIONS GENERALLY [5000. - 9998.12.] > CHAPTER 4. Attorneys [6000. - 6256.] > ARTICLE 4. Admission to the Practice of Law [6060. - 6069.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_cc237c62-0490-11e9-ab56-b19463a6a13d`; SHA-256 of the XML record `f7b98768e99e9acc0dde9cb27a5c04f8d277f2a656e1e878d0c180fcdaeaaf3f`

### (2) Operative text (verbatim)

> It is the duty of an attorney to do all of the following:
>
> (a) To support the Constitution and laws of the United States and of this state.
>
> (b) To maintain the respect due to the courts of justice and judicial officers.
>
> (c) To counsel or maintain those actions, proceedings, or defenses only as appear to him or her legal or just, except the defense of a person charged with a public offense.
>
> (d) To employ, for the purpose of maintaining the causes confided to him or her those means only as are consistent with truth, and never to seek to mislead the judge or any judicial officer by an artifice or false statement of fact or law.
>
> (e) (1) To maintain inviolate the confidence, and at every peril to himself or herself to preserve the secrets, of his or her client.
>
> (2) Notwithstanding paragraph (1), an attorney may, but is not required to, reveal confidential information relating to the representation of a client to the extent that the attorney reasonably believes the disclosure is necessary to prevent a criminal act that the attorney reasonably believes is likely to result in death of, or substantial bodily harm to, an individual.
>
> (f) To advance no fact prejudicial to the honor or reputation of a party or witness, unless required by the justice of the cause with which he or she is charged.
>
> (g) Not to encourage either the commencement or the continuance of an action or proceeding from any corrupt motive of passion or interest.
>
> (h) Never to reject, for any consideration personal to himself or herself, the cause of the defenseless or the oppressed.
>
> (i) To cooperate and participate in any disciplinary investigation or other regulatory or disciplinary proceeding pending against himself or herself. However, this subdivision shall not be construed to deprive an attorney of any privilege guaranteed by the Fifth Amendment to the Constitution of the United States, or any other constitutional or statutory privileges. This subdivision shall not be construed to require an attorney to cooperate with a request that requires him or her to waive any constitutional or statutory privilege or to comply with a request for information or other matters within an unreasonable period of time in light of the time constraints of the attorney’s practice. Any exercise by an attorney of any constitutional or statutory privilege shall not be used against the attorney in a regulatory or disciplinary proceeding against him or her.
>
> (j) To comply with the requirements of Section 6002.1.
>
> (k) To comply with all conditions attached to any disciplinary probation, including a probation imposed with the concurrence of the attorney.
>
> (*l*) To keep all agreements made in lieu of disciplinary prosecution with the State Bar.
>
> (m) To respond promptly to reasonable status inquiries of clients and to keep clients reasonably informed of significant developments in matters with regard to which the attorney has agreed to provide legal services.
>
> (n) To provide copies to the client of certain documents under time limits and as prescribed in a rule of professional conduct which the board shall adopt.
>
> (o) To report to the State Bar, in writing, within 30 days of the time the attorney has knowledge of any of the following:
>
> (1) The filing of three or more lawsuits in a 12-month period against the attorney for malpractice or other wrongful conduct committed in a professional capacity.
>
> (2) The entry of judgment against the attorney in a civil action for fraud, misrepresentation, breach of fiduciary duty, or gross negligence committed in a professional capacity.
>
> (3) The imposition of judicial sanctions against the attorney, except for sanctions for failure to make discovery or monetary sanctions of less than one thousand dollars ($1,000).
>
> (4) The bringing of an indictment or information charging a felony against the attorney.
>
> (5) The conviction of the attorney, including any verdict of guilty, or plea of guilty or no contest, of a felony, or a misdemeanor committed in the course of the practice of law, or in a manner in which a client of the attorney was the victim, or a necessary element of which, as determined by the statutory or common law definition of the misdemeanor, involves improper conduct of an attorney, including dishonesty or other moral turpitude, or an attempt or a conspiracy or solicitation of another to commit a felony or a misdemeanor of that type.
>
> (6) The imposition of discipline against the attorney by a professional or occupational disciplinary agency or licensing board, whether in California or elsewhere.
>
> (7) Reversal of judgment in a proceeding based in whole or in part upon misconduct, grossly incompetent representation, or willful misrepresentation by an attorney.
>
> (8) As used in this subdivision, “against the attorney” includes claims and proceedings against any firm of attorneys for the practice of law in which the attorney was a partner at the time of the conduct complained of and any law corporation in which the attorney was a shareholder at the time of the conduct complained of unless the matter has to the attorney’s knowledge already been reported by the law firm or corporation.
>
> (9) The State Bar may develop a prescribed form for the making of reports required by this section, usage of which it may require by rule or regulation.
>
> (10) This subdivision is only intended to provide that the failure to report as required herein may serve as a basis of discipline.

### (3) ELEMENTS

1. Section intro (applies to every subdivision): “It is the duty of an attorney to do all of the following:” — the actor is “an attorney”.
2. Subd. (d), first clause — means used: “To employ, for the purpose of maintaining the causes confided to him or her those means only as are consistent with truth”. Elements: (i) the attorney employs means “for the purpose of maintaining the causes confided to him or her”; (ii) the means are not “consistent with truth”.
3. Subd. (d), second clause — misleading the court: “never to seek to mislead the judge or any judicial officer by an artifice or false statement of fact or law”. Elements: (i) the attorney seeks to mislead — the statutory words are “seek to mislead” (the text uses the verb "seek"; it contains no words requiring that the court actually be misled); (ii) the target is “the judge or any judicial officer”; (iii) the manner is “an artifice or false statement of fact or law”.

### (4) Nature of the provision / punishment

**Kind: DISCIPLINARY / REGULATORY (State Bar Act duty)**

DISCIPLINARY / REGULATORY. Business and Professions Code, Division 3, Chapter 4 ("Attorneys"), Article 4. The section states duties (“It is the duty of an attorney to do all of the following:”); subdivision (d) contains no punishment or penalty clause, and the section does not itself state the consequence of breaching (d). The only discipline language in the section is in subd. (o)(10): “This subdivision is only intended to provide that the failure to report as required herein may serve as a basis of discipline.” — which is confined to the reporting duties of subd. (o). Subdivision (i) separately imposes a duty “To cooperate and participate in any disciplinary investigation or other regulatory or disciplinary proceeding pending against himself or herself”.

Typographical note: in subdivision (l) the source XML italicises the letter l; it is shown as (*l*).


## 2. Business and Professions Code § 6128 — Attorney deceit or collusion (misdemeanor); subdivision (a)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=BPC&sectionNum=6128> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_130067.lob` (773 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:14Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 1976, Ch. 1125."
- **Effective-date field:** (none recorded in the source table)
- **Official location:** Business and Professions Code DIVISION 3. PROFESSIONS AND VOCATIONS GENERALLY [5000. - 9998.12.] > CHAPTER 4. Attorneys [6000. - 6256.] > ARTICLE 7. Unlawful Practice of Law [6125. - 6133.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_7c992827-291e-11d9-87bf-bcb27e518802`; SHA-256 of the XML record `ae6c93ce55d390384d280155ee6620d50be03b8e3fb2a00cb9bd7704b4d8d4fe`

### (2) Operative text (verbatim)

> Every attorney is guilty of a misdemeanor who either:
>
> (a) Is guilty of any deceit or collusion, or consents to any deceit or collusion, with intent to deceive the court or any party.
>
> (b) Willfully delays his client’s suit with a view to his own gain.
>
> (c) Willfully receives any money or allowance for or on account of any money which he has not laid out or become answerable for.
>
> Any violation of the provisions of this section is punishable by imprisonment in the county jail not exceeding six months, or by a fine not exceeding two thousand five hundred dollars ($2,500), or by both.

### (3) ELEMENTS

1. Section intro: “Every attorney is guilty of a misdemeanor who either:” — the actor is “Every attorney”.
2. Subd. (a), act — ONE of: “Is guilty of any deceit or collusion” OR “consents to any deceit or collusion”.
3. Subd. (a), intent: “with intent to deceive the court or any party”.
4. (Subdivisions (b) and (c) are alternative, separate offenses: “Willfully delays his client’s suit with a view to his own gain.” and “Willfully receives any money or allowance for or on account of any money which he has not laid out or become answerable for.”)

### (4) Nature of the provision / punishment

**Kind: CRIMINAL (misdemeanor) — in the State Bar Act**

CRIMINAL. Class stated: “Every attorney is guilty of a misdemeanor who either:”. Punishment stated: “Any violation of the provisions of this section is punishable by imprisonment in the county jail not exceeding six months, or by a fine not exceeding two thousand five hundred dollars ($2,500), or by both.” Business and Professions Code, Division 3, Chapter 4, Article 7 ("Unlawful Practice of Law").

