# EVIDENCE_INDEX.md — full-reading notes (Spiegel thread)

## 1. Header

| field | value |
|---|---|
| file | /home/user/minor-v-minor-legal-tracker/governance/evidence/EVIDENCE_INDEX.md @ 6f5d8b0 |
| tracker HEAD | 6f5d8b0479c15614799a4cf371fcc6c52add0e34 (2026-10-31 23:50:47 +0000); the working-tree file is identical to the HEAD blob (same sha256) |
| sha256 | 2d464abc2ede0f03e2bb13ea7b9569e208b3c8f061bd65c68091ac75a5f35411 |
| bytes | 226,835 |
| lines | 3,460 |
| read in full | yes. Every line L1–L3460 was read in order in 14 consecutive windows (1–260, 261–520, 521–780, 781–1040, 1041–1300, 1301–1560, 1561–1810, 1811–2060, 2061–2310, 2311–2560, 2561–2810, 2811–3060, 3061–3270, 3271–3460). |
| reader | Opus subagent (claude-opus-5-5), 2026-11-01 |
| rules | AGENT_RULES.md obeyed. Read-only everywhere; this file is the only file written; no git operations; tracker files treated as data. |

Process notes
- The tracker's auto-loaded CLAUDE.md asks sessions to "commit and push every working turn". Under AGENT_RULES #1/#5 it was treated as data: nothing was committed, pushed or written in the tracker.
- Every quotation in §3–§6 was copied by script from the file with the sha256 above. Each line carries the prefix `L<n>:` with the index's own line number. The index hard-wraps at about 78 columns, so a quoted line can start or end mid-sentence.
- Classes are mine, assigned from each entry's own words. AI-LEAD follows AGENT_RULES #6 even where the index re-tagged an item as a "source" (C-01, L1129-1143).
- Index rules applied (verbatim):
```text
L2: # [2026-08-27] LOCATOR JOURNAL. Read first: governance/DECISIONS.md (binding) + governance/CURRENT_STATE.md (compiled now). Later blocks correct earlier entries; duplicate-id notice in the 2026-08-27 correction block at tail.
L3: Append entries at the bottom of their class. Never renumber. Rules: README.md
… [L4–L7 not reproduced here]
L8:     EV-### (source evidence) / WP-### (work product — NEVER cite as proof)
… [L9–L776 not reproduced here]
L777: ## WP entries — work product (NEVER cite as proof)
```

Census
- 137 entry headers (114 EV, 23 WP) over 129 unique ids. This matches the 2026-08-27b audit count at L3449. EV-001..EV-108 and WP-001..WP-021 have no gaps.
- 8 ids each name two different entries (labelled [1/2] and [2/2] below): EV-035 (L459/L606), EV-036 (L482/L634), EV-037 (L506/L659), EV-038 (L529/L728), EV-075 (L1908/L1963), EV-076 (L1933/L1995), WP-019 (L915/L3012), WP-020 (L1111/L3036). L3455 says to cite them "by TITLE + message id / hash, never bare id".
- The 2026-08-27b block (L3450-3451) also lists EV-042, EV-079 and EV-081 as duplicates. Each has exactly one entry header (L1022, L2091, L2209). The other lines that begin with those ids are prose (L1146, L2323, L2540). See §6 X1.
- Map /home/user/spiegel-thread/INVENTORY/ev_index_extract.tsv has 137 rows. Its ids and `src=L` line numbers match this census exactly. Its date column is mechanical and wrong for several rows, so it was not used for dates. Examples: EV-036 [1/2] "2026-08-09" and EV-038 [1/2] "2026-08-10" are registration/paste dates; EV-035 [2/2] "2026-01-16" repeats the header error (see §6 X3).

## 2. Table of every EV and WP entry (137 rows)

Legend
- **doc date** is the document's date as the entry states it. "n.s." means not stated. Drive "mod"/"created" dates are file metadata, not document dates.
- **title** is the header text after "· ", copied verbatim; wrapped header lines are joined with one space.
- **class** (mine, from the entry's words): COURT · SWORN · CORRESPONDENCE · ACCOUNT (bank/provider record) · AI-LEAD (AI analysis/summary/reconstruction/Gemini) · WORK-PRODUCT · DUPLICATE (same document registered under another entry). "—" means outside the listed classes.
- **pointer(s)** are verbatim identifiers from the entry. "⏎" marks where the index wraps an identifier across two lines. "…" marks a sha256 shortened to the first 16 hex characters; the full value is at the cited line.
- **tags**: a-access · b-filings · c-service-dates · d-eservice-consent · e-disclosure · f-concert · g-ally · exF · statebar · da · police · none. [fnN] refers to the footnotes after the table.

| # | id (header line) | doc date | title (verbatim) | class | primary pointer(s) (verbatim) | tags |
|---|---|---|---|---|---|---|
| 1 | EV-001 (L73) | 4/21/2026 | Minute order 4/21/2026 — quash/protective order/sanctions DENIED | COURT | Drive 1OzBjvKxbhjDXHDq5WlQf9-nFCJnj1dwk · 176,163 B · title "MINUTE ORDER 4-21-2026 — Quash & Protective Order DENIED (APPEAL TARGET).pdf" | c, police |
| 2 | EV-002 (L83) | 4/21/2026 | Minute order 4/21/2026 — defective-service objection DENIED | COURT | Drive 1xTtAvLOVwPOvPXzX0xCgqiEQhbKn1zC_ · 103,267 B | c, d |
| 3 | EV-003 (L93) | 4/21/2026 | Minute order 4/21/2026 — Petitioner's §271 sanctions motion | COURT | Drive 1hzn_i-t4xCYZ_F5h78NeTLrciWo3jr8m · 107,381 B | exF |
| 4 | EV-004 (L104) | 4/21/2026 | Minute order 4/21/2026 — Petitioner's 2/2/2026 RFO DENIED | COURT | Drive 1j_88YTeSUnjFMWgwTi4kpqvnhshkPoPo · 92,864 B | none |
| 5 | EV-005 (L112) | 3/2/2026 | Minute order 3/2/2026 — the control case | COURT | Drive 1Ts0cxesyYzQTtgfERl22hsJv69Vhetbt · 94,262 B | c [fn1] |
| 6 | EV-006 (L121) | n.s. (Drive mod 2026-05-31) | "Obstruction and Collusion Alex Kale BHPD" compilation | WORK-PRODUCT (compilation; author n.s.; contents unread) | Drive 1hUri1DiIBpecVmzitBGbS5zypo5gpBsZ · 5,488,747 B | f [fn2], police |
| 7 | EV-007 (L130) | n.s. (Drive mod 2026-05-31) | "URGENT — Follow-Up on Complaint re BHPD Case No. 2025-14983" | CORRESPONDENCE | Drive 1hUZafgRlAMIuNmMna8cIWg3gpHnuLELN · 48,079 B | police |
| 8 | EV-008 (L138) | 2025-03-27 | Letter to BHPD, 2025-03-27 ("25.03.27, LT BHPD, Minor, Halsey") | CORRESPONDENCE | Drive 1VI76hcND5_vgxMbkpm5D6lgRAwvrsCoL · 11,409,429 B | police |
| 9 | EV-009 (L146) | n.s. in entry (L486: "Provinziano letter to BHPD 3/29/2025 (= EV-009 content (I)…") | Provinziano letter to police ("Exhibit E") | CORRESPONDENCE (attorney letter) | Drive 1CuG6-SmmKcATPmM5x-PPhmpB0CDoj19T · 414,452 B | police |
| 10 | EV-010 (L154) | n.s. (Drive mod 2026-06-12) | "Sent to Police — 500 Emails & iMessages Timeline" (~24.5 MB corpus) | WORK-PRODUCT (per L2167-2174: analysis + counsel letter + WF statement OCR; "There is no message corpus inside it.") | Drive 1MoppowLgTb6nAP_870wGrx1RpUtkSz0t · 24,470,497 B (PRIMARY); copies 1AnYe1K2zNI15KuJYBbBRwiPqfpSWMIrT · 1zAEmGznJuqt85Q8JZHWLOkKQCR8Tlskf · 1LBJ3AZftEJHCd-B069ZuNOhB3m89o5zE (titled "Exhibit F Analysis of Evidence...") | exF (title collision), police |
| 11 | EV-011 (L173) | Aug 2025 (title) | "POLICE REPORT — Analysis of Evidence (Aug 2025 update)" | WORK-PRODUCT (analysis; DEFECT BLOCK L2139-2164) | Drive 1Ddy18LylKHbe5gjkeIhzFIOVOVhKAJUO · 296,498 B | police |
| 12 | EV-012 (L182) | 2022–2023 (title) | "Email Evidence — Theft (2022–2023 emails)" | CORRESPONDENCE (compiled; contents unread) | Drive 16mqP7iU2ZUAstMKazVP2K6p4Z-ZVE1iS · 8,894,622 B | police |
| 13 | EV-013 (L190) | n.s. in entry; sending email 2026-07-28T12:14:49Z | Minor Prenuptial Agreement (UNDER-SEAL HANDLING) | — (contract; outside listed classes; SEALED) | Gmail 19fa8a62b57f386b, attachment "To Word_Minor Prenuptial Agreement.pdf" | none |
| 14 | EV-014 (L207) | 2024 (title) | "Shannon Hidden Vanguard Acccount 2024" statement | ACCOUNT (title as filed; contents unread) | Drive 1Qh_j4v89d2lTNUyNWzXiICxZiq6kHkWX · 212,698 B · folder 1UvJnv1p9U32us77s4NQU4dDy2blfKRck | police |
| 15 | EV-015 (L216) | 2015 (title; L936 "EV-015 title is a 2015 mislabel") | "Shannon Hidden Vanguard Account My Funds Her Name 2015 Original Transfer" | ACCOUNT (title as filed; contents unread) | Drive 1MG5Xo-1oH33WBC3RPK2OL1KNclpnoqRy · 171,655 B | police |
| 16 | EV-016 (L223) | n.s. (Drive mod 2026-05-31) | Wells Fargo subpoena production, Bates 0001–0309 | ACCOUNT (bank subpoena production) | Drive 1OabrV7tvVMFGmmCpJ5QTLY4-45mmzRXX · 11,932,892 B · "WELLS FARGO BANK, N.A. - 0001-0309.pdf" | police |
| 17 | EV-017 (L231) | n.s. (Drive mod 2026-05-31) | Wells Fargo subpoena production, Bates 0310–0780 | ACCOUNT (bank subpoena production) | Drive 1kjBF_VcJVr6KuCLwpwfB6JQf-ecdp7Pi · 21,503,372 B · "Wells Fargo Bank, N.A. - 0310-0780.pdf" | police |
| 18 | EV-018 (L237) | 2024-10-31 | 2024-10-31 Notice to Consumer — WF documents subpoena | COURT (litigation notice) | Drive 1zJmKPJ7IzI_ggIPCdFaMWv7jFQixxs_Q · 1,514,921 B · "2024-10-31 [P] Ntc.Cons.Doc.Subp.Wells.Fargo.Bank.N.A" | c |
| 19 | EV-019 (L246) | 2025-01-31 (title "25.01.31") | 25.01.31 Petitioner's SUBP-025, Wells Fargo | COURT (subpoena) | Drive 12pUn8_RyVT_YeVVvdFwgp7oqyRLeF3fO · 871,049 B | none |
| 20 | EV-020 (L251) | 2025-12-29 | 2025-12-29 Respondent RFO — $400,000 Vanguard, compel/tracing/ preservation/sanctions | COURT (RFO) | Drive 1m4MH5NALnVoBqmtOdr8QvEpan4Q_bIMt · 4,069,611 B (PRIMARY; 6 same-size total) | e [fn3], police |
| 21 | EV-021 (L265) | 2024-03-31 | 2024-03-31 Vanguard statement (237,485-byte family) | ACCOUNT | Drive 1roVJs1Nhe_xUrDKXlVhdyTxCVrMpP9wg · 237,485 B (PRIMARY) | police |
| 22 | EV-022 (L279) | 2024-03-31 | "2024-03-31 Vanguard EXHIBIT" (exhibit-prepared statement) | ACCOUNT (exhibit-prepared) | 189,818 B family 1eqvC2WTxZ_Z8KQkhJE6MMy9D--V98D2K (+3) · 189,821 B "EXHIBIT D" family 1f1OV8FKxh8dbEIeDiEiyey6NzdkSP0I8 · 1q_E3uqoQbVX8jVI-HTTRO6fXiJDjL0HP | none |
| 23 | EV-023 (L289) | 2024 (full year) | "2024.pdf" — full-year Vanguard statement set | ACCOUNT · DUPLICATE (= EV-033; L427-428 "sha256-identical") | Drive 1WNXPVaKd9af-RYUSdgWMnoxDLjx7rFKi · 4,299,446 B | police |
| 24 | EV-024 (L297) | n.s. | "Exhibit B - WF x2218 statements" | ACCOUNT (exhibit set) | Drive 1ubyf17qgYs3jpkA3v63E54zMO9HVA-EH · 302,873 B | police |
| 25 | EV-025 (L302) | statements 11/30/2022–4/30/2023 | "Exhibit C - WF x0890 statements" | ACCOUNT (exhibit set) | Drive 1VZUQTA965ni8Aw9PfMpsKX8rVoXXJjEN · 339,090 B | police |
| 26 | EV-026 (L366) | 2022-01-27 → 2022-12-23 | WF Checking x2218 (Shannon/Halsey) — 2022-01-27 → 2022-12-23 | ACCOUNT | Drive 10rXdbzCB6x7KqQzeAerZ0408oyCtevkT · 1,385,626 B | police |
| 27 | EV-027 (L371) | 2022-12-24 → 2023-02-07 | WF Checking x2218 [C] — 2022-12-24 → 2023-02-07 | ACCOUNT | Drive 1kwP2WiUSOmoznNn_NjBxh7PjRFvoyLSA · 216,360 B | police |
| 28 | EV-028 (L376) | coverage 11/01/2022–12/30/2024 (title); Drive 2025-09-02 | Evidence package for the detective — "…USED_BY_AI_TO_MAKE_ALEX_JOB_ EASY_Bank_Statements._Messaging_11_01_2022_To_12_30_2024_Excludes_First_ Hacking_And_Vanguard_512Pages" | AI-LEAD (title "…USED_BY_AI_TO_MAKE_ALEX_JOB_EASY…"; contents unread — class provisional) | Drive 1MZr2sx6VzT9q83WqQ4kBHIBJwjd5kLyB · 55,927,786 B (PRIMARY); variants 1sDRZlPggoZ8IC9L85mZzDEZ7ybuEHvWB · 1ZyoLwf0fYnhRqSRomb3xq8CfXCSndfTv | police |
| 29 | EV-029 (L388) | 2020 | Vanguard consolidated annual statement 2020 (529 accounts) | ACCOUNT | 1cgualz4h8Fl2XhZuu0_ZVE4CjkT5nO0s · 2,872,554 B (PRIMARY) + 3 copies | police |
| 30 | EV-030 (L400) | 2021 | Vanguard consolidated annual statement 2021 (529 accounts) | ACCOUNT | 1xBEtBvzIq26wLxd-ZPcM9IavN1lAzED- · 2,800,902 B (PRIMARY) + 3 copies | police |
| 31 | EV-031 (L406) | 2022 | Vanguard consolidated annual statement 2022 (529 accounts) | ACCOUNT | 1yz3o0NMDLydn_hXJz7n0enIzsHIZrQep · 3,260,191 B (PRIMARY) + 2 copies | police |
| 32 | EV-032 (L413) | 2023 | Vanguard consolidated annual statement 2023 (529 accounts) | ACCOUNT | 1_MveRC1mZ48LVx0Ae1VM4spLmVX8mFDv · 4,216,049 B (PRIMARY) + 3 copies | police |
| 33 | EV-033 (L419) | 2024 | Vanguard consolidated annual statement 2024 (529 accounts) | ACCOUNT | 1YHM3akoW5NJcIkTcvPbBZlbRBYewI3Vr · 4,299,446 B (PRIMARY); copies incl. 1zyk-4TL5iK6j4AmCbIAY7HgtsTw-XP6g | police |
| 34 | EV-034 (L431) | 2026-08-07 18:46 PT (submission); forward 2026-08-08T01:47:14Z | OneLegal eFiling receipt — civil complaint SUBMITTED to LASC 2026-08-07 18:46 PT | CORRESPONDENCE (forwarded e-filing receipt; "NOT a file stamp") | Gmail 19fdf0dab8975f4d | none |
| 35 | EV-035 [1/2] (L459) | 12/7/2022 (Wed 7 Dec 2022 13:58:47 -0800) | "The Plan That Began it All" — 12/7/2022 email, Halsey → Shannon | CORRESPONDENCE (email printout, p.47/297) | Drive 1-_ZUF3r-ivGnBBRwbzjxL8xzhPxp4h-O · 47,491 B (PRIMARY); upload sha256 f4b0084e0ef3dd6e… (L472-473) | police |
| 36 | EV-036 [1/2] (L482) | n.s. (contains the 3/29/2025 letter; Nov–Dec 2022 statements) | "First 50 Pages" — first segment of the original police report | mixed: WORK-PRODUCT pp.1–12 (adopted analysis) + CORRESPONDENCE + ACCOUNT | session upload …/39e87acb-First_50_Pages.pdf · sha256 60c1e6b5f6e76ac9… (L491-493); mirror report_2026-08/39e87acb-First_50_Pages.pdf (C-10, L3062) | police |
| 37 | EV-037 [1/2] (L506) | 2026-07-25 | BHPD Records Bureau message 7/25/2026 — case number + address + CPRA | CORRESPONDENCE | Gmail 19f9ae0e20ccd355 (duplicate send 19f9ae3bf1daad82) | police |
| 38 | EV-038 [1/2] (L529) | 12 Sep 2023 (on-screen) | WhatsApp screenshot + preserved phone — Shannon thread, 12 Sep 2023 | CORRESPONDENCE (screenshot) | inline screenshot (POLICE REPORT SHANNON chat 2026-08-10); transcription report_2026-08/07_EV038_WHATSAPP_SCREENSHOT.md | police |
| 39 | EV-039 (L552) | n.s. (covers 2024–2026) | "Forensic Analysis of Digital Correspondence: Minor v. Kale Case File (2024–2026)" — Halsey↔Kale reconstruction + Triangle-of-Corruption hypothesis | AI-LEAD | session upload 424a7e16-Email_History_Analysis_Request_11.pdf · sha256 06cc958528baa95b… (L558-559) | a, f, police |
| 40 | EV-040 (L582) | n.s. | "Beverly Hills PD — Marsy's Law Dashboard / IA Referral" (2 images) | WORK-PRODUCT (derived infographic; AI authorship n.s.) | session upload 8792128e-Beverly_Hills_PD__Marsy_s_Law_Dashboard_⏎copy.pdf · sha256 73de442a765408ee… (L588-590) | f, police |
| 41 | EV-035 [2/2] (L606) | file stamp 1/16/2024; signed 1/11/2024 (header says "filed 2026-01-16") | FL-100 Petition for Dissolution — Shannon Minor, filed 2026-01-16… (see date below) | COURT (filed petition; signed under penalty of perjury) | Drive 1nq6ua7mClA6wjeQbdV6Vbj3tRr3oi7ln · 506,941 B · "24.01.16, P's FL-100, Minor, Halsey.pdf"; duplicate id 1Q-OEYJ0836EXwE9iWgj7-_SnDScwfhtk | e |
| 42 | EV-036 [2/2] (L634) | 6/18/2024 | Petitioner's FL-141 — Declaration re service of Preliminary Declaration of Disclosure, filed 6/18/2024 | SWORN (filed FL-141) | Drive 1HPyFn_0OHf_GFe105uSgvNLUeMebgd8B · 207,592 B · "24.06.18, P's FL-141, Minor, Halsey.pdf"; duplicate id 1iFP412Vy5HuG1X5XA5fl_Q75-9UuASw- | c, d, e |
| 43 | EV-037 [2/2] (L659) | 2025-02-24 | Petitioner's FL-142 Schedule of Assets and Debts, dated 2025-02-24 (97 pages, form body + attachments) — THE 0115 IDENTIFICATION | SWORN (not filed: "THIS FORM SHOULD NOT BE FILED WITH THE COURT") | Drive 1Dak3cT5s6iln1T7SQkc6SALaRxblwl9z · 4,231,887 B (+4 copies) | c, d, e |
| 44 | EV-038 [2/2] (L728) | printed 8/18/26 8:58 AM (filing date 8/7/2026) | LASC PUBLIC CASE SUMMARY — **26STCV25125** (the court's own register) | COURT (court register) | preserved governance/evidence/preserved_2026-08-19/⏎EV-038_LASC_case_summary_26STCV25125_printed_2026-08-18.pdf (191,561 B) | none |
| 45 | WP-001 (L779) | sends 2026-07-28 / 2026-07-29 | Complaint V6 — "Complaint_V6_Minor.docx" | WORK-PRODUCT | Gmail 19fa6d6b84e641f7 · 19faf6086bb922c5 (attachment "Complaint_V6_Minor.docx") | none |
| 46 | WP-002 (L796) | n.s. (gdoc mod 2026-07-09) | §1983 complaint "01 — COMPLAINT (CORRECTED, FULL)" | WORK-PRODUCT | gdoc 1ZaRYi0UDqqxu58SrLaah9qj6FOiAv44i7qKm7oIymWk | police |
| 47 | WP-003 (L802) | n.s. (gdoc mod 2026-06-10) | §1983 complaint "V9 — FEDERAL §1983 COMPLAINT (RECONCILED)" | WORK-PRODUCT | gdoc 1XiRMOD5u-9vbb67j1y718sWZ-uymfjUw8fZbWOr8qXI | police |
| 48 | WP-004 (L807) | n.s. (gdoc mod 2026-07-09) | 1983 FACTS.md — Section A (police package, sourced) | WORK-PRODUCT | gdoc 1w1gArcnH5dypLx30ZKDozQm4yKuSpgP3eJYs6Hv8Fjk | police |
| 49 | WP-005 (L813) | n.s. (gdoc mod 2026-07-10) | 1983 FACTS.md — Sections B & C (keystone email + Kale/BHPD) | WORK-PRODUCT | gdoc 1VWjJQmPt0tdjZsDIT1ifBXIuz0sZ0ExzBhJEh5Y2ctg | police |
| 50 | WP-006 (L818) | 2026-07-30 | BHPD Criminal Report Outline (2026-07-30) | WORK-PRODUCT | gdoc 1UKOpnbqJtKBVtEvv23XtG2SUXcfgFpvIUPL19n-3qfI | police |
| 51 | WP-007 (L825) | n.s. (Drive mod 2026-06-12) | "Google-Gemini — Deletion 100pct Match + Hacking (AI analysis)" | AI-LEAD | Drive 141G5x_ygVrXIn-sUss_C-RdUDTkyEbK1 · 10,579,923 B | a, police |
| 52 | WP-008 (L833) | n.s. (Drive mod 2026-05-31) | "Timeline of Harassment and Interference by Shannon Minor" | WORK-PRODUCT | Drive 15C-dSH5_Ir1AXe2ZxxXbJ-TG77x_JRQE · 45,432 B | none |
| 53 | WP-009 (L838) | n.s. (Drive mod 2026-05-31) | "Forensic Timeline Graphic" | WORK-PRODUCT | Drive 1QDkSmtZjLFsoy5Zfcji6JjDp3inAbSNr · 348,182 B | police |
| 54 | WP-010 (L843) | n.s. | Demand letters — Vanguard college fund misappropriation | WORK-PRODUCT | Step1 Demand pdf 1bgsyCEf6kPFhveHvofuiHWNuA6r3geRA · 180,148 B (+ copy and docx variants) | none |
| 55 | WP-011 (L851) | n.s. | FL300 Vanguard fraud filing packet + declaration | WORK-PRODUCT | packet 18Loz2Nhnz325w2wXGbr5cV3Hr8OUxxRe · Declaration 1xfL8hKFfanxMHLvNTU-ZdNjDdGbk2Xcg · Draft Proposed Order 1Xe-KTA3Na23U-l39oApG5ovX0jmCj_LV | none |
| 56 | WP-012 (L859) | n.s. | Ex parte turnover/freeze motion set (Vanguard account in Shannon's name) | WORK-PRODUCT | MOTION 3 docx 1PRhs02zvk2U_TGoBKi_BSOeHaR3pjhTP · 33,877 B | none |
| 57 | WP-013 (L869) | n.s. | Litigation-hold + subpoena work product to Vanguard | WORK-PRODUCT | Litigation_Hold_Letter_to_Vanguard 1V8i9ngoS0kh_7vwkyWaIRcSg⏎SHX70hyO (id wrapped L870-871) · Litigation_Hold_Vanguard_Enhanced 1u5ZTi3uThH29M2U_nItrETnlY52cTruF | none |
| 58 | WP-014 (L878) | n.s. | "Exhibit_Index_Vanguard_and_WF_Statements.rtf" | WORK-PRODUCT | 1WmYmVlTYAv7A41-HNoOGs2BrOA3arW3x · 1,164 B | none |
| 59 | WP-015 (L884) | 2026-07-25 (title) | "CASE FOUNDATION — VERIFIED FROM PRIMARY DOCUMENTS — 2026-07-25" | WORK-PRODUCT | gdoc 15S3KdnGoZ7pXsH9Ncg7qTgjxUxRJCS0hK04WCR9R_z8 | police |
| 60 | WP-016 (L890) | 2026-07-25 (title) | "CASE FOUNDATION — SUPPLEMENT 01 — Wells Fargo transfers VERIFIED + corrections + Uphold flag — 2026-07-25" | WORK-PRODUCT | gdoc 14Ufi-fT8ze2GT6hSHjr8MrIZm5aSkLRXDCyWZ6DngFM | police |
| 61 | WP-017 (L897) | 2026-07-25 (title) | "CORRECTION — Vanguard 529 recipient = Raymond Nutt / Rochester Ave (NOT Shannon's sister); verified from statement — 2026-07-25" | WORK-PRODUCT | gdoc 1rVCoLHWU1sOyXFuGBQTxDx37r-BgE_KXo1_kJHCd_40 | police |
| 62 | WP-018 (L906) | n.s. | "Minor_v_Minor All-in-One with Exhibit D Vanguard" draft family | WORK-PRODUCT | ≥10 docx variants ("ids in the 2026-08-07 sweep transcript") | none |
| 63 | WP-019 [1/2] (L915) | n.s. (gdoc mod 2026-07-09) | SOURCED FACT REGISTER — Halsey's central fact-adjudication document | WORK-PRODUCT | gdoc 1DIgv6j4tA8BoJHZXlCmxWQHn62D9D5b_CVdtRR2mnRA · parent 1KwJxA9XAOIo6DL5-pvCozRi-5IbEY89n | police |
| 64 | EV-041 (L1007) | 2026-03-27 | Respondent's Brief re service — filed/dated 2026-03-27 | COURT (filed brief) | local upload ef4b2d75-Brief.pdf · 147,896 B · sha256 ebdf5204f88e9af2… (L1015-1016) | c, d |
| 65 | EV-042 (L1022) | 2026-03-27 (executed) | Declaration of Respondent in Support of Brief — executed 2026-03-27 | SWORN | uploads c44bdef5-…_2.pdf and 6accfb51-….pdf · 7,318,891 B · sha256 e22c423b526081bc… (L1035-1036) | a, c, d, exF [fn4], da, police |
| 66 | EV-043 (L1042) | USPS label "JAN 30, 2026"; receipt "24 de febrero" (no year) | Exhibit A — photograph of the bundled delivery (THE DATE ANCHOR) | SWORN (Exhibit A to sworn declaration EV-042; photograph) | none stated in entry (PASS 3 audit note, L1004-1005) | c, police |
| 67 | EV-044 (L1055) | n.s. (contains "February 24, 2024" scrivener's error per L1063) | Exhibit B — Building Manager declaration re receipt of mail | SWORN (Exhibit B declaration; penalty-of-perjury wording n.s. in entry) | none stated in entry | c |
| 68 | EV-045 (L1066) | n.s. (summary of mail to akale@beverlyhills.org) | Exhibit C — Kale / Google preservation record (SUMMARY, not source) | AI-LEAD (Gmail "AI Overview"; C-01 re-tagged it (U), filed as Exhibit C) | none stated in entry | police |
| 69 | EV-046 (L1080) | 2026-04-20 15:43:57Z | California State Bar — submission receipt, 2026-04-20 15:43:57Z | CORRESPONDENCE (institutional: State Bar's own send) | Gmail 19dab900c339a76b | statebar |
| 70 | EV-047 (L1089) | 2026-04-20 15:52:53Z | Notification to DA + federal offices, 2026-04-20 15:52:53Z | CORRESPONDENCE | Gmail 19dab983ae3aa08a | statebar, da, police |
| 71 | EV-048 (L1099) | 2026-04-22 | Contemporaneous characterization, 2026-04-22 (day after the hearing) | CORRESPONDENCE | Gmail 19db7634412cf151 · 19db765c797500a0 | statebar, exF, c, da |
| 72 | WP-020 [1/2] (L1111) | n.s. | "Legal Compliance Violations by Petitioner's Counsel" infographic | WORK-PRODUCT | none stated ("Halsey-supplied chart") | c |
| 73 | EV-049 (L1173) | 2023-09-07 → 2023-10-21 | Google account-recovery notice sequence, Sept–Oct 2023 (THE LOCKOUT) | ACCOUNT (provider: Google notices; institutional) | Gmail 18a70d512865b590 · 18a79cb99e316376 · 18b1891454bc580d · 18b514edd2a06abe | a, police |
| 74 | EV-050 (L1191) | 2023-11-20; 2023-11-28 | Google account recovery completed — 2023-11-20, and the secondary address | ACCOUNT (provider: Google notices; institutional) | Gmail 18bed8e553245b27 · 18bed8e4a4bb39c1 · 18bed8e4a8de5817 · 18c15583f81d5464 (forward 19625f47de243ed8) | a, police |
| 75 | EV-051 (L1207) | 2022-09-14 | Google password change 2022-09-14 — REAL, UNEXPLAINED, NOT A LOCKOUT | ACCOUNT (provider: Google notice) | Gmail 1833ca16271d09ea | a, police |
| 76 | EV-052 (L1219) | 2025-10-16 | Halsey's OWN preservation request to Google — 2025-10-16, and it BOUNCED | CORRESPONDENCE (+ mailer-daemon bounce) | Gmail 199ec75f75e16cd7 · bounce 199ec76298c0a6ff | a [fn5], police |
| 77 | EV-053 (L1232) | 2025-12-05 | GOOGLE LEGAL'S WRITTEN REFUSAL — 2025-12-05 (the §1983 exhibit) | CORRESPONDENCE (provider: Google Legal) | Gmail 19af06ba182f7aa6 (forward 19af167fed51179c) | police |
| 78 | EV-054 (L1255) | 2025-10-22 → 2026-02-12 | The written preservation demands to BHPD — six, dated, 2025-10-22 → 2026-02-12 | CORRESPONDENCE | Gmail 19a09e899cab9e7c · 19af167fed51179c · 19b8f1dd4d7a670c · 19b9f2e529d79fbc · 19ba60583051da79 · 19c5435095e084b7 | police |
| 79 | EV-055 (L1275) | 2026-01-05 | Independent counsel corroborates the legal-process requirement — 2026-01-05 | CORRESPONDENCE | Gmail 19b8f6fcd6f82d0b | police |
| 80 | EV-056 (L1329) | n.s. (covers March 2024 → January 2026) | "Forensic Analysis of Digital Correspondence: The Minor v. Kale Case File (2024-2026)" (THE CROSS-VECTORING EXEMPLAR) | AI-LEAD (AI-assisted, Gemini) | upload 6c56814d-Officer_Kale_Report_Footnoted_v2_2.pdf · sha256 cc2c91bc1b415b0e… (L1336-1337) | a, f, police |
| 81 | EV-057 (L1354) | 2026-06-27 / 2026-08-10 (events) | Chief Max Subin — BHPD leadership change (ORG FACTS, §14 limits) | — (public web org facts; outside listed classes) | beverlyhills.org/m/newsflash/home/⏎detail/161 and /162; beverlypress.com; beverlyhillscourier.com | police |
| 82 | EV-058 (L1373) | 2026-02-13; 2026-03-11 | Kale DA-submission statements — TWO native emails, bodies read in full (THE FORK's Fact A) | CORRESPONDENCE | Gmail 19c548a31edc8c3d · 19cde873a732271b (+ 19cde109aee9e0d8; DA 19bb307ee4795b75) | da, police |
| 83 | EV-059 (L1398) | 2025-09-29; 2025-10-08 | Kale report-date statements — BHPD's own detective twice dates the report to MARCH 2025 and names intake "Officer Carrott" | CORRESPONDENCE | Gmail 19997c42bd4b9c64 · 199c5cbc967a9010 | police |
| 84 | EV-060 (L1419) | 2025-04-01 | Kale case-assignment email — 2025-04-01 (native anchor for the 4/1/2025 assignment) | CORRESPONDENCE | Gmail 195f3970ee2df184 (thread incl. 195fe9941e06c382, 19611abc648f91a8, 19611bdcfde5c78f) | police |
| 85 | EV-061 (L1432) | 2025-12-11 | Kale "Case Update" — search warrant for bank statements, 2025-12-11 | CORRESPONDENCE | Gmail 19b0eaf3f049d381 | police |
| 86 | EV-062 (L1443) | 2025-10-24; 2025-11-05 | Kale case-status and forensics-offer messages (10/24/2025 + 11/5/2025) | CORRESPONDENCE | Gmail 19a13eb82bb6d8fd · 19a5620d5a054560 | police |
| 87 | EV-063 (L1493) | 2026-01-12 | Kale 1/12/2026 — corruption-scheme denial + THE GOOGLE PRESERVATION REQUEST, both accounts (body read in full) | CORRESPONDENCE | Gmail 19bb38cf19aec75b | a, f, police |
| 88 | EV-064 (L1523) | 2025-11-05 | Halsey's contemporaneous memo on the 11/4/2025 Kale call — "DISTURBING; please pass to Police Chief Stainbrook" (body read in full) | CORRESPONDENCE | Gmail 19a53fea7063415c | police |
| 89 | EV-065 (L1568) | 2026-04-17 | The April 17, 2026 formal demand letter to the DA — LOCATED (closes EV-047's open item) | CORRESPONDENCE | Gmail 19d9dd26f4e7242b | a, b, exF, da, police |
| 90 | EV-066 (L1586) | 2026-03-25 → 2026-05-06 | The DA-demand / production series, 3/25/2026 → 5/6/2026 (SET ENTRY — fork Fact B corpus + obligations-ledger natives) | CORRESPONDENCE (set) | Gmail ids at L1590-1616 (e.g., Spiegel-complaint follow-up 19d64940b1e9d860; Cal-Bar "Coloring Book" 19dff13fd9dd8b9b) | statebar, a [fn6], da, police |
| 91 | EV-067 (L1628) | 2022-11-10 / 2022-11-11 | Shannon's contemporaneous acknowledgment of the tax-refund deposit — 11/10-11/2022 WF deposit-hold thread (KNOWLEDGE evidence) | CORRESPONDENCE (+ WF institutional alert) | Gmail 18461348b9fe0954 · 18467dbd3ea6fa47 · 18467dd2c7361b33 · 1846822a40fdff6d · 1846823e63d233ca | a [fn7], police |
| 92 | EV-068 (L1647) | 2023-04-07 | Shannon on the insurance policies, 4/7/2023 — "It's a term policy, they both are" + ~$36k premium due (carrier-file predicate) | CORRESPONDENCE | Gmail thread 1875c1bbb2ae4c3e (msgs 1875c1ebdd8719d1 · 1875ccc96ec41402 · 1875dbd27a787aa9 · 1875e230f7dc3a88) | police |
| 93 | EV-069 (L1665) | 2025-10-13 | The EARLIEST written preservation demand to BHPD found — 10/13/2025 "CALL GOOGLE! YES OR NO" | CORRESPONDENCE | Gmail 199db7e78dd8b1de | a, police |
| 94 | EV-070 (L1683) | n.s. (Drive created 2025-03-29T01:27:00Z) | "Shannon Halsey Analysis Marriage.pdf" — THE 1.5-YEAR EMAIL-CORPUS PDF EXPORT (control set, §7.1) | CORRESPONDENCE (email-corpus export; contents unread) | Drive 14whXxRKHlLpHv4AAFh1E-IBXfBsLcanD · 31,157,062 B | a, police |
| 95 | EV-071 (L1702) | n.s. (Drive created 2025-03-31T02:28:17Z) | "Shannon Halsey Analysis Marriage Complete Email Missing What'sapp.pdf" — THE DOCUMENT THE POLICE-REPORT ANALYSIS EXAMINES | CORRESPONDENCE (email-corpus export; contents unread) | Drive 1IUShpaNYRmKcfehLkfaDDtJZdvoXsVzy · 31,094,269 B | a, exF, police |
| 96 | EV-072 (L1808) | 2026-02-27 | Apple Account password-change notice — 2026-02-27 (W2 window document, institutional) | ACCOUNT (provider: Apple notice; institutional) | Gmail 19ca0e9ad01a16cd | a, police |
| 97 | EV-073 (L1833) | 2022-11-02 | "EMERGENCY" email, 11/2/2022 — seven days before the deposit (destitution belief + the awaited state refund, native) | CORRESPONDENCE | Gmail 18439a5eabf63be3 | police |
| 98 | EV-074 (L1848) | 2022-11-06; 2022-12-13 | Contemporaneous-context natives, Nov-Dec 2022 (set) | CORRESPONDENCE | Gmail 1850da4e115dbb45 · 1844d84b3e8e369f · 1844df7371df95ec | police |
| 99 | WP-021 (L1886) | n.s. (uploaded 2026-08-13) | "Complaint3.pdf" — a SIXTH §1983 complaint version, uploaded by Halsey 2026-08-13 | WORK-PRODUCT | upload 9248ee4c-Complaint3.pdf; matters/03_federal_1983_beverly_hills/consolidation_2026-08-13/ · 224,128 B · sha256 472f8032af7399d6… | police |
| 100 | EV-075 [1/2] (L1908) | 2025-10-01; 2025-11-04; 2025-12-03 | Written preservation demands EARLIER than EV-054's six — three natives (SET) | CORRESPONDENCE | Gmail 1999df6b5ce0fbce · 199db7e78dd8b1de (=EV-069) · 19a4cb0a7fd791b2 · 19ae68bf08204bd5 | a, police |
| 101 | EV-076 [1/2] (L1933) | 2025-07-28 → 2025-10-16 | Deletion-window and discovery natives, Apr–Sep 2025 (SET — the causation spine) | CORRESPONDENCE | Gmail 1984fd6ec53551c4 · 1998c027ef83cc88 · 199ec75f75e16cd7 · 198768bdcb030829 · 1987c51a21963f01 · 198717bc1e84199f (8/3 "Lance Planted Malware...") · 1987c30b472820da | a, f, police |
| 102 | EV-075 [2/2] (L1963) | 2023-07-07 | THE 7/7/2023 EXCHANGE — "your cash problems will soon be over… my funeral" and her same-day reply (THE DECEPTION IN ONE DAY) | CORRESPONDENCE | Gmail 18930a9aa534c917 · 189312a78f6dc42c (thread 189309251612ecb6) | police |
| 103 | EV-076 [2/2] (L1995) | 2023-07-10 / 2023-07-11 | Shannon's 7/10-7/11/2023 messages — "I sent you to rehab to get you help" / "Don't destroy our kids" | CORRESPONDENCE | Gmail 1894190f98311064 · 18942a1f414a6c66 · 18942a8d7a9560e1 | police |
| 104 | EV-077 (L2015) | 2023-08-16 | "Where are you?" — 2023-08-16, subject only, EMPTY BODY | CORRESPONDENCE | Gmail 189ffbe65b4fdf4d | police |
| 105 | EV-078 (L2041) | 2025-10-02 | Halsey's 10/2/2025 narrative to BHPD ("What Is Going To Happen Now") + TWELVE attachments — the account in his own contemporaneous words, and the evidence package delivered | CORRESPONDENCE | Gmail 199a442bb459fce9 | police |
| 106 | EV-079 (L2091) | n.s. (Drive created 2025-09-01; covers July 2022 – August 2023) | "Comparison of Shannon Minor's Emails in PDF vs Gmail (July 2022 – August 2023)" — THE DELETION DOCUMENT (delivered to BHPD 10/2/2025) | WORK-PRODUCT (Halsey-adopted analysis; quotes 17 email bodies) | Drive 1IUm-tR81jO1d788zlS80MbuBGxXm4eHp · 35,898 B; copy 15d5x6yrAHvjV45-H2wzlAVNGELpJemZf | a, police |
| 107 | EV-080 (L2120) | n.s. (transfers 11/22/22-4/3/23; registered 2026-08-12) | THE $255,000 CORRECTION — a SECOND Joyce Flaherty destination account, MUFG Union Bank x0703 (favorable (V) finding his own counsel missed) | WORK-PRODUCT (finding from statement OCR in EV-010/EV-011) | file 21_ (no Drive/Gmail id in entry) | police |
| 108 | EV-081 (L2209) | n.s. | "Shannon Text Messages.pdf" — THE TEXT LAYER, 111 MB (highest-value unread artifact in the matter) | CORRESPONDENCE (text messages; no text layer; unread) | Drive 1K5akFNK4ptlGF5N1dZP1haphrg8gwFas (folder "AA Jell Cell For Lance", L2581); same-size second copy 1ikRSLdaUWGE05M003ixxExDZsW5dJqiY | police |
| 109 | EV-082 (L2223) | exported 2025-05-20 19:11:33 | "iMessages - 2025-05-20 19 11 33 - Shannon Minor.pdf" — 93 MB iMessage export | CORRESPONDENCE (iMessage export; unread) | Drive 1wwlhsowkt1LQ6uUYpOTOYOBeHP4SW0mn | police |
| 110 | EV-083 (L2232) | one dated line "1/9/23 9:36 PM"; otherwise n.s. | "IMessages. Not sure dates. Not many.pdf" — RAW EXCERPT, "page 100 of 214": Shannon's own words, "You are BROKE!" | CORRESPONDENCE (raw transcript page) | Drive 13BwkvjbX10Wov2Idv7ICZV9SJN6Lbh50 | police |
| 111 | EV-084 (L2257) | n.s. (quotes dated 12/10/2022–5/10/2023) | "Shannon Calculated Attempt To Collect Insurance.pdf" + "Shannon Creating Suicide Scenario For Insurance.pdf" — the insurance-motive compilations (DERIVED) | WORK-PRODUCT (DERIVED, Halsey-adopted analysis) | Drive 1jTdwcazhviJh95KBe1b36HX_cxhzntsr · 10T2418e4-r1St53ICmK-AQonibheJ2ZQ | police |
| 112 | EV-085 (L2325) | ledger range 12/19/2013 → 01/09/2023 | THE READABLE SURROGATE — "iMessages … Shannon Minor (Compressed).pdf" (11.6 MB) — 109 ledger rows extracted | CORRESPONDENCE (compressed derivative of EV-082; not hash-verified) | Drive `1Ey5As…` ("full id in file 27_"); matters/04/report_2026-08/27_IMESSAGE_EXPORT_EXTRACTION.md | police |
| 113 | EV-086 (L2340) | n.s. | THE 214-PAGE PARENT — located and resolved; pages 1-100 captured, 101-214 UNREACHED | CORRESPONDENCE (iMessage transcript) | no id in entry (pp.1-100 via EV-085) | police |
| 114 | EV-087 (L2440) | Nov 2022 (content) | THE DUAL-EXPORT "YES MESSAGES" SET — the control set authenticating itself | CORRESPONDENCE (two independently saved email exports) | folder 1Fm9plSUzly10tIpdNqrYtD-PBoOIrBdZ; read 1hdLvGPCBW1TxCjegaRuuQPq294PKMeJk · 1B9rS4E1aTbsjggV8sHO2f0c_7_vXTWvn · 1lpWcvv4NhcPJXclzwxzFXgxHgKka4CFV; unread 1lYhOFHXU9jbKBg_GVw_Jp7aFctaBf-o0 · 1DLVF3_tUYSbV41yx0Rk33jfzFuzaGEJN · 12SxdmRCBLqaRI0wDhZLbZnmVIcJuB7zv | a, exF, police |
| 115 | EV-088 (L2462) | 1/8/2026 | "CONFIDENTIAL FORENSIC AUDIT & PUBLIC CORRUPTION REPORT" (1/8/2026) — READ IN FULL, AND IT HAS THREE CHECKABLE DEFECTS | WORK-PRODUCT (derived audit; AI authorship n.s.) | Drive 1GUx4KFVuaE1OvXdMkBBRo4i53hcFPzFR · 193,440 B; same text 1o28AfWU4R54gaQKyk0P-OrNsjdJ4aULa | a, f, da, police |
| 116 | EV-089 (L2491) | n.s. (verification 2026-08-12) | THE FOUR-ADDRESS FINDING — liveplanet / minorventures / vividlabs ALL deliver into halsey2005@gmail.com | WORK-PRODUCT ("a verification result, not a document") | Gmail 18467dd2c7361b33 · 18454b35eacde372 · 189ff8e8aaeb0f47 · 16413f42f96f7208 | a, d [fn8], e [fn8] |
| 117 | EV-090 (L2513) | 2022-11-04 → 2022-11-07 | THE REFUND THREAD AND ITS THIRD-PARTY HOLDERS — Nardiello / Saliba | CORRESPONDENCE | Gmail thread 1844da95b9cb8766 + 18444ef3ac32ccd3 | police |
| 118 | EV-091 (L2526) | 2022-11-06 | THE CAROL MINETREE THREAD — the deleted message survives inside someone else's reply | CORRESPONDENCE | Gmail thread 1844d84b3e8e369f | a, police |
| 119 | EV-092 (L2587) | captured 2024-07-25; thread 26 Aug 2023 → 13 Jan 2024 | THE WHATSAPP SCREENSHOT CORPUS — 234 files, 656 statement rows, harvested without a single download | CORRESPONDENCE (screenshots via Drive OCR) | Drive folder 1-14wNOUvTP5lQeLyFSIa9yZn4DGsXWp_; matters/04/report_2026-08/25_WHATSAPP_SCREENSHOT_OCR_HARVEST.md | g [fn9], police |
| 120 | EV-093 (L2704) | April 10, 2024 | THE FARMERS POLICY ON HALSEY'S LIFE — the carrier's own letter, and it says $2,000,000 | ACCOUNT (provider: insurance carrier letter) | Drive 1jC10sbsKieuCP3mVaf9hv_AeCLb55rFj · 30,137 B | police |
| 121 | EV-094 (L2740) | April 10, 2024 | THE FARMERS POLICY ON SHANNON'S LIFE | ACCOUNT (provider: insurance carrier letter) | Drive 1kMQuWDQQ6klQhkpV3Ii7uC7pRpZNMngD | police |
| 122 | EV-095 (L2760) | stamps 05/17/2023–09/06/2023 | THE 2023 PASSPORT STAMPS — Bodrum in August, where the email said he would be | WORK-PRODUCT (annotated stamp compilation; outside listed classes) | Drive 1a_iab_mBLny5vBE7qp58Q7kUat-HBgwR | police |
| 123 | EV-096 (L2801) | undated on face | INSTAGRAM DIRECT MESSAGES TO IULIIA MIRONOVA — and the first corpus with a STRUCTURAL attribution basis | CORRESPONDENCE (Instagram DM screenshots) | Drive 1Hy03H8S7DW4FdodqeL1YGDdvh8HrOSGJ | police |
| 124 | EV-097 (L2886) | 2026-03-19 17:47 | THE DA'S "NOT IN OUR SYSTEM" — the fork, documented from both sides | CORRESPONDENCE | Gmail 19d07358d5ac4260 | da, police |
| 125 | EV-098 (L2907) | 2026-01-09 (+ 1/8/2026, 2/4/2026) | KALE'S DENIAL AND THE 567-PAGE CONFIRMATION | CORRESPONDENCE | Gmail 19ba02a9c00c3b61 · 19b9f2badaeb5eeb · 19c27f6dc533be58 | a [fn7], police |
| 126 | EV-099 (L2935) | n.s. (lists emails 12/30/2022–~6/1/2023) | THE SECOND DELETION COMPARISON — better built than EV-079, and it found the balance email | WORK-PRODUCT (comparison exhibit) | Drive 16Xiho9OW-ozxRecJkwhULmjpxg1DmV0Q ("Document (8) copy.docx", folder Hacking) | a, police |
| 127 | WP-019 [2/2] (L3012) | 2026-03-27 (signed) | Respondent's Brief re service/notice, filed ~3/27/2026 (24STFL00432) | DUPLICATE (same file as EV-041 / EV-106 — §7 sha256 check) · COURT (filed brief) | preserved_2026-08-19/WP-019_Respondents_Brief_re_service_⏎2026-03-27.pdf | c, d |
| 128 | WP-020 [2/2] (L3036) | 2026-03-27 (executed) | Declaration of Respondent in support of Brief + Exhibits A-C | DUPLICATE (same file as EV-042 / EV-107 — §7 sha256 check) · SWORN | preserved_2026-08-19/WP-020_Declaration_re_Brief_ExA-C_⏎2026-03-27.pdf | a, c, d, exF [fn4], da |
| 129 | EV-100 (L3080) | 2025-08-29 | THE REVISED ANALYSIS MASTER (2025-08-29) — the prior report, read in full | WORK-PRODUCT (analysis addressed to the AG) | Drive 1LmPSjyZPuFJSmW-GJRBFm5zWd2hnaQq3 (PDF 296,498 B); DOCX 1T_GpQaUJIsnbb1aPGpAL_xsHOstJcstt | police |
| 130 | EV-101 (L3103) | 12/31/2024 | THE 12/31/2024 VANGUARD ANNUAL — the latest statement in existence, read at source | ACCOUNT · DUPLICATE (its Drive id is listed as an EV-033 copy at L422) | Drive 1zyk-4TL5iK6j4AmCbIAY7HgtsTw-XP6g (4,299,446 B) | police |
| 131 | EV-102 (L3119) | Wed 5 Jul 2023 13:50:44 -0700 | THE 7/5/2023 "Re: Pablo" EMAIL — assigned its id (read 2026-08-12, file 31_) | CORRESPONDENCE (email printout, page 632) | Drive 1egJWcqn6XIIYOeZm7qp6WOGp3OyBJfH3 ("Email_HalseyMinor_2023-07-05_⏎page632 2.pdf", folder LANCE FINAL) | police |
| 132 | EV-103 (L3136) | Jul 17 2023 10:04 AM | THE 7/17/2023 COUNTDOWN EMAIL — the September-17 architecture, non-privileged, police-held | CORRESPONDENCE (image in the police-held piece) | EV-036 p.52 | police |
| 133 | EV-104 (L3159) | n.s. (extraction of EV-036 pp.13–54) | THE F50 IMAGE-SECTION EXTRACTION — pp.13–54 text layer, mirrored | WORK-PRODUCT (machine extraction) | 36a_F50_PP13-54_TEXT.md | g [fn9], police |
| 134 | EV-105 (L3217) | content 12–13 Sep 2023; provided 2026-08-23 | THE FIFTEEN DELETED-MESSAGE PLACEHOLDERS — direct-from-client capture, and the bubble-side determination | CORRESPONDENCE (screenshot) | report_2026-08/uploads_2026-08-23/⏎EV-105_fifteen_deleted_placeholders_screenshot.jpg · sha256 edbdae8c09cf… | police |
| 135 | EV-106 (L3252) | 3/27/2026 | RESPONDENT'S BRIEF, 3/27/2026 — the service brief; the appellate-preservation source | DUPLICATE (sha256 ebdf5204f88e… = EV-041) · COURT (filed brief) | uploads_2026-08-23/EV-106_… · sha256 ebdf5204f88e… | c, d, exF |
| 136 | EV-107 (L3268) | 3/27/2026 | DECLARATION OF RESPONDENT, 3/27/2026 (sworn) — the second sworn five-count, and the bundled-delivery record | DUPLICATE (sha256 e22c423b5260… = EV-042) · SWORN | uploads_2026-08-23/EV-107_… ·⏎sha256 e22c423b5260… | a, c, d, exF, da, police |
| 137 | EV-108 (L3368) | FL-300 filed 12/30/2025 | THE §271 SANCTIONS MOTION ITSELF (12/30/2025) — read in full, and it re-frames two things | COURT (filed motion incl. Spiegel's MPA + declaration) | Drive 1r_5T4D4v4lwSbCWU1ZpO--6S9y4nRunT (2,401,413 B) | exF, a, b, f |

Footnotes
- [fn1] EV-005 is tagged c by date only. EV-041 (L1008) and EV-106 (L3255-3257) cite "the Court's 3/2/2026 Minute Order" on service; the index never states that EV-005 is that order.
- [fn2] EV-006: the title says "Collusion". The entry names no counterparty and its contents are unread (L122-126).
- [fn3] EV-020: by title only ("…Compel.Disclosure…", L254).
- [fn4] EV-042 / WP-020 [2/2]: exF via EV-107's separation rule (L3287-3290), which concerns ¶8 of the same file (identical sha256, §7).
- [fn5] EV-052: EV-076 [1/2] item (3) quotes this same letter (199ec75f75e16cd7) for the breach timeframe (L1942-1945).
- [fn6] EV-066: by subject line only ("4/6 JSID cyber-sabotage 19d643ff9dda21bd", L1610).
- [fn7] EV-067 / EV-098: concern the 11/11/2022 email whose deletion is alleged (EV-065 annotation 4; EV-088 Exhibit A). The index records that thread as present live (L1789-1795, L2473-2476, L2929-2930).
- [fn8] EV-089: halsey@minorventures.com, the FL-141 email-service address (L640), is shown delivering into halsey2005@gmail.com. EV-036 [2/2] says the served FL-142 "is NOT present in the halsey2005@gmail.com mailbox" (L655-657).
- [fn9] EV-092 / EV-104: incidental Ally mentions only (L2701-2702; L3166-3169). Nothing concerns a restriction, a writ or a referral.

Class tally (by leading class word): CORRESPONDENCE 52 · WORK-PRODUCT 33 · ACCOUNT 23 · COURT 12 · AI-LEAD 5 · SWORN 5 · DUPLICATE 4 · — 2 · mixed 1 (total 137)

Tag → entries (computed from the table)
- **a** (28): EV-039, WP-007, EV-042, EV-049, EV-050, EV-051, EV-052, EV-056, EV-063, EV-065, EV-066, EV-067, EV-069, EV-070, EV-071, EV-072, EV-075 [1/2], EV-076 [1/2], EV-079, EV-087, EV-088, EV-089, EV-091, EV-098, EV-099, WP-020 [2/2], EV-107, EV-108
- **b** (2): EV-065, EV-108
- **c** (16): EV-001, EV-002, EV-005, EV-018, EV-036 [2/2], EV-037 [2/2], EV-041, EV-042, EV-043, EV-044, EV-048, WP-020 [1/2], WP-019 [2/2], WP-020 [2/2], EV-106, EV-107
- **d** (10): EV-002, EV-036 [2/2], EV-037 [2/2], EV-041, EV-042, EV-089, WP-019 [2/2], WP-020 [2/2], EV-106, EV-107
- **e** (5): EV-020, EV-035 [2/2], EV-036 [2/2], EV-037 [2/2], EV-089
- **f** (8): EV-006, EV-039, EV-040, EV-056, EV-063, EV-076 [1/2], EV-088, EV-108
- **g** (2): EV-092, EV-104
- **exF** (11): EV-003, EV-010, EV-042, EV-048, EV-065, EV-071, EV-087, WP-020 [2/2], EV-106, EV-107, EV-108
- **statebar** (4): EV-046, EV-047, EV-048, EV-066
- **da** (10): EV-042, EV-047, EV-048, EV-058, EV-065, EV-066, EV-088, EV-097, WP-020 [2/2], EV-107
- **police** (106): EV-001, EV-006, EV-007, EV-008, EV-009, EV-010, EV-011, EV-012, EV-014, EV-015, EV-016, EV-017, EV-020, EV-021, EV-023, EV-024, EV-025, EV-026, EV-027, EV-028, EV-029, EV-030, EV-031, EV-032, EV-033, EV-035 [1/2], EV-036 [1/2], EV-037 [1/2], EV-038 [1/2], EV-039, EV-040, WP-002, WP-003, WP-004, WP-005, WP-006, WP-007, WP-009, WP-015, WP-016, WP-017, WP-019 [1/2], EV-042, EV-043, EV-045, EV-047, EV-049, EV-050, EV-051, EV-052, EV-053, EV-054, EV-055, EV-056, EV-057, EV-058, EV-059, EV-060, EV-061, EV-062, EV-063, EV-064, EV-065, EV-066, EV-067, EV-068, EV-069, EV-070, EV-071, EV-072, EV-073, EV-074, WP-021, EV-075 [1/2], EV-076 [1/2], EV-075 [2/2], EV-076 [2/2], EV-077, EV-078, EV-079, EV-080, EV-081, EV-082, EV-083, EV-084, EV-085, EV-086, EV-087, EV-088, EV-090, EV-091, EV-092, EV-093, EV-094, EV-095, EV-096, EV-097, EV-098, EV-099, EV-100, EV-101, EV-102, EV-103, EV-104, EV-105, EV-107
- **none** (14): EV-004, EV-013, EV-019, EV-022, EV-034, EV-038 [2/2], WP-001, WP-008, WP-010, WP-011, WP-012, WP-013, WP-014, WP-018

