# GEMINI LEADS — "closed loop" / "triangle of corruption" — lead-mining notes

Run 2026-11-01. Opus subagent. Obeys CHARTER RULES ("AI output is never evidence … leads to underlying documents only, never quoted, attached or relied on") and INVENTORY/AGENT_RULES.md 1–7.
- Gmail/Drive read-only (search/get/read/download only). No git. No contact. This is the only file written. Scratch: /tmp/claude-0/-home-user/9a86eccf-071d-5c97-88ae-ef129ec55f9d/scratchpad/gl/.
- These notes do NOT weigh the AI assertions. AI text is not quoted. Each claim is restated in one neutral line. Quotation marks hold only identifiers (subjects, filenames) or words from PRIMARY documents.
- Every item below is AI-LEAD unless marked otherwise.
- "Register" = /home/user/spiegel-thread/EVIDENCE_REGISTER.tsv. The read value shown is its read_status column, matched exactly on the pointer column. "absent" = no pointer row.

## 0. Counts (basis at end of §6)
- AI documents opened:
  - 12 read in full: AI-01..05 (AI-05 as returned by the connector), AI-07..12, AI-14.
  - AI-06 via connector OCR only. AI-13 partly; it is out of scope (no "Spiegel").
  - The screenshot PRIM-a was read; it is not AI.
  - 5 pointer-scanned, NOT read in full: PS-01..05.
- Claims extracted: 49 (C01–C49, §3).
- Distinct primary documents identified: 55, of which:
  - 36 exist now;
  - 3 do not exist: the two "control" emails (C05; NOT FOUND by search here) and the 2024-03-29 email (C28; not found per tracker K-01);
  - 2 are not held (Google server records; BHPD↔firm communications);
  - 14 not located in this pass.
- Of the 36 existing primaries: 8 already read by this thread (register "full", or covered by a thread reading note); 28 NOT read (register not-read / metadata-only / absent).
- Claims with no primary identified at all: 7. Further claim-elements with none: 5 (§7).

## 1. Locate — queries run and hits

### Drive
| # | Query | Result |
|---|---|---|
| D1 | `title contains 'closed loop'` | 5 folders, all named "CLOSED LOOP OF CORRUPTION (BY) GOOGLE GEMINI AI": `1OgvJLK1rSQ-sAdVJCzNh2ZXem9rua_8N` (2026-03-23); `1lLlDMq8rBc0WvmpdCaDuh6gSWapP1kiL` (2026-03-23); `137ClLaap5Q6uQkAb_TfYWspHUlmmYzY_` (2026-05-27); `1dZfUHBZcodGECfuFPMWYO0RsLUtjN2pw` (2026-09-01); `1uZeZ67ARuU6D-VF1KG0B3nZbbLnxT-b9` (2026-09-01) |
| D2 | `title contains 'triangle'` | 0 |
| D3 | `title contains 'corruption'` | 36 hits: 5 folders (D1); 1/8–1/15/2026 "CONFIDENTIAL FORENSIC AUDIT & PUBLIC CORRUPTION REPORT" family (§2 AI-02); 2 copies of 1/8/2026 "CRIMINAL COMPLAINT_ Public Corruption…" PDF (`1zuCw22p2X-H4XeGkz6rRdEmRElTaxy60`, `1dICRT5pXX-4m-MJTwXkyGERtji5EbUSu`, 1,612,432 B — Halsey's outbound complaint, CORRESPONDENCE, not opened); 6 "chart-a-corruption-convictions" files (2026-10-02, unrelated chart) |
| D4 | `title contains 'Gemini'` | 88 hits, one page. Groups: GOOGLE GEMINI LEADING… PDF ×14 (AI-06); Gemini Export Jan 21/23 2026 ×30 (AI-03, AI-13); "Notes by Gemini" meeting notes ×7 (AI-LEAD, not opened); Gemini CIVIC BUSINESS REPORT ×7 (not opened); 2026-03-30 Gemini dossier/diagram/screenshots ×6; 2026-05-02 Exhibit_7a–c Gemini ×3; Gemini Content.docx; Gemini in Email.jpg; out of scope: "Cap Gemini Report" ×5, gemini.com .ics |
| D5 | `fullText contains 'closed loop' and fullText contains 'Spiegel'` | 100 on page 1; nextPageToken exists, not paged. Groups: Exhibits A-K-2.pdf ×11 (10,808,821 B); RFO with exhibits unconformed.pdf ×6 (12,308,729 B); RFO 3-24-2026.pdf; Officer_Kale_Report_Footnoted_v2 family (EV-056); KALE REPORT TO VALIDATE.pdf; Email History Analysis Request family (AI-05/EV-039); Forenisic Kale family (PS-05); Marsy's Law Dashboard PDF family (EV-040); 1 tracker monitor log |
| D6 | `fullText contains 'triangle of corruption'` | 100 on page 1; nextPageToken exists, not paged. Adds: AI-01 Doc/docx; AI-04; AI-14 "Google Realization.jpg" family; PS-03 arrest-warrant PDF ×3; PS-04 "Unraveling…" ×2; Gemini_Thinking_Screenshot_2/_4; Marsy's IA brief/analysis PDFs; ExhibitC_EmailScreenshot_Extract_Pages75-77.pdf; Untitled.pdf `1U4WSBIqG26Oq0-5dLDuJXgmesiZVitfK` |
| D7 | `parentId` = `1OgvJLK1…` | 62 files, one page. Not "7 PNGs": it holds 8 PNGs (AI-07..12, PRIM-a, IMG_0014.PNG) and 54 other files |
| D8 | `parentId` = `1lLlDMq8…` | 52 files. These are the same set with their original createdTimes (2025-02 → 2026-03), plus `Archive.zip` `1Dwx3LyeQ-gCL3nQ8UsNHMLkp3zjIINzY` (58,691,145 B; not opened) |
| D9 | `parentId` in the 3 later folders | 100 on page 1, all copies (" 2" suffixes) of the D7/D8 set, created 2026-09-01; not paged. Nothing seen under `137ClLaap…` |

Class of the non-AI files in the CLOSED LOOP folders (listed, not opened):
- COURT: 2024-01-12 Petition, Summons, UCCJEA, FL cover sheet, Order Share Financial Info; fl105; fl120; FL117 NAR; P's FL-115 (24.03.20).
- CONTRACT: Minor Prenuptial Agreement_OCR.
- CORRESPONDENCE / printouts: June_18_Demand_Letter.pdf; Demand for Immediate Financial Disclosure…; Google_Preservation_Emails_First4.pdf (`1PbG7XPTkYgqrZvGnORhHgSiqMOxjzEdW`, `1ge7ZfMOOFb079Qa396smGyx_yGHyhGOT`); Email_HalseyMinor_2022-12-07_pages97-98; Email_HalseyMinor_2023-07-05_page632; Exhibit2_HalseyMinor_2023-06-06; "The Plan - 2023.06.06" PDFs; IMessages PDF; URGENT- Follow-Up on Complaint re BHPD Case No. 2025-14983 PDF; IMG_0809.jpg.
- Class undetermined: "Email Evidence Theft HM2005.pdf" (`19tkPk0ti76u4dEzE9A-njUJIHR3I8gtp`, created 2025-03-28, 8,894,622 B). It may be an email printout and should be opened.
- Halsey's court filings that contain the phrases: Exhibits A-K-2 / RFO with exhibits. COURT as to what was filed. Contents not opened.

### Gmail (includeTrash)
| # | Query | Result |
|---|---|---|
| G1 | `("closed loop" OR "triangle of corruption")` | Estimated 406 threads; page 1 listed (50). Mostly AI/tech newsletters. Case threads on page 1 are all Halsey's outbound complaints/letters (Jan–Apr 2026) and replies |
| G2 | `"triangle of corruption"` | Estimated 83; page 1 (50) listed. Includes: Kalé `19ba02a9c00c3b61`; DA reply `19bc3db9c2a11195`; Halsey to FBI `19ba0331e15a53ff`; "Production 6: Google Gemini's Analysis of Lance Spiegel — In Its Own Words" `19d3fff4f6f07acf` (SP-0603 EV-066, full); firm thread "Minor - Motion to Strike" `19b9fffde8c412a1` |
| G3 | `"closed loop" (Spiegel OR Lance OR Kale OR Kalé OR ysfamilylaw OR Gemini) before:2026/03/01` | Estimated 40; earliest case hit is January 2026 |

## 2. AI documents — what was read
| Id | Drive id | Title (short) | Created | Bytes | Read |
|---|---|---|---|---|---|
| AI-01 | `1fKqVgsgYt_CSgRRLHb9kDANYNgcS1X3LZpPbB2PWVHM` | "You have identified that is clear that Alex kales ..." (Gemini answer text) | 2026-01-08 | 5,625 | FULL. Copies `1kSVGBfw7BXksrtt4rkw78v_-C-Oz_APB`, `1QWZ94AybFHjz3O39lK1YpistKEEokOGC`, `1whB7FnCm5Lpi1rVj55uN3t5BXdXBITkz` not opened. Register: absent |
| AI-02 | `1qQKPCJ9c4wVKEA6R4arnSKIR61gD8o5AfE-9lI6Be8c` | CONFIDENTIAL FORENSIC AUDIT & PUBLIC CORRUPTION REPORT (dated Jan 8, 2026) | 2026-01-08T17:31Z | 7,121 | FULL. Same family as tracker EV-088 (`1GUx4KFVuaE1OvXdMkBBRo4i53hcFPzFR`, SP-0445 metadata-only). Variants NOT opened: `1y8Bfu94SXxvs1wHJKOAv7mjDNuOSu_2sKFTsXdfAkSY` (19:02Z, 6,545 B); `1SRifsZ7wLFome3anXlEn9qT_eI1BSCEsMqK7neSN5Cw` (01-15, 7,849 B); 129,187-B PDFs; 10,874/11,451/221,549-B docx |
| AI-03 | `1ImkrCWkbavkJ8u2K48uK62WrUxI-2MKeuSPZ2txf3vc` | Gemini Export January 21, 2026 (file index) | 2026-01-21 | 1,808 | FULL. .xlsx copies not opened |
| AI-04 | `13A21iC1ltJN27HExxsNZIKJoXlZxZjvz186aomuyLKA` | Empirical Analysis of Evidence Spoliation | 2026-01-15 | 25,668 | FULL. docx `1XTQHD2x-_yP7GoghQg9Aj40rGVpYsshJ` not opened |
| AI-05 | `1nJjCAa6OIPyMTCzMvCaFU0nmvRNRJbA2BnJTQ0zmiR8` | Email History Analysis Request = "Forensic Analysis of Digital Correspondence: The Minor v. Kale Case File" (tracker EV-039) | 2026-01-18 | 16,628 | FULL as returned. Connector output ends inside works-cited item 7 |
| AI-06 | `1bz14R7V7FE6NnuzR1OipVR29aFpFyDvn` | GOOGLE GEMINI LEADING LANCES MOTION … 100 PERCENT MATCH PLUS HACKING OF EVIDENCE.pdf | 2026-01-22 | 10,579,923 | CONNECTOR OCR ONLY. Download refused (>10 MB), so page count is unverified. OCR = phone screenshots 7:39–7:42 of the AI-01 answer, chat titled "Police Complicity in Evidence Destructi…", plus Halsey's prompt asking for Gmail drafts. Same bytes as WP-007 `141G5x_ygVrXIn-sUss_C-RdUDTkyEbK1` (SP-0925 not-read) and SP-2090 (metadata-only) |
| AI-07 | `13tfj0UM7U8FWknj0_mGqoQUuentp2crp` | ChatGPT Image Feb 9, 2026 ("TIME TAX" service infographic) | 2026-03-24 | 2,693,603 | FULL (rendered) |
| AI-08 | `1qCT38u_a0zp8VqCBnp0qS6WkE5zrZuPE` | AFF2E834… PNG ("TIME TAX", portrait) | 2026-03-24 | 2,326,222 | FULL |
| AI-09 | `1YFiUbewIB3FrHMDdSNdkCWfUWldIkext` | 92CC15E6… PNG ("TIMELINE OF FALSE SERVICE") | 2026-03-24 | 1,618,017 | FULL |
| AI-10 | `1iDR5akJttD_1QvS-gIo-8avibQ_MEpip` | 0E78B074… PNG ("LEGAL COMPLIANCE VIOLATIONS BY PETITIONER'S COUNSEL") | 2026-03-24 | 1,221,682 | FULL |
| AI-11 | `1RdfKAJDaKFnjdzCF7gpTq9gjm-eRE37l` | 197CAD09… PNG ("JUDICIAL AUDIT: FALSE SERVICE") | 2026-03-24 | 629,051 | FULL |
| AI-12 | `1nm1KjUMHYtdpNVo8bNIGxSsyTyL-Fmec` | B7CC5BAB… PNG (same, v2) | 2026-03-24 | 613,927 | FULL |
| AI-13 | `1Udb-jOxNXhReaV26Xi0aXG4FqHGrJX3wPhyCJv5ykbY` | Gemini Export January 23, 2026 1:19:52 | 2026-01-23 | 140,901 | NOT read in full. Its opening concerns IP value creation. Drive `title contains 'Gemini Export' and fullText contains 'Spiegel'` returns 0, so it is out of scope |
| AI-14 | `1r0YvXSxYtso24qIpxXeEImFhd9TGVHzb` | Google Realization.jpg (Gemini screenshot, chat "Police Complicity in Evidence Destruction") | 2026-01-08 | 596,640 | FULL (rendered). Same text as AI-01. Other copies not opened |
| PRIM-a | `1G8diN74YtnKbFF4yHFtjhxUYFZUxIwNx` | "HELP First Hacking - halsey2005@gmail.com - Gmail.jpeg.png" | 2026-03-24 | 503,217 | FULL. NOT AI: a screenshot of Halsey's "HELP" emails to Google of 2024-10-18 and 2024-10-19. Class CORRESPONDENCE (screenshot). Copy `1HdjdmTxUZ8mXaSfx8xDoW8-9rIdJV3OI` |

Pointer-scanned only (identifiers and dates grepped, NOT read in full):
- PS-01: Lance Criminal Evidence.html `12n08LnO_rGlKFYAUacqWvK_HCfU238rQ` (SP-0886, metadata-only).
- PS-02: Criminal Complaint Lance Spiegel (1).html `1tuitpBMWJ4dnmcsEcqeCzyAwVgH3pbEE` (SP-2629).
- PS-03: "This document is a criminal complaint requesting an arrest warrant for Lance Spiegel…" `1qh66rDkZDWfqMdlvut65e0BsMRXe25FR` (9 pp; SP-2547).
- PS-04: "Unraveling Lance Spiegel's Fabricated Evidence Claims.pdf" `1AY9_esiWrokIsdLpn_GNyUw5sacPDwv5` (5 pp; SP-1141).
- PS-05: Forenisic Kale.pdf `16C0A3eXfbtM00A-i9GXtLG5s4RPe54kb` (35 pp, created 2026-01-20; register absent). It carries AI-05's text.

AI-LEAD, NOT opened (named for a next pass; none is evidence):
- Officer_Kale_Report_Footnoted_v2 family (EV-056).
- KALE REPORT TO VALIDATE.pdf `1xhhXdY8lu6pK5cYuoWuPn5xN-6TNXrox`.
- Halsey_Minor_Forensic_Dossier_Gemini.pdf `1x4jR8LzTJ8wVvzDab5i-YO25_CSAdtD1`.
- Gemini_Collusion_Diagram.jpg `11CQfuewDCKUv-GIETAMaVrsrt32iA706`.
- Gemini_Thinking_Screenshot_1–4: `1ACR8_wQcQUP3t4BpfJxAUWrM5swtpaz8`, `1CN3cUj4EIRRjZbaoYiueeYcSxo-5fqqH`, `198LdoE3Ht94Lc91Of61220Qy5yNcjRQr`, `1i50lItQi6NU_dsX9LaOavLD69oCMxn1Z`.
- Exhibit_7a/7b/7c Gemini: `1gpqQkAD7z9KPnLH_xv5ETL9nST7X4don`, `1R3_4MbwbTcWxrtL_62_7rF0h6feXZkTK`, `1YZqEI6kd1sWnx84WuyJm2tonSH-_X67h`.
- Gemini Content.docx `1eoLpOaCOy1t_uPHTNqpXgrFQC14gVs5U`.
- Gmail Analysis and Legal Research.docx `1ofPlhUnPWCdjpu9TE0qrJVaVmY9tGRBV`.
- Attorney Misconduct and Family Law Violations.docx `1mdv9WLSqfY1MsVjsK97BEhA0H2v5lUiY`.
- Forensic Audit of False Service Abuse.docx `14VNfstLrefAfpOq6A-EduUdIuxcCA_x0`.
- "Is that really the best you have for proof of a ha..." `1M2QYorGYAqaVZXne8aAbXZECcW-iW6fe-5F01qIKYGs` (2026-01-08; AI-04 source 3).
- Forensic Report Final `10VrZmwxcEsrHutojDTDKoahpB0-MJYg5VCMn5huEK8A`.
- Forensic Report `100lGC2LfVk6DlkoEE3BLYbxasZkxKZ6Aj8gbA4WV2DY`.
- Action Items.docx `1torrb2awvllSlXHbeYgfqvntV4di2Qfl` (2026-01-07).
- Notes by Gemini meeting notes.

## 3. LEADS table
Legend:
- E = exists (id given); NF = searched and not found; NL = not located in this pass (no search run that would find it); NH = not held.
- Read = register read_status, or "absent".
- Claims are AI assertions restated, not findings.

| C | Claim (one neutral line) | AI src | Cited / implied primary | Exists? id | Read? | Must show for the claim to be documented |
|---|---|---|---|---|---|---|
| C01 | Halsey gave Det. Kalé a confidential "Analysis of Evidence" naming 11/11/2022 emails (date left blank) | AI-01, 02, 06, 14 | The report as given to BHPD | E: `1VUG9LHh4yXNsdAQLQ3Cf4pTe7MKK0sKk` ("Sent To Police Analysis … 500 Emails an iMessages_Optimized_Timeline 2.pdf", created 2025-10-15, 24.5 MB); `1CtcVKanUdoc_ayjnKyu08pVyZTGhpYUt` (POLICE REPORT_Revised Analysis… "Updated with August 2025 Evidence", created 2025-08-29) | absent / absent | Which version reached BHPD, on what date; that it lists the 11/11/2022 email(s) |
| C02 | Only Halsey and BHPD held the report | AI-01, 04, 05 | — | — | — | Distribution record of the report (every recipient, including Halsey's own sends) |
| C03 | Right after the report reached Kalé the account was breached and only report-cited emails were deleted | AI-01, 02, 04, 05 | Google server-side records; the EV-079 comparison | NH (Google); E `1IUm-tR81jO1d788zlS80MbuBGxXm4eHp` (WORK-PRODUCT) | — / not-read | Deletion events with dates and sessions; list of report-cited emails vs. absent emails |
| C04 | Exhibit A, Shannon's 11/11/2022 "Yes! Large number has a 10 day hold" / "From the government!", is deleted | AI-02, 04 | Thread `18461348b9fe0954` | E: all 5 messages present. Labels: INBOX on Shannon msgs `18467dd2c7361b33`, `1846823e63d233ca`; SENT on Halsey msgs `18467dbd3ea6fa47`, `1846822a40fdff6d`. "From the government!" is Halsey's own reply. Subject is "Re: Wells Fargo deposit hold alert" | SP-0042/0044/0045 not-read | Absence at some date, and Google activity/restore records for this thread (tracker EV-088 DEFECT 1 already found it intact) |
| C05 | Same-day Shannon "Schedule for William basketball this weekend" and "Barclays info please" are intact (control group) | AI-02, 04, 05 | Two 2022-11-11 Shannon emails | NF. in:anywhere 2022-11-09..13: 0 hits. Shannon emails with Barclays/basketball subjects exist only 2012–2015 (`14f1850b7b7d1bf9`, `14f183a251cebd77`, `13862d07c58c0a94`, `1437a03ba555edb0`) | — | That these two emails exist, dated 2022-11-11 |
| C06 | The control record was the PDF given to BHPD, compared with "current server logs" | AI-02 | PDF given to BHPD; server logs | E (C01); NH (logs) | absent | A log export with source and date |
| C07 | 1-in-10-billion odds; ~116,000 emails; <10 (or ~5) emails cited in the report | AI-01, 02, 04 | Report's list of cited emails | E (C01) | absent | Exact list of report-cited emails; mailbox count at a date (tracker EV-088 DEFECT 2 on the model) |
| C08 | Spiegel filed a motion "simultaneously"/"immediately" after the deletion to suppress the 11/11/2022 email, seeking $250,000 | AI-01, 02, 04, 05, 06 | sec.271 FL-300 RFO filed 2025-12-30 (EV-108) + service email | E `1r_5T4D4v4lwSbCWU1ZpO--6S9y4nRunT`; E `19b70bba0694f1d9` (mvs@ysfamilylaw.com, "Minor - RFO for Family Code §271 Sanctions") | SP-0397 full; SP-0400 full | That the RFO names the 11/11/2022 email. Tracker EV-108 says it "contains NO list of Shannon emails". Dated record: 2025-07-28 erasure email → 2025-12-30 RFO |
| C09 | Spiegel knew the original was destroyed; only a leak could tell him | AI-01, 02, 04, 05 | — | — | — | A BHPD→firm/Shannon transmittal, or an earlier statement by Halsey to the firm (see C23) |
| C10 | Kalé refused/delayed preservation letters to Google | AI-01, 02, 04, 05 | Kalé 2026-01-09; 2026-01-12; City Records letter 10/9/2026 (tracker row 18) | E `19ba02a9c00c3b61`; E `19bb38cf19aec75b` | SP-0459 not-read; SP-0469 full | Dates of each request and each reply. Kalé (19bb38cf…) says a preservation request was submitted |
| C11 | Firm failed to give standard financial disclosures for ~20 months | AI-01 | Ask emails to firm; Financial_Disclosure_Requests_Index.pdf | E `1OSuascISNQGcqSWL-6Bg6uikw70EAoIp` (index, 2025-08-17, 4,641 B); asks read in ASKS_TO_FIRM_2024/2025_2026 notes | index absent; asks READ | Ask dates and the firm's responses (thread already has these) |
| C12 | Kalé failed to contact Google for a hold → "EVIDENCE DESTROYED PERMANENTLY" | AI-03 | IMG_0903.PNG.jpg | E `1Je7BbaxxX5DJS9tu8Bo8B07-u72imb8M` (2026-01-05, 719,152 B; content unknown) | absent | Whether it is a native record or a made graphic; Google's retention statement |
| C13 | The police report details forensic findings on email destruction | AI-03 | Sent To Police Analysis… | E `1VUG9LHh4yXNsdAQLQ3Cf4pTe7MKK0sKk` | absent | Version and date sent; its deletion section |
| C14 | A "reconstructed smoking gun" email and a statistical-proof report exist | AI-03 | Action Items.docx | E `1torrb2awvllSlXHbeYgfqvntV4di2Qfl` (WORK-PRODUCT/AI) | absent | Not a primary. The native email is C04 |
| C15 | Firm e-served without consent / broke service norms | AI-03 | Motion_to_Quash_Service_CA 2.pdf | NL `1NR6ON-aCIa4Lu7zY4d6euAGBnl74J3bx` (existence not checked) | absent | The firm's POS/e-service records (BEHAVIOR_c notes, read) |
| C16 | "Appearance of undue influence" (judicial concern) | AI-03 | Motion July 15.docx | NL `1l5ToqNDyfTKsnQVdD8JRsreUr_L5Kyov` (not checked) | absent | Halsey's motion as filed; any court ruling |
| C17 | 567-page report given to Kalé March 2025 (AI-05: 3/29/2025; AI-04: maybe Sept 2024) | AI-04, 05 | Transmittal email; Kalé 2025-09-29 email (report filed 3/24/2025, per tracker WP-019 #17) | NL | — | Transmittal date and attachment list |
| C18 | Kalé 2025-06-26: go through Snyder; warrants; "months" | AI-04, 05 | Kalé email 2025-06-26 | NL | — | Text and date |
| C19 | Kalé 2025-12-11: bank warrant served; Shannon interview supplement | AI-04, 05 | Kalé "Case Update" 2025-12-11; AI-04 cites "2025-12-20 11.11.52 copy.pdf" | NL (email); E `1vxZjIaJMMA70iSr7yNGL7rG6iSuVZnS7` (created 2026-01-04) | absent | Kalé's own words and date |
| C20 | Halsey asked >=4 times (Jan 5/8/9 2026) for a Google preservation | AI-04, 05 | Halsey→Kalé 2026-01-05..10, incl. "Fourth Formal Request" | E `19ba60583051da79` (thread `19ba5c6a7d242d18`); E `19b9f2782a3567fa` | SP-0464 not-read; SP-3164 metadata-only | Dates and recipients of each request |
| C21 | Kalé 2026-01-12 denied any scheme and said a preservation request was sent | AI-04, 05 | Kalé 2026-01-12 | E `19bb38cf19aec75b` | SP-0469 full | (documented as a statement) |
| C22 | Deletions matched the report's executive summary exactly | AI-04 | Report executive summary + absence list | E (C01) | absent | Item-by-item match |
| C23 | Halsey had not told opposing counsel about the hack before Spiegel's motion | AI-04 (also AI-05) | Halsey→firm emails Apr–Dec 2025 matching hack/deleted/erased/malware/removed | E: `1987804f00adef63` (2025-08-05, to lances@/annak@/mvs@/vivianh@ + jeff@jjfamilylaw.com, "…Improper Service and Outstanding Disclosure Obligatio…"); `196454d95c2edc21` (2025-04-17, cc lances@); `1978bb2792558e91` (2025-06-20 "Demand Lettter"); `19a0d98e359ce578` (2025-10-22 to annak@). Firm emails in the same hits: `1987c4fea2f6fa3d` (2025-08-05), `19881ad39b42a700` (2025-08-06) | SP-3107, 3034, 3092, 3129, 0294, 0297: all metadata-only | Whether any pre-12/30/2025 email to the firm mentions deleted emails or a hack. Search terms are broad; bodies not read |
| C24 | Spiegel's motion demanded the 11/11/2022 email "live from his computer", plus $250,000 | AI-04, 05; PS-02 | EV-108 RFO; any firm paper using "live"/"native .EML" | E (C08) | SP-0397 full | The words "live" or "native .EML" in a firm paper, with date |
| C25 | Intrusion date "late 2025, unspecified" (conflicts with AI-05 Aug 2025) | AI-04 | — | — | — | Any dated deletion record |
| C26 | Inquiry recommended into BHPD↔firm communications in "the week of the hack" | AI-04 | BHPD/firm communications | NH | — | Records held by BHPD/firm (lawful process only) |
| C27 | Kalé 2025-11-05: send the phone to BHPD | AI-04, 05 | Kalé email 2025-11-05 | NL | — | Text and date |
| C28 | 2024-03-29: Halsey reported a hack and asked BHPD to contact Google | AI-05; PS-01/02 | Halsey email 2024-03-29 | NF (tracker K-01: no 2024 preservation email) | — | The 2024 email |
| C29 | 2025-08-04: Halsey told Kalé he was hacked, with selective deletion of "hundreds" of Shannon emails, and sent screenshots | AI-05 | Halsey→Kalé 2025-08-04 | E `198773659236b416` (2025-08-04T22:31:46Z, "Computer Hacked 100's of Shannons Email PROVABLY removed.", labels SENT + Label_132, 701,135 B) | SP-0288 not-read | Its text and attachments: which emails it names as removed |
| C30 | 2025-08-22: Halsey forwarded the "Analysis of Evidence" to Kalé, saying it was surgically hacked | AI-05 | Halsey→Snyder+Kalé "Files" | E `198d2090543546b3` (2025-08-22T13:47Z; thread `198d1fc3831e042d`) | absent | Text and attachment |
| C31 | 2025-08-24: Halsey sent Kalé an AI report "from Google" about the deleted emails | AI-05 | Halsey→Kalé "Googles AI Ethics Appear to Trump BHPD In Bizarre Report." | E `198de625a75f975d` (2025-08-24T23:20Z) | absent | Its attachment. It would be the EARLIEST Gemini artefact (Aug 2025) |
| C32 | 2025-09-27: Halsey told Kalé the hacker deleted only emails given to BHPD ("ITS FAR WORSE…") | AI-05 | Halsey→Kalé 2025-09-27 | NL | — | Text and date |
| C33 | 2026-01-04: Halsey's "CRITICAL SECURITY BREACH" report says only report-cited emails were deleted | AI-05 | Halsey→Kalé/Dimond/city 2026-01-04 | E (by date and recipients; subject not retrieved) `19b884bc4c8df35c` (thread `19b8836c17e179c2`) | absent | Its text |
| C34 | 2026-01-05: Halsey's FORMAL NOTICE to Spiegel/firm + BHPD (criminal spoliation; preserve firm↔BHPD comms) | AI-05 | Halsey→lances@, vivianh@, annak@, keny@ysfamilylaw.co, jgordon@claritascapital.com; cc Kalé et al. | E `19b8f1dd4d7a670c` (2026-01-05T17:04Z) | SP-0433 (EV-054) metadata-only | Its text: the first dated notice to the firm of the deletion theory (if C23 finds nothing earlier) |
| C35 | 2026-01-05: Kalé sent a screenshot of 11/11/2022 emails and asked if these were the deleted ones | AI-05 | Kalé reply | E `19b8fbc478f4e54b` (2026-01-05T19:57Z) | SP-0435 full | (documented). Its screenshot shows what the live mailbox held on 2026-01-05 |
| C36 | 2026-01-08 (≈4:25 PM): Halsey wrote that the police report was the template for the hack and Spiegel's motion relied on it | AI-05 | Halsey→Kalé 2026-01-08/09 | NL (id not located; the 11:48 AM PST send is `19b9f2782a3567fa`) | — | Text and id |
| C37 | 2026-01-08 (≈7:48 PM): Halsey wrote that Spiegel knew the original was gone when he asked for it "live" | AI-05 | Halsey email + the firm paper with "live" | NL | — | Same as C24 |
| C38 | 2026-01-13 (≈6:17 PM): Halsey said charges were being filed against Spiegel via LAPD | AI-05 | Halsey→Kalé 2026-01-14T02:17Z; any LAPD report | E `19bba4c06df0c280` (by time); NL (LAPD record) | SP-0479 metadata-only | Text; an LAPD report number |
| C39 | Firm "false service" Jun 2025–Feb 2026: Aug exhibit list emailed without consent; Oct I&E, Nov non-service declaration, Dec deposition objections, Jan motion to strike, Feb vexatious-litigant RFO all mailed to Mexico | AI-07, 08, 09; PS-01/02 | Each paper's POS and envelope | E (BEHAVIOR_c_proofs_of_service.notes.md table rows 1–13, e.g. `19a84d3d95de6534`, `19b9fffde8c412a1`) | READ (thread notes) | Declared method/date vs. receipt. No POS was located for the 2/2/2026 RFO (BEHAVIOR_c #13) |
| C40 | Halsey warned the firm: Jun-25 "I am pro se in Mexico", Nov-25 "use Hague Convention", Jan-26 "cease false service" | AI-07, 08, 09 | Halsey→firm emails on those dates | NL | — | Dates and text |
| C41 | 0 valid services, 12 invalid filings, 11 ignored warnings | AI-11, 12 | The 12 POS + 11 warnings (no list given) | partly E (C39) | READ (C39 part) | A list matching each count |
| C42 | Spiegel personally responsible for 57% of counsel's violations; surge Oct–Nov 2025 | AI-10 | — (per-paper signer/server tally) | — | — | Signer/server on each paper (compare 63K A-21's different "92%") |
| C43 | Oct 2024: Halsey told Google his account had been taken over about 6 months earlier and emails deleted | PRIM-a (screenshot) | Halsey→public-data-abuse@google.com "HELP" | E thread `192a1a4d6cf67fe1`; msg `192a763c5ac77892` (2024-10-20T00:46Z = 10-19 19:46 UTC-5, matching the screenshot) | absent | (documented as his statement to Google). A Google reply, if any |
| C44 | The 8/4/2025 date is the day of the deletion ("scalpel executed") | PS-01, 02, 03 (also Halsey's 2/28/2026 complaint) | none cited | — | — | A dated deletion record. See §5 |
| C45 | Spiegel's sec.271 motion was dated 12/29/2025 ("Code Red"), demanded the 11/11/2022 email and native .EML files | PS-01, 02 | EV-108 + service email | E (C08) | full | Those demands in the RFO text. The filing date shown is 12/30/2025 |
| C46 | Between 3/29/2025 and 8/4/2025 Spiegel obtained the confidential 567-page report | PS-02 | — | — | — | Any transmittal or possession record |
| C47 | A keystroke-recording virus on Halsey's device was "documented by bank" and used to forge emails in his name | PS-01, 02, 03 | Bank (Ally) correspondence | E (thread read L1_ally-ecr-64504079 + ALLY_2026-09-04 notes) | READ (thread notes) | A bank statement naming malware/keylogging on his device; any link to the firm |
| C48 | A "terrible documents" email read in court on 1/10/2026 was forged | PS-02, 03, 04 | The email as read/filed; hearing record 1/10/2026 | NL (thread notes 63K A-07 and G1 carry it as account only) | — | The email (headers), the hearing record, and whether it is in Exhibit F |
| C49 | In 2025 Spiegel knew of Halsey's 3/29/2024 hack report and that Google held no preservation order | PS-01, 02 | — | — | — | Any communication showing that knowledge |

## 4. The "scalpel" / "template" claim — rundown
- Emails named as deleted:
  - AI-02 and AI-04 give one, with no message id: 2022-11-11 "Yes! Large number has a 10 day hold" / "From the government!", sender given as Shannon. Mailbox now: present, in thread `18461348b9fe0954`.
    - Shannon msg `18467dd2c7361b33` (2022-11-11T18:04:12Z, INBOX/IMPORTANT/CATEGORY_PERSONAL).
    - Halsey reply `1846822a40fdff6d` (19:20:11Z, SENT), whose body begins "From the government!".
    - Shannon `1846823e63d233ca` (19:21:15Z, INBOX).
    - Halsey forward `18467dbd3ea6fa47` (18:02:50Z, SENT).
    - Wells Fargo alert `18461348b9fe0954` (2022-11-10T11:02:23Z, INBOX).
  - AI-05 says only "hundreds of emails" and gives no list.
  - AI-04 / AI-07 say "<10" or "~5" report-cited emails, with no list.
  - 63K A-26 (Halsey, 5/06/26) speaks of "12 in the police report summary". This matches tracker EX-10's "12 verified absent" from the EV-079 series of 17 (WORK-PRODUCT `1IUm-tR81jO1d788zlS80MbuBGxXm4eHp`, unread).
- "Control" emails said to be intact (no ids given): "Schedule for William basketball this weekend", "Barclays info please" (2022-11-11). Mailbox now: NOT FOUND (in:anywhere, includeTrash, 2022-11-09..13 → 0). The only Shannon emails with those words date from 2012–2015.
- "Template" wording: AI-05 attributes it to Halsey's own email of 2026-01-08 (~4:25 PM PST). That id was not located in this pass. The AI-01 draft subject "URGENT: FINAL PRESERVATION DEMAND - Evidence Leak Confirmed" appears in Gmail as thread `19b9e2e602fb5f38` (started 2026-01-08T15:16Z). Kalé's reply `19b9f303920a4a1a` (19:58Z) is in that thread. Neither is in the register.

## 5. The 2025-08-04 date — what each AI document cites
- AI-01/02/03/06/14 give no date for the deletion.
- AI-04 gives "late 2025 (date unspecified)".
- AI-05, the earliest to name 8/4/2025, places on 8/4/2025 Halsey's REPORT to Kalé, not a deletion. It cites no record. The matching primary exists: `198773659236b416`, 2025-08-04T22:31:46Z, "Computer Hacked 100's of Shannons Email PROVABLY removed." (SP-0288, not-read).
- PS-04 likewise uses 8/4/2025 as the date of Halsey's "second request" to Kalé.
- Only PS-01/02/03 (March 2026) state 8/4/2025 as the deletion date, and they cite nothing. Halsey's 2/28/2026 complaint `19ca3c3b9151b03c` (G1 notes) does the same.
- Dated primaries around it:
  - 2025-07-28 `1984fd6ec53551c4` to Snyder, stating the emails "have now been erased" (EV-076, SP-0282 not-read). It is earlier than 8/4.
  - 2025-08-03 `198717bc1e84199f` to Snyder (SP-0284 not-read).
  - 2025-08-04 `198773659236b416` to Kalé.
- No document seen identifies 8/4/2025 as a deletion date at native level. This agrees with the tracker's EV-076 note.

## 6. Primary documents NOT yet read by this thread — next pass (deduped; priority order)
1. `198773659236b416`: Halsey→Kalé 2025-08-04 "Computer Hacked 100's of Shannons Email PROVABLY removed." (SP-0288 not-read). Source of the 8/4 date; may list the "removed" emails.
2. `1984fd6ec53551c4`: 2025-07-28 erasure email to Snyder (SP-0282 not-read).
3. `198717bc1e84199f`: 2025-08-03 to Snyder (SP-0284 not-read).
4. `19b8f1dd4d7a670c`: 2026-01-05 FORMAL NOTICE to Spiegel/firm + BHPD (SP-0433 metadata-only).
5. C23 set (all metadata-only): `1987804f00adef63` (2025-08-05), `196454d95c2edc21`, `1978bb2792558e91`, `19a0d98e359ce578`, `1987c4fea2f6fa3d`, `19881ad39b42a700`. They test whether the firm was told of the deletions before 12/30/2025.
6. `1VUG9LHh4yXNsdAQLQ3Cf4pTe7MKK0sKk` (Sent To Police Analysis… 24.5 MB) and `1CtcVKanUdoc_ayjnKyu08pVyZTGhpYUt` (POLICE REPORT_Revised…): the report's list of cited emails (absent from register).
7. `198de625a75f975d`: 2025-08-24 "Googles AI Ethics Appear to Trump BHPD In Bizarre Report." and its attachment (absent). Possible earliest AI artefact.
8. `198d2090543546b3` (2025-08-22 "Files") and `1989d4dc17b3d21e` (2025-08-12 "Help! 2025-14983"): both absent.
9. Thread `18461348b9fe0954` (SP-0042/0044/0045 not-read): headers of the "Exhibit A" email.
10. `19b884bc4c8df35c`: 2026-01-04 Halsey→Kalé/BHPD (absent).
11. `19b9e2e602fb5f38` + `19b9f303920a4a1a`: the Gemini-drafted "URGENT: FINAL PRESERVATION DEMAND" and Kalé's reply (absent).
12. `19ba02a9c00c3b61` (SP-0459 not-read; the ledger quotes it), `19ba60583051da79` (SP-0464), `19b9f2782a3567fa` (SP-3164), `19bb480c18e327b1` (SP-0472), `19bba4c06df0c280` (SP-0479).
13. `192a1a4d6cf67fe1`: 2024-10-18/19 "HELP" to public-data-abuse@google.com (absent).
14. `1Je7BbaxxX5DJS9tu8Bo8B07-u72imb8M` (IMG_0903), `1vxZjIaJMMA70iSr7yNGL7rG6iSuVZnS7` (2025-12-20 copy.pdf), `1OSuascISNQGcqSWL-6Bg6uikw70EAoIp` (index): all absent.
15. Work product, not primary: EV-079 `1IUm-tR81jO1d788zlS80MbuBGxXm4eHp` (SP-1410 not-read). Needed to reconcile the "12 absent".

Not located (searches owed):
- Kalé emails of 2025-06-26, 2025-09-29, 2025-11-05 and 2025-12-11.
- Halsey emails of 2025-09-27 and 2026-01-08 ~4:25 PM / ~7:48 PM PST.
- The March 2025 report transmittal.
- Halsey→firm warnings (Jun-25 / Nov-25 / Jan-26).
- The "terrible documents" email and the 1/10/2026 hearing record.
- Motion_to_Quash `1NR6ON-aCIa4Lu7zY4d6euAGBnl74J3bx` and Motion July 15 `1l5ToqNDyfTKsnQVdD8JRsreUr_L5Kyov` (existence not checked).
- An LAPD report number.

Counting basis for §0.

Exists (36):
- Report files: `1VUG9LHh…`, `1CtcVKan…`.
- Thread `18461348b9fe0954`.
- EV-108 `1r_5T4D4…`; firm service email `19b70bba…`.
- Kalé: `19ba02a9…`, `19bb38cf…`, `19bb480c…`, `19b8fbc4…`, `19b9f2ba…`, `19b9f303…`.
- Asks-to-firm set (C11); index `1OSuascI…`; IMG_0903 `1Je7Bbax…`; `1vxZjIaJ…`.
- Halsey: `19ba6058…`, `19b9f278…`.
- C23 set ×6.
- 2025 emails: `19877365…`, `198d2090…`, `198de625…`, `1989d4dc…`, `1984fd6e…`, `198717bc…`.
- 2026-01 Halsey: `19b884bc…`, `19b8f1dd…`, `19bba4c0…`, thread `19b9e2e6…`.
- Service set (C39); `192a1a4d…`; Ally set (C47).

Read (8): EV-108, `19b70bba…`, `19bb38cf…`, `19b8fbc4…`, `19b9f2ba…`, asks set, service set, Ally set.

Not located (14):
- Kalé 2025-06-26, 2025-09-29, 2025-11-05, 2025-12-11.
- The March 2025 transmittal.
- Halsey 2025-09-27, and 2026-01-08 ~4:25 PM and ~7:48 PM PST.
- Halsey→firm warnings.
- The "terrible documents" email; the 1/10/2026 hearing record.
- An LAPD report.
- Motion_to_Quash; Motion July 15.

Excluded as work product or AI: EV-079 `1IUm-tR8…`, Action Items `1torrb2a…`.

## 7. Claims with no primary identified
No primary at all (7):
- C02 (sole possession).
- C09 (Spiegel's knowledge via leak).
- C25 (late-2025 intrusion date).
- C42 (57% attribution).
- C44 (8/4/2025 as deletion date).
- C46 (Spiegel obtained the report 3/29–8/4/2025).
- C49 (Spiegel knew of the 2024 report and the lack of preservation).

Claim-elements with no primary, inside claims that do cite something (5):
- C07's statistic (no primary possible).
- C06's "server logs" (none exist in hand).
- C03's attribution of the breach to the report recipient (no record).
- C22's "exact match" (no list).
- C14's "reconstructed" email (a reconstruction is not a primary).

## 8. Limits
- D5, D6, D9 and G1 were not paged beyond page 1.
- AI-02 variants, AI-13, PS-01..05 and the AI-LEAD files listed in §2 were not read in full.
- AI-06 was read only through connector OCR.
- No AI text above is quoted or relied on; every factual line comes from Gmail/Drive metadata or the register.
