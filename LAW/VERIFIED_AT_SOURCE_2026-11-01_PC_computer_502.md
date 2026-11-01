# Penal Code § 502 — Computer data access and fraud

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `PC_computer_502` · sections: PEN 502 (complete section, subdivisions (a)-(k); no omissions)

## How this file was produced (read first)

1. **Direct fetch of the leginfo HTML page failed.** On 2026-11-01 curl (through the session proxy) and WebFetch received HTTP 403 with a Cloudflare "Just a moment..." JavaScript challenge for `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118` (01:56:59Z) and the same challenge for two other leginfo paths (`/faces/codes.xhtml`, `/faces/codes_displayText.xhtml`; 01:57:38Z). This is the origin site's bot challenge, not an egress-proxy policy denial (the proxy log was clean). No attempt was made to defeat the challenge. The first Exa connector returned HTTP 402 (credit limit) at 01:57:36Z.
2. **Text source actually used.** The Legislature's own data publication behind the leginfo site: `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` (HTTP Last-Modified Mon, 26 Oct 2026 04:26:08 GMT; entries dated 2026-10-25). Read by HTTP byte-range requests: the ZIP central directory, `LAW_SECTION_TBL.dat` (section metadata incl. the official history note), `LAW_TOC_TBL.dat` (official headings) and one `LAW_SECTION_TBL_<n>.lob` XML record per section. Every entry passed its ZIP CRC-32 check; each section's SHA-256 is listed in its source record.
3. **Independent cross-check against the live page.** A second Exa connector fetched live leginfo pages. Penal Code § 118: text identical to the record (machine-compared). Code of Civil Procedure § 1010.6: identical on visual comparison of subdivisions (a)-(e)(4)(C). Code of Civil Procedure § 473: the live page presents a two-version selection list whose history notes match the record. Other sections were not individually cross-checked against the live page.
4. **Rendering.** The source is Legislative Counsel XML. Only whitespace is normalised (source line-wrap whitespace collapsed to single spaces; the XML en-space/em-space spacing elements shown as one space); no word, number, punctuation or subdivision label is altered. Italic markup is shown with asterisks; the source's underlined signature leader (CCP 415.30 form only) is shown as "[underlined signature line]". Curly quotes and apostrophes are as in the source.
5. **Currency as of 2026-11-01.** The publication was generated 2026-10-25. The Legislature's later incremental update files (pubinfo_Mon/Wed/Thu, last-modified 27, 29 and 30 Oct 2026) contain no law-section tables, i.e. no code-section changes between the snapshot and 30 Oct 2026 (no later incremental file had been published at retrieval). The law tables include 2026-session statutes (latest cited: Stats. 2026, ch. 1036). Every bill chaptered in 2025 (991 bills; 4,663 amendment action lines) and in 2026 (1,263 bills; 5,684 action lines) was scanned for amendments to the sections in the whole LAW/ set: the only hits were AB 747 (Stats. 2025, ch. 563 -> CCP § 473) and AB 540 (Stats. 2026, ch. 263 -> CCP § 1010.6); both are handled in `VERIFIED_AT_SOURCE_2026-11-01_CCP_service.md`.
6. **Limits.** No case law, annotations or secondary sources were consulted; "ELEMENTS" are drawn only from the quoted statutory words (every quoted phrase was machine-checked against the retrieved text). Statutes enacted in 2026 that take effect 1 Jan 2027 are not yet in the code tables except as noted. This is legal research support, not legal advice.


> **Completeness note:** the whole of § 502 is reproduced below — subdivision (b) definitions (including "Access" (b)(1), "Computer services" (b)(4) and "Data" (b)(8)), all of (c)(1)-(c)(14), and the civil action in (e). **[omitted: none]**.


## 1. Penal Code § 502 — Computer data access and fraud (full section)

### (1) Source record

- **Status:** VERIFIED at the official source (Legislature's own data publication; the leginfo HTML page was unreachable — see "How this file was produced").
- **Canonical official page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=502> — not fetched individually; the leginfo host answered every path tried (PEN 118 section page, /faces/codes.xhtml, /faces/codes_displayText.xhtml) with the same Cloudflare challenge, HTTP 403.
- **URL actually read for the text:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> — HTTP byte-range read of ZIP entry `LAW_SECTION_TBL_61669.lob` (19,701 bytes; ZIP CRC-32 verified); row metadata from ZIP entry `LAW_SECTION_TBL.dat`.
- **Retrieved (UTC):** 2026-11-01T02:01:12Z
- **Official history note (HISTORY field, whitespace collapsed):** "Amended by Stats. 2019, Ch. 16, Sec. 1. (AB 814) Effective January 1, 2020."
- **Effective-date field:** 2020-01-01
- **Official location:** Penal Code PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 13. OF CRIMES AGAINST PROPERTY [450. - 593g.] > CHAPTER 5. Larceny [484. - 502.9.]
- **Record identifiers:** LAW_SECTION_VERSION_ID `id_9f6099b1-0bdc-11ea-912d-915c88c10a14`; SHA-256 of the XML record `6eef3b31611b417549b70d4d1a2b4c5449ef42ed75e42b6e2ebaef32fc3e214e`

### (2) Operative text (verbatim)

> (a) It is the intent of the Legislature in enacting this section to expand the degree of protection afforded to individuals, businesses, and governmental agencies from tampering, interference, damage, and unauthorized access to lawfully created computer data and computer systems. The Legislature finds and declares that the proliferation of computer technology has resulted in a concomitant proliferation of computer crime and other forms of unauthorized access to computers, computer systems, and computer data.
>
> The Legislature further finds and declares that protection of the integrity of all types and forms of lawfully created computers, computer systems, and computer data is vital to the protection of the privacy of individuals as well as to the well-being of financial institutions, business concerns, governmental agencies, and others within this state that lawfully utilize those computers, computer systems, and data.
>
> (b) For the purposes of this section, the following terms have the following meanings:
>
> (1) “Access” means to gain entry to, instruct, cause input to, cause output from, cause data processing with, or communicate with, the logical, arithmetical, or memory function resources of a computer, computer system, or computer network.
>
> (2) “Computer network” means any system that provides communications between one or more computer systems and input/output devices, including, but not limited to, display terminals, remote systems, mobile devices, and printers connected by telecommunication facilities.
>
> (3) “Computer program or software” means a set of instructions or statements, and related data, that when executed in actual or modified form, cause a computer, computer system, or computer network to perform specified functions.
>
> (4) “Computer services” includes, but is not limited to, computer time, data processing, or storage functions, internet services, electronic mail services, electronic message services, or other uses of a computer, computer system, or computer network.
>
> (5) “Computer system” means a device or collection of devices, including support devices and excluding calculators that are not programmable and capable of being used in conjunction with external files, one or more of which contain computer programs, electronic instructions, input data, and output data, that performs functions, including, but not limited to, logic, arithmetic, data storage and retrieval, communication, and control. A “computer system” includes, without limitation, any such device or system that is located within, connected to, or otherwise integrated with, any motor vehicle as defined in Section 415 of the Vehicle Code.
>
> (6) “Government computer system” means any computer system, or part thereof, that is owned, operated, or used by any federal, state, or local governmental entity.
>
> (7) “Public safety infrastructure computer system” means any computer system, or part thereof, that is necessary for the health and safety of the public including computer systems owned, operated, or used by drinking water and wastewater treatment facilities, hospitals, emergency service providers, telecommunication companies, and gas and electric utility companies.
>
> (8) “Data” means a representation of information, knowledge, facts, concepts, computer software, or computer programs or instructions. Data may be in any form, in storage media, or as stored in the memory of the computer or in transit or presented on a display device.
>
> (9) “Supporting documentation” includes, but is not limited to, all information, in any form, pertaining to the design, construction, classification, implementation, use, or modification of a computer, computer system, computer network, computer program, or computer software, which information is not generally available to the public and is necessary for the operation of a computer, computer system, computer network, computer program, or computer software.
>
> (10) “Injury” means any alteration, deletion, damage, or destruction of a computer system, computer network, computer program, or data caused by the access, or the denial of access to legitimate users of a computer system, network, or program.
>
> (11) “Victim expenditure” means any expenditure reasonably and necessarily incurred by the owner or lessee to verify that a computer system, computer network, computer program, or data was or was not altered, deleted, damaged, or destroyed by the access.
>
> (12) “Computer contaminant” means any set of computer instructions that are designed to modify, damage, destroy, record, or transmit information within a computer, computer system, or computer network without the intent or permission of the owner of the information. They include, but are not limited to, a group of computer instructions commonly called viruses or worms, that are self-replicating or self-propagating and are designed to contaminate other computer programs or computer data, consume computer resources, modify, destroy, record, or transmit data, or in some other fashion usurp the normal operation of the computer, computer system, or computer network.
>
> (13) “Internet domain name” means a globally unique, hierarchical reference to an internet host or service, assigned through centralized internet naming authorities, comprising a series of character strings separated by periods, with the rightmost character string specifying the top of the hierarchy.
>
> (14) “Electronic mail” means an electronic message or computer file that is transmitted between two or more telecommunications devices; computers; computer networks, regardless of whether the network is a local, regional, or global network; or electronic devices capable of receiving electronic messages, regardless of whether the message is converted to hard copy format after receipt, viewed upon transmission, or stored for later retrieval.
>
> (15) “Profile” means either of the following:
>
> (A) A configuration of user data required by a computer so that the user may access programs or services and have the desired functionality on that computer.
>
> (B) An Internet website user’s personal page or section of a page that is made up of data, in text or graphical form, that displays significant, unique, or identifying information, including, but not limited to, listing acquaintances, interests, associations, activities, or personal statements.
>
> (c) Except as provided in subdivision (h), any person who commits any of the following acts is guilty of a public offense:
>
> (1) Knowingly accesses and without permission alters, damages, deletes, destroys, or otherwise uses any data, computer, computer system, or computer network in order to either (A) devise or execute any scheme or artifice to defraud, deceive, or extort, or (B) wrongfully control or obtain money, property, or data.
>
> (2) Knowingly accesses and without permission takes, copies, or makes use of any data from a computer, computer system, or computer network, or takes or copies any supporting documentation, whether existing or residing internal or external to a computer, computer system, or computer network.
>
> (3) Knowingly and without permission uses or causes to be used computer services.
>
> (4) Knowingly accesses and without permission adds, alters, damages, deletes, or destroys any data, computer software, or computer programs which reside or exist internal or external to a computer, computer system, or computer network.
>
> (5) Knowingly and without permission disrupts or causes the disruption of computer services or denies or causes the denial of computer services to an authorized user of a computer, computer system, or computer network.
>
> (6) Knowingly and without permission provides or assists in providing a means of accessing a computer, computer system, or computer network in violation of this section.
>
> (7) Knowingly and without permission accesses or causes to be accessed any computer, computer system, or computer network.
>
> (8) Knowingly introduces any computer contaminant into any computer, computer system, or computer network.
>
> (9) Knowingly and without permission uses the internet domain name or profile of another individual, corporation, or entity in connection with the sending of one or more electronic mail messages or posts and thereby damages or causes damage to a computer, computer data, computer system, or computer network.
>
> (10) Knowingly and without permission disrupts or causes the disruption of government computer services or denies or causes the denial of government computer services to an authorized user of a government computer, computer system, or computer network.
>
> (11) Knowingly accesses and without permission adds, alters, damages, deletes, or destroys any data, computer software, or computer programs which reside or exist internal or external to a public safety infrastructure computer system computer, computer system, or computer network.
>
> (12) Knowingly and without permission disrupts or causes the disruption of public safety infrastructure computer system computer services or denies or causes the denial of computer services to an authorized user of a public safety infrastructure computer system computer, computer system, or computer network.
>
> (13) Knowingly and without permission provides or assists in providing a means of accessing a computer, computer system, or public safety infrastructure computer system computer, computer system, or computer network in violation of this section.
>
> (14) Knowingly introduces any computer contaminant into any public safety infrastructure computer system computer, computer system, or computer network.
>
> (d) (1) Any person who violates any of the provisions of paragraph (1), (2), (4), (5), (10), (11), or (12) of subdivision (c) is guilty of a felony, punishable by imprisonment pursuant to subdivision (h) of Section 1170 for 16 months, or two or three years and a fine not exceeding ten thousand dollars ($10,000), or a misdemeanor, punishable by imprisonment in a county jail not exceeding one year, by a fine not exceeding five thousand dollars ($5,000), or by both that fine and imprisonment.
>
> (2) Any person who violates paragraph (3) of subdivision (c) is punishable as follows:
>
> (A) For the first violation that does not result in injury, and where the value of the computer services used does not exceed nine hundred fifty dollars ($950), by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment.
>
> (B) For any violation that results in a victim expenditure in an amount greater than five thousand dollars ($5,000) or in an injury, or if the value of the computer services used exceeds nine hundred fifty dollars ($950), or for any second or subsequent violation, by a fine not exceeding ten thousand dollars ($10,000), or by imprisonment pursuant to subdivision (h) of Section 1170 for 16 months, or two or three years, or by both that fine and imprisonment, or by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment.
>
> (3) Any person who violates paragraph (6), (7), or (13) of subdivision (c) is punishable as follows:
>
> (A) For a first violation that does not result in injury, an infraction punishable by a fine not exceeding one thousand dollars ($1,000).
>
> (B) For any violation that results in a victim expenditure in an amount not greater than five thousand dollars ($5,000), or for a second or subsequent violation, by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment.
>
> (C) For any violation that results in a victim expenditure in an amount greater than five thousand dollars ($5,000), by a fine not exceeding ten thousand dollars ($10,000), or by imprisonment pursuant to subdivision (h) of Section 1170 for 16 months, or two or three years, or by both that fine and imprisonment, or by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment.
>
> (4) Any person who violates paragraph (8) or (14) of subdivision (c) is punishable as follows:
>
> (A) For a first violation that does not result in injury, a misdemeanor punishable by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment.
>
> (B) For any violation that results in injury, or for a second or subsequent violation, by a fine not exceeding ten thousand dollars ($10,000), or by imprisonment in a county jail not exceeding one year, or by imprisonment pursuant to subdivision (h) of Section 1170, or by both that fine and imprisonment.
>
> (5) Any person who violates paragraph (9) of subdivision (c) is punishable as follows:
>
> (A) For a first violation that does not result in injury, an infraction punishable by a fine not exceeding one thousand dollars ($1,000).
>
> (B) For any violation that results in injury, or for a second or subsequent violation, by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment.
>
> (e) (1) In addition to any other civil remedy available, the owner or lessee of the computer, computer system, computer network, computer program, or data who suffers damage or loss by reason of a violation of any of the provisions of subdivision (c) may bring a civil action against the violator for compensatory damages and injunctive relief or other equitable relief. Compensatory damages shall include any expenditure reasonably and necessarily incurred by the owner or lessee to verify that a computer system, computer network, computer program, or data was or was not altered, damaged, or deleted by the access. For the purposes of actions authorized by this subdivision, the conduct of an unemancipated minor shall be imputed to the parent or legal guardian having control or custody of the minor, pursuant to the provisions of Section 1714.1 of the Civil Code.
>
> (2) In any action brought pursuant to this subdivision the court may award reasonable attorney’s fees.
>
> (3) A community college, state university, or academic institution accredited in this state is required to include computer-related crimes as a specific violation of college or university student conduct policies and regulations that may subject a student to disciplinary sanctions up to and including dismissal from the academic institution. This paragraph shall not apply to the University of California unless the Board of Regents adopts a resolution to that effect.
>
> (4) In any action brought pursuant to this subdivision for a willful violation of the provisions of subdivision (c), where it is proved by clear and convincing evidence that a defendant has been guilty of oppression, fraud, or malice as defined in subdivision (c) of Section 3294 of the Civil Code, the court may additionally award punitive or exemplary damages.
>
> (5) No action may be brought pursuant to this subdivision unless it is initiated within three years of the date of the act complained of, or the date of the discovery of the damage, whichever is later.
>
> (f) This section shall not be construed to preclude the applicability of any other provision of the criminal law of this state which applies or may apply to any transaction, nor shall it make illegal any employee labor relations activities that are within the scope and protection of state or federal labor laws.
>
> (g) Any computer, computer system, computer network, or any software or data, owned by the defendant, that is used during the commission of any public offense described in subdivision (c) or any computer, owned by the defendant, which is used as a repository for the storage of software or data illegally obtained in violation of subdivision (c) shall be subject to forfeiture, as specified in Section 502.01.
>
> (h) (1) Subdivision (c) does not apply to punish any acts which are committed by a person within the scope of lawful employment. For purposes of this section, a person acts within the scope of employment when the person performs acts which are reasonably necessary to the performance of their work assignment.
>
> (2) Paragraph (3) of subdivision (c) does not apply to penalize any acts committed by a person acting outside of their lawful employment, provided that the employee’s activities do not cause an injury, to the employer or another, or provided that the value of supplies or computer services which are used does not exceed an accumulated total of two hundred fifty dollars ($250).
>
> (i) No activity exempted from prosecution under paragraph (2) of subdivision (h) which incidentally violates paragraph (2), (4), or (7) of subdivision (c) shall be prosecuted under those paragraphs.
>
> (j) For purposes of bringing a civil or a criminal action under this section, a person who causes, by any means, the access of a computer, computer system, or computer network in one jurisdiction from another jurisdiction is deemed to have personally accessed the computer, computer system, or computer network in each jurisdiction.
>
> (k) In determining the terms and conditions applicable to a person convicted of a violation of this section the court shall consider the following:
>
> (1) The court shall consider prohibitions on access to and use of computers.
>
> (2) Except as otherwise required by law, the court shall consider alternate sentencing, including community service, if the defendant shows remorse and recognition of the wrongdoing, and an inclination not to repeat the offense.

### (3) ELEMENTS

1. Lead-in to every offense: “Except as provided in subdivision (h), any person who commits any of the following acts is guilty of a public offense:” — (i) the actor is “any person”; (ii) the act is one of the fourteen listed in (c)(1)–(c)(14); (iii) the subdivision (h) exceptions do not apply.
2. Mental state: each of paragraphs (c)(1)–(c)(14) begins with “Knowingly”.
3. Absence of permission: paragraphs (c)(1)–(c)(7) and (c)(9)–(c)(13) each contain the words "without permission" (for example (c)(3): “Knowingly and without permission uses or causes to be used computer services.”). Paragraphs (c)(8) and (c)(14) do not contain those words: “Knowingly introduces any computer contaminant into any computer, computer system, or computer network.”
4. Defined terms apply: “For the purposes of this section, the following terms have the following meanings:” Of the terms you flagged:
   - "Access" (b)(1): “means to gain entry to, instruct, cause input to, cause output from, cause data processing with, or communicate with, the logical, arithmetical, or memory function resources of a computer, computer system, or computer network”.
   - "Computer services" (b)(4): “includes, but is not limited to, computer time, data processing, or storage functions, internet services, electronic mail services, electronic message services, or other uses of a computer, computer system, or computer network”.
   - "Data" (b)(8): “means a representation of information, knowledge, facts, concepts, computer software, or computer programs or instructions. Data may be in any form, in storage media, or as stored in the memory of the computer or in transit or presented on a display device.”
   - Other defined terms used in (c): computer network (b)(2), computer program or software (b)(3), computer system (b)(5), government computer system (b)(6), public safety infrastructure computer system (b)(7), supporting documentation (b)(9), injury (b)(10), victim expenditure (b)(11), computer contaminant (b)(12), internet domain name (b)(13), electronic mail (b)(14), profile (b)(15) — all in the verbatim text above.
5. Act elements — ONE of the following (each is a separate offense):
   - (c)(1) “accesses and without permission alters, damages, deletes, destroys, or otherwise uses any data, computer, computer system, or computer network” PLUS a purpose: “in order to either (A) devise or execute any scheme or artifice to defraud, deceive, or extort, or (B) wrongfully control or obtain money, property, or data”.
   - (c)(2) “accesses and without permission takes, copies, or makes use of any data from a computer, computer system, or computer network, or takes or copies any supporting documentation”.
   - (c)(3) “uses or causes to be used computer services”.
   - (c)(4) “accesses and without permission adds, alters, damages, deletes, or destroys any data, computer software, or computer programs which reside or exist internal or external to a computer, computer system, or computer network”.
   - (c)(5) “disrupts or causes the disruption of computer services or denies or causes the denial of computer services to an authorized user of a computer, computer system, or computer network”.
   - (c)(6) “provides or assists in providing a means of accessing a computer, computer system, or computer network in violation of this section”.
   - (c)(7) “accesses or causes to be accessed any computer, computer system, or computer network”.
   - (c)(8) “introduces any computer contaminant into any computer, computer system, or computer network”.
   - (c)(9) “uses the internet domain name or profile of another individual, corporation, or entity in connection with the sending of one or more electronic mail messages or posts and thereby damages or causes damage to a computer, computer data, computer system, or computer network”.
   - (c)(10) “disrupts or causes the disruption of government computer services or denies or causes the denial of government computer services to an authorized user of a government computer, computer system, or computer network”.
   - (c)(11) “accesses and without permission adds, alters, damages, deletes, or destroys any data, computer software, or computer programs which reside or exist internal or external to a public safety infrastructure computer system computer, computer system, or computer network”.
   - (c)(12) “disrupts or causes the disruption of public safety infrastructure computer system computer services or denies or causes the denial of computer services to an authorized user of a public safety infrastructure computer system computer, computer system, or computer network”.
   - (c)(13) “provides or assists in providing a means of accessing a computer, computer system, or public safety infrastructure computer system computer, computer system, or computer network in violation of this section”.
   - (c)(14) “introduces any computer contaminant into any public safety infrastructure computer system computer, computer system, or computer network”.
6. Employment exception (subd. (h)(1)): “Subdivision (c) does not apply to punish any acts which are committed by a person within the scope of lawful employment.” Scope: “a person acts within the scope of employment when the person performs acts which are reasonably necessary to the performance of their work assignment”. Narrower exception for (c)(3): subd. (h)(2) (quoted in full above).
7. Multi-jurisdiction access (subd. (j)): “a person who causes, by any means, the access of a computer, computer system, or computer network in one jurisdiction from another jurisdiction is deemed to have personally accessed the computer, computer system, or computer network in each jurisdiction”.
8. CIVIL ACTION (subd. (e)(1)) — plaintiff must show: (i) status: “the owner or lessee of the computer, computer system, computer network, computer program, or data”; (ii) harm: “who suffers damage or loss”; (iii) causation by a violation: “by reason of a violation of any of the provisions of subdivision (c)”; remedy: “compensatory damages and injunctive relief or other equitable relief”. Compensatory damages “shall include any expenditure reasonably and necessarily incurred by the owner or lessee to verify that a computer system, computer network, computer program, or data was or was not altered, damaged, or deleted by the access”.
9. Civil action — fees, punitive damages, limitations, minors: attorney's fees are discretionary (“the court may award reasonable attorney’s fees”); punitive damages require a “willful violation” and “clear and convincing evidence that a defendant has been guilty of oppression, fraud, or malice as defined in subdivision (c) of Section 3294 of the Civil Code”; time limit: “No action may be brought pursuant to this subdivision unless it is initiated within three years of the date of the act complained of, or the date of the discovery of the damage, whichever is later.” Minors: “the conduct of an unemancipated minor shall be imputed to the parent or legal guardian having control or custody of the minor, pursuant to the provisions of Section 1714.1 of the Civil Code”.

### (4) Nature of the provision / punishment

**Kind: CRIMINAL (with a CIVIL action in subd. (e))**

CRIMINAL, with a parallel CIVIL cause of action in subdivision (e). Stated punishment classes (subd. (d)):

- (d)(1) — violations of (c)(1), (2), (4), (5), (10), (11), (12): “is guilty of a felony, punishable by imprisonment pursuant to subdivision (h) of Section 1170 for 16 months, or two or three years and a fine not exceeding ten thousand dollars ($10,000), or a misdemeanor, punishable by imprisonment in a county jail not exceeding one year, by a fine not exceeding five thousand dollars ($5,000), or by both that fine and imprisonment”.
- (d)(2) — violations of (c)(3): graded by injury, victim expenditure, value of services and prior violations. (A) first violation that does not result in injury and where the value of the computer services used does not exceed $950: “by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment”. (B) a violation that results in a victim expenditure greater than $5,000 or in an injury, or where the value of the services exceeds $950, or any second or subsequent violation: “by a fine not exceeding ten thousand dollars ($10,000), or by imprisonment pursuant to subdivision (h) of Section 1170 for 16 months, or two or three years, or by both that fine and imprisonment, or by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment”.
- (d)(3) — violations of (c)(6), (7), (13): (A) “For a first violation that does not result in injury, an infraction punishable by a fine not exceeding one thousand dollars ($1,000).” (B) victim expenditure not greater than $5,000, or a second or subsequent violation: “by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment”. (C) victim expenditure greater than $5,000: “by a fine not exceeding ten thousand dollars ($10,000), or by imprisonment pursuant to subdivision (h) of Section 1170 for 16 months, or two or three years, or by both that fine and imprisonment, or by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment”.
- (d)(4) — violations of (c)(8), (14): (A) “For a first violation that does not result in injury, a misdemeanor punishable by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment.” (B) injury or a second or subsequent violation: “by a fine not exceeding ten thousand dollars ($10,000), or by imprisonment in a county jail not exceeding one year, or by imprisonment pursuant to subdivision (h) of Section 1170, or by both that fine and imprisonment”.
- (d)(5) — violations of (c)(9): (A) first violation without injury: “an infraction punishable by a fine not exceeding one thousand dollars ($1,000)”; (B) injury or a second or subsequent violation: “by a fine not exceeding five thousand dollars ($5,000), or by imprisonment in a county jail not exceeding one year, or by both that fine and imprisonment”.

Other provisions: forfeiture of the defendant's computer used in the offense (subd. (g), by reference to § 502.01); sentencing considerations (subd. (k)); “This section shall not be construed to preclude the applicability of any other provision of the criminal law of this state which applies or may apply to any transaction” (subd. (f)).

Relevance note: subd. (e)(1) provides that “the conduct of an unemancipated minor shall be imputed to the parent or legal guardian having control or custody of the minor” for purposes of the civil action.

