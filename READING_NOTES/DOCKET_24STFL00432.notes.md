# DOCKET 24STFL00432 — LASC register of actions (court printouts) — reading notes

- **Reader:** Opus subagent (claude-opus-5-5), 2026-11-01. Drive read-only (search_files / get_file_metadata / read_file_content / download_file_content only). Nothing on Drive or in the tracker was changed.
- **Class:** COURT (the court's own public case-access page, printed from a browser). **Not used:** Google Doc "Register of Actions — KEY DATES LOCKED (24STFL00432)" `1BPYr5canO7MruSeWbXdwX-D1zs2CU9Vhh9CbdQ6zB1c` (AI-LEAD work product; not opened).
- **Quotation rule:** entry text below is verbatim from the pdftotext `-layout` text layer, with the printout's line wraps joined by one space. Typos are the court's (e.g. "$62.876.00", "NO service dated listed", "Oﬀ"/"Off"). Filer is shown as the page shows it ("Filed by Petitioner" / "Filed by Respondent"); where the page prints "Filed by" with nothing after it, this file writes "(none shown)".
- **Document images:** the printouts have **no per-entry document-image link**. The only image reference is a case-level line on p.1: "Click here to access document images for this case." (link annotation → `https://www.lacourt.ca.gov/paos/v2web3/DocumentImages/SearchCaseNumber?casenumber=24STFL00432`) and "If this link fails, you may go to the Case Document Images site and search using the case number displayed on this page". Every other link in the PDF is an in-page section anchor (checked with pypdf). So for **every** entry below: document image referenced = **no** (case-level link only).

---

## 1. Sources read

| # | Drive ID | Title (as on Drive) | Drive created | Bytes | sha256 | Pages | Print date on pages | Read |
|---|---|---|---|---|---|---|---|---|
| A (primary) | `1_DDqsvDpbPrC5SeDSgX5DrCjAmNkEsDM` | Superior Court of Los Angeles County _ Family Law Case Access.pdf | 2026-06-01T19:45:12Z | 896,779 | a2777133b2101b334edfbb0ab0e72a420fed6bda322af8c689492be8dcbc247f | 27 | header on every page "6/1/26, 12:28 PM … LASC - Case Summary"; PDF CreationDate Mon Jun 1 19:28:49 2026 UTC; PDF Title "Superior Court of Los Angeles County \| Family Law Case Access" | **READ IN FULL** — all 1,269 text lines, pp.1–27 |
| B (later) | `14Jb4plwC-EiGSisWEz5-0G5MlwRgwFM1` "Register of Actions.pdf" (created 2026-09-01); byte-identical copies `1sjbl15BSEYSL62spyuMsxHftDQcPaTfu` "2026-07-13__gmail.com__Register of Actions.pdf" (created 2026-08-21) and `1McWgToq51bEEL9w8wVC_zFK0EBAvD-Q7` "Register Of Actions.pdf" (created 2026-08-14) | — | — | 907,832 | 4edee6df7b3ada18b129107874f3e5e4b9231306a03b11d7d41d0fd2f8a1088d (all three identical) | 27 | "7/13/26, 1:05 PM … LASC - Case Summary"; CreationDate Mon Jul 13 20:05:47 2026 UTC | **READ IN FULL by comparison**: whitespace-insensitive diff of the whole text (page furniture removed) against A, every differing line read. Differences = the 5 new entries + 2 party rows in §2.2, plus same-date entries printed in a different order in the "Register of Actions" list. No other text differs. |
| C | `1dyif2YxS1TKv3Cx5wql18k5YCPdTsIXi` (copies `17FS72fsZrTWBpxxXlOrIb_1wzRRlPRUJ`, `1kPdz46RjYa47ES98POCRIygREl3v4vwI`, same size 682,542) | Superior Court of Los Angeles County _ Family Law Case Access.pdf | 2026-01-02 | 682,542 | 86032fe34e879a0caf127d4bad6762d787d971f540f77695c91774098f431e4d | 16 | "1/2/26, 12:34 AM" | entries compared with B by script (date + first 4 words); party block, future hearings read. Not read line by line otherwise. Copies not hashed. |
| D | `1Iz3hQ28t9WR1Hv4LYvWaeu8UY1_r94oG` (same size as `1bZ_Fv0kuFLY5Pwc6FBakCbyX_kpswmfR`) | Superior Court of Los Angeles County \| Access a Case.pdf | 2026-09-01 (copy created 2026-02-09) | 173,904 | bc86458092bb99c62fc2042f17850fcdddff71be535ffcdbe71ee5cbfa5f7236 | 27 | footer "2/8/26, 12 41 AM"; CreationDate Sun Feb 8 05:41:47 2026 UTC | compared by script as for C; party block, future hearings read |
| E | `1TYSwE3W_MJQqqI-vRSWGf7rbHntCXoOS` (same size: `11hBJXJg_AGDXSd58OrKaHuv-VfRscJcj`, `1S4GAUVBg6ZmTgdKzVWra8d7WRXFYb5ja`, `1uYrlEzgcMgC0LRSf8saN1lMaXQ3if8cr`, `1kgIh6mxa7FgBIXpl6Xi01lcpSUQe4nwn` "2025-05-21__provinziano.com__…") | Register of actions minor (1).pdf | 2025-05-21 | 224,346 | 44bef4e09f73cc765ac6fb62e473623e41ed972460440757f580bcf59a55dffa | 11 | PDF Title "LASC - Case Access"; CreationDate Wed May 21 19:01:12 2025 UTC (no print-date header in text) | compared by script; case info, future hearings, party block, proceedings held read |
| F | `1ed4vTjCji-rAlLMeiJf50-hDv1w0bHU_` | 2024-07-24__jjfamilylaw.com__LASC - Case Access.pdf 7.24.24.pdf | 2026-08-24 | 124,776 | 3cee94e42bfccc797d3d17fe0b434e68037d39dcdb29d33564e8c6e4cac8df67 | 3 | CreationDate Wed Jul 24 15:24:45 2024 UTC | text layer is garbled (font encoding); **all 3 pages read as rendered images** |

Script comparison result: every entry (date + first four words) in C, D and E also appears in B. D's 22 "unmatched" keys were all Proceedings-Held lines laid out differently, not filings.

### 1.1 Searches run (Drive) and what came back
- `title contains 'Case Access'` → C (3 copies), D (2 copies), F, A, and `1DZJPwuz7WvYUqInyK2KYibVUEp3tpYF_` "2026-06-01__gmail.com__Superior Court of Los Angeles County _ Family Law Case Access.pdf" (896,779 B, same size as A; **not downloaded or hashed**).
- `title contains 'Register of Actions'` → B (3 copies), E (5 copies), and the AI-LEAD Google Doc (excluded).
- `title contains 'case summary'` → nothing.
- `title contains 'docket'` → only Google Docs "MINOR CASE — DOCKET ALERT 2026-10-xx" (analyses; ignored; 50 shown, more pages not listed).
- `fullText contains 'Register of Actions' and fullText contains '24STFL00432'` (PDF) and `fullText contains 'LASC - Case Summary'` (PDF) → the files above plus compiled bundles:
  - `14iazThcrgMA48l8bFVpwsd4I0yoMbiP3` "UPLOAD_TO_PROJECT_24STFL00432_2026-09-05.pdf" (37.6 MB; AI-LEAD transfer bundle, "PROJECT TRANSFER • SEPTEMBER 5, 2026"). Too large to download (>10 MB limit). Its Drive text rendering (302,389 chars) was searched, **not read in full**: the docket snapshot embedded in it carries the header "7/13/26, 1:05 PM / LASC - Case Summary", i.e. printout B. No page header with a later print date was found in it.
  - `1wRkMXYwhGIz8ww0s0nhF0T-kH5ujGBJM` "UPLOAD_ONCE_24STFL00432_PORTABLE_CASE_CAPSULE.pdf" (117 pp., LibreOffice, created 2026-08-31; AI-LEAD "Upload this single PDF … to a new ChatGPT Project"). Contains no "LASC - Case Summary" page. **Not read in full.**
- `fullText contains '24STFL00432' and fullText contains 'Documents Filed' and createdTime > '2026-07-13'` (PDF) → no other register printout.

**Result: no register printout dated after 7/13/2026 was found on Drive.** No register text covers August 2026, so nothing here covers the writs/levy period of August 2026.

---

## 2. Case information, parties, attorneys

### 2.1 Case information (A and B, identical)
"CASE INFORMATION: 24STFL00432 / Case Title: MINOR, SHANNON VS MINOR, HALSEY / Filing Courthouse: Stanley Mosk Courthouse / Filing Date: 1/16/2024 / Case Type: Dissolution w/ Minor Children (General Jurisdiction) / Status: Statistical Disposition on 10/23/2024". F (7/24/2024): "Status: Open 01/16/2024". E (5/21/2025): "Status: Statistical Disposition 10/23/2024".

### 2.2 Party information as each printout shows it (no dates, no firm names are printed in any printout)
| Printout | Party block verbatim |
|---|---|
| F 7/24/2024 | "MINOR HALSEY - Respondent" · "MINOR SHANNON - Petitioner" · "SPIEGEL LANCE STEPHEN - Attorney for Petitioner" |
| E 5/21/2025 | "MINOR HALSEY - Respondent" · "MINOR SHANNON - Petitioner" · "PROVINZIANO ALPHONSE FRANCIS - Attorney for Respondent for Respondent" · "SPIEGEL LANCE STEPHEN - Attorney for Petitioner" |
| C 1/2/2026 | "MINOR HALSEY Respondent" · "MINOR SHANNON Petitioner" · "SPIEGEL LANCE STEPHEN Attorney for Petitioner" |
| D 2/8/2026 | same three rows as C |
| A 6/1/2026 | same three rows as C |
| B 7/13/2026 | "AVALOS ORSON Depositor" · "MINOR HALSEY Respondent" · "MINOR HALSEY Appellant" · "MINOR SHANNON Petitioner" · "SPIEGEL LANCE STEPHEN Attorney for Petitioner" |

- The register never names a firm. The firm name "YOUNG, SPIEGEL & HOSP, LLP." appears on the FL-141 (see READING_NOTES/COURT_ORDERS_and_FL141.notes.md L41), not in the register.
- Individual docket entries never name an attorney; the filer is only "Petitioner" or "Respondent". In this file, "entries by the firm" = entries "Filed by Petitioner" while Spiegel is the only attorney listed for Petitioner in all six printouts.
- The register does not record who substituted in or out, or the dates any attorney joined or left; see §4.3 for the substitution and withdrawal entries.

### 2.3 Register date range
- Earliest entry: **1/16/2024** (Petition, Summons, UCCJEA, FAM-020, FAM 111).
- Latest entry in A: **5/27/2026** ("Proof of Service - Mail", Filed by Respondent). Latest in B: **7/7/2026**.
- Entries in "Documents Filed": A = 350; B = 355.

### 2.4 Entries after 2026-06-01 (only in B, printed 7/13/2026), verbatim
| Date | Entry text | Filer |
|---|---|---|
| 6/18/2026 | Appeal - Notice of Appeal/Cross Appeal Filed General Appeal | Respondent |
| 6/26/2026 | Appeal - Notice of Filing of Notice of Appeal | (none shown) |
| 7/7/2026 | Appeal - Notice of Default Issued for NOA filed 6/18/2026. DEFAULT FOR DESIGNATION. | Respondent |
| 7/7/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 7/7/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |

B's Register-of-Actions list shows these as "Clerk's Certificate - Proof of Electronic Service", "Responsive Declaration", "Appeal - Notice of Default Issued", "Appeal - Notice of Filing of Notice of Appeal", "Appeal - Notice of Appeal/Cross Appeal Filed". B shows **no** new Proceedings-Held rows after 5/12/2026. Its Future Hearings line is unchanged from A: "7/21/2026 8:30 Department 315 111 North Hill Street, Los Angeles, CA 90012 RFO - Family Law".

---

## 3. Hearings with results

### 3.1 "PROCEEDINGS HELD" (A; identical in B), verbatim, page order (newest first)
| Date / time | Dept | Proceeding | Result |
|---|---|---|---|
| 5/12/2026 1:30 PM | Department 315 | Ex Parte Hearing | Not Held - Court's Motion |
| 4/21/2026 1:30 PM | Department 23 | RFO - Compel Initial | Denied |
| 4/21/2026 1:30 PM | Department 23 | RFO - Family Law | Denied |
| 4/21/2026 1:30 PM | Department 23 | RFO - Family Law | Denied |
| 4/21/2026 1:30 PM | Department 23 | RFO - Quash | Denied |
| 4/21/2026 1:30 PM | Department 23 | RFO - Sanctions | Denied |
| 4/21/2026 1:30 PM | Department 23 | RFO - Sanctions | Denied |
| 3/4/2026 8:30 AM | Department 23 | Non-Appearance Case Review | Not Held - Court's Motion |
| 3/2/2026 8:30 AM | Department 23 | RFO - Quash | Held - Order Made |
| 3/2/2026 8:30 AM | Department 23 | RFO - Sanctions | Held - Continued |
| 2/11/2026 8:30 AM | Department 23 | Restraining Order Hearing | Denied - Without Prejudice |
| 2/11/2026 8:30 AM | Department 23 | Restraining Order Hearing | Denied - Without Prejudice |
| 2/9/2026 8:30 AM | Department 23 | RFOMOD - Child Support | Denied |
| 1/12/2026 8:30 AM | Department 23 | RFO - Family Law | Held - Order Made |
| 1/9/2026 1:30 PM | Department 23 | Ex Parte Hearing | Not Held - Court's Motion |
| 12/10/2025 8:30 AM | Department 23 | Restraining Order Hearing | Held - Continued |
| 12/10/2025 8:30 AM | Department 23 | Restraining Order Hearing | Held - Continued |
| 11/25/2025 8:30 AM | Department 22 | Restraining Order Hearing | Held - Continued |
| 11/19/2025 8:30 AM | Department 23 | Restraining Order Hearing | Held - Continued |
| 11/4/2025 8:30 AM | Department 23 | RFOMOD - Spousal Support | Denied |
| 10/29/2025 8:30 AM | Department 23 | Restraining Order Hearing | Held - Continued |
| 10/29/2025 1:30 PM | Department 23 | Ex Parte Hearing | Not Held - Court's Motion |
| 10/27/2025 8:30 AM | Department 23 | RFO - Family Law | Held - Order Made |
| 10/8/2025 8:30 AM | Department 23 | Restraining Order Hearing | Held - Continued |
| 9/17/2025 1:30 PM | Department 23 | Restraining Order Hearing | Dismissed - TRO-Lack of Prosecution |
| 8/28/2025 8:30 AM | Department 23 | Trial Setting Conference | Held - Trial Date Set |
| 8/28/2025 1:30 PM | Department 23 | Ex Parte Hearing | Not Held - Court's Motion |
| 8/27/2025 8:30 AM | Department 23 | Restraining Order Hearing | Held - Continued, TRO Reissued |
| 8/26/2025 1:30 PM | Department 23 | Ex Parte Hearing | Not Held - Court's Motion |
| 8/22/2025 1:30 PM | Department 23 | Ex Parte Hearing | Held - Order Made |
| 8/6/2025 8:30 AM | Department 23 | Restraining Order Hearing | Held - Continued, TRO Reissued |
| 7/16/2025 8:30 AM | Department 23 | Restraining Order Hearing | Held - Continued, TRO Reissued |
| 6/24/2025 8:30 AM | Department 23 | Motion Hearing | Denied |
| 6/24/2025 8:30 AM | Department 23 | Motion Hearing | Denied |
| 6/16/2025 8:30 AM | Department 23 | RFO - Compel Initial | Off Calendar - Moving Party |
| 6/5/2025 8:30 AM | Department 23 | RFO - Withdraw/Be Relieved as Counsel of Record | Granted |
| 6/5/2025 8:30 AM | Department 23 | Request for Order re: Modification Hearing | Held - Continued |
| 6/3/2025 1:30 PM | Department 23 | Ex Parte Hearing | Not Held - Court's Motion |
| 5/12/2025 8:30 AM | Department 23 | Request for Order re: Modification Hearing | Held - Order Made |
| 10/7/2024 8:30 AM | Department 23 | RFO - Custody, Visitation, Child and Spousal Support | Dismissed - TRO-Lack of Prosecution |

- E (5/21/2025) adds the judge: "05/12/2025 at 8:30 AM in Department 23, White, Ryan D., Presiding / Request for Order re: Modification Hearing - Held - Order Made" and "10/07/2024 at 8:30 AM in Department 23, White, Ryan D., Presiding / RFO - Custody, Visitation, Child and Spousal Support - Dismissed - TRO-Lack of Prosecution".
- C (1/2/2026) prints every past-proceeding time as "12:00 AM" (e.g. "6/5/2025 12:00 AM").

### 3.2 Future hearings as each printout showed them (verbatim, condensed)
- F 7/24/2024: "None".
- E 5/21/2025: "06/05/2025 at 8:30 AM in Department 2 … Request for Order re: Modification Hearing" (×2); "06/16/2025 … Department 23 … RFO - Compel Initial"; "06/24/2025 … Department 23 … Motion Hearing" (×2).
- C 1/2/2026: 1/12/2026 RFO - Family Law; 2/9/2026 RFOMOD - Child Support; 2/11/2026 Restraining Order Hearing (×2); 3/2/2026 RFO - Quash; 3/2/2026 RFO - Sanctions (all "8:30 Department 23").
- D 2/8/2026: 2/9/2026 RFOMOD - Child Support; 2/11/2026 Restraining Order Hearing (×2); 3/2/2026 RFO - Quash; 3/2/2026 RFO - Sanctions; 3/9/2026 RFO - Compel Initial; 3/9/2026 RFO - Family Law; 3/9/2026 RFO - Quash; 3/24/2026 RFO - Sanctions; 4/20/2026 RFO - Family Law (all 8:30, Department 23).
- A 6/1/2026 and B 7/13/2026: "7/21/2026 8:30 Department 315 111 North Hill Street, Los Angeles, CA 90012 RFO - Family Law".

---

## 4. Filtered transcriptions (verbatim; ascending date; within one date, printout order). Source = B "Documents Filed"; entries before 6/1/2026 are identical in A. Doc image referenced = no, for every row (see header).

### 4.1 Proofs of service / declarations re service / clerk's certificates / declarations of due diligence (77 entries)
Selected by the words Proof of Service, Proof of Electronic Service, Declaration - Service, Declaration of Due Diligence. The register shows no entry titled POS-010/020/030/040/050, FL-330 or FL-335 by form number. 11/12/2025 "Proof of Service DV-200" (Respondent) is included.

| Date | Entry text (verbatim) | Filer as shown |
|---|---|---|
| 3/14/2024 | Notice - Status Conference Review: Proof of Service Noticed by LASC | (none shown) |
| 3/20/2024 | Proof of Service of Summons via Email; NO service dated listed; NOAR filed 03/08/2024 | Petitioner |
| 6/18/2024 | Declaration - Service of Preliminary Dec. of Disclosure Declaration - Service of Preliminary Dec. of Disclosure (Declarations) | Petitioner |
| 7/1/2024 | Proof of Service Proof of Service | Respondent |
| 7/1/2024 | Proof of Service Proof of Service | Respondent |
| 7/1/2024 | Proof of Service Proof of Service | Respondent |
| 7/1/2024 | Proof of Service Proof of Service | Respondent |
| 8/15/2024 | Proof of Service Proof of Service (Comment) | Petitioner |
| 8/22/2024 | Declaration - Service of Preliminary Dec. of Disclosure Declaration - Service of Preliminary Dec. of Disclosure (Declarations) | Respondent |
| 1/8/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 1/14/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 2/19/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 3/13/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 3/19/2025 | Proof of Service Proof of Service (Comment) | Respondent |
| 4/25/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 5/6/2025 | Proof of Service Proof of Service (Comment) | Respondent |
| 5/9/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 6/3/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 6/3/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 6/4/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent |
| 6/4/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent |
| 6/4/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent |
| 6/4/2025 | Proof of Service Proof of electronic Service (Comment) | Respondent |
| 6/5/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent |
| 6/25/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner |
| 8/6/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 8/7/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 8/7/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner |
| 8/7/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner |
| 8/21/2025 | Proof of Service Personal | Respondent |
| 8/25/2025 | Proof of Service Electronic | Respondent |
| 8/26/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 8/26/2025 | Proof of Service | Respondent |
| 8/26/2025 | Proof of Service | Respondent |
| 8/28/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 8/28/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 9/17/2025 | Proof of Service Electronic | Respondent |
| 9/17/2025 | Proof of Service - Mail | Respondent |
| 9/22/2025 | Proof of Service Electronic | Respondent |
| 9/22/2025 | Proof of Service - Mail | Respondent |
| 10/7/2025 | Declaration of Due Diligence | Respondent |
| 10/7/2025 | Proof of Service | Respondent |
| 10/27/2025 | Declaration of Due Diligence | Respondent |
| 10/29/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 11/12/2025 | Proof of Service DV-200 | Respondent |
| 11/17/2025 | Proof of Service Electronic | Respondent |
| 11/17/2025 | Proof of Service Electronic - RFO 1-12-2026 | Respondent |
| 11/17/2025 | Proof of Service Proof of Service (Comment) | Petitioner |
| 11/17/2025 | Proof of Service - Mail | Respondent |
| 11/17/2025 | Proof of Service - Mail RFO 1-12-2026 | Respondent |
| 12/8/2025 | Proof of Service Electronic | Respondent |
| 12/8/2025 | Proof of Service - Mail | Respondent |
| 1/6/2026 | Proof of Service Electronic | Respondent |
| 1/6/2026 | Proof of Service Electronic | Respondent |
| 1/6/2026 | Proof of Service Electronic | Respondent |
| 1/6/2026 | Proof of Service - Mail | Respondent |
| 1/6/2026 | Proof of Service - Mail | Respondent |
| 1/6/2026 | Proof of Service - Mail | Respondent |
| 1/9/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 1/22/2026 | Proof of Service | Respondent |
| 1/22/2026 | Proof of Service - Mail | Respondent |
| 1/27/2026 | Proof of Service Proof of Service (Comment) | Petitioner |
| 1/27/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner |
| 2/5/2026 | Declaration of Due Diligence | Respondent |
| 2/18/2026 | Proof of Service Electronic | Respondent |
| 2/18/2026 | Proof of Service - Mail | Respondent |
| 3/2/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 3/4/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 3/27/2026 | Proof of Service Electronic | Respondent |
| 3/27/2026 | Proof of Service - Mail | Respondent |
| 4/20/2026 | Proof of Service Proof of Service (Comment) | Petitioner |
| 4/20/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner |
| 5/12/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 5/12/2026 | Proof of Service Proof of Electronic Service (Comment) | Petitioner |
| 5/12/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner |
| 5/27/2026 | Proof of Service - Mail | Respondent |
| 7/7/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |

### 4.2 Declarations of disclosure / income and expense / financial statements (25 entries)
Selected by Disclosure, Income and Expense, Statement - Financial. The register shows no entry titled FL-140, FL-142, FL-144 or FL-160 by form number. The 8/22/2024 "Stipulation - Waiver of Final Declaration of Disclosure" is the FL-144 per COURT_ORDERS_and_FL141.notes.md L47 (that is a pointer, not register text).

| Date | Entry text (verbatim) | Filer as shown |
|---|---|---|
| 6/18/2024 | Declaration - Service of Preliminary Dec. of Disclosure Declaration - Service of Preliminary Dec. of Disclosure (Declarations) | Petitioner |
| 7/15/2024 | Statement - Financial Statement - Financial | Petitioner |
| 7/15/2024 | Statement - Financial Statement - Financial | Petitioner |
| 7/15/2024 | Statement - Financial Statement financial | Petitioner |
| 7/18/2024 | Statement - Financial Response - Dissolution, Nullity, Legal Separation | Petitioner |
| 7/18/2024 | Statement - Financial Statement - Financial | Petitioner |
| 7/18/2024 | Statement - Financial Statement - Financial | Petitioner |
| 7/18/2024 | Statement - Financial Statement - Financial | Petitioner |
| 7/18/2024 | Statement - Financial Statement - Financial | Petitioner |
| 7/18/2024 | Statement - Financial Statement - Financial | Petitioner |
| 7/18/2024 | Statement - Financial Statement - Financial | Petitioner |
| 7/18/2024 | Statement - Financial Statement - Financial | Petitioner |
| 8/14/2024 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner |
| 8/22/2024 | Declaration - Service of Preliminary Dec. of Disclosure Declaration - Service of Preliminary Dec. of Disclosure (Declarations) | Respondent |
| 8/22/2024 | Stipulation - Waiver of Final Declaration of Disclosure Stipulation - Waiver of Final Declaration of Disclosure (Declarations) | Petitioner |
| 1/8/2025 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner |
| 4/18/2025 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner |
| 4/29/2025 | Declaration - Income and Expense Declaration - Income and Expense (respondent) | Respondent |
| 8/7/2025 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner |
| 8/26/2025 | Declaration - Income and Expense | Respondent |
| 10/22/2025 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner |
| 12/5/2025 | Declaration - Income and Expense | Respondent |
| 1/5/2026 | RFO/MTN - Compel Initial Other: Compel Preliminary/Final Declarations of Disclosure; Monetary Sanctions - See #7 | Respondent |
| 1/27/2026 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner |
| 2/23/2026 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner |

### 4.3 Substitutions of attorney / appearance / withdrawal (7 entries)
No entry titled "Notice of Appearance" or "Association" exists. Not listed above: remote-appearance notices "Notice - Remote Appearance - RA 010" (5/9/2025 Petitioner and Respondent; 8/21/2025 Respondent) and the RA 020 orders (5/9/2025 and 8/21/2025 proposed by Respondent; 5/12/2025 and 8/28/2025 orders). The register names no attorney on any substitution entry. Outcome of the 6/2/2025 withdrawal RFO: 6/5/2025 "RFO - Withdraw/Be Relieved as Counsel of Record — Granted" (§3.1).

| Date | Entry text (verbatim) | Filer as shown |
|---|---|---|
| 3/8/2024 | Notice - Acknowledgment of Receipt of Summons & Petition | Petitioner |
| 8/22/2024 | Appearance, Stipulations and Waivers Appearance, Stipulations and Waivers (Appearances) | Petitioner |
| 10/18/2024 | Substitution of Attorney | Respondent |
| 10/28/2024 | Substitution of Attorney Substitution of Attorney | Respondent |
| 1/21/2025 | Substitution of Attorney Substitution of Attorney (Comment) | Respondent |
| 6/2/2025 | Declaration Declaration in Support of Attorney's Motion to be relieved as Counsel (Declarations) | Respondent |
| 6/2/2025 | RFO/MTN - Withdraw/Be Relieved as Counsel of Record | Respondent |

### 4.4 Requests for order and related papers (RFOs, ex parte RFOs, FAM 119/120, continuances, reissuance, off-calendar notices, responsive declarations, replies, motions) (113 entries)
Hearing dates and outcomes come only from §3.1 / §3.2. The register does not link a hearing row to a filing row.

| Date | Entry text (verbatim) | Filer as shown |
|---|---|---|
| 8/14/2024 | RFO/MTN - Custody, Visitation, Child and Spousal Support Other: Attachment 8 | Petitioner |
| 1/8/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 1/8/2025 | RFO/MTN - Modification | Petitioner |
| 1/27/2025 | Proposed Order - Reschedule/ Reissuance of RFO (Agreement) | Respondent |
| 1/29/2025 | Application and Order - Reissuance of RFO | (none shown) |
| 2/10/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 2/10/2025 | RFO/MTN - Compel Initial Motion to Compel Deposition Notice and Production of Documents | Petitioner |
| 3/13/2025 | Proposed Order - Reschedule/ Reissuance of RFO | Petitioner |
| 3/13/2025 | Request - Continue Hearing | Petitioner |
| 3/14/2025 | Notice - New Hearing and Order on Reissuance of RFO | (none shown) |
| 3/17/2025 | Responsive Declaration Responsive Declaration (Declarations) | Respondent |
| 4/29/2025 | Responsive Declaration Responsive Declaration to RFO | Respondent |
| 5/5/2025 | Motion RESPONDENTS MOTION TO STRIKE PETITIONERS NOTICE OF LODGING AND OR/OBJECTION TO THE LODGING OF THE DEPOSITION TRANSCRIPT OF RESPONDENT (Motions) | Respondent |
| 5/5/2025 | Motion RESPONDENTS MOTION TO STRIKE PETITIONERS UNTIMELY FILED 04- 25-25 FURTHER SUPPLEMENTAL DECLARATION (Motions) | Respondent |
| 5/5/2025 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner |
| 5/5/2025 | Reply Reply (Comment) | Petitioner |
| 5/7/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent |
| 5/7/2025 | Request - Continue Hearing | Respondent |
| 5/7/2025 | Responsive Declaration | Petitioner |
| 5/7/2025 | Responsive Declaration | Petitioner |
| 5/30/2025 | Notice Notice of Taking Hearing Off Calendar | Petitioner |
| 6/2/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 6/2/2025 | RFO/MTN - Withdraw/Be Relieved as Counsel of Record | Respondent |
| 6/3/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent |
| 6/3/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) |
| 6/3/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent |
| 6/3/2025 | Responsive Declaration Responsive Declaration to Ex Parte (Declarations) | Petitioner |
| 6/4/2025 | Notice - Hearing Notice - Hearing (Notices) | Respondent |
| 6/5/2025 | Order Briefing Schedule Order | (none shown) |
| 6/24/2025 | Declaration - Ex Parte Notice (Notice Given) Declaration - Ex Parte Notice (Notice Given) (Declarations) | Petitioner |
| 7/14/2025 | Proposed Form 116 - Reissuance TRO | Respondent |
| 7/14/2025 | Request to Continue and Reissue TRO (Form 115) | Respondent |
| 7/16/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | (none shown) |
| 8/6/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Petitioner |
| 8/21/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent |
| 8/21/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent |
| 8/22/2025 | Responsive Declaration Exparte | Petitioner |
| 8/25/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent |
| 8/25/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) |
| 8/25/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent |
| 8/25/2025 | Reply | Respondent |
| 8/26/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent |
| 8/26/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) |
| 8/26/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent |
| 8/26/2025 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |
| 8/27/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Petitioner |
| 8/28/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) |
| 8/28/2025 | Order Briefing Schedule Order | (none shown) |
| 8/28/2025 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |
| 9/8/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 9/8/2025 | RFO/MTN - Family Law | Respondent |
| 9/17/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 9/17/2025 | RFO/MTN - Mod - Spousal Support | Respondent |
| 10/8/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Respondent |
| 10/14/2025 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |
| 10/20/2025 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner |
| 10/22/2025 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |
| 10/27/2025 | Notice - Ruling Notice - Ruling (Notices) | Petitioner |
| 10/28/2025 | Declaration - Ex Parte Notice (Notice Given) | Petitioner |
| 10/28/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Petitioner |
| 10/29/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) |
| 10/29/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Respondent |
| 10/29/2025 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner |
| 11/12/2025 | RFO/MTN - Family Law | Respondent |
| 11/13/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 11/13/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 11/17/2025 | Proof of Service Electronic - RFO 1-12-2026 | Respondent |
| 11/17/2025 | Proof of Service - Mail RFO 1-12-2026 | Respondent |
| 11/19/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Respondent |
| 11/25/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Petitioner |
| 12/5/2025 | RFO/MTN - Mod - Child Support | Respondent |
| 12/10/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Petitioner |
| 12/10/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Respondent |
| 12/29/2025 | RFO/MTN - Quash | Petitioner |
| 12/29/2025 | Responsive Declaration | Petitioner |
| 12/30/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 12/30/2025 | RFO/MTN - Sanctions Attorney Fees | Petitioner |
| 1/5/2026 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 1/5/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 | Petitioner |
| 1/5/2026 | RFO/MTN - Compel Initial Other: Compel Preliminary/Final Declarations of Disclosure; Monetary Sanctions - See #7 | Respondent |
| 1/5/2026 | RFO/MTN - Family Law Other: Objection to Defective Service and Request for Continuance or to Take Matter Off Calendar | Respondent |
| 1/5/2026 | RFO/MTN - Quash Other: Motion to Quash; Protective Order and Sanctions - See #7 | Respondent |
| 1/9/2026 | Declaration - Ex Parte Notice (Notice Given) | Respondent |
| 1/9/2026 | Ex Parte RFO Emergency Orders for Support | (none shown) |
| 1/9/2026 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent |
| 1/21/2026 | Notice Notice of Taking Hearing Off-Calendar | Petitioner |
| 1/22/2026 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 1/22/2026 | RFO/MTN - Sanctions | Respondent |
| 1/27/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |
| 2/2/2026 | Proposed Order - Vexatious Litigant - Motion/RFO/Other | Petitioner |
| 2/2/2026 | RFO/MTN - Family Law | Petitioner |
| 2/2/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |
| 2/2/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |
| 2/3/2026 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 2/18/2026 | Responsive Declaration | Respondent |
| 2/23/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner |
| 2/23/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner |
| 2/23/2026 | Reply Reply (Comment) | Petitioner |
| 2/24/2026 | Responsive Declaration Responsive Declaration - MTC.FDD (Declarations) | Petitioner |
| 2/24/2026 | Responsive Declaration Responsive Declaration - MTQ (Declarations) | Petitioner |
| 2/24/2026 | Responsive Declaration Responsive Declaration - Obj.Def.Serv (Declarations) | Petitioner |
| 3/2/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 | Petitioner |
| 3/2/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 - MTC.FDD (Judgments) | Petitioner |
| 3/2/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 - Obj.Def.Serv (Judgments) | Petitioner |
| 4/8/2026 | Responsive Declaration | Petitioner |
| 4/14/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner |
| 4/15/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner |
| 5/11/2026 | Declaration - Ex Parte Notice (Notice Given) | Respondent |
| 5/11/2026 | Proposed Ex Parte RFO Emergency Orders for Other | Respondent |
| 5/12/2026 | Ex Parte RFO Emergency Orders for Other | (none shown) |
| 5/13/2026 | RFO/MTN - Family Law | Respondent |
| 5/14/2026 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) |
| 7/7/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner |

### 4.5 Minute orders (44 entries)
Filer is blank for every minute order. Minute-order content is not in the register.

| Date | Entry text (verbatim) | Filer as shown |
|---|---|---|
| 10/7/2024 | Minute Order | (none shown) |
| 5/12/2025 | Minute Order | (none shown) |
| 6/3/2025 | Minute Order | (none shown) |
| 6/5/2025 | Minute Order | (none shown) |
| 6/5/2025 | Minute Order | (none shown) |
| 6/5/2025 | Minute Order as Order After Hearing | (none shown) |
| 6/16/2025 | Minute Order | (none shown) |
| 6/24/2025 | Minute Order | (none shown) |
| 6/24/2025 | Minute Order | (none shown) |
| 7/16/2025 | Minute Order | (none shown) |
| 8/6/2025 | Minute Order | (none shown) |
| 8/22/2025 | Minute Order | (none shown) |
| 8/26/2025 | Minute Order | (none shown) |
| 8/27/2025 | Minute Order | (none shown) |
| 8/28/2025 | Minute Order | (none shown) |
| 8/28/2025 | Minute Order | (none shown) |
| 9/17/2025 | Minute Order | (none shown) |
| 10/8/2025 | Minute Order | (none shown) |
| 10/27/2025 | Minute Order | (none shown) |
| 10/29/2025 | Minute Order | (none shown) |
| 10/29/2025 | Minute Order | (none shown) |
| 11/4/2025 | Minute Order | (none shown) |
| 11/19/2025 | Minute Order | (none shown) |
| 11/25/2025 | Minute Order | (none shown) |
| 12/10/2025 | Minute Order | (none shown) |
| 12/10/2025 | Minute Order | (none shown) |
| 1/9/2026 | Minute Order | (none shown) |
| 1/12/2026 | Minute Order | (none shown) |
| 2/9/2026 | Minute Order | (none shown) |
| 2/11/2026 | Minute Order | (none shown) |
| 2/11/2026 | Minute Order | (none shown) |
| 3/2/2026 | Minute Order | (none shown) |
| 3/2/2026 | Minute Order | (none shown) |
| 3/4/2026 | Minute Order | (none shown) |
| 4/21/2026 | Minute Order | (none shown) |
| 4/21/2026 | Minute Order | (none shown) |
| 4/21/2026 | Minute Order | (none shown) |
| 4/21/2026 | Minute Order | (none shown) |
| 4/21/2026 | Minute Order | (none shown) |
| 4/21/2026 | Minute Order | (none shown) |
| 4/21/2026 | Minute Order as Order After Hearing | (none shown) |
| 4/21/2026 | Minute Order as Order After Hearing | (none shown) |
| 4/21/2026 | Minute Order as Order After Hearing | (none shown) |
| 5/12/2026 | Minute Order | (none shown) |

### 4.6 Writs / abstracts / earnings assignments / levies (6 entries)
The register (through 7/13/2026) contains **no** entry for an abstract of judgment, earnings assignment, levy, notice of levy, or writ return. Only the six 4/28/2026 entries below. The amounts are as printed ("$62.876.00").

| Date | Entry text (verbatim) | Filer as shown |
|---|---|---|
| 4/28/2026 | Application - Issue Writ E/P/S Los Angeles - $11,000.00 Attorney's Fees based on Order 5/12/2025 | Petitioner |
| 4/28/2026 | Application - Issue Writ E/P/S Los Angeles - $21,857.00 Spousal Support based on Order 5/12/2025 | Petitioner |
| 4/28/2026 | Application - Issue Writ E/P/S Los Angeles - $62.876.00 Child Support based on Order 5/12/2025 | Petitioner |
| 4/28/2026 | Writ - Execution Los Angeles - $11,000.00 Attorney's Fees based on Order 5/12/2025 - Issued 4/28/2026 | Petitioner |
| 4/28/2026 | Writ - Execution Los Angeles - $21,857.00 Spousal Support based on Order 5/12/2025 - Issued 4/28/2026 | Petitioner |
| 4/28/2026 | Writ - Execution Los Angeles - $62.876.00 Child Support based on Order 5/12/2025 - Issued 4/28/2026 | Petitioner |

### 4.7 Sanctions (4 entries)
Hearing results (§3.1): 3/2/2026 "RFO - Sanctions — Held - Continued"; 4/21/2026 "RFO - Sanctions — Denied" (×2); 4/21/2026 "RFO - Compel Initial — Denied"; 4/21/2026 "RFO - Quash — Denied". The register does not say which sanctions RFO each hearing row belongs to. Related text elsewhere: 5/5/2025 "Motion RESPONDENTS MOTION TO STRIKE …" entries (§4.4).

| Date | Entry text (verbatim) | Filer as shown |
|---|---|---|
| 12/30/2025 | RFO/MTN - Sanctions Attorney Fees | Petitioner |
| 1/5/2026 | RFO/MTN - Compel Initial Other: Compel Preliminary/Final Declarations of Disclosure; Monetary Sanctions - See #7 | Respondent |
| 1/5/2026 | RFO/MTN - Quash Other: Motion to Quash; Protective Order and Sanctions - See #7 | Respondent |
| 1/22/2026 | RFO/MTN - Sanctions | Respondent |

### 4.8 Appeal (B only) (3 entries)


| Date | Entry text (verbatim) | Filer as shown |
|---|---|---|
| 6/18/2026 | Appeal - Notice of Appeal/Cross Appeal Filed General Appeal | Respondent |
| 6/26/2026 | Appeal - Notice of Filing of Notice of Appeal | (none shown) |
| 7/7/2026 | Appeal - Notice of Default Issued for NOA filed 6/18/2026. DEFAULT FOR DESIGNATION. | Respondent |


---

## 5. Service entries by the firm ("Filed by Petitioner"): 22 entries

Method column = only the words the docket text itself contains. "Paper" = the docket text names no paper served unless shown. Column "Other Petitioner entries, same date or up to 7 days before" lists register entries only; **the register does not link any POS to any paper.**

| # | Date | Docket text (verbatim) | Method stated in docket text | Other Petitioner entries, same date or ≤7 days before (register only) | Matching POS already read (READING_NOTES) | Not stated in the docket |
|---|---|---|---|---|---|---|
| 1 | 3/20/2024 | Proof of Service of Summons via Email; NO service dated listed; NOAR filed 03/08/2024 | "via Email" | none (3/8/2024 "Notice - Acknowledgment of Receipt of Summons & Petition" is 12 days before) | SERVICE_VIOLATIONS_LOG.notes.md, table row "Main 1" (that file says the POS image is not in the corpus) | declarant; email address; date of service ("NO service dated listed") |
| 2 | 6/18/2024 | Declaration - Service of Preliminary Dec. of Disclosure Declaration - Service of Preliminary Dec. of Disclosure (Declarations) | none | none | FL-141, Drive `1HPyFn_0OHf_GFe105uSgvNLUeMebgd8B`: COURT_ORDERS_and_FL141.notes.md L40–45 ("X Other (specify): Email: halsey@minorventures.com on (date): June 18, 2024"; declarant "Anna Kralle"); SERVICE_VIOLATIONS_LOG.notes.md "Main 2" | method; recipient/address; declarant; documents served |
| 3 | 8/15/2024 | Proof of Service Proof of Service (Comment) | none | 8/14/2024 RFO/MTN - Custody, Visitation, Child and Spousal Support Other: Attachment 8; 8/14/2024 Declaration - Income and Expense | none found | paper; method; recipient/address; declarant; service date |
| 4 | 1/8/2025 | Proof of Service Proof of Service (Comment) | none | 1/8/2025 RFO/MTN - Modification; 1/8/2025 Declaration Declaration re Address Verification (Declarations); 1/8/2025 Declaration - Income and Expense | SERVICE_VIOLATIONS_LOG.notes.md row "C4" (no POS in the corpus copy of the RFO; docket line only) | all of the above |
| 5 | 1/14/2025 | Proof of Service Proof of Service (Comment) | none | the three 1/8/2025 entries above | none found | all |
| 6 | 2/19/2025 | Proof of Service Proof of Service (Comment) | none | none | none found (the 2/24/2025 FL-142 POS on Provinziano's office in BEHAVIOR_b_e_primary.notes.md L138 / SVL "Main 3" has **no** docket entry; the register has no entry dated 2/24/2025) | all |
| 7 | 3/13/2025 | Proof of Service Proof of Service (Comment) | none | 3/13/2025 Proposed Order - Reschedule/ Reissuance of RFO; 3/13/2025 Request - Continue Hearing | none found | all |
| 8 | 4/25/2025 | Proof of Service Proof of Service (Comment) | none | 4/18/2025 Supplemental; 4/18/2025 Declaration - Income and Expense; 4/25/2025 Declaration Supplemental Declaration (Declarations); 4/25/2025 Notice - Lodging | none found (BEHAVIOR_b_e_primary.notes.md L39 records the 4/25/2025 Further Supp. Decl. of Spiegel as read; no POS from it is quoted there) | all |
| 9 | 5/9/2025 | Proof of Service Proof of Service (Comment) | none | 5/5/2025 Post-Judgment RFO Case Mgmt Statement FAM 119; 5/5/2025 Reply; 5/7/2025 Responsive Declaration (×2); 5/8/2025 Objection Evidentiary Objections and Request to Strike; 5/9/2025 Notice - Remote Appearance - RA 010 | none found | all |
| 10 | 6/3/2025 | Proof of Service Proof of Service (Comment) | none | 5/29/2025 Trial Brief / Exhibit List / Witness List (Preliminary … for Evidentiary Hearing); 5/30/2025 Notice Notice of Taking Hearing Off Calendar; 6/3/2025 Responsive Declaration to Ex Parte | none found | all |
| 11 | 6/25/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | "Mail" | 6/24/2025 Request - DV Prevention w/o Minor Child … Petitioner's Request for DVRO; Proposed Form 109; Proposed Form 110; Declaration - Ex Parte Notice | none found | paper; address; declarant; service date; tracking |
| 12 | 8/6/2025 | Proof of Service Proof of Service (Comment) | none | 8/4/2025 Exhibit List; 8/6/2025 Notice - Hearing & Order on Reissuance TRO (Form 116) | none found (63K_BAR_AND_JANINA_EXTRACT.notes.md L353 lists 8/6/2025 AnnaK emails "Minor - Service of Documents", Gmail `19881ad39b42a700` · `19881b493805982e`, attachments not opened; not a POS) | all |
| 13 | 8/7/2025 | Proof of Service Proof of Service (Comment) | none | 8/7/2025 Trial Brief; Witness List; Exhibit List; Notice - Lodging; Declaration - Income and Expense; 8/6/2025 Form 116; 8/4/2025 Exhibit List | none found (63K notes L354: 8/7/2025 AnnaK email "Halsey - Trial Setting Conference Documents", Gmail `198858d3a85cd7ea`, attachments not opened) | all |
| 14 | 8/7/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | "Mail" | same as #13 | none found | paper; address; declarant; service date; tracking |
| 15 | 8/7/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | "Mail" | same as #13 | none found | same |
| 16 | 11/17/2025 | Proof of Service Proof of Service (Comment) | none | 11/14/2025 Declaration Declaration (Declarations) | none found | all |
| 17 | 1/27/2026 | Proof of Service Proof of Service (Comment) | none | 1/21/2026 Notice Notice of Taking Hearing Off-Calendar; 1/27/2026 Responsive Declaration; 1/27/2026 Declaration - Income and Expense | none found | all |
| 18 | 1/27/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | "Mail" | same as #17 | none found | paper; address; declarant; service date; tracking |
| 19 | 4/20/2026 | Proof of Service Proof of Service (Comment) | none | 4/14/2026 and 4/15/2026 Post-Judgment Request for Order Case Mgmt Statement FAM 119 | SERVICE_VIOLATIONS_LOG.notes.md row "C5" (docket line only; content unknown) | all |
| 20 | 4/20/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | "Mail" | same as #19 | SVL row "C5" | paper; address; declarant; service date; tracking |
| 21 | 5/12/2026 | Proof of Service Proof of Electronic Service (Comment) | "Electronic" | none (Petitioner) | SVL row "C6" (docket line only) | paper; email address(es); declarant; service date |
| 22 | 5/12/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | "Mail" | none (Petitioner) | SVL row "C6" (docket line only; the docket line does not show whether tracking details are recited) | paper; address; declarant; service date; tracking |

Counts by the words in the docket text: "Email" 1 (#1); "Electronic" 1 (#21); "Mail" 6 (#11, 14, 15, 18, 20, 22); no method word 14.
- `READING_NOTES/BEHAVIOR_c_proofs_of_service.notes.md` **does not exist** (checked 2026-11-01).
- Firm POS described in SERVICE_VIOLATIONS_LOG.notes.md with **no matching register entry**: "Main 3" (2/24/2025 FL-142 POS, electronic, to Provinziano's office; there is no 2/24/2025 entry); "Main 4" (12/26/2025 POS on Petitioner's Objections to Respondent's Notice of Deposition, mail + electronic; no 12/26/2025 entry. That file places the POS inside the 12/29/2025 protective-order PDF; the register's 12/29/2025 Petitioner entries are "RFO/MTN - Quash" and "Responsive Declaration"); "C1–C3" (SUBP-025 notices 10/31/2024, 1/31/2025, 2/21/2025; no register entries on those dates).
- The register has **no** Petitioner POS entry dated after 5/12/2026 through 7/13/2026. Its only Petitioner entry after 6/1/2026 is the 7/7/2026 "Responsive Declaration".
- Writs of execution (4/28/2026): the register shows no proof-of-service, levy, or return entry for them through 7/13/2026.

### 5.1 Every entry mentioning "email" or "electronic" (all filers), verbatim
| Date | Entry | Filer |
|---|---|---|
| 3/20/2024 | Proof of Service of Summons via Email; NO service dated listed; NOAR filed 03/08/2024 | Petitioner |
| 6/3/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 6/4/2025 | Proof of Service Proof of Electronic Service (Comment) — ×3 | Respondent |
| 6/4/2025 | Proof of Service Proof of electronic Service (Comment) | Respondent |
| 6/5/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent |
| 8/25/2025 | Proof of Service Electronic | Respondent |
| 8/26/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 8/28/2025 | Clerk's Certificate - Proof of Electronic Service — ×2 | (none shown) |
| 9/17/2025 | Proof of Service Electronic | Respondent |
| 9/22/2025 | Proof of Service Electronic | Respondent |
| 10/29/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 11/17/2025 | Proof of Service Electronic | Respondent |
| 11/17/2025 | Proof of Service Electronic - RFO 1-12-2026 | Respondent |
| 12/8/2025 | Proof of Service Electronic | Respondent |
| 1/6/2026 | Proof of Service Electronic — ×3 | Respondent |
| 1/9/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 2/18/2026 | Proof of Service Electronic | Respondent |
| 3/2/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 3/4/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 3/27/2026 | Proof of Service Electronic | Respondent |
| 5/12/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) |
| 5/12/2026 | Proof of Service Proof of Electronic Service (Comment) | Petitioner |
| 7/7/2026 | Clerk's Certificate - Proof of Electronic Service (B only) | (none shown) |

Total: 28 entries in B (27 in A): 2 Petitioner (1 "Email", 1 "Electronic"), 16 Respondent, 10 clerk's certificates with no filer shown (9 in A).
Note: the "Register of Actions" list (pp.17–27 of A) shortens titles. For example, the Respondent entries "Proof of Service Electronic" and the Petitioner entry "Proof of Electronic Service" both appear there as "Proof of Service", and the summons entry appears there as "Proof of Service of Summons".


---

## 6. Appendix — complete "Documents Filed" list, printout B (7/13/2026), all 355 entries, ascending date, verbatim
Tags are this reader's filter labels only (SVC service, DISC disclosure, ATTY attorney, RFO request-for-order papers, MO minute order, WRIT, SANC sanctions, APPEAL; "-" = none). Doc image referenced = no, for every row.

| # | Date | Entry text (verbatim, "Documents Filed" section) | Filer as shown | Tags |
|---|---|---|---|---|
| 1 | 1/16/2024 | Declaration - UCCJEA Declaration - UCCJEA (Declarations) | Petitioner | - |
| 2 | 1/16/2024 | Family Law Case Cover Sheet - FAM-020 Family Law Case Cover Sheet - FAM- 020 (Comment) | Petitioner | - |
| 3 | 1/16/2024 | Order - Financial Information (FAM 111) | (none shown) | - |
| 4 | 1/16/2024 | Petition - Dissolution w/ Minor Child | Petitioner | - |
| 5 | 1/16/2024 | Summons Summons (Summons) | Petitioner | - |
| 6 | 3/8/2024 | Notice - Acknowledgment of Receipt of Summons & Petition | Petitioner | ATTY |
| 7 | 3/14/2024 | Notice - Status Conference Review: Proof of Service Noticed by LASC | (none shown) | SVC |
| 8 | 3/20/2024 | Proof of Service of Summons via Email; NO service dated listed; NOAR filed 03/08/2024 | Petitioner | SVC |
| 9 | 6/18/2024 | Declaration - Service of Preliminary Dec. of Disclosure Declaration - Service of Preliminary Dec. of Disclosure (Declarations) | Petitioner | SVC,DISC |
| 10 | 7/1/2024 | Proof of Service Proof of Service | Respondent | SVC |
| 11 | 7/1/2024 | Proof of Service Proof of Service | Respondent | SVC |
| 12 | 7/1/2024 | Proof of Service Proof of Service | Respondent | SVC |
| 13 | 7/1/2024 | Proof of Service Proof of Service | Respondent | SVC |
| 14 | 7/2/2024 | Exhibit List Exhibit List | Petitioner | - |
| 15 | 7/15/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 16 | 7/15/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 17 | 7/15/2024 | Statement - Financial Statement financial | Petitioner | DISC |
| 18 | 7/18/2024 | Statement - Financial Response - Dissolution, Nullity, Legal Separation | Petitioner | DISC |
| 19 | 7/18/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 20 | 7/18/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 21 | 7/18/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 22 | 7/18/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 23 | 7/18/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 24 | 7/18/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 25 | 7/18/2024 | Statement - Financial Statement - Financial | Petitioner | DISC |
| 26 | 7/25/2024 | Declaration - Separate Property | Respondent | - |
| 27 | 7/25/2024 | Declaration - UCCJEA | Respondent | - |
| 28 | 7/25/2024 | Miscellaneous Chargeback Notice fees due 8/19/2024 | Respondent | - |
| 29 | 7/25/2024 | Response - Dissolution, Nullity, Legal Separation | Respondent | - |
| 30 | 8/14/2024 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner | DISC |
| 31 | 8/14/2024 | Order - Attend Mediation | (none shown) | - |
| 32 | 8/14/2024 | Order - Family-Centered Case Resolution Conference (FAM 112) | (none shown) | - |
| 33 | 8/14/2024 | RFO/MTN - Custody, Visitation, Child and Spousal Support Other: Attachment 8 | Petitioner | RFO |
| 34 | 8/15/2024 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 35 | 8/22/2024 | Appearance, Stipulations and Waivers Appearance, Stipulations and Waivers (Appearances) | Petitioner | ATTY |
| 36 | 8/22/2024 | Declaration - Default FL170 Declaration - Default FL170 (Declarations) | Petitioner | - |
| 37 | 8/22/2024 | Declaration - Service of Preliminary Dec. of Disclosure Declaration - Service of Preliminary Dec. of Disclosure (Declarations) | Respondent | SVC,DISC |
| 38 | 8/22/2024 | Stipulation - Waiver of Final Declaration of Disclosure Stipulation - Waiver of Final Declaration of Disclosure (Declarations) | Petitioner | DISC |
| 39 | 10/7/2024 | Minute Order | (none shown) | MO |
| 40 | 10/18/2024 | Substitution of Attorney | Respondent | ATTY |
| 41 | 10/23/2024 | Judgment | (none shown) | - |
| 42 | 10/23/2024 | Notice - Entry of Judgment | (none shown) | - |
| 43 | 10/28/2024 | Substitution of Attorney Substitution of Attorney | Respondent | ATTY |
| 44 | 1/8/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 45 | 1/8/2025 | Declaration Declaration re Address Verification (Declarations) | Petitioner | - |
| 46 | 1/8/2025 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner | DISC |
| 47 | 1/8/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 48 | 1/8/2025 | RFO/MTN - Modification | Petitioner | RFO |
| 49 | 1/14/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 50 | 1/21/2025 | Substitution of Attorney Substitution of Attorney (Comment) | Respondent | ATTY |
| 51 | 1/27/2025 | Proposed Order - Reschedule/ Reissuance of RFO (Agreement) | Respondent | RFO |
| 52 | 1/29/2025 | Application and Order - Reissuance of RFO | (none shown) | RFO |
| 53 | 2/10/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 54 | 2/10/2025 | RFO/MTN - Compel Initial Motion to Compel Deposition Notice and Production of Documents | Petitioner | RFO |
| 55 | 2/19/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 56 | 3/13/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 57 | 3/13/2025 | Proposed Order - Reschedule/ Reissuance of RFO | Petitioner | RFO |
| 58 | 3/13/2025 | Request - Continue Hearing | Petitioner | RFO |
| 59 | 3/14/2025 | Notice - New Hearing and Order on Reissuance of RFO | (none shown) | RFO |
| 60 | 3/17/2025 | Declaration Declaration (Declarations) | Respondent | - |
| 61 | 3/17/2025 | Declaration Declaration (Declarations) | Respondent | - |
| 62 | 3/17/2025 | Exhibit List Exhibit List (Comment) | Respondent | - |
| 63 | 3/17/2025 | Memorandum - Points and Authorities Memorandum - Points and Authorities (Memos) | Respondent | - |
| 64 | 3/17/2025 | Responsive Declaration Responsive Declaration (Declarations) | Respondent | RFO |
| 65 | 3/19/2025 | Proof of Service Proof of Service (Comment) | Respondent | SVC |
| 66 | 3/21/2025 | Stipulation and Order | (none shown) | - |
| 67 | 4/18/2025 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner | DISC |
| 68 | 4/18/2025 | Supplemental | Petitioner | - |
| 69 | 4/25/2025 | Declaration Supplemental Declaration (Declarations) | Petitioner | - |
| 70 | 4/25/2025 | Notice - Lodging | Petitioner | - |
| 71 | 4/25/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 72 | 4/29/2025 | Declaration - Income and Expense Declaration - Income and Expense (respondent) | Respondent | DISC |
| 73 | 4/29/2025 | Responsive Declaration Responsive Declaration to RFO | Respondent | RFO |
| 74 | 5/5/2025 | Motion RESPONDENTS MOTION TO STRIKE PETITIONERS NOTICE OF LODGING AND OR/OBJECTION TO THE LODGING OF THE DEPOSITION TRANSCRIPT OF RESPONDENT (Motions) | Respondent | RFO |
| 75 | 5/5/2025 | Motion RESPONDENTS MOTION TO STRIKE PETITIONERS UNTIMELY FILED 04- 25-25 FURTHER SUPPLEMENTAL DECLARATION (Motions) | Respondent | RFO |
| 76 | 5/5/2025 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner | RFO |
| 77 | 5/5/2025 | Reply Reply (Comment) | Petitioner | RFO |
| 78 | 5/6/2025 | Proof of Service Proof of Service (Comment) | Respondent | SVC |
| 79 | 5/7/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent | RFO |
| 80 | 5/7/2025 | Objection Objection - Evidentiary (engel) | Respondent | - |
| 81 | 5/7/2025 | Objection Objection - Evidentiary (petitioner) | Respondent | - |
| 82 | 5/7/2025 | Objection Objection - Evidentiary (spiegel) | Respondent | - |
| 83 | 5/7/2025 | Request - Continue Hearing | Respondent | RFO |
| 84 | 5/7/2025 | Responsive Declaration | Petitioner | RFO |
| 85 | 5/7/2025 | Responsive Declaration | Petitioner | RFO |
| 86 | 5/8/2025 | Objection Evidentiary Objections and Request to Strike (Objections) | Petitioner | - |
| 87 | 5/8/2025 | Witness List Witness List (Comment) | Respondent | - |
| 88 | 5/9/2025 | Notice - Remote Appearance - RA 010 Notice - Remote Appearance - RA 010 (Appearances) | Petitioner | - |
| 89 | 5/9/2025 | Notice - Remote Appearance - RA 010 Notice - Remote Appearance - RA 010 (Appearances) | Respondent | - |
| 90 | 5/9/2025 | Order | (none shown) | - |
| 91 | 5/9/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 92 | 5/9/2025 | Proposed Order - Remote Appearance - RA 020 | Respondent | - |
| 93 | 5/12/2025 | Minute Order | (none shown) | MO |
| 94 | 5/12/2025 | Order Stipulation and Order to Use Certified Shorthand Court Reporter | (none shown) | - |
| 95 | 5/12/2025 | Order - Remote Appearance - RA 020 | (none shown) | - |
| 96 | 5/12/2025 | XSpouse Printout | (none shown) | - |
| 97 | 5/29/2025 | Exhibit List Exhibit List (Comment) | Respondent | - |
| 98 | 5/29/2025 | Exhibit List Preliminary Exhibit List for Evidentiary Hearing (Comment) | Petitioner | - |
| 99 | 5/29/2025 | Miscellaneous Respondent's Trial Setting Conference Statement (Comment) | Respondent | - |
| 100 | 5/29/2025 | Trial Brief Preliminary Brief for Evidentiary Hearing (Briefs) | Petitioner | - |
| 101 | 5/29/2025 | Witness List Preliminary Exhibit List for Evidentiary Hearing (Comment) | Petitioner | - |
| 102 | 5/29/2025 | Witness List Witness List (Comment) | Respondent | - |
| 103 | 5/30/2025 | Notice Notice of Taking Hearing Off Calendar | Petitioner | RFO |
| 104 | 6/2/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 105 | 6/2/2025 | Declaration Declaration in Support of Attorney's Motion to be relieved as Counsel (Declarations) | Respondent | ATTY |
| 106 | 6/2/2025 | RFO/MTN - Withdraw/Be Relieved as Counsel of Record | Respondent | ATTY,RFO |
| 107 | 6/3/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 108 | 6/3/2025 | Declaration Declaration (Declarations) | Respondent | - |
| 109 | 6/3/2025 | Declaration Declaration (Declarations) | Respondent | - |
| 110 | 6/3/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent | RFO |
| 111 | 6/3/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) | RFO |
| 112 | 6/3/2025 | Memorandum - Points and Authorities Memorandum - Points and Authorities (Memos) | Respondent | - |
| 113 | 6/3/2025 | Minute Order | (none shown) | MO |
| 114 | 6/3/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 115 | 6/3/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent | RFO |
| 116 | 6/3/2025 | Responsive Declaration Responsive Declaration to Ex Parte (Declarations) | Petitioner | RFO |
| 117 | 6/4/2025 | Notice - Hearing Notice - Hearing (Notices) | Respondent | RFO |
| 118 | 6/4/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent | SVC |
| 119 | 6/4/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent | SVC |
| 120 | 6/4/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent | SVC |
| 121 | 6/4/2025 | Proof of Service Proof of electronic Service (Comment) | Respondent | SVC |
| 122 | 6/5/2025 | Minute Order | (none shown) | MO |
| 123 | 6/5/2025 | Minute Order | (none shown) | MO |
| 124 | 6/5/2025 | Minute Order as Order After Hearing | (none shown) | MO |
| 125 | 6/5/2025 | Order Briefing Schedule Order | (none shown) | RFO |
| 126 | 6/5/2025 | Proof of Service Proof of Electronic Service (Comment) | Respondent | SVC |
| 127 | 6/16/2025 | Minute Order | (none shown) | MO |
| 128 | 6/24/2025 | Declaration - Ex Parte Notice (Notice Given) Declaration - Ex Parte Notice (Notice Given) (Declarations) | Petitioner | RFO |
| 129 | 6/24/2025 | Minute Order | (none shown) | MO |
| 130 | 6/24/2025 | Minute Order | (none shown) | MO |
| 131 | 6/24/2025 | Notice - Court Hearing (Form 109) | (none shown) | - |
| 132 | 6/24/2025 | Proposed Form 109 - Notice - Court Hearing Proposed Form 109 - Notice - Court Hearing (Notices) | Petitioner | - |
| 133 | 6/24/2025 | Proposed Form 110 Temporary Restraining Order Proposed Form 110 Temporary Restraining Order (Orders) | Petitioner | - |
| 134 | 6/24/2025 | Request - DV Prevention w/o Minor Child (w/in Existing Case) Petitioner's Request for DVRO (Comment) | Petitioner | - |
| 135 | 6/24/2025 | Temporary Restraining Order (Form 110) | (none shown) | - |
| 136 | 6/25/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner | SVC |
| 137 | 7/14/2025 | Proposed Form 116 - Reissuance TRO | Respondent | RFO |
| 138 | 7/14/2025 | Request to Continue and Reissue TRO (Form 115) | Respondent | RFO |
| 139 | 7/16/2025 | Minute Order | (none shown) | MO |
| 140 | 7/16/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | (none shown) | RFO |
| 141 | 8/4/2025 | Exhibit List Exhibit List (Comment) | Petitioner | - |
| 142 | 8/6/2025 | Minute Order | (none shown) | MO |
| 143 | 8/6/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Petitioner | RFO |
| 144 | 8/6/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 145 | 8/7/2025 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner | DISC |
| 146 | 8/7/2025 | Exhibit List Exhibit List (Comment) | Petitioner | - |
| 147 | 8/7/2025 | Notice - Lodging Notice - Lodging (Notices) | Petitioner | - |
| 148 | 8/7/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 149 | 8/7/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner | SVC |
| 150 | 8/7/2025 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner | SVC |
| 151 | 8/7/2025 | Trial Brief Trial Brief (Briefs) | Petitioner | - |
| 152 | 8/7/2025 | Witness List Witness List (Comment) | Petitioner | - |
| 153 | 8/11/2025 | Declaration Declaration (Declarations) | Petitioner | - |
| 154 | 8/21/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent | RFO |
| 155 | 8/21/2025 | Notice - Remote Appearance - RA 010 | Respondent | - |
| 156 | 8/21/2025 | Proof of Service Personal | Respondent | SVC |
| 157 | 8/21/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent | RFO |
| 158 | 8/21/2025 | Proposed Order - Remote Appearance - RA 020 | Respondent | - |
| 159 | 8/22/2025 | Minute Order | (none shown) | MO |
| 160 | 8/22/2025 | Responsive Declaration Exparte | Petitioner | RFO |
| 161 | 8/25/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent | RFO |
| 162 | 8/25/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) | RFO |
| 163 | 8/25/2025 | Memorandum - Points and Authorities | Respondent | - |
| 164 | 8/25/2025 | Proof of Service Electronic | Respondent | SVC |
| 165 | 8/25/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent | RFO |
| 166 | 8/25/2025 | Reply | Respondent | RFO |
| 167 | 8/26/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 168 | 8/26/2025 | Declaration - Ex Parte Notice (Notice Given) | Respondent | RFO |
| 169 | 8/26/2025 | Declaration - Income and Expense | Respondent | DISC |
| 170 | 8/26/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) | RFO |
| 171 | 8/26/2025 | Minute Order | (none shown) | MO |
| 172 | 8/26/2025 | Proof of Service | Respondent | SVC |
| 173 | 8/26/2025 | Proof of Service | Respondent | SVC |
| 174 | 8/26/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent | RFO |
| 175 | 8/26/2025 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner | RFO |
| 176 | 8/27/2025 | Minute Order | (none shown) | MO |
| 177 | 8/27/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Petitioner | RFO |
| 178 | 8/28/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 179 | 8/28/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 180 | 8/28/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) | RFO |
| 181 | 8/28/2025 | Minute Order | (none shown) | MO |
| 182 | 8/28/2025 | Minute Order | (none shown) | MO |
| 183 | 8/28/2025 | Order Briefing Schedule Order | (none shown) | RFO |
| 184 | 8/28/2025 | Order - Remote Appearance - RA 020 | (none shown) | - |
| 185 | 8/28/2025 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner | RFO |
| 186 | 9/8/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 187 | 9/8/2025 | RFO/MTN - Family Law | Respondent | RFO |
| 188 | 9/17/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 189 | 9/17/2025 | Minute Order | (none shown) | MO |
| 190 | 9/17/2025 | Notice - Change of Address | Respondent | - |
| 191 | 9/17/2025 | Notice - Court Hearing (Form 109) | (none shown) | - |
| 192 | 9/17/2025 | Proof of Service Electronic | Respondent | SVC |
| 193 | 9/17/2025 | Proof of Service - Mail | Respondent | SVC |
| 194 | 9/17/2025 | Proposed Form 109 - Notice - Court Hearing | Respondent | - |
| 195 | 9/17/2025 | Proposed Form 110 Temporary Restraining Order | Respondent | - |
| 196 | 9/17/2025 | Proposed Form 130 Restraining Order After Hearing | Petitioner | - |
| 197 | 9/17/2025 | RFO/MTN - Mod - Spousal Support | Respondent | RFO |
| 198 | 9/17/2025 | Request - DV Prevention w/Minor Child (w/in Existing Case) | Petitioner | - |
| 199 | 9/22/2025 | Proof of Service Electronic | Respondent | SVC |
| 200 | 9/22/2025 | Proof of Service - Mail | Respondent | SVC |
| 201 | 10/7/2025 | Declaration of Due Diligence | Respondent | SVC |
| 202 | 10/7/2025 | Proof of Service | Respondent | SVC |
| 203 | 10/8/2025 | Minute Order | (none shown) | MO |
| 204 | 10/8/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Respondent | RFO |
| 205 | 10/14/2025 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner | RFO |
| 206 | 10/20/2025 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner | RFO |
| 207 | 10/22/2025 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner | DISC |
| 208 | 10/22/2025 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner | RFO |
| 209 | 10/27/2025 | Declaration of Due Diligence | Respondent | SVC |
| 210 | 10/27/2025 | Minute Order | (none shown) | MO |
| 211 | 10/27/2025 | Notice - Ruling Notice - Ruling (Notices) | Petitioner | RFO |
| 212 | 10/28/2025 | Declaration - Ex Parte Notice (Notice Given) | Petitioner | RFO |
| 213 | 10/28/2025 | Proposed Ex Parte RFO Emergency Orders for Support | Petitioner | RFO |
| 214 | 10/29/2025 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 215 | 10/29/2025 | Ex Parte RFO Emergency Orders for Support | (none shown) | RFO |
| 216 | 10/29/2025 | Minute Order | (none shown) | MO |
| 217 | 10/29/2025 | Minute Order | (none shown) | MO |
| 218 | 10/29/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Respondent | RFO |
| 219 | 10/29/2025 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner | RFO |
| 220 | 11/4/2025 | Minute Order | (none shown) | MO |
| 221 | 11/4/2025 | Notice - Court Hearing (Form 109) | (none shown) | - |
| 222 | 11/4/2025 | Proposed Form 109 - Notice - Court Hearing Proposed Form 109 - Notice - Court Hearing (Notices) | Petitioner | - |
| 223 | 11/4/2025 | Proposed Form 110 Temporary Restraining Order Proposed Form 110 Temporary Restraining Order (Orders) | Petitioner | - |
| 224 | 11/4/2025 | Request - DV Prevention w/Minor Child (w/in Existing Case) DV w/ Minor Child - Within Existing Case (Comment) | Petitioner | - |
| 225 | 11/4/2025 | Temporary Restraining Order (Form 110) | (none shown) | - |
| 226 | 11/12/2025 | Memorandum - Points and Authorities | Respondent | - |
| 227 | 11/12/2025 | Proof of Service DV-200 | Respondent | SVC |
| 228 | 11/12/2025 | RFO/MTN - Family Law | Respondent | RFO |
| 229 | 11/13/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 230 | 11/13/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 231 | 11/14/2025 | Declaration Declaration (Declarations) | Petitioner | - |
| 232 | 11/17/2025 | Proof of Service Electronic | Respondent | SVC |
| 233 | 11/17/2025 | Proof of Service Electronic - RFO 1-12-2026 | Respondent | SVC,RFO |
| 234 | 11/17/2025 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 235 | 11/17/2025 | Proof of Service - Mail | Respondent | SVC |
| 236 | 11/17/2025 | Proof of Service - Mail RFO 1-12-2026 | Respondent | SVC,RFO |
| 237 | 11/17/2025 | Witness List | Respondent | - |
| 238 | 11/19/2025 | Minute Order | (none shown) | MO |
| 239 | 11/19/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Respondent | RFO |
| 240 | 11/25/2025 | Minute Order | (none shown) | MO |
| 241 | 11/25/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Petitioner | RFO |
| 242 | 12/5/2025 | Declaration - Income and Expense | Respondent | DISC |
| 243 | 12/5/2025 | Notice - Change of Address | Respondent | - |
| 244 | 12/5/2025 | RFO/MTN - Mod - Child Support | Respondent | RFO |
| 245 | 12/8/2025 | Proof of Service Electronic | Respondent | SVC |
| 246 | 12/8/2025 | Proof of Service - Mail | Respondent | SVC |
| 247 | 12/10/2025 | Minute Order | (none shown) | MO |
| 248 | 12/10/2025 | Minute Order | (none shown) | MO |
| 249 | 12/10/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Petitioner | RFO |
| 250 | 12/10/2025 | Notice - Hearing & Order on Reissuance TRO (Form 116) | Respondent | RFO |
| 251 | 12/29/2025 | Order - Family-Centered Case Resolution Conference (FAM 112) | (none shown) | - |
| 252 | 12/29/2025 | RFO/MTN - Quash | Petitioner | RFO |
| 253 | 12/29/2025 | Responsive Declaration | Petitioner | RFO |
| 254 | 12/30/2025 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 255 | 12/30/2025 | RFO/MTN - Sanctions Attorney Fees | Petitioner | RFO,SANC |
| 256 | 1/5/2026 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 257 | 1/5/2026 | Memorandum - Points and Authorities Memo of Ps and As in support of Motion to Compel | Respondent | - |
| 258 | 1/5/2026 | Memorandum - Points and Authorities Memo of Ps and As in support of Motion to Quash | Respondent | - |
| 259 | 1/5/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 | Petitioner | RFO |
| 260 | 1/5/2026 | RFO/MTN - Compel Initial Other: Compel Preliminary/Final Declarations of Disclosure; Monetary Sanctions - See #7 | Respondent | DISC,RFO,SANC |
| 261 | 1/5/2026 | RFO/MTN - Family Law Other: Objection to Defective Service and Request for Continuance or to Take Matter Off Calendar | Respondent | RFO |
| 262 | 1/5/2026 | RFO/MTN - Quash Other: Motion to Quash; Protective Order and Sanctions - See #7 | Respondent | RFO,SANC |
| 263 | 1/6/2026 | Proof of Service Electronic | Respondent | SVC |
| 264 | 1/6/2026 | Proof of Service Electronic | Respondent | SVC |
| 265 | 1/6/2026 | Proof of Service Electronic | Respondent | SVC |
| 266 | 1/6/2026 | Proof of Service - Mail | Respondent | SVC |
| 267 | 1/6/2026 | Proof of Service - Mail | Respondent | SVC |
| 268 | 1/6/2026 | Proof of Service - Mail | Respondent | SVC |
| 269 | 1/8/2026 | Objection Objection and Request to Strike (Objections) | Petitioner | - |
| 270 | 1/9/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 271 | 1/9/2026 | Declaration - Ex Parte Notice (Notice Given) | Respondent | RFO |
| 272 | 1/9/2026 | Ex Parte RFO Emergency Orders for Support | (none shown) | RFO |
| 273 | 1/9/2026 | Memorandum - Points and Authorities | Respondent | - |
| 274 | 1/9/2026 | Minute Order | (none shown) | MO |
| 275 | 1/9/2026 | Proposed Ex Parte RFO Emergency Orders for Support | Respondent | RFO |
| 276 | 1/12/2026 | Minute Order | (none shown) | MO |
| 277 | 1/12/2026 | Order | (none shown) | - |
| 278 | 1/21/2026 | Notice Notice of Taking Hearing Off-Calendar | Petitioner | RFO |
| 279 | 1/22/2026 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 280 | 1/22/2026 | Memorandum - Points and Authorities | Respondent | - |
| 281 | 1/22/2026 | Proof of Service | Respondent | SVC |
| 282 | 1/22/2026 | Proof of Service - Mail | Respondent | SVC |
| 283 | 1/22/2026 | RFO/MTN - Sanctions | Respondent | RFO,SANC |
| 284 | 1/27/2026 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner | DISC |
| 285 | 1/27/2026 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 286 | 1/27/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner | SVC |
| 287 | 1/27/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner | RFO |
| 288 | 2/2/2026 | Proposed Order - Vexatious Litigant - Motion/RFO/Other | Petitioner | RFO |
| 289 | 2/2/2026 | RFO/MTN - Family Law | Petitioner | RFO |
| 290 | 2/2/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner | RFO |
| 291 | 2/2/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner | RFO |
| 292 | 2/3/2026 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 293 | 2/5/2026 | Declaration of Due Diligence | Respondent | SVC |
| 294 | 2/9/2026 | Minute Order | (none shown) | MO |
| 295 | 2/11/2026 | Minute Order | (none shown) | MO |
| 296 | 2/11/2026 | Minute Order | (none shown) | MO |
| 297 | 2/18/2026 | Objection | Respondent | - |
| 298 | 2/18/2026 | Proof of Service Electronic | Respondent | SVC |
| 299 | 2/18/2026 | Proof of Service - Mail | Respondent | SVC |
| 300 | 2/18/2026 | Responsive Declaration | Respondent | RFO |
| 301 | 2/23/2026 | Declaration - Income and Expense Declaration - Income and Expense (Declarations) | Petitioner | DISC |
| 302 | 2/23/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner | RFO |
| 303 | 2/23/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner | RFO |
| 304 | 2/23/2026 | Reply Reply (Comment) | Petitioner | RFO |
| 305 | 2/24/2026 | Responsive Declaration Responsive Declaration - MTC.FDD (Declarations) | Petitioner | RFO |
| 306 | 2/24/2026 | Responsive Declaration Responsive Declaration - MTQ (Declarations) | Petitioner | RFO |
| 307 | 2/24/2026 | Responsive Declaration Responsive Declaration - Obj.Def.Serv (Declarations) | Petitioner | RFO |
| 308 | 3/2/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 309 | 3/2/2026 | Minute Order | (none shown) | MO |
| 310 | 3/2/2026 | Minute Order | (none shown) | MO |
| 311 | 3/2/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 | Petitioner | RFO |
| 312 | 3/2/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 - MTC.FDD (Judgments) | Petitioner | RFO |
| 313 | 3/2/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 - Obj.Def.Serv (Judgments) | Petitioner | RFO |
| 314 | 3/4/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 315 | 3/4/2026 | Minute Order | (none shown) | MO |
| 316 | 3/27/2026 | Brief | Petitioner | - |
| 317 | 3/27/2026 | Brief | Respondent | - |
| 318 | 3/27/2026 | Declaration Declaration in Support of Brief | Respondent | - |
| 319 | 3/27/2026 | Proof of Service Electronic | Respondent | SVC |
| 320 | 3/27/2026 | Proof of Service - Mail | Respondent | SVC |
| 321 | 4/8/2026 | Responsive Declaration | Petitioner | RFO |
| 322 | 4/14/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner | RFO |
| 323 | 4/15/2026 | Post-Judgment Request for Order Case Mgmt Statement FAM 119 Post- Judgment Request for Order Case Mgmt Statement FAM 119 (Judgments) | Petitioner | RFO |
| 324 | 4/20/2026 | Proof of Service Proof of Service (Comment) | Petitioner | SVC |
| 325 | 4/20/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner | SVC |
| 326 | 4/21/2026 | Minute Order | (none shown) | MO |
| 327 | 4/21/2026 | Minute Order | (none shown) | MO |
| 328 | 4/21/2026 | Minute Order | (none shown) | MO |
| 329 | 4/21/2026 | Minute Order | (none shown) | MO |
| 330 | 4/21/2026 | Minute Order | (none shown) | MO |
| 331 | 4/21/2026 | Minute Order | (none shown) | MO |
| 332 | 4/21/2026 | Minute Order as Order After Hearing | (none shown) | MO |
| 333 | 4/21/2026 | Minute Order as Order After Hearing | (none shown) | MO |
| 334 | 4/21/2026 | Minute Order as Order After Hearing | (none shown) | MO |
| 335 | 4/28/2026 | Application - Issue Writ E/P/S Los Angeles - $11,000.00 Attorney's Fees based on Order 5/12/2025 | Petitioner | WRIT |
| 336 | 4/28/2026 | Application - Issue Writ E/P/S Los Angeles - $21,857.00 Spousal Support based on Order 5/12/2025 | Petitioner | WRIT |
| 337 | 4/28/2026 | Application - Issue Writ E/P/S Los Angeles - $62.876.00 Child Support based on Order 5/12/2025 | Petitioner | WRIT |
| 338 | 4/28/2026 | Writ - Execution Los Angeles - $11,000.00 Attorney's Fees based on Order 5/12/2025 - Issued 4/28/2026 | Petitioner | WRIT |
| 339 | 4/28/2026 | Writ - Execution Los Angeles - $21,857.00 Spousal Support based on Order 5/12/2025 - Issued 4/28/2026 | Petitioner | WRIT |
| 340 | 4/28/2026 | Writ - Execution Los Angeles - $62.876.00 Child Support based on Order 5/12/2025 - Issued 4/28/2026 | Petitioner | WRIT |
| 341 | 5/11/2026 | Declaration - Ex Parte Notice (Notice Given) | Respondent | RFO |
| 342 | 5/11/2026 | Proposed Ex Parte RFO Emergency Orders for Other | Respondent | RFO |
| 343 | 5/12/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 344 | 5/12/2026 | Ex Parte RFO Emergency Orders for Other | (none shown) | RFO |
| 345 | 5/12/2026 | Minute Order | (none shown) | MO |
| 346 | 5/12/2026 | Proof of Service Proof of Electronic Service (Comment) | Petitioner | SVC |
| 347 | 5/12/2026 | Proof of Service - Mail Proof of Service - Mail (Proof of Service) | Petitioner | SVC |
| 348 | 5/13/2026 | RFO/MTN - Family Law | Respondent | RFO |
| 349 | 5/14/2026 | Court Order for Post-Judgment Requests for Orders FAM 120 | (none shown) | RFO |
| 350 | 5/27/2026 | Proof of Service - Mail | Respondent | SVC |
| 351 | 6/18/2026 | Appeal - Notice of Appeal/Cross Appeal Filed General Appeal | Respondent | APPEAL |
| 352 | 6/26/2026 | Appeal - Notice of Filing of Notice of Appeal | (none shown) | APPEAL |
| 353 | 7/7/2026 | Appeal - Notice of Default Issued for NOA filed 6/18/2026. DEFAULT FOR DESIGNATION. | Respondent | APPEAL |
| 354 | 7/7/2026 | Clerk's Certificate - Proof of Electronic Service | (none shown) | SVC |
| 355 | 7/7/2026 | Responsive Declaration Responsive Declaration (Declarations) | Petitioner | RFO |

---

## 7. Scope statement
- A: read in full (every line, pp.1–27). B: read in full through a whole-text diff against A plus a parse of all 355 entries. C, D, E: compared entry by entry by script; party, future-hearing and proceedings blocks read; not read line by line otherwise. F: all 3 pages read as images.
- Not downloaded or hashed: `1DZJPwuz7WvYUqInyK2KYibVUEp3tpYF_` (same size as A) and the duplicate copies of C, D, E.
- Not read in full: the 9/5/2026 transfer bundle `14iazThcrgMA48l8bFVpwsd4I0yoMbiP3` and the case capsule `1wRkMXYwhGIz8ww0s0nhF0T-kH5ujGBJM` (both AI-LEAD compilations); searched only for embedded register printouts.
- No document images (POS, orders) were opened for this file; the register text is the only source for §2–§6 except the pointers to other READING_NOTES files.
- Scratch: /tmp/claude-0/-home-user/9a86eccf-071d-5c97-88ae-ef129ec55f9d/scratchpad/dk/ (reg1.txt = A text; roa_14Jb.txt = B text; docs_0713.tsv = parsed entries).
