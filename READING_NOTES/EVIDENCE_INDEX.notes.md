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

## 3. Verbatim operative text for every entry tagged a, b, c, d, e, f, g, exF or statebar

Each subsection gives the entry's operative lines verbatim (`L<n>:` = index line), then every correction, withdrawal or cross-note in the index that applies to it. Long blocks that apply to several entries are reproduced once, in §3b (B1–B9), and referenced by label. Lines outside the operative range are marked "not reproduced here".

### 3a. Per entry

#### EV-001 (L73) — tags: c, police
Title: Minute order 4/21/2026 — quash/protective order/sanctions DENIED

Operative text (verbatim):
```text
L73: EV-001 · Minute order 4/21/2026 — quash/protective order/sanctions DENIED
L74: - What: 9-page LASC minute order, Halsey's 1/5/2026 motion; the appeal target.
L75: - Original: Drive 1OzBjvKxbhjDXHDq5WlQf9-nFCJnj1dwk · 176,163 B · 2026-06-12.
L76:   Title: "MINUTE ORDER 4-21-2026 — Quash & Protective Order DENIED (APPEAL TARGET).pdf".
L77: - Hash: not computed — Drive id + byte size recorded.
L78: - Tag: (V/Q) — holdings quoted with locators in CANON §3.2(1).
L79: - Used by: FAMILY + POLICE (carries the Marsy's Law/Finkelstein holding the
L80:   criminal activity must argue around — matters/04).
L81: - Notes: 2026-08-07 registered.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-018 cross-reference:
```text
L240: - Hash: not computed. Tag: (X) contents; this is the notice whose service/
L241:   timeliness the quash fight concerned — cross-ref EV-001 (the 4/21/2026
L242:   order, F-01/F-02 corrections).
```

#### EV-002 (L83) — tags: c, d
Title: Minute order 4/21/2026 — defective-service objection DENIED

Operative text (verbatim):
```text
L83: EV-002 · Minute order 4/21/2026 — defective-service objection DENIED
L84: - What: 1-page order; also imposes the standing trackable-mail + electronic
L85:   backstop service order ("the thing he won while losing").
L86: - Original: Drive 1xTtAvLOVwPOvPXzX0xCgqiEQhbKn1zC_ · 103,267 B · 2026-06-12.
L87: - Hash: not computed — Drive id + byte size recorded.
L88: - Tag: (V/Q) — CANON §3.2(2).
L89: - Used by: FAMILY.
L90: - Notes: 2026-08-07 registered. Every Petitioner POS after 4/21/2026 is
L91:   auditable against this order (CANON OPEN-6).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- WP-019 [2/2] notes on this order:
```text
L3025: - Notes: 2026-08-20 registered. EV-002 (4/21/2026 order) is the RULING on
L3026:   this posture: objection DENIED (no appearance by Respondent; court found
L3027:   notice given), BUT the prospective protocol ordered — "trackable method
L3028:   via the mail, and any proof of service shall include tracking details.
L3029:   As a backstop, all service shall also be effectuated by electronic
L3030:   means" — substantially ADOPTS the brief's own proposed protocol.
L3031:   EV-002 read at source 2026-08-20 (Q). Note: the order makes electronic
L3032:   service a mandatory BACKSTOP (supplement), not the sole formal method —
L3033:   the brief's red line. Whether it validly compels e-service on a
L3034:   non-consenting pro se is the preserved appellate question.
```

#### EV-003 (L93) — tags: exF
Title: Minute order 4/21/2026 — Petitioner's §271 sanctions motion

Operative text (verbatim):
```text
L93: EV-003 · Minute order 4/21/2026 — Petitioner's §271 sanctions motion
L94: - What: 3-page order; §271 violation found, amount RESERVED TO TRIAL — no
L95:   dollar amount ordered (KNOWN_FALSE F-06); contains the Exhibit F
L96:   fabrication finding.
L97: - Original: Drive 1hzn_i-t4xCYZ_F5h78NeTLrciWo3jr8m · 107,381 B · 2026-06-12.
L98: - Hash: not computed — Drive id + byte size recorded.
L99: - Tag: (V/Q) — CANON §3.2(3).
L100: - Used by: FAMILY. Notes flag: every activity must KNOW this order exists
L101:   (credibility exposure) without arguing it — see EV-010 title-collision note.
L102: - Notes: 2026-08-07 registered.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-010 title-collision warning:
```text
L168: - Notes: 2026-08-07 registered. **WARNING — title collision:** the fourth
L169:   copy's "Exhibit F" title is NOT the "Exhibit F" the court found fabricated
L170:   in EV-003 (that was six emails signed "Lance"). Never conflate them; verify
L171:   exhibit history at source before using the "Exhibit F" title anywhere.
```
- EV-048 note:
```text
L1108: - Notes: 2026-08-10. Establishes contemporaneous characterization, NOT the
L1109:   authenticity of Exhibit F. Forecloses "objection manufactured after loss."
```
- §7.6 GATE (full text in B1).
- EV-107 separation rule:
```text
L3287: - **SEPARATION RULE (binding for v1):** ¶8's planted-documents claim and
L3288:   the court's Exhibit-F finding are DIFFERENT FACTS — his on-record
L3289:   "narrative summary… was a mistake" explanation (EV-003) and this sworn ¶8
L3290:   are both stated, never merged, never offered as answering each other.
```
- EV-108 on the challenged exhibit:
```text
L3374: - **THE CHALLENGED EXHIBIT, ON ITS FACE:** a chronological "log" of
L3375:   purported Halsey↔"Lance" emails 8/10/2021–7/25/2023 about obtaining his
L3376:   FINANCIAL STATEMENTS — citing FINRA Rule 2231 (a broker-dealer
L3377:   obligation), referencing a "client portal" and "my assistant Janine,"
L3378:   and carrying unfilled generator placeholders ("[User's Name]",
L3379:   "Lance [Last Name]", "[link]"). Spiegel's declaration: not retained
L3380:   until early 2024; never had an assistant named Janine; does not send
L3381:   links. **The document reads as an AI-generated narrative reconstruction
L3382:   with the wrong correspondent name attached — fully consistent BOTH with
L3383:   the court's fabrication finding AND with Halsey's on-record "narrative
L3384:   summary… was a mistake" explanation. v1 states both, adopts neither.**
L3385: - **CONSEQUENCE 1 — §7.6 CONFIRMED FROM THE MOTION ITSELF:** the
L3386:   challenged corpus is purported ATTORNEY correspondence about statement
L3387:   requests; it shares no correspondents and no content with the
L3388:   Halsey↔Shannon export family the report cites. Different set, now
L3389:   verified at the exhibit level, not just the order's description.
```
- EV-003 §271 POSTURE (full text in B2).

#### EV-005 (L112) — tags: c [fn1]
Title: Minute order 3/2/2026 — the control case

Operative text (verbatim):
```text
L112: EV-005 · Minute order 3/2/2026 — the control case
L113: - What: quash motion dismissed; Halsey PRESENT via LACourtConnect, testified;
L114:   reporter Adrian Sosa #15020. Defeats "his equipment is unreliable."
L115: - Original: Drive 1Ts0cxesyYzQTtgfERl22hsJv69Vhetbt · 94,262 B · 2026-06-12.
L116: - Hash: not computed — Drive id + byte size recorded.
L117: - Tag: (V/Q) — CANON §3.3.
L118: - Used by: FAMILY.
L119: - Notes: 2026-08-07 registered.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-041 / EV-106 on "the Court's 3/2/2026 Minute Order":
```text
L1007: EV-041 · Respondent's Brief re service — filed/dated 2026-03-27
L1008: - What: 5-page brief answering the Court's 3/2/2026 Minute Order on service.
… [L1009–L3254 not reproduced here]
L3255: - Holds: the court's own 3/2/2026 order "already recognized that the
L3256:   sanctions RFO could not proceed because the timing required for service
L3257:   to Mexico had not been satisfied"; the 2/24/2026 bundled-delivery
```

#### EV-006 (L121) — tags: f [fn2], police
Title: "Obstruction and Collusion Alex Kale BHPD" compilation

Operative text (verbatim):
```text
L121: EV-006 · "Obstruction and Collusion Alex Kale BHPD" compilation
L122: - What: PDF concerning the investigation's conduct (contents unread this
L123:   session).
L124: - Original: Drive 1hUri1DiIBpecVmzitBGbS5zypo5gpBsZ · 5,488,747 B · 2026-05-31.
L125: - Hash: not computed — Drive id + byte size recorded.
L126: - Tag: (X) — existence verified; contents not read at source this session.
L127: - Used by: **1983-ONLY** (system conduct — firewall).
L128: - Notes: 2026-08-07 registered.
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-010 (L154) — tags: exF, police
Title: "Sent to Police — 500 Emails & iMessages Timeline" (~24.5 MB corpus)

Operative text (verbatim):
```text
L154: EV-010 · "Sent to Police — 500 Emails & iMessages Timeline" (~24.5 MB corpus)
L155: - What: the evidence compilation sent to police (500 emails/iMessages,
L156:   optimized timeline) — proves the telling AND carries the underlying acts.
L157: - Original (PRIMARY): Drive 1MoppowLgTb6nAP_870wGrx1RpUtkSz0t · 24,470,497 B
L158:   · 2026-06-12 (police folder, curated title).
L159: - Copies, identical byte size 24,470,497 (I — same document inferred from
L160:   exact size match; contents not byte-diffed):
L161:   1AnYe1K2zNI15KuJYBbBRwiPqfpSWMIrT (2026-05-31);
L162:   1zAEmGznJuqt85Q8JZHWLOkKQCR8Tlskf ("...Timeline 2", 2026-05-31);
L163:   1LBJ3AZftEJHCd-B069ZuNOhB3m89o5zE (2026-05-31, titled "Exhibit F Analysis
L164:   of Evidence...").
L165: - Hash: not computed — Drive ids + byte size recorded.
L166: - Tag: (X) as to contents this session; sent-to-police status (U/V — CANON §7).
L167: - Used by: CIVIL + POLICE + 1983.
L168: - Notes: 2026-08-07 registered. **WARNING — title collision:** the fourth
L169:   copy's "Exhibit F" title is NOT the "Exhibit F" the court found fabricated
L170:   in EV-003 (that was six emails signed "Lance"). Never conflate them; verify
L171:   exhibit history at source before using the "Exhibit F" title anywhere.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EVIDENTIARY-WEAKNESS NOTE 1:
```text
L2167: 1. **EV-010 is misnamed.** Titled "Sent to Police — 500 Emails & iMessages
L2168:    Timeline," its actual content is an ANALYSIS of EV-071 plus the
L2169:    Provinziano letter plus ~76% Wells Fargo statement OCR. Searches for
L2170:    From:/To:/Subject:/Sent:/iMessage return ZERO. **There is no message
L2171:    corpus inside it.** Every message quote in it is a quotation-within-an-
L2172:    advocacy-document, not a native. The 500-message corpus is therefore
L2173:    still UNLOCATED as a native set — it is a hunt target, and its absence
L2174:    explains why the text-layer evidence keeps coming up short.
```
- §7.6 GATE disambiguation rule:
```text
L3209: Exhibit F pages from the 11/12/25 RFO (the Drive "Exhibit Tab F" files are
L3210: divider pages only). **DISAMBIGUATION RULE: the police package's own
L3211: "Exhibit F" (the 24.5MB 500-emails timeline) is a DIFFERENT DOCUMENT from
L3212: the court's Exhibit F — v1 renames its exhibit references to avoid the
L3213: collision.**
```

#### EV-018 (L237) — tags: c
Title: 2024-10-31 Notice to Consumer — WF documents subpoena

Operative text (verbatim):
```text
L237: EV-018 · 2024-10-31 Notice to Consumer — WF documents subpoena
L238: - Original: Drive 1zJmKPJ7IzI_ggIPCdFaMWv7jFQixxs_Q · 1,514,921 B ·
L239:   2026-05-31. Title: "2024-10-31 [P] Ntc.Cons.Doc.Subp.Wells.Fargo.Bank.N.A".
L240: - Hash: not computed. Tag: (X) contents; this is the notice whose service/
L241:   timeliness the quash fight concerned — cross-ref EV-001 (the 4/21/2026
L242:   order, F-01/F-02 corrections).
L243: - Used by: FAMILY + CIVIL.
L244: - Notes: 2026-08-07 registered.
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-020 (L251) — tags: e [fn3], police
Title: 2025-12-29 Respondent RFO — $400,000 Vanguard, compel/tracing/ preservation/sanctions

Operative text (verbatim):
```text
L251: EV-020 · 2025-12-29 Respondent RFO — $400,000 Vanguard, compel/tracing/
L252: preservation/sanctions
L253: - Original (PRIMARY): Drive 1m4MH5NALnVoBqmtOdr8QvEpan4Q_bIMt · 4,069,611 B
L254:   · title "2025-12-29 [P] Resp.RFO.$400,000.Vanguard.Compel.Disclosure.
L255:   Tracing.Preservation.Sanctions.pdf".
L256: - Copies, identical byte size 4,069,611 (I — same document by exact size):
L257:   1bTkGX3SUFZdA7TC3yv53uvOm-ZlwwB4x · 1SvLI2RTWERuqhzS6vZm-bFjWN5et6_kK ·
L258:   1egaSQ2H5gm2DTiVfMh_7Ejx3TCVQ29GA · 1gSZOaRPTl2gj7RSnTHjEDEDYGTfM87jx ·
L259:   10nyevU9zTKWkU9gHrQQKWI0PmM9mLahz (6 total).
L260: - Hash: not computed. Tag: (X) contents; court-record filing per title.
L261:   Used by: FAMILY + CIVIL + POLICE.
L262: - Notes: 2026-08-07 registered. Likely the 11/12/25-posture $400K fund
L263:   fight in filed form — read at source before citing (X).
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-039 (L552) — tags: a, f, police — class AI-LEAD
Title: "Forensic Analysis of Digital Correspondence: Minor v. Kale Case File (2024–2026)" — Halsey↔Kale reconstruction + Triangle-of-Corruption hypothesis

Operative text (verbatim):
```text
L552: EV-039 · "Forensic Analysis of Digital Correspondence: Minor v. Kale Case File
L553: (2024–2026)" — Halsey↔Kale reconstruction + Triangle-of-Corruption hypothesis
L554: - What: 11-page work-product/AI-assisted reconstruction of the ~2-year Halsey–
L555:   Det. Kale email history, plus the leak/"Scalpel"/insider-knowledge/Spiegel-
L556:   collusion theory, Marsy's dashboard metrics, and a 1-in-10B statistic.
L557: - Original: session upload 424a7e16-Email_History_Analysis_Request_11.pdf ·
L558:   231.6 KB · sha256 06cc958528baa95b7238570be464d4a1f7aad147612a3d708fc5ebc84
L559:   a99fa55 (copy in report_2026-08/). Cites Halsey's Drive doc
L560:   13A21iC1ltJN27HExxsNZlKJoXlZxZjvz186aomuyLKA ("Empirical Analysis of
L561:   Evidence Spoliation" — L, unverified).
L562: - Tag: (I/X) — AI-derived reconstruction; its email date-stamps are Halsey's
L563:   characterizations, NOT re-sourced to native Gmail this session. Underlying
L564:   Kale emails must be pulled before any date/quote ships.
L565: - Used by: **1983-ONLY as argument** (system-conduct/leak/corruption). POLICE
L566:   use limited to OBJECTIVE notice/escalation facts re-sourced to natives
L567:   (reporting dates 3/29/2024 + 3/29/2025; Kale assignment 4/1/2025; warrant +
L568:   Shannon interview 12/11/2025; Joyce interview ~1/7/2026; TURKEY collision +
L569:   $1.13M per 5/2025 TSC witness notice; insurance $4.5M). See firewall note,
L570:   report_2026-08/08_INTAKE.
L571: - Notes: 2026-08-10 registered.
L572: - Note appended 2026-08-10 (conforming, OP.COND. §§8/10 + ADDENDUM §3): this
L573:   is a Halsey-ADOPTED document and therefore a SOURCE — at minimum (U), his
L574:   account (§8.1); the (I/X) tag above states verification level only, never
L575:   legitimacy. The "1983-ONLY as argument" line is a CLASSIFICATION under
L576:   ADDENDUM §3 (legal-theory material vs factual history), not my submission
L577:   ruling — what enters any packet is Halsey's call. Tests owed: date-stamps
L578:   vs the native Kale emails; the 1-in-10B figure's method per OP.COND. §7.5.
L579:   The "3/29/2024 first report" line: K-01 test found no 2024 preservation
L580:   email in the mailbox; year untested against a native.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- WP-019 [1/2] key correction #17:
```text
L937:   DROP "$2.5M" total, theft spine = $1,134,000; (#17) report date ~3/24/2025
L938:   (Kale email) + 3/29/2025 counsel letter — EV-039's "3/29/2024" unverified;
```
- C-04 standing rule:
```text
L1167: **C-04 · STANDING RULE for this index.** No future entry is tagged (X), "not a
L1168: source," or "roadmap only" on the ground that an AI, calculator, dashboard, or
L1169: assistant produced it. Where verification is incomplete, write exactly what is
L1170: unverified and against which record — never a status label that reads as
L1171: disqualification. (X) keeps its narrow meaning only: OPERATING_CONDITIONS §7.4.
```
- CONVERSION BLOCK standing rule:
```text
L1322: **STANDING RULE FOR THIS INDEX (replaces C-04's framing, keeps its substance):**
L1323: Every item enters. The Tag line records what has been TESTED and against what
L1324: — never whether the item is permitted. No entry is ever refused, removed, or
L1325: labelled unusable because of how it was produced or because a test is still
L1326: owed. Where I believe something is wrong, I say so once, in the Notes, with the
L1327: evidence — as a finding for Halsey to weigh, not a ruling.
```
- ANNOTATIONS 2026-08-12 item 2 (EV-039 interview date corrected):
```text
L1741: 2. JOYCE FLAHERTY INTERVIEW DATE NATIVE-SOURCED: register #18 email
L1742:    19ba02a9c00c3b61 body read in full. Kale, 2026-01-09 (Q): "For your
L1743:    knowledge, I did interview Joyce Flaherty yesterday. That is a case
L1744:    update for you." → interview = 2026-01-08, from the detective's own
L1745:    email (EV-039's "~1/7/2026" corrected to 1/8). Also (Q): "we have the
```

#### EV-040 (L582) — tags: f, police
Title: "Beverly Hills PD — Marsy's Law Dashboard / IA Referral" (2 images)

Operative text (verbatim):
```text
L582: EV-040 · "Beverly Hills PD — Marsy's Law Dashboard / IA Referral" (2 images)
L583: - What: §1983 internal-affairs-referral / Marsy's-Law-compliance infographic
L584:   (682 days in violation; 10/14 rights; 150+ emails / 0.67% response; 654 days
L585:   to Google; 1-in-10B; Triangle of Corruption; 11-official non-response
L586:   scorecard naming Kale, Dimond, Stainbrook (Chief), Weiner, Nazarian,
L587:   Hunt-Coffey, Coulter, Albanese).
L588: - Original: session upload 8792128e-Beverly_Hills_PD__Marsy_s_Law_Dashboard_
L589:   copy.pdf · 624 KB · sha256 73de442a765408ee5b1c82bd9fbc0de99ad152d402f8ffe57
L590:   5535cfd19b11b83 (copy in report_2026-08/); two page-images also pasted inline.
L591: - Tag: (I/X) — derived infographic; metrics unverified at source.
L592: - Used by: **1983-ONLY.** POLICE use limited to identity/contact facts (Chief
L593:   = Stainbrook, now fired; "Hunt-Coffey" = the hard-bounced nhuntcoffey addr,
L594:   NEVER email). Corruption metrics do NOT enter the police report (firewall).
L595: - Notes: 2026-08-10 registered.
L596: - Note appended 2026-08-10 (conforming, OP.COND. §§8/10 + ADDENDUM §3):
L597:   Halsey-adopted → a SOURCE, at minimum (U) (§8.1). "Do NOT enter the police
L598:   report" above is withdrawn as my phrasing; the operative rule is ADDENDUM
L599:   §3's classification (§1983 legal-theory material barred from the packet;
L600:   underlying facts permitted as case history) and the submission call is
L601:   Halsey's. Tests owed: the day-count metrics' input years (K-01: 654 vs 289
L602:   — arithmetic verified, first-request year untested); the response-rate and
L603:   rights-violated tallies against the native request/response record.
L604:   Count note: written preservation demands = at least five (EV-054/K-06).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- CONVERSION BLOCK opening (prohibitions withdrawn):
```text
L1302: ## CONVERSION BLOCK — 2026-08-10 · prohibitions become annotations (append-only)
L1303: Governed by OPERATING_CONDITIONS §10. Everywhere in this repo I wrote "do not
L1304: plead," "not pleadable," "fenced," "gated," or "does not go in this packet,"
L1305: **that was a submission ruling I had no standing to make.** Those words are
L1306: withdrawn wherever they appear. The items below are IN THE RECORD. Each carries
L1307: its tested status and the specific test still owed. **The decision to use any
L1308: of them is Halsey's.**
```

#### EV-035 [2/2] (L606) — tags: e
Title: FL-100 Petition for Dissolution — Shannon Minor, filed 2026-01-16… (see date below)

Operative text (verbatim):
```text
L606: EV-035 · FL-100 Petition for Dissolution — Shannon Minor, filed 2026-01-16… (see date below)
L607: - What: Petition (FL-100), Petitioner SHANNON MINOR by LANCE S. SPIEGEL (SBN
L608:   51625), Young, Spiegel & Hosp LLP. READ AT SOURCE 2026-08-19.
L609: - Key contents (Q, transcribed exactly): file stamp "Electronically FILED by
L610:   Superior Court of California, County of Los Angeles 1/16/2024 9:23 AM David
L611:   W. Slayton, Executive Officer/Clerk of Court, By J. Esplana, Deputy Clerk
L612:   24STFL00432"; "Assigned for all purposes to: Ryan D. White, (Department,
L613:   ST23)"; signed by Shannon Minor 1/11/2024 under penalty of perjury. Date of
L614:   marriage 06/27/2006; date of separation 08/02/2023; 17 years 2 months.
L615:   Children: Grace Caroline Minor 12/18/2007; James Easton Minor 05/04/2011;
L616:   William Henry Minor 05/04/2011; Charlotte Elizabeth Minor 07/08/2012.
L617:   Item 10a marked X: "There are no such assets or debts that I know of to be
L618:   divided by the court" (COMMUNITY AND QUASI-COMMUNITY PROPERTY). Item 11c
L619:   requests "An order that the Prenuptial Agreement dated June 23, 2006 is
L620:   valid and enforceable." The word "AMENDED" appears near the case number —
L621:   whether this copy is an amended petition is (X), unresolved.
L622: - Original: Drive 1nq6ua7mClA6wjeQbdV6Vbj3tRr3oi7ln · 506,941 B · title
L623:   "24.01.16, P's FL-100, Minor, Halsey.pdf". Duplicate id
L624:   1Q-OEYJ0836EXwE9iWgj7-_SnDScwfhtk (same size).
L625: - Hash: not computed — Drive id + byte size recorded.
L626: - Tag: (V/Q) — read at source 2026-08-19; checkbox marks on a garbled OCR
L627:   layout for items 9/10 read with care, item 10a legible as marked.
L628: - Used by: FAMILY + CIVIL.
L629: - Notes: 2026-08-19 registered. Item 11c CORROBORATES complaint [P012]
L630:   ("neither party has contested the validity of the agreement") from
L631:   Petitioner's own sworn filing. Item 10a is the sworn no-community-assets
L632:   statement made 1/11/2024.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- 2026-08-27b duplicate-id rules (full text in B8).

#### EV-036 [2/2] (L634) — tags: c, d, e
Title: Petitioner's FL-141 — Declaration re service of Preliminary Declaration of Disclosure, filed 6/18/2024

Operative text (verbatim):
```text
L634: EV-036 · Petitioner's FL-141 — Declaration re service of Preliminary
L635: Declaration of Disclosure, filed 6/18/2024
L636: - What: FL-141 by Young, Spiegel & Hosp for PETITIONER SHANNON MINOR. Boxes
L637:   marked: Petitioner's · Preliminary. Item 2 states the Preliminary
L638:   Declaration of Disclosure (FL-140), current FL-150, and completed Schedule
L639:   of Assets and Debts (FL-142) "were served on: (date): June 18, 2024",
L640:   service method Email to halsey@minorventures.com. Item 3 (FINAL declaration
L641:   of disclosure) is BLANK — no final disclosure declared served as of this
L642:   form. Declared under penalty of perjury by Anna Kralle, June 18, 2024.
L643: - Original: Drive 1HPyFn_0OHf_GFe105uSgvNLUeMebgd8B · 207,592 B · title
L644:   "24.06.18, P's FL-141, Minor, Halsey.pdf". Duplicate id
L645:   1iFP412Vy5HuG1X5XA5fl_Q75-9UuASw-.
L646: - Hash: not computed. Tag: (V/Q) — read at source 2026-08-19.
L647: - Used by: FAMILY + CIVIL.
L648: - Notes: 2026-08-19 registered. COMPUTATION (I, from EV-035 + EV-036): petition
L649:   filed 1/16/2024; preliminary disclosure served 6/18/2024 = 154 days; a
L650:   60-day service requirement would have expired 3/16/2024, making service 94
L651:   days late. The 60-day rule (Fam. Code § 2104(f)) has NOT been read at
L652:   source — leginfo is blocked by this environment's egress proxy — so the
L653:   RULE is (X) while the two DATES are (V). Halsey confirms (U) he consented
L654:   to service by email, so the email service method is not in dispute.
L655:   The FL-142 itself is never filed with the court (the form so states); it
L656:   was served to halsey@minorventures.com and is NOT present in the
L657:   halsey2005@gmail.com mailbox (V — searched 2026-08-19).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- WP-020 [1/2] / C-03 / K-08 on the "Anna Kralle" surname:
```text
L1114: - Tag: (U/X) work product. **NOT FILING-READY — defects recorded 2026-08-10:**
L1115:   "Anna Kralle" surname unverified (only AnnaK@ is (V)); "Matt" vs the
L1116:   record's "Matthew" Sirriyeh; the 57/43 split states no denominator; bar
… [L1117–L1155 not reproduced here]
L1156: - **Kept, because they are checkable and he would want them caught:** "Anna
L1157:   Kralle" surname is unverified (only AnnaK@ is (V)); the record shows
L1158:   "Matthew" Sirriyeh, not "Matt"; the 57/43 split states no denominator; the
… [L1159–L1318 not reproduced here]
L1319: | K-08 | **WP-020 infographic** | IN as his adopted work product (already converted at C-03). | Verify the "Anna Kralle" surname and the 57/43 denominator. | Only AnnaK@ is verified; record shows "Matthew" Sirriyeh. Two checkable fixes, not a verdict. |
```
- EV-089 alias-delivery finding and its stated limit:
```text
L2491: EV-089 · THE FOUR-ADDRESS FINDING — liveplanet / minorventures / vividlabs ALL deliver into halsey2005@gmail.com
L2492: - What: a verification result, not a document. Messages exist in
L2493:   halsey2005@gmail.com with that address in **neither To nor Cc**:
L2494:   `18467dd2c7361b33` (To: halsey@minorventures.com only, no Cc);
L2495:   `18454b35eacde372` (To: minorventures; Cc: chad/dan/liveplanet);
L2496:   `189ff8e8aaeb0f47` (To: liveplanet + minorventures);
… [L2497–L2506 not reproduced here]
L2507: - **LIMIT, stated:** this proves alias mail is DELIVERED here. It does not
L2508:   prove the mailbox retains everything delivered — which is the allegation
L2509:   itself. Alias delivery makes an absence test meaningful; it does not make
L2510:   any particular absence innocent or guilty.
```
- WP-020 [2/2] consent-scope consistency flag:
```text
L3051: - Notes: 2026-08-20 registered. Feeds SERVICE_VIOLATIONS_LOG rows (the
L3052:   2/24/2026 bundled-delivery event now has sworn + photographic + witness
L3053:   locators). CONSISTENCY FLAG for future filings: Halsey stated in-session
L3054:   2026-08-19 (U) that he "consented to initial service by email ... so we
L3055:   could exchange documents" — reconcilable with ¶3 (scope: informal
L3056:   exchange vs formal e-service, no EFS-005-CV) but every future filing
L3057:   should state the consent scope identically to avoid impeachment.
```
- EV-003 POSTURE on email-service rights and disclosures:
```text
L3412: non-conforming Mexico-mail-service method such that in "~7 motions" he never
L3413: saw the motions before they were heard; that he was "held to the US time
L3414: clock" though in Mexico; that he was then required to give up email-service
L3415: rights after the 5-page brief he demanded (EV-106) exposed the problem; and
L3416: that he did not receive Petitioner's initial financial disclosures, which the
L3417: court permitted. He states he contacted the California State Bar about
```
- 2026-08-27b duplicate-id rules (full text in B8).

#### EV-037 [2/2] (L659) — tags: c, d, e
Title: Petitioner's FL-142 Schedule of Assets and Debts, dated 2025-02-24 (97 pages, form body + attachments) — THE 0115 IDENTIFICATION

Operative text (verbatim):
```text
L659: EV-037 · Petitioner's FL-142 Schedule of Assets and Debts, dated 2025-02-24
L660: (97 pages, form body + attachments) — THE 0115 IDENTIFICATION
L661: - What: Shannon Minor's Schedule of Assets and Debts by Young, Spiegel & Hosp.
L662:   Header banner "THIS FORM SHOULD NOT BE FILED WITH THE COURT"; no court file
L663:   stamp anywhere on its face. Read at source 2026-08-19, all 97 pages.
L664: - Original: Drive 1Dak3cT5s6iln1T7SQkc6SALaRxblwl9z · 4,231,887 B. Copies:
L665:   10QdLF7WNpkXFUdOTplanSYtFqjwKzWL6 · 1mB-QU6D9Lt8Vxq9zckQBU-s3skny0e40 ·
L666:   1opjWR98Lz_7tsktrnbZby6QQqyCnHbUb · 1WwEjL9zFx-wO9rQfDMT3tkFIXfy84Hna.
L667: - Tag: (V/Q) — quoted with page locators below.
L668: - Used by: CIVIL + FAMILY.
L669: - KEY CONTENTS (Q, page locators are PDF pages of this file):
L670:   * p.8 and p.17 (duplicate filing of the same WF statement, period 1/1/2025-
L671:     1/31/2025): account holders printed under "Account number: [redacted]0890
L672:     (primary account)" are "SHANNON A MINOR" and "JOYCE FLAHERTY". Mailing
L673:     block p.6/p.15: SHANNON A MINOR / JOYCE FLAHERTY / 350 S SPALDING DR
L674:     UNIT 7 / BEVERLY HILLS CA 90212-3634.
L675:   * p.8/p.17, "Overdraft Protection — Your account is linked to the
L676:     following": "Savings - [redacted]0115".
L677:   * p.8/p.17 transaction line: "Online Transfer From Flaherty J Savings
L678:     Xxxxxx0115 Ref #Ib0Qvvbv5D On 01/08/25", amount 50,000.00, running
L679:     balance 78,039.26. 0890 balances: 1/1 39,296.53; deposits 61,780.06;
L680:     withdrawals -65,524.99; 1/31 $35,551.60.
L681:     => 0115 is a WELLS FARGO SAVINGS account described as "Flaherty J",
L682:     linked to 0890 for overdraft. NOTE (V): no holder NAME field for 0115
L683:     appears; the only naming is descriptive inside the transaction text.
L684:   * Item 6 CHECKING (p.2): WF X0890 P 05/28/2010 35,551 / 0; X4249 P
L685:     06/07/2024 906; X4215 P 06/07/2024 668; X5631 P 07/19/2021 464.
L686:     Item 5 SAVINGS: X1074 (Sep.Prop. blank) 06/13/2016 101; X1530 P 419.
L687:   * Item 16 OTHER ASSETS (p.3): VANGUARD 529 X0245-01 FTBO GRACE C. MINOR
L688:     2015 197,701; -02 FTBO JAMES E. MINOR 2015 197,862; -03 FTBO WILLIAM H.
L689:     MINOR 2015 197,862; -04 FTBO CHARLOTTE E. MINOR 2015 197,862.
L690:   * Item 10 LIFE INSURANCE (p.3), FOUR policies, all "NO CASH VALUE":
L691:     FARMERS TERM LIFE X9383 P 10/02/2018; BRIGHTHOUSE TERM LIFE X24UT P
L692:     05/02/2017; FARMERS TERM LIFE X1056 (blank) 04/18/2019; BRIGHTHOUSE
L693:     TERM LIFE X21UT (blank) 05/02/2017. ** First named carriers for the
L694:     life-insurance allegations at [P002]/[P033]/[P035]. Whose lives these
L695:     insure is NOT stated on the form — (X). **
L696:   * Item 4 VEHICLES (p.2): "2023 MERCEDES EQS (LEASED)", all columns N/A.
L697:     Relates to [P029].
L698:   * Item 23 CREDIT CARDS (p.4), five: AMERICAN EXPRESS X13002 P 21,195 AS OF
L699:     02/12/2025; AMERICAN EXPRESS X44001 P 4,054 AS OF 02/17/2025; CAPITAL ONE
L700:     X8655 P 13,704 AS OF 02/07/2025; CHASE X7496 P 33,605 AS OF 02/02/2025;
L701:     CITI X6730 P 43,195 AS OF 02/10/2025. TOTAL 115,753 (computed).
L702:   * p.4 signed under penalty of perjury, "FEBRUARY 24, 2025", SHANNON MINOR,
L703:     DocuSign. Envelope ID as printed: 0E5BC6D0-6765-4FEE-986F-DD8678AEF5.
L704:   * p.97 PROOF OF SERVICE: served February 24, 2025 BY ELECTRONIC
L705:     COMMUNICATION on Alphonse F. Provinziano, Provinziano & Associates
L706:     (al@provinziano.com / service@provinziano.com), from mvs@ysfamilylaw.com,
L707:     executed by MATTHEW SIRRIYEH. => the Feb 2025 SAD went to Halsey's THEN
L708:     COUNSEL, not to him — it should exist in the Provinziano client file.
L709:   * PDF metadata (not page face): created D:20250224215037-08'00', author MVS.
L710: - NEGATIVE FINDINGS (V — all 97 pages read):
L711:   * NO transfer of $100,000 anywhere; NO $50,000 transfer dated on/about
L712:     2022-11-22. The string "2022" does not appear in the document at all.
L713:     ** The transfers pleaded at [P021] are NOT sourced from this document.
L714:     Their source must be identified before [P021] is relied on — candidate
L715:     EV-025 "Exhibit C - WF x0890 statements". **
L716:   * The prior pass's "0115" hits on pp.69/71 were FALSE POSITIVES — substring
L717:     of merchant reference "FACTS TUITION AND FEES 084870011599979" on an
L718:     American Express statement. Corrected here.
L719: - CROSS-FORM DISCREPANCY (I, computed): her FL-150 signed 1/7/2025 lists five
L720:   cards totaling 144,328 (ELITE MASTERCARD 37,267; CAPITAL ONE 10,579; CHASE
L721:   SAPPHIRE 36,220; AMERICAN EXPRESS 28,173; AMERICAN EXPRESS 32,089). This
L722:   FL-142 signed 2/24/2025 lists five cards totaling 115,753 — a 28,575 drop in
L723:   ~6 weeks. "ELITE MASTERCARD" appears only on the FL-150; "CITI" only on the
L724:   FL-142. Both are sworn. May be innocent renaming/paydown — DO NOT plead as
L725:   concealment until reconciled at source.
L726: - Notes: 2026-08-19 registered.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- CONVERSION BLOCK (dated 2026-08-10) withdrawing "do not plead" wording; this entry was registered 2026-08-19:
```text
L1302: ## CONVERSION BLOCK — 2026-08-10 · prohibitions become annotations (append-only)
L1303: Governed by OPERATING_CONDITIONS §10. Everywhere in this repo I wrote "do not
L1304: plead," "not pleadable," "fenced," "gated," or "does not go in this packet,"
L1305: **that was a submission ruling I had no standing to make.** Those words are
L1306: withdrawn wherever they appear. The items below are IN THE RECORD. Each carries
L1307: its tested status and the specific test still owed. **The decision to use any
L1308: of them is Halsey's.**
```
- 2026-08-27b duplicate-id rules (full text in B8).

#### WP-007 (L825) — tags: a, police — class AI-LEAD
Title: "Google-Gemini — Deletion 100pct Match + Hacking (AI analysis)"

Operative text (verbatim):
```text
L825: WP-007 · "Google-Gemini — Deletion 100pct Match + Hacking (AI analysis)"
L826: - What: AI-generated analysis of deletion/spoliation and hacking indicators.
L827: - Original: Drive 141G5x_ygVrXIn-sUss_C-RdUDTkyEbK1 · 10,579,923 B ·
L828:   2026-06-12 (Google-spoliation folder). Tag (I/X — AI-derived; its
L829:   underlying artifacts must be sourced independently before anything it says
L830:   is used). Used by: CIVIL + POLICE + 1983 (analysis-support only).
L831: - Notes: 2026-08-07 registered.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- C-04 standing rule:
```text
L1167: **C-04 · STANDING RULE for this index.** No future entry is tagged (X), "not a
L1168: source," or "roadmap only" on the ground that an AI, calculator, dashboard, or
L1169: assistant produced it. Where verification is incomplete, write exactly what is
L1170: unverified and against which record — never a status label that reads as
L1171: disqualification. (X) keeps its narrow meaning only: OPERATING_CONDITIONS §7.4.
```

#### EV-041 (L1007) — tags: c, d
Title: Respondent's Brief re service — filed/dated 2026-03-27

Operative text (verbatim):
```text
L1007: EV-041 · Respondent's Brief re service — filed/dated 2026-03-27
L1008: - What: 5-page brief answering the Court's 3/2/2026 Minute Order on service.
L1009:   Holdings: CRC 5.92(f)(3) routes post-appearance RFOs to CCP §1010 et seq.;
L1010:   Mexico has OBJECTED to Hague Art. 10 postal channels (Water Splash);
L1011:   CCP §1005(b) adds 20 calendar days for foreign addresses; mail service here
L1012:   was not proper (Mullane/Jones/Peralta); no retroactive validation; no
L1013:   unconsented email as sole formal service. Conclusion ¶4 EXPRESSLY PRESERVES
L1014:   appellate review under CRC 8.104 / CCP §904.1 and all CCP §473(d) rights.
L1015: - Original: local upload ef4b2d75-Brief.pdf · 147,896 B · sha256
L1016:   ebdf5204f88e9af20990115707fa4a41ba6e09fd48e22fc6d689924981193815.
L1017:   AES-128 encrypted, empty user password; text extracted and read in full.
L1018: - Tag: (V) text read at source this session. Used by: FAMILY (+CIVIL context).
L1019: - Notes: 2026-08-10. Bears on CANON NC-1/OPEN-1 — preservation, not answer.
L1020:   DURABLE MIRROR NEEDED: local upload only.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- same file registered again as WP-019 [2/2] and EV-106 (identical sha256, §7):
```text
L3012: WP-019 · Respondent's Brief re service/notice, filed ~3/27/2026 (24STFL00432)
… [L3013–L3021 not reproduced here]
L3022: - Preserved: preserved_2026-08-19/WP-019_Respondents_Brief_re_service_
L3023:   2026-03-27.pdf. Tag (U/Q — his filing; court-file conformed copy not
L3024:   in hand). Used by: FAMILY (+CIVIL context).
… [L3025–L3251 not reproduced here]
L3252: EV-106 · RESPONDENT'S BRIEF, 3/27/2026 — the service brief; the appellate-preservation source
L3253: - What: 5-page filed brief (24STFL00432), read IN FULL 2026-08-23. Mirror:
L3254:   uploads_2026-08-23/EV-106_… · sha256 ebdf5204f88e…
```

#### EV-042 (L1022) — tags: a, c, d, exF [fn4], da, police
Title: Declaration of Respondent in Support of Brief — executed 2026-03-27

Operative text (verbatim):
```text
L1022: EV-042 · Declaration of Respondent in Support of Brief — executed 2026-03-27
L1023: - What: 15pp sworn declaration, executed at Cancún under penalty of perjury.
L1024:   ¶3 no EFS-005-CV / never authorized email service. ¶4 the 2026-02-24
L1025:   bundled delivery, papers "previously claimed as served on different dates."
L1026:   ¶6 hearing dates already passed on receipt. ¶8 documents "created and
L1027:   inserted into my files that I had never authored… created using my accounts
L1028:   during the period of unauthorized access." ¶9 "at least five separate
L1029:   occasions" requesting a Google evidentiary hold; refused each time; "the
L1030:   officer contacted Google only after an internal affairs inquiry was
L1031:   initiated." ¶10 criminal referral re opposing counsel under DA review;
L1032:   electronic communications "cannot be treated as reliable for purposes of
L1033:   service." ¶11 reserves §473(d).
L1034: - Original: uploads c44bdef5-…_2.pdf and 6accfb51-….pdf — BYTE-IDENTICAL,
L1035:   7,318,891 B each · sha256
L1036:   e22c423b526081bc7f67889871b792880f13cbe7217ac5dd0a6cdd38ea69d451.
L1037: - Tag: (V/Q) text decoded and read in full this session.
L1038: - Used by: FAMILY + CIVIL (¶8 → V6 13th c/a) + POLICE (¶8, ¶9) + 1983 (¶9).
L1039: - Notes: 2026-08-10. ¶9's "five" CONFLICTS with register #25's "four" — see
L1040:   EV-045 and the audit note §7.1. Not citable as a count until resolved.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- C-02:
```text
L1145: **C-02 · The four-vs-five conflict is NOT an AI problem — restated.**
L1146: EV-042 ¶9 (sworn) says "at least five separate occasions." Fact register #25
L1147: says four [Gmail 19c31c2994519631, "Fourth Formal Request"]. EV-045 says "at
L1148: least four times." The conflict is between **Halsey's own sworn filing and his
L1149: own register** — it exists whatever produced Exhibit C, and would exist if a
L1150: paralegal had typed it. Plead neither count until the native emails resolve
L1151: it. Nothing about this reflects on EV-045's status as a source.
```
- EV-054 notes:
```text
L1267: - Notes: 2026-08-10. **RESOLVES FOUR-vs-FIVE IN HALSEY'S FAVOUR.** The
L1268:   1/10/2026 email calls itself the FOURTH formal request and is NOT the last —
L1269:   2/12/2026 follows it. So there are at least FIVE written requests and EV-042
L1270:   ¶9's sworn "at least five separate occasions" is CORRECT. Register #25's
L1271:   "four" was a snapshot at the "Fourth Formal Request," accurate that day and
L1272:   overtaken by events — not a contradiction, and neither source was wrong.
L1273:   **Plead the LIST, not the adjective — a list cannot be impeached.**
```
- K-06:
```text
L1317: | K-06 | **Preservation-request COUNT** | RESOLVED IN HIS FAVOUR. | Open the six threads in EV-054, confirm each is distinct. | The 1/10/2026 "Fourth Formal Request" is not the last (2/12/2026 follows). At least five written. The sworn "at least five" is CORRECT. |
```
- EV-063 sequence note:
```text
L1515:   SEQUENCE CORROBORATION: IA complaint filed 1/10/2026 (register #37,
L1516:   19ba8ab4ac49e9ab) → Kale's Google request 1/12/2026 — the native order
L1517:   matches EV-042 ¶9's sworn "The officer contacted Google only after an
L1518:   internal affairs inquiry was initiated." Also documents the request
```
- EV-069 note:
```text
L1675: - Notes: 2026-08-12 registered. PRECEDES EV-054's six (10/22/2025 →
L1676:   2/12/2026): the dated written-demand LIST now numbers at least SEVEN and
L1677:   its earliest date moves to 10/13/2025. EV-042 ¶9's sworn "at least five"
L1678:   remains correct and conservative. Evidence-sheet doc_status:
```
- KALE CHRONOLOGY item 1 (full text in B5).
- 2026-08-27 block D-1:
```text
L3436: - Per governance/DECISIONS.md **D-1**: every "candidate sixth/seventh demand"
L3437:   phrasing in this index and its notes is **SUPERSEDED**. The asserted
L3438:   preservation-demand count is FIVE (his ruling; EV-054 criteria). Located
L3439:   demand-like documents beyond the five (EV-069; the EV-075 demand set;
L3440:   Gmail 199db7e78dd8b1de) remain library documents under D-6 and enter no
L3441:   count absent his express reclassification.
```
- same file registered again as WP-020 [2/2] and EV-107 (identical sha256, §7); EV-107's count and separation statements:
```text
L3036: WP-020 · Declaration of Respondent in support of Brief + Exhibits A-C
… [L3037–L3046 not reproduced here]
L3047: - Preserved: preserved_2026-08-19/WP-020_Declaration_re_Brief_ExA-C_
L3048:   2026-03-27.pdf. Tag (U/Q). Used by: FAMILY (+CIVIL P036-P037 corroboration
… [L3049–L3267 not reproduced here]
L3268: EV-107 · DECLARATION OF RESPONDENT, 3/27/2026 (sworn) — the second sworn five-count, and the bundled-delivery record
L3269: - What: 3-page sworn declaration + Exhibits A/B/C (image-bound), read IN
L3270:   FULL 2026-08-23 (decrypted; AES). Mirror: uploads_2026-08-23/EV-107_… ·
L3271:   sha256 e22c423b5260…
… [L3272–L3282 not reproduced here]
L3283: - **CONSEQUENCE FOR THE COUNT:** the five-request figure is now **sworn
L3284:   twice** (EV-042 ¶9 + this ¶9). The four-vs-five discipline holds — no
L3285:   count pleaded until natives resolve it — but the packet may state "sworn
L3286:   on two occasions as at least five" as exactly that.
L3287: - **SEPARATION RULE (binding for v1):** ¶8's planted-documents claim and
L3288:   the court's Exhibit-F finding are DIFFERENT FACTS — his on-record
L3289:   "narrative summary… was a mistake" explanation (EV-003) and this sworn ¶8
L3290:   are both stated, never merged, never offered as answering each other.
```

#### EV-043 (L1042) — tags: c, police
Title: Exhibit A — photograph of the bundled delivery (THE DATE ANCHOR)

Operative text (verbatim):
```text
L1042: EV-043 · Exhibit A — photograph of the bundled delivery (THE DATE ANCHOR)
L1043: - What: photo showing USPS label "JAN 30, 2026 · $29.70 · Retail"; return
L1044:   address Young, Spiegel & Hosp, LLP, 301 N. Canon Dr., Ste 300, Beverly
L1045:   Hills CA 90210; handwritten receipt by Francisco Javier Franco Morales
L1046:   ("recibí el correo del señor Halsey Minor el día 24 de febrero sin recibir
L1047:   ninguna Nota solo el correo Por Parte del personal de correos de Mexico" —
L1048:   NO YEAR STATED); stamp PUNTA DEL MAR CANCUN S.A DE C.V. PMC160822IT5
L1049:   ENTREGADO, signed.
L1050: - Tag: (V) read this session. Used by: FAMILY + POLICE (spoliation timing).
L1051: - Notes: 2026-08-10. **This exhibit settles the year.** Mail postmarked
L1052:   1/30/2026 cannot have been delivered 2/24/2024; Exhibit B's typed "2024"
L1053:   is a scrivener's error. Do not spend time litigating the typo.
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-044 (L1055) — tags: c
Title: Exhibit B — Building Manager declaration re receipt of mail

Operative text (verbatim):
```text
L1055: EV-044 · Exhibit B — Building Manager declaration re receipt of mail
L1056: - What: bilingual declaration on the LASC caption, Punta Del Mar official
L1057:   stamp and signature. Postal worker "simply dropped the packages at the
L1058:   front desk and left"; no receipt or signature requested of staff or
L1059:   resident; sender listed = Lance Spiegel's firm; staff handed over a batch
L1060:   of TEN (10) sealed envelopes; packages bearing earlier dates all arrived in
L1061:   one batch. Independent, non-party institutional witness.
L1062: - Tag: (V) read from scan this session. Used by: FAMILY + CIVIL.
L1063: - Notes: 2026-08-10. Contains the "February 24, 2024" scrivener's error
L1064:   (see EV-043). Strong under OPERATING_CONDITIONS §7.2 — third-party custody.
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-046 (L1080) — tags: statebar
Title: California State Bar — submission receipt, 2026-04-20 15:43:57Z

Operative text (verbatim):
```text
L1080: EV-046 · California State Bar — submission receipt, 2026-04-20 15:43:57Z
L1081: - What: complaint@calbar.ca.gov → Halsey, "Successful submission of Attorney
L1082:   Misconduct Complaint." Complaint against Lance Spiegel, Bar No. 51625.
L1083: - Original: Gmail msg 19dab900c339a76b.
L1084: - Tag: (V) — INSTITUTIONAL: authenticated by the State Bar's own send, not by
L1085:   Halsey's mailbox (OPERATING_CONDITIONS §7.4).
L1086: - Used by: FAMILY + CIVIL + POLICE (case history only — addendum §3).
L1087: - Notes: 2026-08-10. Filed ONE DAY before the 4/21/2026 hearing.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-003 POSTURE on the State Bar complaint:
```text
L3416: that he did not receive Petitioner's initial financial disclosures, which the
L3417: court permitted. He states he contacted the California State Bar about
L3418: opposing counsel **before** the ruling issued.
… [L3419–L3421 not reproduced here]
L3422: §473(d)); EV-046 is the State Bar's 4/20/2026 submission receipt for a
L3423: complaint against Lance Spiegel (Bar No. 51625), **one day before** the
L3424: 4/21/2026 order, complaint no. 24-O-18793 (a 2024-origin number).
… [L3425–L3425 not reproduced here]
L3426: finding was entered in a proceeding he contends he was not validly served in
L3427: and is appealing, and a Bar complaint against opposing counsel predated the
```

#### EV-047 (L1089) — tags: statebar, da, police
Title: Notification to DA + federal offices, 2026-04-20 15:52:53Z

Operative text (verbatim):
```text
L1089: EV-047 · Notification to DA + federal offices, 2026-04-20 15:52:53Z
L1090: - What: Halsey → info@da.lacounty.gov (DA Hochman), cc LA_OPCA@fbi.gov,
L1091:   CRM.CivilRights@usdoj.gov (hard-bounced), oig.hotline@usdoj.gov,
L1092:   piu@doj.ca.gov. Subject: "BHPD Case No. 2025-14983 — State Bar Complaint
L1093:   Filed Today Against Opposing Counsel Lance Spiegel (Bar No. 51625)."
L1094:   References "my formal demand letter of April 17, 2026."
L1095: - Original: Gmail msg 19dab983ae3aa08a. Tag: (V/Q) read this session.
L1096: - Used by: FAMILY + POLICE + 1983. Notes: 2026-08-10. The 4/17/2026 demand
L1097:   letter is referenced but NOT yet located — open item.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-065 closes the open item:
```text
L1581: - Notes: 2026-08-12 registered. EV-047 (4/20/2026) references "my formal
L1582:   demand letter of April 17, 2026" — this is it; open item closed. Subject
```
- EV-066 cross-reference:
```text
L1612:   19d64940cdcfe614 · 4/17 formal demand = EV-065 · 4/20 State Bar notice =
L1613:   EV-047 · 4/27 CPRA to DA Public Records Unit 19dcf83c478a060c · 5/4
```

#### EV-048 (L1099) — tags: statebar, exF, c, da
Title: Contemporaneous characterization, 2026-04-22 (day after the hearing)

Operative text (verbatim):
```text
L1099: EV-048 · Contemporaneous characterization, 2026-04-22 (day after the hearing)
L1100: - What: Halsey → shannonminor@gmail.com (Q): "I am so happy I filed a
L1101:   complaint with the California bar association a day before the one hour
L1102:   ambush over janine. I alerted them to the fraud that was coming and the da
L1103:   as well… You made my case 1 day after they received the warning." Same
L1104:   thread: "You realize what the judges ruling means. Mail to Mexico is not
L1105:   sufficient."
L1106: - Original: Gmail msgs 19db7634412cf151 (22:50:29Z) and 19db765c797500a0
L1107:   (22:53:13Z). Tag: (V/Q). Used by: FAMILY + CIVIL.
L1108: - Notes: 2026-08-10. Establishes contemporaneous characterization, NOT the
L1109:   authenticity of Exhibit F. Forecloses "objection manufactured after loss."
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### WP-020 [1/2] (L1111) — tags: c
Title: "Legal Compliance Violations by Petitioner's Counsel" infographic

Operative text (verbatim):
```text
L1111: WP-020 · "Legal Compliance Violations by Petitioner's Counsel" infographic
L1112: - What: Halsey-supplied chart (violations over time; 57%/43% attribution pie;
L1113:   violation-type bars).
L1114: - Tag: (U/X) work product. **NOT FILING-READY — defects recorded 2026-08-10:**
L1115:   "Anna Kralle" surname unverified (only AnnaK@ is (V)); "Matt" vs the
L1116:   record's "Matthew" Sirriyeh; the 57/43 split states no denominator; bar
L1117:   heights disagree with the chart's own axis; no source cited for any data
L1118:   point; the firm has ≥5 staff on its own mail, not two.
L1119: - Used by: none until rebuilt. Notes: rebuild from the POS signatory audit
L1120:   (CANON OPEN-6), one violation per sourced document.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- C-03 (verdict withdrawn, defects kept):
```text
L1153: **C-03 · WP-020 (violations infographic) — VERDICT WITHDRAWN, defects kept.**
L1154: - Withdrawn: my categorical "**NOT FILING-READY**" and "Used by: none until
L1155:   rebuilt." That was my call to make and it was not mine (§8.6).
L1156: - **Kept, because they are checkable and he would want them caught:** "Anna
L1157:   Kralle" surname is unverified (only AnnaK@ is (V)); the record shows
L1158:   "Matthew" Sirriyeh, not "Matt"; the 57/43 split states no denominator; the
L1159:   bar heights disagree with the chart's own axis; the firm shows ≥5 staff on
L1160:   its own mail. A wrong surname in a filed exhibit is the F-01 failure family
L1161:   — that is why these stay on the record.
L1162: - **Corrected status: (U) work product, Halsey-adopted. Usable at his
L1163:   direction.** Fix the surname and the denominator before it goes anywhere,
L1164:   and the rebuild from the POS signatory audit (CANON OPEN-6) makes it
L1165:   stronger — it is not a precondition to its existing as a source.
```
- K-08:
```text
L1319: | K-08 | **WP-020 infographic** | IN as his adopted work product (already converted at C-03). | Verify the "Anna Kralle" surname and the 57/43 denominator. | Only AnnaK@ is verified; record shows "Matthew" Sirriyeh. Two checkable fixes, not a verdict. |
```

#### EV-049 (L1173) — tags: a, police
Title: Google account-recovery notice sequence, Sept–Oct 2023 (THE LOCKOUT)

Operative text (verbatim):
```text
L1173: EV-049 · Google account-recovery notice sequence, Sept–Oct 2023 (THE LOCKOUT)
L1174: - What: four notices from no-reply@accounts.google.com, subject "Critical
L1175:   security alert," each reading (Q, search-result snippet): "We'll send a link
L1176:   to sign in to your account in 30 days · halsey2005@gmail.com · Google
L1177:   received a request to recover your account halsey2005@gmail.com."
L1178:   2023-09-07 18:08:46Z (18a70d512865b590) · 2023-09-09 11:55:00Z
L1179:   (18a79cb99e316376) · 2023-10-10 07:50:54Z (18b1891454bc580d) ·
L1180:   2023-10-21 08:16:44Z (18b514edd2a06abe).
L1181: - Tag: **(V) — INSTITUTIONAL.** Machine-generated and sent BY GOOGLE;
L1182:   authenticated by Google's own send, not by his mailbox (OP. COND. §7.4).
L1183: - Used by: 1983 (primary) + CIVIL (§502 count) + POLICE.
L1184: - Notes: 2026-08-10. Four recovery attempts across 44 days, none restoring
L1185:   access. Google's own "30 days" language matches Halsey's from-memory
L1186:   description exactly. **His further explanation — "it resets whenever she
L1187:   logs in" — is (U) and is NOT in these notices; do not attribute it to
L1188:   Google.** Sept 17 2023 (F-12) falls between notices 2 and 3: state the
L1189:   sequence, assert no causal link.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- K-02:
```text
L1313: | K-02 | **"Sept & Oct 2022 locking me out"** (his 1/8/2026 email to BHPD, F-22) | The STATEMENT stands as his adopted, sent statement to law enforcement. The 2022 lockout is UNCORROBORATED. | Search 2022 for recovery notices in the backup account and any other address; check whether a 2022 episode exists that this mailbox would not show. | In THIS mailbox, 2022-07-01→2023-07-15 has no recovery notices; the notice sequence is 2023. A real, unexplained 2022-09-14 password change DOES exist (EV-051). |
```

#### EV-050 (L1191) — tags: a, police
Title: Google account recovery completed — 2023-11-20, and the secondary address

Operative text (verbatim):
```text
L1191: EV-050 · Google account recovery completed — 2023-11-20, and the secondary address
L1192: - What: 2023-11-20 16:26:45Z "Your password was changed" (18bed8e553245b27);
L1193:   16:26:46Z "Your Google Account was recovered successfully — Welcome back to
L1194:   your account" (18bed8e4a4bb39c1); 16:26:46Z new sign-in on Android
L1195:   (18bed8e4a8de5817). Then 2023-11-28 09:52:31Z "Recovery email verified":
L1196:   "The recovery email halsey@liveplanet.net was verified for your account"
L1197:   (18c15583f81d5464).
L1198: - Tag: (V) — INSTITUTIONAL, same basis as EV-049.
L1199: - Used by: 1983 + CIVIL + POLICE.
L1200: - Notes: 2026-08-10. Corroborates Halsey's "She was done with my account in
L1201:   November, and I got it back using my secondary address." **Lockout duration,
L1202:   computed from Google's timestamps: 2023-09-07 → 2023-11-20 = 74 days.** That
L1203:   figure is safe to use. Also (V): on 2025-04-11 17:45:01Z he forwarded the
L1204:   11/20/2023 alert to himself (19625f47de243ed8) — he was preserving this as
L1205:   evidence sixteen months before the January 2026 hold.
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-051 (L1207) — tags: a, police
Title: Google password change 2022-09-14 — REAL, UNEXPLAINED, NOT A LOCKOUT

Operative text (verbatim):
```text
L1207: EV-051 · Google password change 2022-09-14 — REAL, UNEXPLAINED, NOT A LOCKOUT
L1208: - What: 2022-09-14 15:32:29Z, "Your password was changed · halsey2005@gmail.com
L1209:   … If you didn't change it, you should recover your account"
L1210:   (1833ca16271d09ea); then 15:34:42Z SaneBox and 15:37:41Z Airmail iOS granted
L1211:   account access.
L1212: - Tag: (V) as to the event. **(X) as to who did it and why — unexplained.**
L1213: - Used by: 1983 + POLICE, as an open question only.
L1214: - Notes: 2026-08-10. Registered because it is the ONLY 2022 account event
L1215:   found, and because his 1/8/2026 email to police claims a Sept–Oct 2022
L1216:   lockout that the record does NOT support (F-22). Do not assume the author;
L1217:   do not assume it was innocent; do not call it a lockout.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- K-02:
```text
L1313: | K-02 | **"Sept & Oct 2022 locking me out"** (his 1/8/2026 email to BHPD, F-22) | The STATEMENT stands as his adopted, sent statement to law enforcement. The 2022 lockout is UNCORROBORATED. | Search 2022 for recovery notices in the backup account and any other address; check whether a 2022 episode exists that this mailbox would not show. | In THIS mailbox, 2022-07-01→2023-07-15 has no recovery notices; the notice sequence is 2023. A real, unexplained 2022-09-14 password change DOES exist (EV-051). |
```

#### EV-052 (L1219) — tags: a [fn5], police
Title: Halsey's OWN preservation request to Google — 2025-10-16, and it BOUNCED

Operative text (verbatim):
```text
L1219: EV-052 · Halsey's OWN preservation request to Google — 2025-10-16, and it BOUNCED
L1220: - What: 2025-10-16 09:59:37Z, Halsey → legal-support@google.com, "Preservation
L1221:   Request – Gmail Account halsey2005@gmail.com," formal letter block ("Google
L1222:   LLC – Legal Investigations Support, Attn: Custodian of Records")
L1223:   (199ec75f75e16cd7). At 09:59:50Z — thirteen seconds later — mailer-daemon:
L1224:   "Address not found … legal-support@google.com" (199ec76298c0a6ff).
L1225: - Tag: (V) by header and bounce record.
L1226: - Used by: 1983 (primary) + POLICE.
L1227: - Notes: 2026-08-10. This is the "emails to Google asking them to preserve my
L1228:   account" Halsey remembered. It exists. **Its date is 2025, not 2023** — his
L1229:   recollection tied it to the Turkey period; the document does not. Register
L1230:   the document's date, not the recollection.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-076 [1/2] item (3) quoting this letter:
```text
L1942:   time of the breach." (3) Halsey's 10/16/25 letter to Google (Q): breach
L1943:   "[i]n the timeframe between April 2025 and September 2025"; requests
L1944:   preservation of emails deleted "between approximately April 1, 2025 and
L1945:   September 1, 2025". (4) Snyder 2025-08-04 (Q): "You have to report the
```

#### EV-056 (L1329) — tags: a, f, police — class AI-LEAD
Title: "Forensic Analysis of Digital Correspondence: The Minor v. Kale Case File (2024-2026)" (THE CROSS-VECTORING EXEMPLAR)

Operative text (verbatim):
```text
L1329: EV-056 · "Forensic Analysis of Digital Correspondence: The Minor v. Kale Case File (2024-2026)" (THE CROSS-VECTORING EXEMPLAR)
L1330: - What: 68-page footnoted forensic reconstruction of the Halsey↔Kale
L1331:   correspondence, March 2024 → January 2026; chronological script + forensic
L1332:   commentary; frames "Investigative Latency" / "Procedural Dissonance"; names
L1333:   the "Triangle of Corruption" HYPOTHESIS (police files leaked to opposing
L1334:   counsel; targeted cyber-intrusion to sanitize evidence) and builds toward
L1335:   it. AI-assisted (Gemini), adopted and supplied by Halsey 2026-08-11.
L1336: - Original: upload 6c56814d-Officer_Kale_Report_Footnoted_v2_2.pdf · sha256
L1337:   cc2c91bc1b415b0e7d2c4a52d4a551c75480ed29e36f76f04f5a1e0ff15f5402.
L1338:   DURABLE MIRROR NEEDED (upload is container-cache; F-16) — first commit task
L1339:   for the new police thread: copy into repo or Drive and record the locator.
L1340: - Tag: (U) — Halsey-adopted work product (§8). Opening sections read
L1341:   2026-08-10/11; full extraction + per-section registration assigned to the
L1342:   police thread (LESSONS #14).
L1343: - Used by: POLICE (primary) + CIVIL + 1983. Method exemplar under §15.
L1344: - Notes: 2026-08-11. Cross-checks from the opening pages: asserts first
L1345:   formal contact MARCH 29, 2024 (K-01 now documented on both sides — with
L1346:   EV-045 for 2024, against the register's ≈3/24/2025 + the 2025- case prefix
L1347:   + commit 1d5744a's mailbox-negative; NATIVE email settles it, search BOTH
L1348:   accounts); theft stated "$1.135M-$2.5M" ($1.135M ≈ the register's deposit
L1349:   $1,135,356.93; "$2.5M" is register-dropped #15; packet usage is Halsey's
L1350:   call §10); conflates case numbers ("BHPD Case #2025-14983 (later referenced
L1351:   as 24STFL00432)") — carry both numbers correctly.
L1352:   Full detail: runbooks/audit_notes/2026-08-11_halsey_statements_kale_report_intake_and_postmortem.md §2.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-056 ANNOTATION item 1 (page count corrected):
```text
L1463: --- EV-056 ANNOTATION — 2026-08-12 (append-only; full-extraction pass complete) ---
L1464: Full per-section extraction committed:
L1465: matters/04/report_2026-08/15_EV056_FULL_EXTRACTION.md. Corrections/finds:
L1466: 1. PAGE COUNT: the mirrored PDF is 34 pages, not the 68 recorded at intake
L1467:    (sha256 unchanged and re-verified this session — the count, not the file,
L1468:    was wrong). Binding anomaly: the chronology's reading order is pp.1-4 →
L1469:    p.17 → pp.5-7 (p.17 misbound inside the "Three Emails" section).
```
- C-04 standing rule:
```text
L1167: **C-04 · STANDING RULE for this index.** No future entry is tagged (X), "not a
L1168: source," or "roadmap only" on the ground that an AI, calculator, dashboard, or
L1169: assistant produced it. Where verification is incomplete, write exactly what is
L1170: unverified and against which record — never a status label that reads as
L1171: disqualification. (X) keeps its narrow meaning only: OPERATING_CONDITIONS §7.4.
```

#### EV-063 (L1493) — tags: a, f, police
Title: Kale 1/12/2026 — corruption-scheme denial + THE GOOGLE PRESERVATION REQUEST, both accounts (body read in full)

Operative text (verbatim):
```text
L1493: EV-063 · Kale 1/12/2026 — corruption-scheme denial + THE GOOGLE PRESERVATION REQUEST, both accounts (body read in full)
L1494: - What: 2026-01-12T18:51:48Z (10:51 AM PT), akale@beverlyhills.org →
L1495:   halsey@minorventures.com cc halsey2005@gmail.com, "RE: Fwd:". Full body
L1496:   (Q): "I am sorry you think I am part of some elaborate corruption scheme
L1497:   to hide/destroy evidence. I can assure you this is not the case, as I
L1498:   would not know how to be a part of a 'Scalpel-like hacking' operation." ·
L1499:   "we still have that original 567-page document you sent us. That document
L1500:   has not been compromised at all." · "Regarding the Gmail emails you spoke
L1501:   about from November of 2022 – we have that page of the document showing
L1502:   the emails between you and Shannon, as seen below: [image003.png]" ·
L1503:   **"I have submitted a preservation request to Google for those emails
L1504:   (assuming they are still preservable). The request was made for two
L1505:   accounts: Halsey2005@gmail.com and Shannonminor@gmail.com."**
L1506: - Original: Gmail 19bb38cf19aec75b (3 image attachments incl. the
L1507:   567-page-document page showing the Nov 2022 emails — extraction owed).
L1508: - Hash: not computed — Gmail message.
L1509: - Tag: (V/Q) — body read at source 2026-08-12.
L1510: - Used by: POLICE (primary) + 1983 + CIVIL.
L1511: - Notes: 2026-08-12 registered. CLOSES straw-man GAP #8: the native
L1512:   1/12/2026 preservation action (EV-045's "hold finally initiated on
L1513:   January 12, 2026" now has Kale's own words; precision — he "submitted a
L1514:   preservation request," qualified "assuming they are still preservable").
L1515:   SEQUENCE CORROBORATION: IA complaint filed 1/10/2026 (register #37,
L1516:   19ba8ab4ac49e9ab) → Kale's Google request 1/12/2026 — the native order
L1517:   matches EV-042 ¶9's sworn "The officer contacted Google only after an
L1518:   internal affairs inquiry was initiated." Also documents the request
L1519:   covered SHANNON's account too — a fact for the DEMAND section (what did
L1520:   Google return, and to whom). Kale's denial quote is the G5 disclosure
L1521:   counterpart to any leak-adjacent framing (which stays §1983 anyway).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- KALE CHRONOLOGY item 2 (full text in B5).

#### EV-065 (L1568) — tags: a, b, exF, da, police
Title: The April 17, 2026 formal demand letter to the DA — LOCATED (closes EV-047's open item)

Operative text (verbatim):
```text
L1568: EV-065 · The April 17, 2026 formal demand letter to the DA — LOCATED (closes EV-047's open item)
L1569: - What: 2026-04-17T23:41:46Z, halsey2005@gmail.com → info@da.lacounty.gov,
L1570:   cc LA_OPCA@fbi.gov, CRM.CivilRights@usdoj.gov (bounced), oig.hotline,
L1571:   piu@doj.ca.gov, henrynicholas/henryn. Subject (Q): "BHPD Case No.
L1572:   2025-14983 — Formal Demand for Action Under California Constitution Art.
L1573:   I, § 28(b) (Marsy's Law) — $2.5 Million Grand Theft, Computer Fraud,
L1574:   Evidence Tampering, and Institutional Obstruction." Opening (Q, snippet):
L1575:   "This letter constitutes a formal demand, under the California
L1576:   Constitution and the Penal Code, that your office fulfill its mandatory
L1577:   obligations to me as a crime victim."
L1578: - Original: Gmail 19d9dd26f4e7242b (SENT). Body not yet opened in full.
L1579: - Tag: (V) header/subject/snippet; (U) contents as his adopted demand.
L1580: - Used by: POLICE (fork Fact B; obligations ledger) + 1983.
L1581: - Notes: 2026-08-12 registered. EV-047 (4/20/2026) references "my formal
L1582:   demand letter of April 17, 2026" — this is it; open item closed. Subject
L1583:   carries "$2.5 Million" (register #15: documented spine differs — disclose,
L1584:   packet uses sourced figures).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-065 BODY READ annotation, header and items 3-5:
```text
L1762: --- EV-065 BODY READ IN FULL — 2026-08-12 annotation (append-only) ---
L1763: The 4/17/2026 formal demand's full text carries (all U — his adopted
L1764: account, with checkable specifics; LESSONS #8 phrasing for others' acts):
… [L1765–L1775 not reproduced here]
L1776: 3. W2 WINDOW DOCUMENT (new, third-party, §7.3 acquisition list): "On
L1777:    February 27, 2026, Apple issued a security alert identifying 730 of
L1778:    1,074 stored passwords as compromised. Forensic review traced the
L1779:    intrusion vector to a Screens Connect remote-access vulnerability…"
L1780:    HUNT: locate the Apple alert native (institution's own send, §7.4).
L1781: 4. DELETION-DATE CLAIM (the causation gap's candidate answer, MASTER FIX
L1782:    PLAN): "Spiegel specifically demanded the November 11, 2022 email — the
L1783:    exact email that had been surgically deleted on August 4, 2025." Also:
L1784:    "Thirty emails from late November 2022, in which Shannon Minor
L1785:    discussed her claim that the stolen funds were owed to her mother…
L1786:    surgically deleted… counted through forensic analysis of surviving
L1787:    metadata." Tests owed: the metadata forensics output (§7.5 — method or
L1788:    no number); the 8/4/2025 date's source.
L1789: 5. **CROSS-VECTOR, RECORDED WITHOUT SMOOTHING (F-02): EV-067 — the
L1790:    11/10-11/2022 WF deposit-hold thread (18461348b9fe0954 /
L1791:    18467dd2c7361b33 family, Shannon's "Yes! Large number has a 10 day
L1792:    hold") — was FOUND LIVE in the mailbox 2026-08-12** by this thread's
L1793:    search. The adopted 4/17/26 claim says "the November 11, 2022 email"
L1794:    was deleted 8/4/2025. Both facts stand. Possible reconciliations (all
L1795:    untested): different 11/11/22 message (his 1/8/26 email to Kale calls
L1796:    it the email "confirming receipt of the tax refund"); restoration;
L1797:    thread-vs-message deletion. TEST: identify from Spiegel's motion +
L1798:    Exhibit C/diff output WHICH 11/11/22 message was demanded/deleted,
L1799:    then compare against the live EV-067 thread. §7.6 gate applies to any
L1800:    Exhibit-F-family item. This is exactly the "same set or different
L1801:    sets?" question in miniature — answerable from documents.
```
- H-8 ASYMMETRY-TEST FINDING (full text in B7).
- EV-076 [1/2] on the "August 4, 2025" date:
```text
L1960:   preservable" hedge). Complaint3's specific "August 4, 2025" deletion
L1961:   date remains UNSOURCED at native level — test owed.
```
- EV-088 DEFECT 1:
```text
L2471: - **DEFECT 1 — Exhibit A asserts a deletion that did not occur.** It states
L2472:   the 11/11/2022 "Yes! Large number has a 10 day hold" email is "DELETED
L2473:   (Surgically removed from server)." **Tested live 2026-08-12: thread
L2474:   `18461348b9fe0954` is INTACT, all five messages** — `18461348b9fe0954`,
L2475:   `18467dbd3ea6fa47`, `18467dd2c7361b33`, `1846822a40fdff6d`,
L2476:   `1846823e63d233ca`. It is also the basis of EV-067. Innocent readings
L2477:   stated: post-audit Google recovery (EV-049/050), or the assertion was never
L2478:   checked.
```
- EV-108 on the §271 motion's contents:
```text
L3390: - **CONSEQUENCE 2 — THE PLANNED "LANCE-MOTION OVERLAP TABLE" HAD A FALSE
L3391:   PREMISE AND IS REPLACED.** This motion challenges the Spiegel log only —
L3392:   it contains NO list of Shannon emails. The documentable overlap is
```

#### EV-066 (L1586) — tags: statebar, a [fn6], da, police
Title: The DA-demand / production series, 3/25/2026 → 5/6/2026 (SET ENTRY — fork Fact B corpus + obligations-ledger natives)

Operative text (verbatim):
```text
L1586: EV-066 · The DA-demand / production series, 3/25/2026 → 5/6/2026 (SET ENTRY — fork Fact B corpus + obligations-ledger natives)
L1587: - What: Halsey's dated written demands and evidence productions to the LA
L1588:   County DA (and parallel federal/AG offices), each carrying BHPD Case No.
L1589:   2025-14983. Native ids, headers verified 2026-08-12 (bodies unopened
L1590:   except as noted): 3/25 "WHERE IS WALDO (EVIDENCE FILE 2)" 19d225c4bcd23b69
L1591:   · 3/27 "Staged Production of Files" 19d2d33646672aa2 (3/27 reply from
L1592:   Andrea.Hernandez@firstcitizens.com "Are these being sent to me in error?"
L1593:   19d30b35c8ae890e — misdirection on the record) · 3/29 Marsy's §28(b)(9)
L1594:   confer demand 19d3ac1d78697485 · 3/30 "Preserved Evidence… Immediate
L1595:   Subpoena Required" 19d3fc9b6c9ad1cb · 3/30 Production 6 19d3fff4f6f07acf ·
L1596:   3/30 Production 7 19d401f9c749fe9d · 3/31 AG Marsy's complaint
L1597:   19d44d1f89f62183 · 3/31 FBI package 19d44d9196e48486 ("7+ productions
L1598:   totaling more than 80 evidence files. The DA has received every one") ·
L1599:   3/31 point-of-contact set: DOJ-Crim 19d44dcafa9aa501, DOJ-CivRights
L1600:   19d44dcbbcc2f313, DOJ-OIG 19d44dcc48115c2b, DA 19d44dccfa89510f (Q: "You
L1601:   initially asked to speak with me and provided a phone number. Then
L1602:   nothing. Zero responses since."), BHPD-IA 19d44dcda6a7a9ef (Q: "I filed a
L1603:   formal internal affairs complaint against Detective Alex Kale 31 days
L1604:   ago. I have not received a case number.") · 3/31 Production 8
L1605:   19d44f7ee240732b · 4/6 §28(b)(9) FORMAL DEMAND 19d64912dc3b7a28 · 4/6
L1606:   CPRA to DA Requests 1-3 of 3: 19d6446ffc5f53b3 / 19d6447025040635 /
L1607:   19d644707b536cd4 · 4/6 SUPPLEMENTAL CPRAs: Kale-DA communications
L1608:   19d647a32c6b3cad, internal case-file access metadata 19d647a2b8bd4d86, AG
L1609:   actions 19d647a41419da17 · 4/6 Marsy's-overdue follow-up 19d6442dba0dabce
L1610:   · 4/6 JSID cyber-sabotage 19d643ff9dda21bd · 4/6 Spiegel-complaint
L1611:   follow-up "37 Days, No Response" 19d64940b1e9d860 + IA demand
L1612:   19d64940cdcfe614 · 4/17 formal demand = EV-065 · 4/20 State Bar notice =
L1613:   EV-047 · 4/27 CPRA to DA Public Records Unit 19dcf83c478a060c · 5/4
L1614:   "FINAL NOTICE — Overdue CPRA Responses" 19df520c1952a8e6 (adds named DA
L1615:   staff cc: jcastano, Nodonnell, SSahab @da.lacounty.gov) · 5/6 Cal-Bar
L1616:   "Coloring Book" cc DA 19dff13fd9dd8b9b.
L1617: - DA-side responses found in this sweep: the 1/12/2026 "Please explain in
L1618:   greater detail your reason for contacting this office" (19bb307ee4795b75)
L1619:   and the reported phone-number offer (U — his 3/31 statement). No
L1620:   substantive acknowledgment of the Kale submission located.
L1621: - Tag: (V) headers; bodies unopened except where quoted from snippets.
L1622: - Used by: POLICE (fork Fact B; 12_OBLIGATIONS rows; §28(b) history) + 1983.
L1623: - Notes: 2026-08-12 registered. Precision for the packet: his conferral
L1624:   demands cite §28(b)(9); 13_ §4 maps conferral to (b)(6) — state the right
L1625:   subdivision in Section 13 and note the variance where his sent demands
L1626:   are quoted (G5). Statutory CPRA windows still unverified at source (X).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- C-09 (the DA did respond):
```text
L2868: --- CORRECTION C-09 · THE DA DID RESPOND — our own record was wrong — 2026-08-12 ---
L2869: **File 12_ (OBLIGATIONS LEDGER, Completion Pass 2) states: "Last DA message on
L2870: record remains 1/12/2026." THAT IS FALSE.** A sweep
L2871: `in:anywhere from:da.lacounty.gov` returns **nine threads with at least SIX
L2872: substantive DA responses**, two from **named DA staff**, through **3/19/2026**:
L2873: 1/8/2026 (`19b9fe124c63613a`) · 1/12/2026 (`19bb307ee4795b75`) · **1/12/2026
L2874: AWise@da.lacounty.gov** (`19bb3ad9899c0a6d`, JSID: "JSID does not generally
L2875: initiate criminal investigations") · 1/15/2026 (`19bc3db9c2a11195`) ·
L2876: 1/22/2026 (`19be735cadc9e828`) · 1/30/2026 (`19c102e73a5cbca7`, "Please
L2877: contact JSID at (213) 974-3888") · **3/19/2026 jcastano@** (`19d07358d5ac4260`).
L2878: **WHAT SURVIVES:** the post-**4/17/2026** silence through all three EV-065
L2879: deadlines (5/1, 5/17, 6/16/2026) — that sweep returned zero and is unaffected.
L2880: **WHAT MUST NEVER BE SAID AGAIN: "the DA never responded."** One reply
L2881: produced by the other side would have cost the packet its credibility on
L2882: everything else in it. Correct framing: **form responses and one substantive
L2883: statement through March 2026, then silence after 4/17/2026 through every
L2884: deadline in the formal demand.**
```

#### EV-067 (L1628) — tags: a [fn7], police
Title: Shannon's contemporaneous acknowledgment of the tax-refund deposit — 11/10-11/2022 WF deposit-hold thread (KNOWLEDGE evidence)

Operative text (verbatim):
```text
L1628: EV-067 · Shannon's contemporaneous acknowledgment of the tax-refund deposit — 11/10-11/2022 WF deposit-hold thread (KNOWLEDGE evidence)
L1629: - What: (1) 2022-11-10T11:02:23Z, alerts@notify.wellsfargo.com → halsey2005,
L1630:   "Wells Fargo deposit hold alert" re "your recent deposit to your Wells
L1631:   Fargo account XXXXXX2218" (18461348b9fe0954 — INSTITUTIONAL, Google/WF
L1632:   machine send, §7.4). (2) 11/11 18:02Z Halsey forwards to
L1633:   shannonminor@gmail.com: "?" (18467dbd3ea6fa47). (3) 11/11 18:04Z Shannon
L1634:   (Q): "Yes! Large number has a 10 day hold" (18467dd2c7361b33). (4) 11/11
L1635:   19:20Z Halsey (Q): "From the government!" (1846822a40fdff6d). (5) 11/11
L1636:   19:21Z Shannon (Q): "Yes" (1846823e63d233ca).
L1637: - Tag: (V/Q) — thread read from search-result bodies/snippets 2026-08-12;
L1638:   full-body opens owed before exhibit print.
L1639: - Used by: POLICE (Incident Group One — knowledge/intent: her written
L1640:   acknowledgment of the deposit and its government source, 2 days after the
L1641:   11/9/22 deposit and 4 days before the first transfer 11/15/22) + CIVIL.
L1642: - Notes: 2026-08-12 registered (Hunt #7 pass 1). Cross-vector: the register
L1643:   error-correction #6 noted an email saying "Nov 11" vs the bank's Nov 9
L1644:   deposit date — THIS thread is that email family: the ALERT is 11/10 and
L1645:   her acknowledgment 11/11; deposit date on the statement stays 11/9.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-065 annotation item 5:
```text
L1789: 5. **CROSS-VECTOR, RECORDED WITHOUT SMOOTHING (F-02): EV-067 — the
L1790:    11/10-11/2022 WF deposit-hold thread (18461348b9fe0954 /
L1791:    18467dd2c7361b33 family, Shannon's "Yes! Large number has a 10 day
L1792:    hold") — was FOUND LIVE in the mailbox 2026-08-12** by this thread's
L1793:    search. The adopted 4/17/26 claim says "the November 11, 2022 email"
L1794:    was deleted 8/4/2025. Both facts stand. Possible reconciliations (all
L1795:    untested): different 11/11/22 message (his 1/8/26 email to Kale calls
L1796:    it the email "confirming receipt of the tax refund"); restoration;
L1797:    thread-vs-message deletion. TEST: identify from Spiegel's motion +
L1798:    Exhibit C/diff output WHICH 11/11/22 message was demanded/deleted,
L1799:    then compare against the live EV-067 thread. §7.6 gate applies to any
L1800:    Exhibit-F-family item. This is exactly the "same set or different
L1801:    sets?" question in miniature — answerable from documents.
```
- EV-088 DEFECT 1:
```text
L2471: - **DEFECT 1 — Exhibit A asserts a deletion that did not occur.** It states
L2472:   the 11/11/2022 "Yes! Large number has a 10 day hold" email is "DELETED
L2473:   (Surgically removed from server)." **Tested live 2026-08-12: thread
L2474:   `18461348b9fe0954` is INTACT, all five messages** — `18461348b9fe0954`,
L2475:   `18467dbd3ea6fa47`, `18467dd2c7361b33`, `1846822a40fdff6d`,
L2476:   `1846823e63d233ca`. It is also the basis of EV-067. Innocent readings
L2477:   stated: post-audit Google recovery (EV-049/050), or the assertion was never
L2478:   checked.
```
- EV-098 dispute over the same email:
```text
L2927: - **WHAT THE DISPUTE WAS ABOUT** (`19c27f6dc533be58`, 2/4/2026, Q): "I am
L2928:   specifically talking about the **November 11, 2022 email confirming receipt
L2929:   of the tax refund**" — **the exact email EV-088's Exhibit A calls
L2930:   "surgically removed," and which is PRESENT in the live account today.**
L2931:   The one test that could rehabilitate that exhibit: **Google account activity
L2932:   and recovery records for thread `18461348b9fe0954`.**
```
- KALE CHRONOLOGY item 5 (full text in B5).

#### EV-069 (L1665) — tags: a, police
Title: The EARLIEST written preservation demand to BHPD found — 10/13/2025 "CALL GOOGLE! YES OR NO"

Operative text (verbatim):
```text
L1665: EV-069 · The EARLIEST written preservation demand to BHPD found — 10/13/2025 "CALL GOOGLE! YES OR NO"
L1666: - What: 2025-10-13T02:55:22Z, halsey2005@gmail.com → akale, snazarian,
L1667:   ealbanese, nhuntcoffey (bounces), ddimond, mayorandcitycouncil. Subject
L1668:   (Q): "MY COMPUTER HACKED. EMAIL EVIDENCE SPOILAGE. CALL GOOGLE! YES OR
L1669:   NO". Snippet: FirstUnion/SVB-successor bank cyber head "described the
L1670:   virus. It moves through attachments, such as legal documents" — a W2
L1671:   window-establishing lead (the bank's virus detection, OP.COND. §7.3).
L1672: - Original: Gmail 199db7e78dd8b1de (SENT). Body-open owed.
L1673: - Tag: (V) header/subject; (U) contents.
L1674: - Used by: POLICE + 1983 (preservation-demand list; W2 window).
L1675: - Notes: 2026-08-12 registered. PRECEDES EV-054's six (10/22/2025 →
L1676:   2/12/2026): the dated written-demand LIST now numbers at least SEVEN and
L1677:   its earliest date moves to 10/13/2025. EV-042 ¶9's sworn "at least five"
L1678:   remains correct and conservative. Evidence-sheet doc_status:
L1679:   `2703f-demand`. Conservative duration anchors update: 91 days from
L1680:   10/13/2025 to the 1/12/2026 request (EV-063) — use the list, not an
L1681:   adjective.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- 2026-08-27 block D-1:
```text
L3436: - Per governance/DECISIONS.md **D-1**: every "candidate sixth/seventh demand"
L3437:   phrasing in this index and its notes is **SUPERSEDED**. The asserted
L3438:   preservation-demand count is FIVE (his ruling; EV-054 criteria). Located
L3439:   demand-like documents beyond the five (EV-069; the EV-075 demand set;
L3440:   Gmail 199db7e78dd8b1de) remain library documents under D-6 and enter no
L3441:   count absent his express reclassification.
```

#### EV-070 (L1683) — tags: a, police
Title: "Shannon Halsey Analysis Marriage.pdf" — THE 1.5-YEAR EMAIL-CORPUS PDF EXPORT (control set, §7.1)

Operative text (verbatim):
```text
L1683: EV-070 · "Shannon Halsey Analysis Marriage.pdf" — THE 1.5-YEAR EMAIL-CORPUS PDF EXPORT (control set, §7.1)
L1684: - What: 31,157,062-byte PDF, per Halsey (U, 2026-08-12, this thread): one of
L1685:   "several pdfs of extracted email files" — "I extracted 1.5 years of emails
L1686:   between Shannon and I, to use a pdf to do ai analysis on the full email
L1687:   data set, just the two of us to show her abuse and the lies she told" —
L1688:   downloaded "after the Turkish [hijacking], before the hacking when I get
L1689:   my mac" (post-Turkey, pre-W2). "The diffs in old pdfs vs the current
L1690:   account are all hacks."
L1691: - Original: Drive 14whXxRKHlLpHv4AAFh1E-IBXfBsLcanD · 31,157,062 B ·
L1692:   createdTime 2025-03-29T01:27:00Z · modified 2025-03-31 · parent
L1693:   1mgU2f2IZ3u_w8gzBf8nbQCptChsWFxnn. (Drive fixation date 3/29/2025 = the
L1694:   report-delivery window: report 3/24-25/25, counsel letter 3/29/25.)
L1695: - Hash: not computed — Drive id + byte size recorded (tamper tripwire).
L1696: - Tag: (U) purpose/provenance per Halsey; (V) Drive metadata live-fetched
L1697:   2026-08-12. CONTENTS UNREAD (31MB — subagent extraction pass owed).
L1698: - Used by: POLICE + CIVIL + 1983 — §7.1 CONTROL SET: the authentication
L1699:   BASELINE; the live account is the degraded copy.
L1700: - Notes: 2026-08-12 registered on Halsey's direction. Companion of EV-071.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- STRUCTURAL FINDING test (full text in B6).
- H-8 test (a):
```text
L1875: deletion (Lesson 1) — the affirmative tests remain: (a) the EV-070/071
L1876: control-set PDFs (contents queued for Halsey's Mac — if the 30 emails
L1877: appear there, PDF-vs-live diff = the deletion exhibit); (b) the
```

#### EV-071 (L1702) — tags: a, exF, police
Title: "Shannon Halsey Analysis Marriage Complete Email Missing What'sapp.pdf" — THE DOCUMENT THE POLICE-REPORT ANALYSIS EXAMINES

Operative text (verbatim):
```text
L1702: EV-071 · "Shannon Halsey Analysis Marriage Complete Email Missing What'sapp.pdf" — THE DOCUMENT THE POLICE-REPORT ANALYSIS EXAMINES
L1703: - What: 31,094,269-byte PDF. First 50 Pages p.1 (Q): "This report examines
L1704:   the evidence contained in 'Shannon Halsey Analysis Marriage Complete
L1705:   Email Missing WhatsApp.pdf'…" — i.e., THIS file is the corpus underlying
L1706:   the adopted analysis delivered to BHPD (pp.1-12 of the package). Same
L1707:   extraction family as EV-070 (63KB size delta between the two — versions;
L1708:   diff owed).
L1709: - Original: Drive 1IUShpaNYRmKcfehLkfaDDtJZdvoXsVzy · 31,094,269 B ·
L1710:   createdTime 2025-03-31T02:28:17Z · same parent as EV-070.
L1711: - Hash: not computed — Drive id + byte size recorded.
L1712: - Tag: (U/V) as EV-070. CONTENTS UNREAD — subagent extraction owed.
L1713: - Used by: POLICE + CIVIL + 1983 (control set; §7.6 diff question inputs).
L1714: - Notes: 2026-08-12 registered. Related smaller exhibits located same
L1715:   sweep: "Shannon Demanding Email.pdf" / "…Email 2.pdf" — 69,709 B,
L1716:   ≥19 copies across folders, earliest createdTime 2025-07-28 / 2025-10-15
L1717:   (ids incl. 16-VlO2manuZKCQbEM6enWKG0JkWmFxAv, 1ylJgPvIqoXHtX-YdpbCyDQ-
L1718:   j8_iHnXrp) — register individually on first read. STANDING SIGNIFICANCE
L1719:   (§7.5): EV-070/071 + the live account + the diff output are the three
L1720:   inputs that answer both the §7.6 Exhibit-F question and the deletion
L1721:   proof. TESTS OWED: (1) sha256 both files (Halsey's Mac or container with
L1722:   Drive download); (2) subagent content extraction + per-email inventory;
L1723:   (3) diff inventory vs live Gmail for the report-cited emails (pp.1-12
L1724:   quotes = the target list); (4) establish whether either file is
L1725:   byte-identical to what BHPD received (§7.2 fixes it permanently).
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-072 (L1808) — tags: a, police
Title: Apple Account password-change notice — 2026-02-27 (W2 window document, institutional)

Operative text (verbatim):
```text
L1808: EV-072 · Apple Account password-change notice — 2026-02-27 (W2 window document, institutional)
L1809: - What: appleid@id.apple.com → halsey@minorventures.com,
L1810:   2026-02-27T21:03:09Z. Full body read (Q): "The following changes to your
L1811:   Apple Account, halsey@minorventures.com, were made on February 27, 2026
L1812:   at 4:03:08 PM EST: Password. If you did not make these changes or you
L1813:   believe an unauthorized person has accessed your account, you should
L1814:   change your password as soon as possible…"
L1815: - Original: Gmail 19ca0e9ad01a16cd.
L1816: - Hash: not computed — Gmail message.
L1817: - Tag: (V) — INSTITUTIONAL (Apple's own machine send, OP.COND. §7.4);
L1818:   body read at source 2026-08-12.
L1819: - Used by: POLICE (Incident Group Three / W2) + 1983 + CIVIL.
L1820: - Notes: 2026-08-12 registered. PRECISION: this documents an Apple Account
L1821:   PASSWORD CHANGE on 2/27/2026 — the same date EV-065's adopted demand
L1822:   letter cites for "Apple issued a security alert identifying 730 of 1,074
L1823:   stored passwords as compromised." This notice is NOT that alert (the
L1824:   compromised-passwords list is an on-device iCloud Keychain "Security
L1825:   Recommendations" screen, not an email) — it corroborates that a security
L1826:   event/response occurred on the cited date. TESTS OWED: (a) whether the
L1827:   change was made by Halsey (responsive step) or unknown — his statement;
L1828:   (b) the on-device 730/1,074 screen — screenshot from Halsey's device;
L1829:   (c) Screens Connect vulnerability analysis document — locate. W2 window
L1830:   acquisition list (§7.3) grows: Apple device history, this notice, the
L1831:   bank virus-detection notice (EV-069 lead), Mac purchase record.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-065 annotation item 3:
```text
L1776: 3. W2 WINDOW DOCUMENT (new, third-party, §7.3 acquisition list): "On
L1777:    February 27, 2026, Apple issued a security alert identifying 730 of
L1778:    1,074 stored passwords as compromised. Forensic review traced the
L1779:    intrusion vector to a Screens Connect remote-access vulnerability…"
L1780:    HUNT: locate the Apple alert native (institution's own send, §7.4).
```

#### EV-075 [1/2] (L1908) — tags: a, police
Title: Written preservation demands EARLIER than EV-054's six — three natives (SET)

Operative text (verbatim):
```text
L1908: EV-075 · Written preservation demands EARLIER than EV-054's six — three natives (SET)
L1909: - What: (1) 2025-10-01T04:10Z, "Hacking of Computer Matching Report to BHPD"
L1910:   (Q): "Every day you don't contact Google, emails get destroyed for good.
L1911:   ... police have a separate, more efficient way of preventing the
L1912:   destruction of evidence that occurs each day, yet you continue to do
L1913:   nothing." — THE EARLIEST written demand now known, 12 days before EV-069.
L1914:   (2) 2025-11-04, (Q): "Alex, I want you to inform Google that an
L1915:   evidentiary packet, including emails provided to you, led to a hacking of
L1916:   my computer." (3) 2025-12-03, (Q): "I am asking, under Marcy's Law,
L1917:   whether you intend to contact Google to stop the scheduled deletion of
L1918:   emails from Shannon Minor that precisely match the police report you
L1919:   received".
L1920: - Original: Gmail 1999df6b5ce0fbce · 199db7e78dd8b1de (=EV-069) ·
L1921:   19a4cb0a7fd791b2 · 19ae68bf08204bd5.
L1922: - Tag: (V/Q) — read at source by the verification agent 2026-08-13 (run
L1923:   wf_0bba0c9f-b95); full-body re-open owed before exhibit print.
L1924: - Used by: 1983 (primary) + POLICE.
L1925: - Notes: 2026-08-13 registered. With EV-054's six and EV-069, the dated
L1926:   written-demand LIST numbers at least TEN (10/1, 10/13, 10/22, 11/4, 12/3,
L1927:   12/6, 1/5, 1/8, 1/10, 2/12). Plead the list, never an adjective.
L1928:   Computed anchors: 103 days (10/1/25 → 1/12/26 request); 91 days
L1929:   (10/13/25 →). The 10/1 email also states "The email account takeover and
L1930:   deletion occurred in October 2023" — keep the two deletion events
L1931:   distinct (W1 2023 vs W2 2025, OP.COND. §7.3/§9).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- 2026-08-27 block (D-1 and duplicate-id notice):
```text
L3436: - Per governance/DECISIONS.md **D-1**: every "candidate sixth/seventh demand"
L3437:   phrasing in this index and its notes is **SUPERSEDED**. The asserted
L3438:   preservation-demand count is FIVE (his ruling; EV-054 criteria). Located
L3439:   demand-like documents beyond the five (EV-069; the EV-075 demand set;
L3440:   Gmail 199db7e78dd8b1de) remain library documents under D-6 and enter no
L3441:   count absent his express reclassification.
L3442: - **DUPLICATE-ID NOTICE:** "EV-075" and "EV-076" were each assigned to TWO
L3443:   different entries (the Apr–Sep 2025 demand/deletion-window sets AND the
L3444:   July-2023 exchange/message entries). Until the owning thread renumbers by
L3445:   append, citations to these four entries must use TITLE + MESSAGE ID, not
L3446:   the bare EV number. (Allocation lessons 2026-08-07 / 2026-08-12.)
```
- KALE CHRONOLOGY item 1 (full text in B5).

#### EV-076 [1/2] (L1933) — tags: a, f, police
Title: Deletion-window and discovery natives, Apr–Sep 2025 (SET — the causation spine)

Operative text (verbatim):
```text
L1933: EV-076 · Deletion-window and discovery natives, Apr–Sep 2025 (SET — the causation spine)
L1934: - What: (1) DISCOVERY 2025-07-28T06:51Z to counsel Snyder (Q): "The emails
L1935:   have now been erased in my email account. All I have now are print outs.
L1936:   ... Thankfully I exported up to August 2024 but recent emails are gone.
L1937:   ... Google can likely still can retrieve it but its like 6 months".
L1938:   (2) 2025-09-27 to Kale (Q): "the messages erased in this recent
L1939:   cyberattack 4 months ago PRECISELY match the incriminating evidence I
L1940:   entrusted to your department" + "Exclusive Possession: Only your
L1941:   department possessed that exact collection of incriminating emails at the
L1942:   time of the breach." (3) Halsey's 10/16/25 letter to Google (Q): breach
L1943:   "[i]n the timeframe between April 2025 and September 2025"; requests
L1944:   preservation of emails deleted "between approximately April 1, 2025 and
L1945:   September 1, 2025". (4) Snyder 2025-08-04 (Q): "You have to report the
L1946:   hacking to the police department. I will contact Det. Kale"; Snyder
L1947:   2025-08-05 (Q): "In scores of investigations, emails and metadata were
L1948:   recovered from the providers including Google several years after the
L1949:   date of the original communication."
L1950: - Original: Gmail 1984fd6ec53551c4 · 1998c027ef83cc88 · 199ec75f75e16cd7
L1951:   (letter; bounce = EV-052) · 198768bdcb030829 · 1987c51a21963f01 ·
L1952:   198717bc1e84199f (8/3 "Lance Planted Malware...") · 1987c30b472820da.
L1953: - Tag: (V/Q) — read at source by the verification agent 2026-08-13;
L1954:   full-body re-open owed before exhibit print.
L1955: - Used by: 1983 (primary) + POLICE + CIVIL.
L1956: - Notes: 2026-08-13 registered. Deletion (~Apr–Sep 2025, discovered
L1957:   7/28/25) PRECEDES every written demand — so the §1983 causation theory
L1958:   must ride the provider-side recoverability window (Snyder's years-later
L1959:   recovery statement + Kale's own 1/12/26 "assuming they are still
L1960:   preservable" hedge). Complaint3's specific "August 4, 2025" deletion
L1961:   date remains UNSOURCED at native level — test owed.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- 2026-08-27 duplicate-id notice:
```text
L3442: - **DUPLICATE-ID NOTICE:** "EV-075" and "EV-076" were each assigned to TWO
L3443:   different entries (the Apr–Sep 2025 demand/deletion-window sets AND the
L3444:   July-2023 exchange/message entries). Until the owning thread renumbers by
L3445:   append, citations to these four entries must use TITLE + MESSAGE ID, not
L3446:   the bare EV number. (Allocation lessons 2026-08-07 / 2026-08-12.)
```

#### EV-079 (L2091) — tags: a, police
Title: "Comparison of Shannon Minor's Emails in PDF vs Gmail (July 2022 – August 2023)" — THE DELETION DOCUMENT (delivered to BHPD 10/2/2025)

Operative text (verbatim):
```text
L2091: EV-079 · "Comparison of Shannon Minor's Emails in PDF vs Gmail (July 2022 – August 2023)" — THE DELETION DOCUMENT (delivered to BHPD 10/2/2025)
L2092: - What: 4-page analysis cross-referencing the pre-hacking PDF export against
L2093:   the live Gmail account, listing SEVENTEEN Shannon Minor emails present in
L2094:   the PDF and not found in Gmail, WITH THEIR FULL BODY TEXT. Footnotes cite
L2095:   the source by PDF page ("pdf page 152 of 567") — the 567-page package BHPD
L2096:   holds. Full recovered text + my independent live-account verification:
L2097:   matters/04/report_2026-08/23_DELETED_EMAILS_RECOVERED_TEXT_2026-08-12.md.
L2098: - Original: Drive 1IUm-tR81jO1d788zlS80MbuBGxXm4eHp · 35,898 B · created
L2099:   2025-09-01 · parent 1UvJnv1p9U32us77s4NQU4dDy2blfKRck. Copy:
L2100:   15d5x6yrAHvjV45-H2wzlAVNGELpJemZf. Delivered to BHPD as an EV-078
L2101:   attachment 2025-10-02.
L2102: - Hash: not computed — Drive id + byte size recorded.
L2103: - Tag: (V) read in full at source 2026-08-12; (U) as Halsey-adopted analysis.
L2104: - Used by: POLICE (PRIMARY) + CIVIL + 1983.
L2105: - Notes: 2026-08-12 registered. **INDEPENDENTLY VERIFIED BY THIS THREAD, from
L2106:   the live account, today: #12 (12/30/2022 "we are broke… There is NO money")
L2107:   ABSENT; #16 (5/28/2023 "You owe Joyce over 2 million dollars") ABSENT; #11
L2108:   (11/13/2022 "Please go get Grace") ABSENT.** **DEFECT RECORDED, LOUDLY AND
L2109:   ONCE (F-02): entry #17 (8/16/2023 "Where are you?") is listed as missing
L2110:   but IS LIVE (EV-077, 189ffbe65b4fdf4d) — and the document's own footnote 22
L2111:   links to it.** The document also offers its own alternative explanation
L2112:   (Q): "likely because they were sent to a different email address or have
L2113:   since been removed" — and several entries were addressed to
L2114:   halsey@liveplanet.net / the CPA, so absence from the main mailbox does not
L2115:   establish deletion for those. FORM: the packet verifies each entry
L2116:   individually across BOTH accounts and cites the verified subset; it never
L2117:   pleads "seventeen deletions" on the document's say-so. Thirteen entries
L2118:   remain untested pending secondary-account access.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-089 "cuts both ways":
```text
L2503: - **CUTS BOTH WAYS, stated: it weakens EV-079's own innocent explanation.**
L2504:   "Likely sent to a different email address" cannot explain absence for any
L2505:   address inside this family. It survives only for addresses outside it
L2506:   (dan@asacpa.com, chad@nt-llp.com, chminetree@gmail.com).
```
- C-08:
```text
L2539: --- CORRECTION C-08 · EV-079 DATES FOR ENTRIES #3/#4 — 2026-08-12 ---
L2540: EV-079 dates the Carol Minetree messages **#3 Nov 5, 2022 1:47 PM** and
L2541: **#4 Nov 5, 2022 4:03 PM**. **Both the pre-intrusion export (EV-087) and the
L2542: live account date the thread Nov 6, 2022.** The ABSENCE finding is unaffected
L2543: and is now independently verified (EV-091). **The DATES are not confirmed and
L2544: must not be pleaded as EV-079 states them** until the original is obtained
L2545: from Carol Minetree. F-01 family: a checkable date that is wrong costs more
L2546: than the point it was meant to carry.
```
- EV-078 upgrade: delivery to BHPD confirmed:
```text
L2561: **TWELVE ATTACHMENTS ENUMERATED EXACTLY** (file 29_ §6.1) — this is what BHPD
L2562: received on 10/2/2025. **EV-079's delivery to BHPD is now confirmed from the
L2563: sent message itself, not inferred.** Attachment 12's filename states **512
L2564: pages**, scope 11/01/2022–12/30/2024, "Excludes First Hacking And Vanguard" —
L2565: **512 ≠ the 567 EV-079's footnotes cite**; joins the unresolved 54/51/24
L2566: conflict, and no [PKG line N] cite is final until settled.
```
- EV-099 running total:
```text
L2945: - **ALL FIVE VERIFIED BY ME TODAY.** Two overlap EV-079 (12/30/2022 #12;
L2946:   5/10/2023 #15 — and this supplies the subject line EV-079 omitted, **"There
L2947:   is no money!"**). **Three are NEW:** 12/31/2022 "Happy New Year"; the
L2948:   3/7/2023 balance email; ~6/1/2023 "there is zero cash". `from:
L2949:   shannonminor@gmail.com after:2022/12/30 before:2023/01/03` → **empty**;
L2950:   `"318,248"` and `"zero cash"` → no 2022-23 hit. **Running total: 15 verified
L2951:   absences, 2 verified present, 3 undated.**
```
- EV-108 consequence 2:
```text
L3390: - **CONSEQUENCE 2 — THE PLANNED "LANCE-MOTION OVERLAP TABLE" HAD A FALSE
L3391:   PREMISE AND IS REPLACED.** This motion challenges the Spiegel log only —
L3392:   it contains NO list of Shannon emails. The documentable overlap is
L3393:   different and needs no probability figure: **the emails verified absent
L3394:   from the live account ARE emails cited in the analysis package given to
L3395:   BHPD** — EV-079 was constructed exactly that way (report-package
L3396:   citations vs live Gmail), and 15 of its 17 entries verified absent
L3397:   (30_/35_). v1 §8 states that overlap from the verified rows and leaves
L3398:   the leak QUESTION as a question (what it is), supported by the
L3399:   selectivity proof — never by the discarded statistic.
```

#### EV-087 (L2440) — tags: a, exF, police
Title: THE DUAL-EXPORT "YES MESSAGES" SET — the control set authenticating itself

Operative text (verbatim):
```text
L2440: EV-087 · THE DUAL-EXPORT "YES MESSAGES" SET — the control set authenticating itself
L2441: - What: six files in Drive folder FORENSIC EVIDENCE
L2442:   (`1Fm9plSUzly10tIpdNqrYtD-PBoOIrBdZ`) presenting the SAME November 2022
L2443:   conversations from **two independently saved 1.5-year PDF exports**. The
L2444:   first file's own opening (Q): "2 DIFFERENT SAVED PDFS ~1.5 YEARS ALL
L2445:   COMMUNICATION"; the second block is headed "2ND FILE OF SAVED EMAILS."
L2446:   The two exports paginate differently (**"N / 62"** vs **"N / 58"**), so
L2447:   they are not one file copied — yet their overlapping content is
L2448:   **character-for-character identical**.
L2449: - Ids READ IN FULL 2026-08-12: `1hdLvGPCBW1TxCjegaRuuQPq294PKMeJk` (437,008 B),
L2450:   `1B9rS4E1aTbsjggV8sHO2f0c_7_vXTWvn` (205,862 B),
L2451:   `1lpWcvv4NhcPJXclzwxzFXgxHgKka4CFV` (164,918 B).
L2452:   Ids UNREAD (the full exports): `1lYhOFHXU9jbKBg_GVw_Jp7aFctaBf-o0`
L2453:   (58,768,722 B), `1DLVF3_tUYSbV41yx0Rk33jfzFuzaGEJN` and
L2454:   `12SxdmRCBLqaRI0wDhZLbZnmVIcJuB7zv` (58,783,197 B each).
L2455: - **WHY IT MATTERS:** where the same message exists in the export and in the
L2456:   live account, the headers match **to the second** — verified on four
L2457:   messages (11/6, 11/7, 11/11 ×2). This is the §7.1/§7.2 authentication
L2458:   baseline demonstrated rather than asserted.
L2459: - Tag: (V) as to the three files read and the four header comparisons run.
L2460: - Used by: POLICE (PRIMARY) + CIVIL.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- C-08 (export vs EV-079 dates):
```text
L2539: --- CORRECTION C-08 · EV-079 DATES FOR ENTRIES #3/#4 — 2026-08-12 ---
L2540: EV-079 dates the Carol Minetree messages **#3 Nov 5, 2022 1:47 PM** and
L2541: **#4 Nov 5, 2022 4:03 PM**. **Both the pre-intrusion export (EV-087) and the
L2542: live account date the thread Nov 6, 2022.** The ABSENCE finding is unaffected
L2543: and is now independently verified (EV-091). **The DATES are not confirmed and
L2544: must not be pleaded as EV-079 states them** until the original is obtained
L2545: from Carol Minetree. F-01 family: a checkable date that is wrong costs more
L2546: than the point it was meant to carry.
```
- §7.6 GATE affirmative authentication:
```text
L3205: (Halsey's direction, 2026-08-23) discloses the finding in the order's words,
L3206: states his explanation, states the different-set fact, then the affirmative
L3207: authentication (EV-087 dual export; to-the-second live matches; third-party
L3208: originals; bank/carrier corroboration). Residual named: pull the actual
```

#### EV-088 (L2462) — tags: a, f, da, police
Title: "CONFIDENTIAL FORENSIC AUDIT & PUBLIC CORRUPTION REPORT" (1/8/2026) — READ IN FULL, AND IT HAS THREE CHECKABLE DEFECTS

Operative text (verbatim):
```text
L2462: EV-088 · "CONFIDENTIAL FORENSIC AUDIT & PUBLIC CORRUPTION REPORT" (1/8/2026) — READ IN FULL, AND IT HAS THREE CHECKABLE DEFECTS
L2463: - What: 1/8/2026 audit asserting a "Scalpel Protocol" — selective deletion of
L2464:   only the emails cited in the confidential police report, therefore a BHPD
L2465:   leak. Drive `1GUx4KFVuaE1OvXdMkBBRo4i53hcFPzFR` (193,440 B); same text also
L2466:   at `1o28AfWU4R54gaQKyk0P-OrNsjdJ4aULa` (129,187 B). Closing section
L2467:   addresses the FBI and the DA.
L2468: - **The strong part, which survives everything below:** the deletions were
L2469:   SELECTIVE, not a wipe — some messages from a sender on a given day gone,
L2470:   others from the same sender the same day intact.
L2471: - **DEFECT 1 — Exhibit A asserts a deletion that did not occur.** It states
L2472:   the 11/11/2022 "Yes! Large number has a 10 day hold" email is "DELETED
L2473:   (Surgically removed from server)." **Tested live 2026-08-12: thread
L2474:   `18461348b9fe0954` is INTACT, all five messages** — `18461348b9fe0954`,
L2475:   `18467dbd3ea6fa47`, `18467dd2c7361b33`, `1846822a40fdff6d`,
L2476:   `1846823e63d233ca`. It is also the basis of EV-067. Innocent readings
L2477:   stated: post-audit Google recovery (EV-049/050), or the assertion was never
L2478:   checked.
L2479: - **DEFECT 2 — the statistic does not measure what it claims.** "P = 1 /
L2480:   C(116,000, 5)" → "One in Ten Billion" models a blind draw; an intruder with
L2481:   account access selects by search, not by chance, so the competing
L2482:   explanation is not excluded. F-21 family.
L2483: - **DEFECT 3 — wrong case number on the cover.** "CASE REF: BHPD Case
L2484:   #24STFL00432" — 24STFL00432 is the FAMILY COURT number; BHPD's is
L2485:   2025-14983 (EV-037).
L2486: - Tag: (V) as to its contents, read in full. **(X) as to Exhibit A's
L2487:   deletion claim — CONTRADICTED at source.**
L2488: - Notes: this document has already gone to authorities. Correction is
L2489:   Halsey's decision (§10); recorded here as a finding with its tests.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-098 on the same email:
```text
L2927: - **WHAT THE DISPUTE WAS ABOUT** (`19c27f6dc533be58`, 2/4/2026, Q): "I am
L2928:   specifically talking about the **November 11, 2022 email confirming receipt
L2929:   of the tax refund**" — **the exact email EV-088's Exhibit A calls
L2930:   "surgically removed," and which is PRESENT in the live account today.**
L2931:   The one test that could rehabilitate that exhibit: **Google account activity
L2932:   and recovery records for thread `18461348b9fe0954`.**
```

#### EV-089 (L2491) — tags: a, d [fn8], e [fn8]
Title: THE FOUR-ADDRESS FINDING — liveplanet / minorventures / vividlabs ALL deliver into halsey2005@gmail.com

Operative text (verbatim):
```text
L2491: EV-089 · THE FOUR-ADDRESS FINDING — liveplanet / minorventures / vividlabs ALL deliver into halsey2005@gmail.com
L2492: - What: a verification result, not a document. Messages exist in
L2493:   halsey2005@gmail.com with that address in **neither To nor Cc**:
L2494:   `18467dd2c7361b33` (To: halsey@minorventures.com only, no Cc);
L2495:   `18454b35eacde372` (To: minorventures; Cc: chad/dan/liveplanet);
L2496:   `189ff8e8aaeb0f47` (To: liveplanet + minorventures);
L2497:   `16413f42f96f7208` (2018, To: **halsey@liveplanet.net alone**).
L2498: - **CLOSES A DECISION-QUEUE ITEM.** "Access to halsey@liveplanet.net —
L2499:   thirteen of the seventeen can only be finished there" was my own premise
L2500:   and it was **wrong**. There is no separate mailbox to obtain; the twelve
L2501:   remaining EV-079 entries are testable now, by me, with no access Halsey
L2502:   has to grant.
L2503: - **CUTS BOTH WAYS, stated: it weakens EV-079's own innocent explanation.**
L2504:   "Likely sent to a different email address" cannot explain absence for any
L2505:   address inside this family. It survives only for addresses outside it
L2506:   (dan@asacpa.com, chad@nt-llp.com, chminetree@gmail.com).
L2507: - **LIMIT, stated:** this proves alias mail is DELIVERED here. It does not
L2508:   prove the mailbox retains everything delivered — which is the allegation
L2509:   itself. Alias delivery makes an absence test meaningful; it does not make
L2510:   any particular absence innocent or guilty.
L2511: - Tag: (V) — four named message ids, queries reproducible.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-099 confirms the alias finding:
```text
L2940: - **IT CONFIRMS THE ALIAS FINDING FROM HALSEY'S OWN CORPUS.** Header (Q):
L2941:   "halsey2005@gmail.com or Halsey@minorventures.com (**aliases delivering to
L2942:   the same Gmail inbox**) and/or halsey@liveplanet.net." **He had already
L2943:   documented what I treated for a session as a blocker needing his
L2944:   intervention. The answer was in the corpus.**
```

#### EV-091 (L2526) — tags: a, police
Title: THE CAROL MINETREE THREAD — the deleted message survives inside someone else's reply

Operative text (verbatim):
```text
L2526: EV-091 · THE CAROL MINETREE THREAD — the deleted message survives inside someone else's reply
L2527: - What: live thread `1844d84b3e8e369f`, read 2026-08-12. Two messages:
L2528:   Carol Minetree 11/6/2022 07:17, Shannon 11/6 09:22 (Q) "Carol, Fuck off!"
L2529: - **Shannon's earlier message — "the gravy train doesn't exist anymore," the
L2530:   $750/month, "No bills will be paid or addressed till January" — is NOT
L2531:   present as its own message.** Its text survives **only as a block quoted
L2532:   inside Carol's reply**. Sweep `in:anywhere "gravy train"` returns no
L2533:   Shannon message in 2022 or 2023 → **FOURTH VERIFIED DELETION**
L2534:   (with 12/30/22, 5/28/23, 11/13/22).
L2535: - **Carol Minetree holds the original in her own mailbox** and is a friendly
L2536:   third party — an ask, not a subpoena.
L2537: - Tag: (V) absence; (Q) the surviving quoted text.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- C-08:
```text
L2539: --- CORRECTION C-08 · EV-079 DATES FOR ENTRIES #3/#4 — 2026-08-12 ---
L2540: EV-079 dates the Carol Minetree messages **#3 Nov 5, 2022 1:47 PM** and
L2541: **#4 Nov 5, 2022 4:03 PM**. **Both the pre-intrusion export (EV-087) and the
L2542: live account date the thread Nov 6, 2022.** The ABSENCE finding is unaffected
L2543: and is now independently verified (EV-091). **The DATES are not confirmed and
L2544: must not be pleaded as EV-079 states them** until the original is obtained
L2545: from Carol Minetree. F-01 family: a checkable date that is wrong costs more
L2546: than the point it was meant to carry.
```

#### EV-092 (L2587) — tags: g [fn9], police
Title: THE WHATSAPP SCREENSHOT CORPUS — 234 files, 656 statement rows, harvested without a single download

Operative text (verbatim):
```text
L2587: EV-092 · THE WHATSAPP SCREENSHOT CORPUS — 234 files, 656 statement rows, harvested without a single download
L2588: - What: Drive folder `1-14wNOUvTP5lQeLyFSIa9yZn4DGsXWp_` (owner
L2589:   Halsey@realitylab.com, all 234 objects ingested 2024-11-23). Composition:
L2590:   **118** "Shannon A.Minor" thread screenshots captured on the handset on
L2591:   **2024-07-25 between 11:48:48 and 12:31:53** (a single deliberate capture
L2592:   session), **68** other screenshots, **48** dated camera photographs
L2593:   (27 Aug – 26 Nov 2023). Full harvest + ledger:
L2594:   matters/04/report_2026-08/25_WHATSAPP_SCREENSHOT_OCR_HARVEST.md.
L2595: - Method: Google's server-side OCR index read through the connector. **No file
L2596:   downloaded** — this is the channel that defeats the 10 MB cap and the Drive
L2597:   egress block for images.
L2598: - **Coverage, stated honestly: OCR obtained for 88 of 118 thread screenshots.
L2599:   The other 30 have NO Drive OCR record — their content is UNHARVESTED, not
L2600:   absent, and must be read from the images.**
L2601: - Thread date range captured: **26 Aug 2023 → 13 Jan 2024**, 22 date dividers.
L2602: - Tag: (Q) as to text; **(X) as to every speaker — see below**.
… [L2603–L2696 not reproduced here]
L2697: **9. ALSO IN THE FOLDER, non-thread:** a helium-cylinder supplier web page
L2698: screenshot dated **6 Oct 2023** (`11kdVWKj8IkOxLZ3FKdqJtfj6Ygapsqib`, OCR'd in
L2699: full, same supplier region as the 11 Sep in-thread link) — a browser capture,
L2700: not a message, so no sender question arises but the custodian question does;
L2701: an **Anthem Blue Cross member-ID email**, 29 Aug 2023; and an **Ally account
L2702: 1113860942 at −$76.97**, 19 Sep 2023 — two days after the second attempt.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- ATTRIBUTION rule:
```text
L2604:   **ATTRIBUTION — ALL 656 ROWS ARE `UNDETERMINED` (§17.6, held absolutely).**
L2605:   A `✓` delivery-receipt glyph does appear in the OCR, and in WhatsApp renders
L2606:   only on outgoing messages. **It was NOT used as a side marker**, for four
L2607:   documented reasons: Drive's OCR flattens the two-column bubble layout into
L2608:   one stream with timestamps demonstrably transposed against their bodies; the
L2609:   glyph OCRs inconsistently as ✓/✔/v/Q/p/D/♡/y or drops entirely; a correctly
L2610:   read glyph still cannot be bound to a specific adjacent message; and bubble
L2611:   alignment and colour — the only reliable indicators — do not survive an OCR
L2612:   channel at all. It is logged as `[✓ nearby]`, an investigative pointer,
L2613:   expressly not an attribution. **No line goes to an investigator as a named
L2614:   person's words until the side is fixed from the images or the handset.**
```

#### EV-098 (L2907) — tags: a [fn7], police
Title: KALE'S DENIAL AND THE 567-PAGE CONFIRMATION

Operative text (verbatim):
```text
L2907: EV-098 · KALE'S DENIAL AND THE 567-PAGE CONFIRMATION
L2908: - What: `19ba02a9c00c3b61`, **1/9/2026**, akale@beverlyhills.org (Q): "Halsey,
L2909:   **I'm sorry you think I destroyed evidence, but I assure you I did not. I
L2910:   would not risk my career over something as silly as that.** Like I said —
L2911:   **we have the 567-page document you sent us**…"
L2912: - **(a) The package count is answered from BHPD's own side: 567 pages.**
L2913:   Against the 632 in the 7/5/2023 email's filename and the 512 in the EV-078
L2914:   attachment filename. It does not dissolve the conflict — those objects
L2915:   exist and must be identified — but it fixes **what BHPD holds**, which is
L2916:   the count that governs any `[PKG line N]` cite to a police-held exhibit.
L2917: - **(b) His denial goes in the RECORD, quoted in full.** The report is a
L2918:   two-instrument document; quoting the investigating officer's own denial is
L2919:   what makes the surrounding account credible.
L2920: - **ADVERSE FACT, RECORDED DELIBERATELY:** `19b9f2badaeb5eeb`, 1/8/2026, Kale
L2921:   (Q): "**I emailed you on Monday asking you one question about those very
L2922:   same emails, and you did not respond.** See below email I sent you on
L2923:   **01/05/2026 at 11:57AM** and please answer:" — the record shows the
L2924:   detective attempting contact on **1/5/2026** and Halsey's substantive reply
L2925:   arriving **2/4/2026** (`19c27f6dc533be58`), **27 days later**. Any packet
L2926:   that omits this is one document away from collapsing.
L2927: - **WHAT THE DISPUTE WAS ABOUT** (`19c27f6dc533be58`, 2/4/2026, Q): "I am
L2928:   specifically talking about the **November 11, 2022 email confirming receipt
L2929:   of the tax refund**" — **the exact email EV-088's Exhibit A calls
L2930:   "surgically removed," and which is PRESENT in the live account today.**
L2931:   The one test that could rehabilitate that exhibit: **Google account activity
L2932:   and recovery records for thread `18461348b9fe0954`.**
L2933: - Tag: (V)/(Q).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- KALE CHRONOLOGY item 5 (full text in B5).

#### EV-099 (L2935) — tags: a, police
Title: THE SECOND DELETION COMPARISON — better built than EV-079, and it found the balance email

Operative text (verbatim):
```text
L2935: EV-099 · THE SECOND DELETION COMPARISON — better built than EV-079, and it found the balance email
L2936: - What: `16Xiho9OW-ozxRecJkwhULmjpxg1DmV0Q` · "Document (8) copy.docx" ·
L2937:   folder Hacking · **READ IN FULL 2026-08-12.** "Exhibit: Emails present in
L2938:   your PDF but not in your Gmail today." **Five entries, each stating the
L2939:   exact Gmail queries run** — checkable, which EV-079 is not.
L2940: - **IT CONFIRMS THE ALIAS FINDING FROM HALSEY'S OWN CORPUS.** Header (Q):
L2941:   "halsey2005@gmail.com or Halsey@minorventures.com (**aliases delivering to
L2942:   the same Gmail inbox**) and/or halsey@liveplanet.net." **He had already
L2943:   documented what I treated for a session as a blocker needing his
L2944:   intervention. The answer was in the corpus.**
L2945: - **ALL FIVE VERIFIED BY ME TODAY.** Two overlap EV-079 (12/30/2022 #12;
L2946:   5/10/2023 #15 — and this supplies the subject line EV-079 omitted, **"There
L2947:   is no money!"**). **Three are NEW:** 12/31/2022 "Happy New Year"; the
L2948:   3/7/2023 balance email; ~6/1/2023 "there is zero cash". `from:
L2949:   shannonminor@gmail.com after:2022/12/30 before:2023/01/03` → **empty**;
L2950:   `"318,248"` and `"zero cash"` → no 2022-23 hit. **Running total: 15 verified
L2951:   absences, 2 verified present, 3 undated.**
… [L2952–L2977 not reproduced here]
L2978: - Tag: (Q) text from the exhibit; (V) as to the five absences, tested by me.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- C-11:
```text
L3070: --- CORRECTION C-11 · EV-099 ENTRY #5 IS MAY 23, 2023 — and it is her reply
L3071: to the polygraph demand ---
L3072: The "zero cash / Our marriage is over / putting us on the street" email,
L3073: estimated "~6/1/2023" in EV-099, is dated **May 23, 2023** on the face of
L3074: the police-held image [EV-036 p.46], where it appears as Shannon's direct
L3075: reply to Halsey's (Q) "I want to have a lie detector t[est]…" and "Get the
L3076: $250k back from your mom." Absence-from-live-Gmail verification unaffected
L3077: (the sweep was date-agnostic). Sequence preserved on one page: polygraph
L3078: demand → "Our marriage is over… zero cash." Fourteen days before The Plan.
```

#### WP-019 [2/2] (L3012) — tags: c, d — DUPLICATE of EV-041 / EV-106
Title: Respondent's Brief re service/notice, filed ~3/27/2026 (24STFL00432)

Operative text (verbatim):
```text
L3012: WP-019 · Respondent's Brief re service/notice, filed ~3/27/2026 (24STFL00432)
L3013: - What: Halsey's 5-page brief answering the court's 3/2/2026 minute-order
L3014:   questions. Read at source 2026-08-20. Key positions (Q): CRC 5.92(f)(3)
L3015:   governs post-appearance RFO service (not Hague Central Authority); Mexico
L3016:   has objected to Hague Art. 10 postal channels, so if Hague applies, mail
L3017:   is unavailable; the mail service used failed Mullane/Jones v. Flowers
L3018:   (bundled 2/24/2026 delivery, months late); court should not retroactively
L3019:   validate defective service nor make unconsented email the sole formal
L3020:   method (CCP 1010.6(c), CRC 2.251(c)(3)(B)); ¶4 expressly preserves
L3021:   appellate review + CCP 473(d). Signed 3/27/2026.
L3022: - Preserved: preserved_2026-08-19/WP-019_Respondents_Brief_re_service_
L3023:   2026-03-27.pdf. Tag (U/Q — his filing; court-file conformed copy not
L3024:   in hand). Used by: FAMILY (+CIVIL context).
L3025: - Notes: 2026-08-20 registered. EV-002 (4/21/2026 order) is the RULING on
L3026:   this posture: objection DENIED (no appearance by Respondent; court found
L3027:   notice given), BUT the prospective protocol ordered — "trackable method
L3028:   via the mail, and any proof of service shall include tracking details.
L3029:   As a backstop, all service shall also be effectuated by electronic
L3030:   means" — substantially ADOPTS the brief's own proposed protocol.
L3031:   EV-002 read at source 2026-08-20 (Q). Note: the order makes electronic
L3032:   service a mandatory BACKSTOP (supplement), not the sole formal method —
L3033:   the brief's red line. Whether it validly compels e-service on a
L3034:   non-consenting pro se is the preserved appellate question.
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### WP-020 [2/2] (L3036) — tags: a, c, d, exF [fn4], da — DUPLICATE of EV-042 / EV-107
Title: Declaration of Respondent in support of Brief + Exhibits A-C

Operative text (verbatim):
```text
L3036: WP-020 · Declaration of Respondent in support of Brief + Exhibits A-C
L3037: - What: sworn declaration, executed 3/27/2026, Cancún. Key content (Q):
L3038:   ¶3 "I have not filed Judicial Council form EFS-005-CV or any other
L3039:   written consent to electronic service... never affirmatively authorized
L3040:   ... email as formal service of motion papers"; ¶¶4-6 bundled delivery
L3041:   2/24/2026 of multiple months-late mailings (Ex A photos + front-desk
L3042:   records; Ex B witness declarations); ¶8 fabricated documents inserted in
L3043:   his files during unauthorized access; ¶9 five requests to the
L3044:   investigating officer for a Google evidentiary hold; ¶10 criminal
L3045:   referral re Petitioner's counsel under DA review. 15 pages; Exhibits
L3046:   A/B/C are image pages (not OCR'd this pass).
L3047: - Preserved: preserved_2026-08-19/WP-020_Declaration_re_Brief_ExA-C_
L3048:   2026-03-27.pdf. Tag (U/Q). Used by: FAMILY (+CIVIL P036-P037 corroboration
L3049:   context; ¶¶8-10 touch police-activity subject matter — cite only the
L3050:   service content from this thread).
L3051: - Notes: 2026-08-20 registered. Feeds SERVICE_VIOLATIONS_LOG rows (the
L3052:   2/24/2026 bundled-delivery event now has sworn + photographic + witness
L3053:   locators). CONSISTENCY FLAG for future filings: Halsey stated in-session
L3054:   2026-08-19 (U) that he "consented to initial service by email ... so we
L3055:   could exchange documents" — reconcilable with ¶3 (scope: informal
L3056:   exchange vs formal e-service, no EFS-005-CV) but every future filing
L3057:   should state the consent scope identically to avoid impeachment.
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-104 (L3159) — tags: g [fn9], police
Title: THE F50 IMAGE-SECTION EXTRACTION — pp.13–54 text layer, mirrored

Operative text (verbatim):
```text
L3159: EV-104 · THE F50 IMAGE-SECTION EXTRACTION — pp.13–54 text layer, mirrored
L3160: - What: 36a_F50_PP13-54_TEXT.md — machine extraction of EV-036 pp.13–15 and
L3161:   31–54 (pp.16–30 partially; 16–18 image-only). New dated ledger rows
L3162:   catalogued in 36_ §3.6, including: his 12/30/2022 accounting demand
L3163:   ("Pool? Basketball court? Deer valley?… where $650,000 went in 2
L3164:   months"); the 1/23-24/2023 "**The money you took out of the $1.15 mm**"
L3165:   (earliest direct taking accusation); the 1/31/2023 expulsion/degradation
L3166:   set ("**No, you actually need to go**… Go get it!" · "crashed a car…3
L3167:   credit cards 'stolen'. Gig is up"); 3/21/2023 "I have zero cash" → Lilly:
L3168:   "**There is cash now in the ally account**" (Ally's first appearance;
L3169:   cross-vector EV-092's Ally 1113860942); the completed 4/7/2023 insurance
… [L3170–L3184 not reproduced here]
L3185: - Tag: (Q) per page cite [F50 p.N]; senders as shown on the images; every
L3186:   quote checkable against the hash-verified PDF.
```
Applicable corrections / withdrawals: none specific to this entry; only the index-wide blocks B3/B4/B8 apply.

#### EV-106 (L3252) — tags: c, d, exF — DUPLICATE of EV-041 / WP-019 [2/2]
Title: RESPONDENT'S BRIEF, 3/27/2026 — the service brief; the appellate-preservation source

Operative text (verbatim):
```text
L3252: EV-106 · RESPONDENT'S BRIEF, 3/27/2026 — the service brief; the appellate-preservation source
L3253: - What: 5-page filed brief (24STFL00432), read IN FULL 2026-08-23. Mirror:
L3254:   uploads_2026-08-23/EV-106_… · sha256 ebdf5204f88e…
L3255: - Holds: the court's own 3/2/2026 order "already recognized that the
L3256:   sanctions RFO could not proceed because the timing required for service
L3257:   to Mexico had not been satisfied"; the 2/24/2026 bundled-delivery
L3258:   evidence framing; Hague/CRC 5.92(f)(3)/Mullane/Jones v. Flowers/Peralta
L3259:   argument; **¶4: express preservation for appellate review (CRC 8.104;
L3260:   CCP 904.1; §473(d)) of "the validity of all prior orders entered without
L3261:   constitutionally adequate service and notice."**
L3262: - USE: one posture sentence in §12's §271 confrontation — the finding is
L3263:   disclosed AND its pendency inside a preserved service challenge with an
L3264:   appeal in process (U as to filing status) is stated, sourced here. The
L3265:   family-court-grievance exclusion otherwise holds.
L3266: - Tag: (V)/(Q) — filed document, adopted source (§8).
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- EV-003 POSTURE (full text in B2).

#### EV-107 (L3268) — tags: a, c, d, exF, da, police — DUPLICATE of EV-042 / WP-020 [2/2]
Title: DECLARATION OF RESPONDENT, 3/27/2026 (sworn) — the second sworn five-count, and the bundled-delivery record

Operative text (verbatim):
```text
L3268: EV-107 · DECLARATION OF RESPONDENT, 3/27/2026 (sworn) — the second sworn five-count, and the bundled-delivery record
L3269: - What: 3-page sworn declaration + Exhibits A/B/C (image-bound), read IN
L3270:   FULL 2026-08-23 (decrypted; AES). Mirror: uploads_2026-08-23/EV-107_… ·
L3271:   sha256 e22c423b5260…
L3272: - ¶3: no e-service consent ever filed (no EFS-005-CV). ¶¶4-6: the 2/24/2026
L3273:   bundled delivery — photographs, front-desk records, and **two witness
L3274:   declarations** (Exhibits A/B). **¶8 (sworn): "documents that had been
L3275:   created and inserted into my files that I had never authored… created
L3276:   using my accounts during the period of unauthorized access."** **¶9
L3277:   (sworn): the Google evidentiary-hold request was made "on at least five
L3278:   separate occasions"; "The officer declined to do so on each occasion. The
L3279:   officer contacted Google only after an internal affairs inquiry was
L3280:   initiated"** — with documentary Exhibit C. ¶10: criminal referral re
L3281:   Petitioner's counsel "currently under review by the District Attorney's
L3282:   office" (his sworn characterization).
L3283: - **CONSEQUENCE FOR THE COUNT:** the five-request figure is now **sworn
L3284:   twice** (EV-042 ¶9 + this ¶9). The four-vs-five discipline holds — no
L3285:   count pleaded until natives resolve it — but the packet may state "sworn
L3286:   on two occasions as at least five" as exactly that.
L3287: - **SEPARATION RULE (binding for v1):** ¶8's planted-documents claim and
L3288:   the court's Exhibit-F finding are DIFFERENT FACTS — his on-record
L3289:   "narrative summary… was a mistake" explanation (EV-003) and this sworn ¶8
L3290:   are both stated, never merged, never offered as answering each other.
L3291: - Tag: (V)/(Q) sworn filed document, adopted source; exhibits image-bound.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- KALE CHRONOLOGY item 1 (full text in B5).
- 2026-08-27 block D-1:
```text
L3436: - Per governance/DECISIONS.md **D-1**: every "candidate sixth/seventh demand"
L3437:   phrasing in this index and its notes is **SUPERSEDED**. The asserted
L3438:   preservation-demand count is FIVE (his ruling; EV-054 criteria). Located
L3439:   demand-like documents beyond the five (EV-069; the EV-075 demand set;
L3440:   Gmail 199db7e78dd8b1de) remain library documents under D-6 and enter no
L3441:   count absent his express reclassification.
```

#### EV-108 (L3368) — tags: exF, a, b, f
Title: THE §271 SANCTIONS MOTION ITSELF (12/30/2025) — read in full, and it re-frames two things

Operative text (verbatim):
```text
L3368: EV-108 · THE §271 SANCTIONS MOTION ITSELF (12/30/2025) — read in full, and it re-frames two things
L3369: - What: "Lance's Motion for 271 Sanctions 3-2-2026.pdf", Drive
L3370:   `1r_5T4D4v4lwSbCWU1ZpO--6S9y4nRunT` (2,401,413 B): the FL-300 (filed
L3371:   12/30/2025, $250,000 demand), Spiegel's MPA + declaration, Exhibit 1
L3372:   (Halsey's own 10/31/2025 declaration) and Exhibit 2 (the challenged
L3373:   email log itself). **READ IN FULL 2026-08-23.**
L3374: - **THE CHALLENGED EXHIBIT, ON ITS FACE:** a chronological "log" of
L3375:   purported Halsey↔"Lance" emails 8/10/2021–7/25/2023 about obtaining his
L3376:   FINANCIAL STATEMENTS — citing FINRA Rule 2231 (a broker-dealer
L3377:   obligation), referencing a "client portal" and "my assistant Janine,"
L3378:   and carrying unfilled generator placeholders ("[User's Name]",
L3379:   "Lance [Last Name]", "[link]"). Spiegel's declaration: not retained
L3380:   until early 2024; never had an assistant named Janine; does not send
L3381:   links. **The document reads as an AI-generated narrative reconstruction
L3382:   with the wrong correspondent name attached — fully consistent BOTH with
L3383:   the court's fabrication finding AND with Halsey's on-record "narrative
L3384:   summary… was a mistake" explanation. v1 states both, adopts neither.**
L3385: - **CONSEQUENCE 1 — §7.6 CONFIRMED FROM THE MOTION ITSELF:** the
L3386:   challenged corpus is purported ATTORNEY correspondence about statement
L3387:   requests; it shares no correspondents and no content with the
L3388:   Halsey↔Shannon export family the report cites. Different set, now
L3389:   verified at the exhibit level, not just the order's description.
L3390: - **CONSEQUENCE 2 — THE PLANNED "LANCE-MOTION OVERLAP TABLE" HAD A FALSE
L3391:   PREMISE AND IS REPLACED.** This motion challenges the Spiegel log only —
L3392:   it contains NO list of Shannon emails. The documentable overlap is
L3393:   different and needs no probability figure: **the emails verified absent
L3394:   from the live account ARE emails cited in the analysis package given to
L3395:   BHPD** — EV-079 was constructed exactly that way (report-package
L3396:   citations vs live Gmail), and 15 of its 17 entries verified absent
L3397:   (30_/35_). v1 §8 states that overlap from the verified rows and leaves
L3398:   the leak QUESTION as a question (what it is), supported by the
L3399:   selectivity proof — never by the discarded statistic.
L3400: - ALSO IN EXHIBIT 1 (his own 10/31/2025 declaration), for the conflict
L3401:   log: it renders the prenup high-value threshold as ">$7,000" — the
L3402:   prenup as quoted in counsel's 3/29/2025 letter [F50 p.14] says
L3403:   **$5,000/FC §852**. v1 quotes the prenup only from its own text.
L3404: - Tag: (V)/(Q) — filed documents, read at source.
```
Applicable corrections / withdrawals / cross-notes (verbatim):
- §7.6 GATE (full text in B1).

### 3b. Blocks that apply to several tagged entries (verbatim, reproduced once)

#### B1 — §7.6 GATE — RESOLVED (different set), 2026-08-23. Applies to EV-003, EV-010, EV-087, EV-108
```text
L3188: --- THE §7.6 GATE — RESOLVED (different set), 2026-08-23 ---
L3189: **EV-003 READ IN FULL** (first time; 3-page minute order). The order's own
L3190: description: Exhibit F was purported correspondence "**between him and
L3191: counsel for Petitioner** from **8/10/21 to 7/25/23**," six emails signed
L3192: "**Lance**," one referencing assistant "Janine"; per Spiegel's declaration
L3193: the correspondence "did not in fact occur, and could not have occurred…
L3194: several years before counsel was retained." Findings quoted: submission
L3195: "intentional and… designed to mislead"; **§271 violation found; the
L3196: sanctions RFO DENIED; the $250,000 demand withdrawn 2/23/26; fee showing
L3197: "inadequate"; "The issue of 271 sanctions is reserved to the time of
L3198: trial."** Halsey's on-record response: "filing a narrative summary in a
L3199: document that resembles 'emails' **was a mistake**"; he sought to withdraw
L3200: the exhibit.
L3201: **RESOLUTION: the fabricated set was Halsey↔OPPOSING-COUNSEL correspondence;
L3202: every email the report cites is Halsey↔Shannon/family/CPA/staff — DIFFERENT
L3203: CORRESPONDENTS, DIFFERENT CORPUS, and per the order the Exhibit F items were
L3204: fictional compositions, not altered exports.** The §12 confrontation
L3205: (Halsey's direction, 2026-08-23) discloses the finding in the order's words,
L3206: states his explanation, states the different-set fact, then the affirmative
L3207: authentication (EV-087 dual export; to-the-second live matches; third-party
L3208: originals; bank/carrier corroboration). Residual named: pull the actual
L3209: Exhibit F pages from the 11/12/25 RFO (the Drive "Exhibit Tab F" files are
L3210: divider pages only). **DISAMBIGUATION RULE: the police package's own
L3211: "Exhibit F" (the 24.5MB 500-emails timeline) is a DIFFERENT DOCUMENT from
L3212: the court's Exhibit F — v1 renames its exhibit references to avoid the
L3213: collision.**
```

#### B2 — EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23. Applies to EV-003, EV-046, EV-106; bears on c, d, e, exF, statebar
```text
L3406: --- EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23 (his account; packet uses the tight version only) ---
L3407: Halsey's fuller statement (PK/U), recorded for retrievability; NOT imported
L3408: wholesale into the packet (governance bar on family-court-grievance material):
L3409: he is appealing the §271 ruling — and the entire underlying case — on the
L3410: ground that he was **not validly served, "14 out of 14 times,"** in the
L3411: proceedings that produced the orders; that the family court adopted a
L3412: non-conforming Mexico-mail-service method such that in "~7 motions" he never
L3413: saw the motions before they were heard; that he was "held to the US time
L3414: clock" though in Mexico; that he was then required to give up email-service
L3415: rights after the 5-page brief he demanded (EV-106) exposed the problem; and
L3416: that he did not receive Petitioner's initial financial disclosures, which the
L3417: court permitted. He states he contacted the California State Bar about
L3418: opposing counsel **before** the ruling issued.
L3419: **Corroboration in the register:** EV-106 ¶4 expressly preserves for
L3420: appellate review "the validity of all prior orders entered without
L3421: constitutionally adequate service and notice" (CRC 8.104; CCP 904.1;
L3422: §473(d)); EV-046 is the State Bar's 4/20/2026 submission receipt for a
L3423: complaint against Lance Spiegel (Bar No. 51625), **one day before** the
L3424: 4/21/2026 order, complaint no. 24-O-18793 (a 2024-origin number).
L3425: **What the packet uses (§8.5, §12(9)):** two sourced sentences only — the
L3426: finding was entered in a proceeding he contends he was not validly served in
L3427: and is appealing, and a Bar complaint against opposing counsel predated the
L3428: ruling. The service mechanics (Hague/CRC 5.92/CCP 1013/the judge's method)
L3429: stay OUT of the packet body — zero value to a detective, reads as
L3430: family-court grievance, which the 7/30 outline's own rule forbids. Recorded
L3431: here so the reasoning is retrievable, not re-derived.
```

#### B3 — CORRECTION BLOCK 2026-08-10, C-01..C-04. Applies to EV-045, EV-042, WP-020 [1/2] and index-wide
```text
L1124: ## CORRECTION BLOCK — 2026-08-10 · adoption, not authorship (append-only)
L1125: Governed by OPERATING_CONDITIONS §8, added this date on Halsey's instruction.
L1126: These entries' original text stands above unaltered (append-only discipline);
L1127: where it conflicts with this block, **THIS BLOCK CONTROLS.**
L1128: 
L1129: **C-01 · EV-045 (Exhibit C — Kale/Google) — TAG SUPERSEDED.**
L1130: - Original tag, now withdrawn: "**(I/X)** — an AI-generated SUMMARY of emails,
L1131:   not the emails… treat as a roadmap to the native messages only." The header
L1132:   line "(SUMMARY, not source)" is likewise withdrawn.
L1133: - **Corrected tag: (U) — Halsey's adopted, filed exhibit.** It was submitted to
L1134:   the court as **Exhibit C** to his declaration. He stands behind it. It is a
L1135:   source, and it is citable as his account of the preservation record.
L1136: - Grounds: the tag disqualified it for being AI-produced. That is not an
L1137:   evidentiary category (§8.1). What I actually had against it was that it is a
L1138:   SUMMARY — true of any summary, by anyone (§8.4).
L1139: - What genuinely remains, stated correctly: the native Kale emails are still
L1140:   worth obtaining, because an opponent will compare exhibit to underlying
L1141:   record and because they settle the count conflict below. That is a strength
L1142:   task, not a defect. **The 654-day figure is VERIFIED arithmetic** on the
L1143:   exhibit's own two dates (F-20) and needs no apology.
L1144: 
L1145: **C-02 · The four-vs-five conflict is NOT an AI problem — restated.**
L1146: EV-042 ¶9 (sworn) says "at least five separate occasions." Fact register #25
L1147: says four [Gmail 19c31c2994519631, "Fourth Formal Request"]. EV-045 says "at
L1148: least four times." The conflict is between **Halsey's own sworn filing and his
L1149: own register** — it exists whatever produced Exhibit C, and would exist if a
L1150: paralegal had typed it. Plead neither count until the native emails resolve
L1151: it. Nothing about this reflects on EV-045's status as a source.
L1152: 
L1153: **C-03 · WP-020 (violations infographic) — VERDICT WITHDRAWN, defects kept.**
L1154: - Withdrawn: my categorical "**NOT FILING-READY**" and "Used by: none until
L1155:   rebuilt." That was my call to make and it was not mine (§8.6).
L1156: - **Kept, because they are checkable and he would want them caught:** "Anna
L1157:   Kralle" surname is unverified (only AnnaK@ is (V)); the record shows
L1158:   "Matthew" Sirriyeh, not "Matt"; the 57/43 split states no denominator; the
L1159:   bar heights disagree with the chart's own axis; the firm shows ≥5 staff on
L1160:   its own mail. A wrong surname in a filed exhibit is the F-01 failure family
L1161:   — that is why these stay on the record.
L1162: - **Corrected status: (U) work product, Halsey-adopted. Usable at his
L1163:   direction.** Fix the surname and the denominator before it goes anywhere,
L1164:   and the rebuild from the POS signatory audit (CANON OPEN-6) makes it
L1165:   stronger — it is not a precondition to its existing as a source.
L1166: 
L1167: **C-04 · STANDING RULE for this index.** No future entry is tagged (X), "not a
L1168: source," or "roadmap only" on the ground that an AI, calculator, dashboard, or
L1169: assistant produced it. Where verification is incomplete, write exactly what is
L1170: unverified and against which record — never a status label that reads as
L1171: disqualification. (X) keeps its narrow meaning only: OPERATING_CONDITIONS §7.4.
```

#### B4 — CONVERSION BLOCK 2026-08-10, K-01..K-09 and standing rule. Index-wide
```text
L1302: ## CONVERSION BLOCK — 2026-08-10 · prohibitions become annotations (append-only)
L1303: Governed by OPERATING_CONDITIONS §10. Everywhere in this repo I wrote "do not
L1304: plead," "not pleadable," "fenced," "gated," or "does not go in this packet,"
L1305: **that was a submission ruling I had no standing to make.** Those words are
L1306: withdrawn wherever they appear. The items below are IN THE RECORD. Each carries
L1307: its tested status and the specific test still owed. **The decision to use any
L1308: of them is Halsey's.**
L1309: 
L1310: | # | Item | Status | Test that settles it | What I found |
L1311: |---|---|---|---|---|
L1312: | K-01 | **"654 days"** (EV-045 / F-20 / F-21) | Arithmetic VERIFIED (2024-03-29 → 2026-01-12 = 654 exactly). Input year UNTESTED. | Read the first preservation request's date header, with its year, from the native email. | Case's other "March 29" is the 3/29/2025 counsel letter; BHPD reporting ≈3/24/2025; a Sent subject search for preserve/preservation/legal hold returned 16 threads, none in 2024. **If the year is 2025 the figure is 289.** Both figures are in the record; neither is deleted. |
L1313: | K-02 | **"Sept & Oct 2022 locking me out"** (his 1/8/2026 email to BHPD, F-22) | The STATEMENT stands as his adopted, sent statement to law enforcement. The 2022 lockout is UNCORROBORATED. | Search 2022 for recovery notices in the backup account and any other address; check whether a 2022 episode exists that this mailbox would not show. | In THIS mailbox, 2022-07-01→2023-07-15 has no recovery notices; the notice sequence is 2023. A real, unexplained 2022-09-14 password change DOES exist (EV-051). |
L1314: | K-03 | **$1.3M → $500–600K drop** vs the **$1,134,000** spine | Both figures IN. Their relationship UNTESTED. | Pull the statements spanning the drop plus two prior months; reconcile line by line. | Not yet run. Different arithmetic, so they may be distinct events, overlapping, or the same — unknown, not excluded. |
L1315: | K-04 | **"She probably didn't do it the month before"** | Halsey's own stated read, IN as his read. | The same statements as K-03 — the prior two months answer it directly. | Not yet run. |
L1316: | K-05 | **The February account shutdown** | IN as his account. Year and account UNIDENTIFIED. | Halsey names the year and institution, or a statement/closure letter is pulled. | "After I survived" points to the Sept 17 2023 event, which would suggest Feb 2024 — my inference only, never his statement. |
L1317: | K-06 | **Preservation-request COUNT** | RESOLVED IN HIS FAVOUR. | Open the six threads in EV-054, confirm each is distinct. | The 1/10/2026 "Fourth Formal Request" is not the last (2/12/2026 follows). At least five written. The sworn "at least five" is CORRECT. |
L1318: | K-07 | **EV-053 Google Legal refusal** | IN. Header, sender, date, subject and the quoted line all verified. Body not yet opened. | One successful get_message on 19af06ba182f7aa6 (the call returned "service unavailable" 2026-08-10). | The quoted line is the operative one: "Google only takes steps to preserve data upon being properly served with valid legal process." |
L1319: | K-08 | **WP-020 infographic** | IN as his adopted work product (already converted at C-03). | Verify the "Anna Kralle" surname and the 57/43 denominator. | Only AnnaK@ is verified; record shows "Matthew" Sirriyeh. Two checkable fixes, not a verdict. |
L1320: | K-09 | **A recording of the Kale call** | Not an evidence item — an OPEN REQUEST. | The BHPD records demand (matters/04). | Nothing to withdraw here: asking for a record is the correct form, and "no recordings retained" is itself a finding. |
L1321: 
L1322: **STANDING RULE FOR THIS INDEX (replaces C-04's framing, keeps its substance):**
L1323: Every item enters. The Tag line records what has been TESTED and against what
L1324: — never whether the item is permitted. No entry is ever refused, removed, or
L1325: labelled unusable because of how it was produced or because a test is still
L1326: owed. Where I believe something is wrong, I say so once, in the Notes, with the
L1327: evidence — as a finding for Halsey to weigh, not a ruling.
```

#### B5 — THE KALE CHRONOLOGY (file 38_), items 1, 2 and 5. Applies to EV-042/EV-107 ¶9, EV-063, EV-067, EV-075 [1/2], EV-098
```text
L3293: --- THE KALE CHRONOLOGY (file 38_) — the count resolved, the interval computed, and the adverse offer — 2026-08-23 ---
L3294: Full sweep of from:/to:/cc:akale@beverlyhills.org, both directions, to
L3295: exhaustion (38_KALE_CHRONOLOGY.md; ~140 messages tabled; last Kale message
L3296: in the mailbox: 3/11/2026).
L3297: 
L3298: **1. THE FOUR-VS-FIVE CONFLICT IS RESOLVED — both numbers were true of
L3299: different things.** Emails to Kale reporting compromise/hacking/deletions:
L3300: **22 distinct messages** (each quoted with id in 38_ §2). Dated written
L3301: demands that Kale contact Google: **at least seven** (10/01, 10/06, 10/13,
L3302: 11/04/2025, 12/03/2025, 01/08, 01/10/2026). Halsey's own formal-request
L3303: NUMBERING ran #1–#4 (register #25's "four"); **distinct compromise events
L3304: reported: five** (the sworn "at least five" — EV-042 ¶9, EV-107 ¶9).
L3305: Packet language: report the 22 / the ≥7 / the 5 as what each is; plead no
L3306: bare count.
L3307: 
L3308: **2. A VERIFIED DURATION REPLACES THE SUSPECT ONES (F-20/F-21 family closed
L3309: for this use): 103 DAYS** — first dated written contact-Google demand
L3310: 10/01/2025 (`1999df6b5ce0fbce`) → Kale's first written statement that a
L3311: Google preservation request was submitted **01/12/2026** (`19bb38cf19aec75b`,
L3312: "for two accounts: Halsey2005@gmail.com and Shannonminor@gmail.com").
L3313: 161 days from the first written hack report (08/04/2025,
L3314: `198773659236b416`). Both endpoints are message ids; the IA complaint
L3315: (filed 1/10/2026, register #37) precedes Kale's stated preservation by two
L3316: days — consistent with the sworn "only after an internal affairs inquiry."
… [L3317–L3346 not reproduced here]
L3347: **5. KALE'S 1/5/2026 QUESTION FOUND** (`19b8fbc478f4e54b`): "are you
L3348: talking about these emails below?… I know you mentioned some emails from
L3349: November 11, 2022 were 'deleted'" — and Halsey's direct answer 1/8
L3350: (`19b9f646568c79a0`): "the critical tax-refund email was **surgically
L3351: removed from my account after I gave it to you**, not that it never
L3352: existed." The Wells Fargo thread is PRESENT live today (30_ §4) — the
L3353: recovered/restored question (D-P1) is now dated to a live dispute window.
```

#### B6 — STRUCTURAL FINDING 2026-08-12. a: the deletion reading; applies to EV-070/EV-071
```text
L2024: --- STRUCTURAL FINDING — 2026-08-12 (append-only) ---
L2025: **SHANNON'S 2023 EMAIL RECORD IS NEARLY EMPTY.** Full sweep
L2026: `in:anywhere from:shannonminor@gmail.com after:2023/02/07 before:2023/12/31`
L2027: returns **NINE threads across ten months** — the period covering the
L2028: alleged deception campaign, the 6/6/2023 suicide-plan email, the collision,
L2029: and the 9/12/2023 deleted-message burst. Also swept: his own Sent mail for
L2030: broke/no money/cash problems/penniless across 2023 → five threads, only the
L2031: 7/7 exchange on point. TWO READINGS, both recorded: (a) the money-fiction
L2032: communications were NOT email — they lived in text/iMessage/WhatsApp, which
L2033: is why the preserved phone (EV-038, demand R-9) and the iMessage export
L2034: PDFs carry this part of the case; (b) deletion. THE TEST THAT SEPARATES
L2035: THEM: the EV-070/071 pre-hacking control-set PDFs — any 2023 Shannon email
L2036: present there and absent from the live account is a documented deletion,
L2037: provable with no third party's cooperation. This also relocates the search
L2038: for V6 ¶24's fabricated BALANCE communications for the CLOSED x2218 — the
L2039: single highest-value untried target in the matter — to the text layer.
```

#### B7 — H-8 ASYMMETRY-TEST FINDING 2026-08-12. a: applies to EV-065
```text
L1865: --- H-8 ASYMMETRY-TEST FINDING (§9.5) — 2026-08-12 (append-only) ---
L1866: Sweep `in:anywhere to:shannonminor (mother OR Joyce OR owe OR owed OR
L1867: loan) 2022/11/01-2023/03/01` returned FOUR threads — NONE is a late-Nov
L1868: 2022 Shannon message about money owed her mother. EV-065's adopted claim:
L1869: "Thirty emails from late November 2022, in which Shannon Minor discussed
L1870: her claim that the stolen funds were owed to her mother Joyce Flaherty,
L1871: were surgically deleted." FINDING (stated per §9.5's asymmetry logic,
L1872: nothing smoothed): the described Shannon-side mother-money messages are
L1873: ABSENT from this mailbox in the swept window, while his side of
L1874: money-distress traffic survives (EV-073, EV-074). Absence is not proof of
L1875: deletion (Lesson 1) — the affirmative tests remain: (a) the EV-070/071
L1876: control-set PDFs (contents queued for Halsey's Mac — if the 30 emails
L1877: appear there, PDF-vs-live diff = the deletion exhibit); (b) the
L1878: metadata-forensics output EV-065 cites; (c) Google's return from Kale's
L1879: 1/12/2026 preservation request (EV-063 — demand D-item: what did Google
L1880: return). Shannon's surviving 1/25/2023 message (185ea400074e635b, Q: "you
L1881: owe me a huge apology…") shows her side is not uniformly absent — the
L1882: absence is TOPIC-SPECIFIC, which is the §9.5 pattern worth stating.
```

#### B8 — CORRECTION BLOCKS 2026-08-27 and 2026-08-27b (D-1 count; duplicate ids)
```text
L3433: ---
L3434: 
L3435: ## CORRECTION BLOCK — 2026-08-27 · the decisions gate + duplicate ids (append-only)
L3436: - Per governance/DECISIONS.md **D-1**: every "candidate sixth/seventh demand"
L3437:   phrasing in this index and its notes is **SUPERSEDED**. The asserted
L3438:   preservation-demand count is FIVE (his ruling; EV-054 criteria). Located
L3439:   demand-like documents beyond the five (EV-069; the EV-075 demand set;
L3440:   Gmail 199db7e78dd8b1de) remain library documents under D-6 and enter no
L3441:   count absent his express reclassification.
L3442: - **DUPLICATE-ID NOTICE:** "EV-075" and "EV-076" were each assigned to TWO
L3443:   different entries (the Apr–Sep 2025 demand/deletion-window sets AND the
L3444:   July-2023 exchange/message entries). Until the owning thread renumbers by
L3445:   append, citations to these four entries must use TITLE + MESSAGE ID, not
L3446:   the bare EV number. (Allocation lessons 2026-08-07 / 2026-08-12.)
L3447: 
L3448: ## CORRECTION BLOCK — 2026-08-27b · ELEVEN duplicate ids (audit A/C; supersedes the two-id notice above)
L3449: Independent audit measured 137 entry headers over 129 unique ids. The
L3450: following ids each name TWO DIFFERENT documents: **EV-035 · EV-036 · EV-037 ·
L3451: EV-038 · EV-042 · EV-075 · EV-076 · EV-079 · EV-081 · WP-019 · WP-020.**
L3452: Roughly 211 citations reference the previously unacknowledged ones, and
L3453: preserved PDFs on disk are named by the SECOND assignment — so a bare-id
L3454: citation can silently resolve to the wrong exhibit. RULES, effective now:
L3455: (1) cite these eleven by TITLE + message id / hash, never bare id; (2) the
L3456: owning threads renumber the second assignments BY APPEND (new id, old entry
L3457: cross-noted — nothing rewritten); (3) before any NEW id is assigned, grep the
L3458: full index for it (the max()+1 allocator caused this five separate times);
L3459: (4) any on-disk mirror named by a colliding id gets a README line in its
L3460: directory stating which assignment it is.
```

#### B9 — PASS 3 header (service filings, State Bar chain, Kale record)
```text
L1003: --- PASS 3 (2026-08-10) · service filings, State Bar chain, Kale record ---
L1004: Full detail, verbatim quotes and method:
L1005: runbooks/audit_notes/2026-08-10_service_declaration_statebar_and_kale.md
```

### 3c. Every line in the index that names Spiegel, "Lance", the firm, its staff, opposing/Petitioner's counsel or the State Bar (mechanical, verbatim)

Pattern (case-insensitive): spiegel | \blance\b | ysfamilylaw | kralle | sirriyeh | janine | opposing counsel | petitioner's counsel | counsel for petitioner | 51625 | 24-O-18793 | calbar | state bar | cal-bar | bar complaint. The bracket gives the nearest preceding entry header or block heading.

```text
L170 [EV-010]:   in EV-003 (that was six emails signed "Lance"). Never conflate them; verify
L555 [EV-039]:   Det. Kale email history, plus the leak/"Scalpel"/insider-knowledge/Spiegel-
L607 [EV-035 [2/2]]: - What: Petition (FL-100), Petitioner SHANNON MINOR by LANCE S. SPIEGEL (SBN
L608 [EV-035 [2/2]]:   51625), Young, Spiegel & Hosp LLP. READ AT SOURCE 2026-08-19.
L636 [EV-036 [2/2]]: - What: FL-141 by Young, Spiegel & Hosp for PETITIONER SHANNON MINOR. Boxes
L642 [EV-036 [2/2]]:   form. Declared under penalty of perjury by Anna Kralle, June 18, 2024.
L661 [EV-037 [2/2]]: - What: Shannon Minor's Schedule of Assets and Debts by Young, Spiegel & Hosp.
L706 [EV-037 [2/2]]:     (al@provinziano.com / service@provinziano.com), from mvs@ysfamilylaw.com,
L707 [EV-037 [2/2]]:     executed by MATTHEW SIRRIYEH. => the Feb 2025 SAD went to Halsey's THEN
L1003 [--- PASS 3 (2026-08-10) · service filings, State Bar chain, Kale record ---]: --- PASS 3 (2026-08-10) · service filings, State Bar chain, Kale record ---
L1031 [EV-042]:   initiated." ¶10 criminal referral re opposing counsel under DA review;
L1044 [EV-043]:   address Young, Spiegel & Hosp, LLP, 301 N. Canon Dr., Ste 300, Beverly
L1059 [EV-044]:   resident; sender listed = Lance Spiegel's firm; staff handed over a batch
L1080 [EV-046]: EV-046 · California State Bar — submission receipt, 2026-04-20 15:43:57Z
L1081 [EV-046]: - What: complaint@calbar.ca.gov → Halsey, "Successful submission of Attorney
L1082 [EV-046]:   Misconduct Complaint." Complaint against Lance Spiegel, Bar No. 51625.
L1084 [EV-046]: - Tag: (V) — INSTITUTIONAL: authenticated by the State Bar's own send, not by
L1092 [EV-047]:   piu@doj.ca.gov. Subject: "BHPD Case No. 2025-14983 — State Bar Complaint
L1093 [EV-047]:   Filed Today Against Opposing Counsel Lance Spiegel (Bar No. 51625)."
L1102 [EV-048]:   ambush over janine. I alerted them to the fraud that was coming and the da
L1111 [WP-020 [1/2]]: WP-020 · "Legal Compliance Violations by Petitioner's Counsel" infographic
L1115 [WP-020 [1/2]]:   "Anna Kralle" surname unverified (only AnnaK@ is (V)); "Matt" vs the
L1116 [WP-020 [1/2]]:   record's "Matthew" Sirriyeh; the 57/43 split states no denominator; bar
L1157 [## CORRECTION BLOCK — 2026-08-10 · adoption, not authorship (append-only)]:   Kralle" surname is unverified (only AnnaK@ is (V)); the record shows
L1158 [## CORRECTION BLOCK — 2026-08-10 · adoption, not authorship (append-only)]:   "Matthew" Sirriyeh, not "Matt"; the 57/43 split states no denominator; the
L1319 [## CONVERSION BLOCK — 2026-08-10 · prohibitions become annotations (append-only)]: | K-08 | **WP-020 infographic** | IN as his adopted work product (already converted at C-03). | Verify the "Anna Kralle" surname and the 57/43 denominator. | Only AnnaK@ is verified; record shows "Matthew" Sirriyeh. Two checkable fixes, not a verdict. |
L1610 [EV-066]:   · 4/6 JSID cyber-sabotage 19d643ff9dda21bd · 4/6 Spiegel-complaint
L1612 [EV-066]:   19d64940cdcfe614 · 4/17 formal demand = EV-065 · 4/20 State Bar notice =
L1615 [EV-066]:   staff cc: jcastano, Nodonnell, SSahab @da.lacounty.gov) · 5/6 Cal-Bar
L1782 [--- EV-065 BODY READ IN FULL — 2026-08-12 annotation (append-only) ---]:    PLAN): "Spiegel specifically demanded the November 11, 2022 email — the
L1797 [--- EV-065 BODY READ IN FULL — 2026-08-12 annotation (append-only) ---]:    thread-vs-message deletion. TEST: identify from Spiegel's motion +
L1952 [EV-076 [1/2]]:   198717bc1e84199f (8/3 "Lance Planted Malware...") · 1987c30b472820da.
L2581 [--- THE SECOND 111 MB FILE — RESOLVED 2026-08-12 ---]: `1K5akFNK4ptlGF5N1dZP1haphrg8gwFas` → "AA Jell Cell For Lance";
L3045 [WP-020 [2/2]]:   referral re Petitioner's counsel under DA review. 15 pages; Exhibits
L3121 [EV-102]:   page632 2.pdf", folder LANCE FINAL — page-stamped 632 of a larger
L3191 [--- THE §7.6 GATE — RESOLVED (different set), 2026-08-23 ---]: counsel for Petitioner** from **8/10/21 to 7/25/23**," six emails signed
L3192 [--- THE §7.6 GATE — RESOLVED (different set), 2026-08-23 ---]: "**Lance**," one referencing assistant "Janine"; per Spiegel's declaration
L3201 [--- THE §7.6 GATE — RESOLVED (different set), 2026-08-23 ---]: **RESOLUTION: the fabricated set was Halsey↔OPPOSING-COUNSEL correspondence;
L3281 [EV-107]:   Petitioner's counsel "currently under review by the District Attorney's
L3369 [EV-108]: - What: "Lance's Motion for 271 Sanctions 3-2-2026.pdf", Drive
L3371 [EV-108]:   12/30/2025, $250,000 demand), Spiegel's MPA + declaration, Exhibit 1
L3375 [EV-108]:   purported Halsey↔"Lance" emails 8/10/2021–7/25/2023 about obtaining his
L3377 [EV-108]:   obligation), referencing a "client portal" and "my assistant Janine,"
L3379 [EV-108]:   "Lance [Last Name]", "[link]"). Spiegel's declaration: not retained
L3380 [EV-108]:   until early 2024; never had an assistant named Janine; does not send
L3390 [EV-108]: - **CONSEQUENCE 2 — THE PLANNED "LANCE-MOTION OVERLAP TABLE" HAD A FALSE
L3391 [EV-108]:   PREMISE AND IS REPLACED.** This motion challenges the Spiegel log only —
L3417 [--- EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23 (his account; packet uses]: court permitted. He states he contacted the California State Bar about
L3418 [--- EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23 (his account; packet uses]: opposing counsel **before** the ruling issued.
L3422 [--- EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23 (his account; packet uses]: §473(d)); EV-046 is the State Bar's 4/20/2026 submission receipt for a
L3423 [--- EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23 (his account; packet uses]: complaint against Lance Spiegel (Bar No. 51625), **one day before** the
L3424 [--- EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23 (his account; packet uses]: 4/21/2026 order, complaint no. 24-O-18793 (a 2024-origin number).
L3427 [--- EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23 (his account; packet uses]: and is appealing, and a Bar complaint against opposing counsel predated the
```
(53 lines.) Two lines mention "Lance" only as part of a Drive folder name: L2581 ("AA Jell Cell For Lance", the folder holding the EV-081 copy 1K5akFNK4ptlGF5N1dZP1haphrg8gwFas) and L3121 (folder "LANCE FINAL", holding EV-102). The index says nothing more about either folder.

## 4. Every statement in the index about what the court found, ordered or ruled (verbatim)

Attribution matters. Lines from the minute-order entries (EV-001..EV-005) and from the §7.6 GATE (which records EV-003 "READ IN FULL") are the index's descriptions of the orders. Lines in EV-041/EV-106/EV-048/the POSTURE block are a party's characterizations, labelled as such.

- EV-001 (4/21/2026 minute order):
```text
L73: EV-001 · Minute order 4/21/2026 — quash/protective order/sanctions DENIED
L74: - What: 9-page LASC minute order, Halsey's 1/5/2026 motion; the appeal target.
L75: - Original: Drive 1OzBjvKxbhjDXHDq5WlQf9-nFCJnj1dwk · 176,163 B · 2026-06-12.
L76:   Title: "MINUTE ORDER 4-21-2026 — Quash & Protective Order DENIED (APPEAL TARGET).pdf".
L77: - Hash: not computed — Drive id + byte size recorded.
L78: - Tag: (V/Q) — holdings quoted with locators in CANON §3.2(1).
L79: - Used by: FAMILY + POLICE (carries the Marsy's Law/Finkelstein holding the
L80:   criminal activity must argue around — matters/04).
```
- EV-002 (4/21/2026 minute order):
```text
L83: EV-002 · Minute order 4/21/2026 — defective-service objection DENIED
L84: - What: 1-page order; also imposes the standing trackable-mail + electronic
L85:   backstop service order ("the thing he won while losing").
… [L86–L89 not reproduced here]
L90: - Notes: 2026-08-07 registered. Every Petitioner POS after 4/21/2026 is
L91:   auditable against this order (CANON OPEN-6).
```
- EV-003 (4/21/2026 minute order), as registered 2026-08-07:
```text
L93: EV-003 · Minute order 4/21/2026 — Petitioner's §271 sanctions motion
L94: - What: 3-page order; §271 violation found, amount RESERVED TO TRIAL — no
L95:   dollar amount ordered (KNOWN_FALSE F-06); contains the Exhibit F
L96:   fabrication finding.
… [L97–L98 not reproduced here]
L99: - Tag: (V/Q) — CANON §3.2(3).
L100: - Used by: FAMILY. Notes flag: every activity must KNOW this order exists
L101:   (credibility exposure) without arguing it — see EV-010 title-collision note.
```
- EV-004 (4/21/2026 minute order):
```text
L104: EV-004 · Minute order 4/21/2026 — Petitioner's 2/2/2026 RFO DENIED
L105: - What: 1-page order.
```
- EV-005 (3/2/2026 minute order):
```text
L112: EV-005 · Minute order 3/2/2026 — the control case
L113: - What: quash motion dismissed; Halsey PRESENT via LACourtConnect, testified;
L114:   reporter Adrian Sosa #15020. Defeats "his equipment is unreliable."
```
- EV-010 note on the court's Exhibit F finding:
```text
L168: - Notes: 2026-08-07 registered. **WARNING — title collision:** the fourth
L169:   copy's "Exhibit F" title is NOT the "Exhibit F" the court found fabricated
L170:   in EV-003 (that was six emails signed "Lance"). Never conflate them; verify
L171:   exhibit history at source before using the "Exhibit F" title anywhere.
```
- EV-018 cross-reference to the quash fight:
```text
L240: - Hash: not computed. Tag: (X) contents; this is the notice whose service/
L241:   timeliness the quash fight concerned — cross-ref EV-001 (the 4/21/2026
L242:   order, F-01/F-02 corrections).
```
- EV-041: brief "answering the Court's 3/2/2026 Minute Order" (the positions listed after it are the brief's, not the court's):
```text
L1007: EV-041 · Respondent's Brief re service — filed/dated 2026-03-27
L1008: - What: 5-page brief answering the Court's 3/2/2026 Minute Order on service.
```
- EV-048: Halsey's contemporaneous characterization of the ruling (his words, not a court statement):
```text
L1103:   as well… You made my case 1 day after they received the warning." Same
L1104:   thread: "You realize what the judges ruling means. Mail to Mexico is not
L1105:   sufficient."
… [L1106–L1107 not reproduced here]
L1108: - Notes: 2026-08-10. Establishes contemporaneous characterization, NOT the
L1109:   authenticity of Exhibit F. Forecloses "objection manufactured after loss."
```
- C-01: Exhibit C was submitted to the court:
```text
L1133: - **Corrected tag: (U) — Halsey's adopted, filed exhibit.** It was submitted to
L1134:   the court as **Exhibit C** to his declaration. He stands behind it. It is a
L1135:   source, and it is citable as his account of the preservation record.
```
- DEFECT BLOCK reference to the Exhibit-F finding:
```text
L2152: material misstatement, traceable to a document Halsey submitted. That is the
L2153: F-01/F-02 failure family and it is exactly what would destroy the packet's
L2154: credibility with a new chief — the same structural risk as the §7.6
L2155: Exhibit-F finding.
```
- WP-019 [2/2] notes: EV-002 "is the RULING on this posture":
```text
L3025: - Notes: 2026-08-20 registered. EV-002 (4/21/2026 order) is the RULING on
L3026:   this posture: objection DENIED (no appearance by Respondent; court found
L3027:   notice given), BUT the prospective protocol ordered — "trackable method
L3028:   via the mail, and any proof of service shall include tracking details.
L3029:   As a backstop, all service shall also be effectuated by electronic
L3030:   means" — substantially ADOPTS the brief's own proposed protocol.
L3031:   EV-002 read at source 2026-08-20 (Q). Note: the order makes electronic
L3032:   service a mandatory BACKSTOP (supplement), not the sole formal method —
L3033:   the brief's red line. Whether it validly compels e-service on a
L3034:   non-consenting pro se is the preserved appellate question.
```
- §7.6 GATE: EV-003 read in full 2026-08-23 (order's description, findings quoted, Halsey's on-record response, the index's resolution):
```text
L3188: --- THE §7.6 GATE — RESOLVED (different set), 2026-08-23 ---
L3189: **EV-003 READ IN FULL** (first time; 3-page minute order). The order's own
L3190: description: Exhibit F was purported correspondence "**between him and
L3191: counsel for Petitioner** from **8/10/21 to 7/25/23**," six emails signed
L3192: "**Lance**," one referencing assistant "Janine"; per Spiegel's declaration
L3193: the correspondence "did not in fact occur, and could not have occurred…
L3194: several years before counsel was retained." Findings quoted: submission
L3195: "intentional and… designed to mislead"; **§271 violation found; the
L3196: sanctions RFO DENIED; the $250,000 demand withdrawn 2/23/26; fee showing
L3197: "inadequate"; "The issue of 271 sanctions is reserved to the time of
L3198: trial."** Halsey's on-record response: "filing a narrative summary in a
L3199: document that resembles 'emails' **was a mistake**"; he sought to withdraw
L3200: the exhibit.
L3201: **RESOLUTION: the fabricated set was Halsey↔OPPOSING-COUNSEL correspondence;
L3202: every email the report cites is Halsey↔Shannon/family/CPA/staff — DIFFERENT
L3203: CORRESPONDENTS, DIFFERENT CORPUS, and per the order the Exhibit F items were
L3204: fictional compositions, not altered exports.** The §12 confrontation
L3205: (Halsey's direction, 2026-08-23) discloses the finding in the order's words,
L3206: states his explanation, states the different-set fact, then the affirmative
L3207: authentication (EV-087 dual export; to-the-second live matches; third-party
L3208: originals; bank/carrier corroboration). Residual named: pull the actual
L3209: Exhibit F pages from the 11/12/25 RFO (the Drive "Exhibit Tab F" files are
L3210: divider pages only). **DISAMBIGUATION RULE: the police package's own
L3211: "Exhibit F" (the 24.5MB 500-emails timeline) is a DIFFERENT DOCUMENT from
L3212: the court's Exhibit F — v1 renames its exhibit references to avoid the
L3213: collision.**
```
- EV-106: the brief's characterization of the 3/2/2026 order, and how the finding is to be used:
```text
L3255: - Holds: the court's own 3/2/2026 order "already recognized that the
L3256:   sanctions RFO could not proceed because the timing required for service
L3257:   to Mexico had not been satisfied"; the 2/24/2026 bundled-delivery
… [L3258–L3261 not reproduced here]
L3262: - USE: one posture sentence in §12's §271 confrontation — the finding is
L3263:   disclosed AND its pendency inside a preserved service challenge with an
L3264:   appeal in process (U as to filing status) is stated, sourced here. The
L3265:   family-court-grievance exclusion otherwise holds.
```
- EV-107 separation rule:
```text
L3287: - **SEPARATION RULE (binding for v1):** ¶8's planted-documents claim and
L3288:   the court's Exhibit-F finding are DIFFERENT FACTS — his on-record
L3289:   "narrative summary… was a mistake" explanation (EV-003) and this sworn ¶8
L3290:   are both stated, never merged, never offered as answering each other.
```
- EV-108: the motion, and its consistency with the court's finding:
```text
L3368: EV-108 · THE §271 SANCTIONS MOTION ITSELF (12/30/2025) — read in full, and it re-frames two things
L3369: - What: "Lance's Motion for 271 Sanctions 3-2-2026.pdf", Drive
L3370:   `1r_5T4D4v4lwSbCWU1ZpO--6S9y4nRunT` (2,401,413 B): the FL-300 (filed
L3371:   12/30/2025, $250,000 demand), Spiegel's MPA + declaration, Exhibit 1
L3372:   (Halsey's own 10/31/2025 declaration) and Exhibit 2 (the challenged
L3373:   email log itself). **READ IN FULL 2026-08-23.**
… [L3374–L3379 not reproduced here]
L3380:   until early 2024; never had an assistant named Janine; does not send
L3381:   links. **The document reads as an AI-generated narrative reconstruction
L3382:   with the wrong correspondent name attached — fully consistent BOTH with
L3383:   the court's fabrication finding AND with Halsey's on-record "narrative
L3384:   summary… was a mistake" explanation. v1 states both, adopts neither.**
```
- EV-003 §271 ORDER — POSTURE (Halsey's account, and the index's two-sentence use):
```text
L3406: --- EV-003 §271 ORDER — POSTURE, per Halsey 2026-08-23 (his account; packet uses the tight version only) ---
L3407: Halsey's fuller statement (PK/U), recorded for retrievability; NOT imported
L3408: wholesale into the packet (governance bar on family-court-grievance material):
L3409: he is appealing the §271 ruling — and the entire underlying case — on the
L3410: ground that he was **not validly served, "14 out of 14 times,"** in the
L3411: proceedings that produced the orders; that the family court adopted a
L3412: non-conforming Mexico-mail-service method such that in "~7 motions" he never
L3413: saw the motions before they were heard; that he was "held to the US time
L3414: clock" though in Mexico; that he was then required to give up email-service
L3415: rights after the 5-page brief he demanded (EV-106) exposed the problem; and
L3416: that he did not receive Petitioner's initial financial disclosures, which the
L3417: court permitted. He states he contacted the California State Bar about
L3418: opposing counsel **before** the ruling issued.
L3419: **Corroboration in the register:** EV-106 ¶4 expressly preserves for
L3420: appellate review "the validity of all prior orders entered without
L3421: constitutionally adequate service and notice" (CRC 8.104; CCP 904.1;
L3422: §473(d)); EV-046 is the State Bar's 4/20/2026 submission receipt for a
L3423: complaint against Lance Spiegel (Bar No. 51625), **one day before** the
L3424: 4/21/2026 order, complaint no. 24-O-18793 (a 2024-origin number).
L3425: **What the packet uses (§8.5, §12(9)):** two sourced sentences only — the
L3426: finding was entered in a proceeding he contends he was not validly served in
L3427: and is appealing, and a Bar complaint against opposing counsel predated the
L3428: ruling. The service mechanics (Hague/CRC 5.92/CCP 1013/the judge's method)
L3429: stay OUT of the packet body — zero value to a detective, reads as
L3430: family-court grievance, which the 7/30 outline's own rule forbids. Recorded
L3431: here so the reasoning is retrievable, not re-derived.
```
- Other court-record statements (not findings): FL-100 file stamp and assignment (EV-035 [2/2]):
```text
L609: - Key contents (Q, transcribed exactly): file stamp "Electronically FILED by
L610:   Superior Court of California, County of Los Angeles 1/16/2024 9:23 AM David
L611:   W. Slayton, Executive Officer/Clerk of Court, By J. Esplana, Deputy Clerk
L612:   24STFL00432"; "Assigned for all purposes to: Ryan D. White, (Department,
L613:   ST23)"; signed by Shannon Minor 1/11/2024 under penalty of perjury. Date of
```
- Other court-record statements (not findings): LASC register for civil case 26STCV25125 (EV-038 [2/2]):
```text
L744:   * **Filing Date: 8/7/2026**  ← the file-stamp date; relates back to the
L745:     One Legal submission (EV-034), exactly as that receipt predicted.
L746:   * Case Type: "Contractual Fraud (General Jurisdiction)"
L747:   * Status: "Pending"
L748: - JUDGE / DEPARTMENT (Q, Register of Actions, 8/11/2026): "Case assigned to
L749:   Hon. Maureen Duffy-Lewis in Department 412 Stanley Mosk Courthouse",
L750:   111 North Hill Street, Los Angeles, CA 90012.
L751: - FUTURE HEARINGS (Q) — both **11/30/2026 at 08:30, Department 412**:
L752:   * "Case Management Conference"
L753:   * "Order to Show Cause Re: Failure to File Proof of Service"
… [L754–L757 not reproduced here]
L758: - DOCUMENTS FILED (Q): 8/7/2026 Complaint (by Halsey Minor, Plaintiff);
L759:   8/7/2026 Notice of Case Assignment — Unlimited Civil Case (Clerk);
L760:   8/7/2026 Alternative Dispute Resolution Packet (Clerk); 8/11/2026 Summons
L761:   on Complaint (Plaintiff); 8/11/2026 Civil Case Cover Sheet (Plaintiff);
L762:   8/13/2026 Notice of Case Management Conference (Clerk, x2); 8/13/2026
L763:   Order to Show Cause Failure to File Proof of Service (Clerk, x2).
L764: - **NO PROOF OF SERVICE APPEARS ON THE DOCKET (V)** — as of the 8/18 print,
L765:   no defendant has been served of record.
```

## 5. Everything the index itself marks as unverified, AI-derived, withdrawn, duplicate or "never cite" (verbatim)

### 5a. Per entry (mechanical scan of every entry block)

An entry block runs from its header to the line before the next header or block delimiter (`---`, `## `, `=== `). A line is listed if it carries an authentication tag containing X, U, I, L, D or PK (e.g. "(X)", "(U/Q)", "(I/X)", "(PK)"; "(V)", "(Q)", "(V/Q)", "(R)" do not qualify), or a marker word (unverified/unread/not read/owed/AI/Gemini/withdrawn/superseded/duplicate/byte-identical/same document/never/unsourced/UNDETERMINED/untested/not hash/derived/mislabel/FALSE/WRONG/DEFECT/CONTRADICTED/discard/roadmap/unresolved/hypothesis/corrected/inferred/DO NOT/must not, and similar). Marked lines that sit in non-entry blocks are in §5b.

#### EV-006 (block L121–L129)
```text
L122: - What: PDF concerning the investigation's conduct (contents unread this
L126: - Tag: (X) — existence verified; contents not read at source this session.
```
#### EV-007 (block L130–L137)
```text
L134: - Tag: (X) — contents not read at source this session.
```
#### EV-008 (block L138–L145)
```text
L142: - Tag: (X) — contents not read at source this session.
```
#### EV-009 (block L146–L153)
```text
L150: - Tag: (X) — contents not read at source this session.
```
#### EV-010 (block L154–L172)
```text
L159: - Copies, identical byte size 24,470,497 (I — same document inferred from
L166: - Tag: (X) as to contents this session; sent-to-police status (U/V — CANON §7).
```
#### EV-011 (block L173–L181)
```text
L177: - Tag: (X) — contents not read at source this session.
L180:   civic officials (X — not asserted; confirm with Halsey).
```
#### EV-012 (block L182–L189)
```text
L186: - Tag: (X) — contents not read at source this session.
```
#### EV-013 (block L190–L206)
```text
L199: - Tag: (U) as document; handling instruction (Q) from the sending email:
L203: - Notes: 2026-08-07 registered. **SEALED — never quote or attach publicly;
```
#### EV-014 (block L207–L215)
```text
L212: - Tag: (X) — contents not read at source this session; title as filed.
```
#### EV-015 (block L216–L222)
```text
L219: - Hash: not computed. Tag: (X). Used by: CIVIL + POLICE + 1983.
```
#### EV-016 (block L223–L230)
```text
L226: - Hash: not computed. Tag: (X) contents; Bates numbering per title.
```
#### EV-017 (block L231–L236)
```text
L234: - Hash: not computed. Tag: (X). Used by: CIVIL + POLICE + 1983.
```
#### EV-018 (block L237–L245)
```text
L240: - Hash: not computed. Tag: (X) contents; this is the notice whose service/
```
#### EV-019 (block L246–L250)
```text
L248: - Hash: not computed. Tag: (X). Used by: FAMILY + CIVIL.
```
#### EV-020 (block L251–L264)
```text
L256: - Copies, identical byte size 4,069,611 (I — same document by exact size):
L260: - Hash: not computed. Tag: (X) contents; court-record filing per title.
L263:   fight in filed form — read at source before citing (X).
```
#### EV-021 (block L265–L278)
```text
L269:   count recorded, ids not duplicated here).
L276: - Hash: not computed. Tag: (X). Used by: CIVIL + POLICE + 1983.
```
#### EV-022 (block L279–L288)
```text
L286: - Hash: not computed. Tag: (X). Used by: CIVIL.
```
#### EV-023 (block L289–L296)
```text
L293: - Hash: not computed. Tag: (X). Used by: CIVIL + POLICE + 1983.
```
#### EV-024 (block L297–L301)
```text
L299: - Hash: not computed. Tag: (X). Used by: CIVIL + POLICE.
```
#### EV-025 (block L302–L365)
```text
L338: - **0115 HOLDER — still not established (V, important):** the document
L350:   received the $1,134,000. Document prints "VGI" only; it never spells out
L351:   an institution name (Vanguard Group Inc. is (I), not printed).
```
#### EV-026 (block L366–L370)
```text
L368: - Hash: not computed. Tag: (X). Used by: CIVIL + POLICE.
```
#### EV-027 (block L371–L375)
```text
L373: - Hash: not computed. Tag: (X). Used by: CIVIL + POLICE.
```
#### EV-028 (block L376–L387)
```text
L383: - Hash: not computed. Tag: (X) contents; (U) purpose per title (prepared
L386:   sent to civic officials (X — confirm with Halsey; also see EV-011).
```
#### EV-029 (block L388–L399)
```text
L390:   document copied into each account's year tree (I — inferred from
L391:   byte-identical size across all four accounts).
L396: - Hash: not computed — ids + byte size recorded. Tag: (X) contents unread.
```
#### EV-030 (block L400–L405)
```text
L404: - Tag: (X). Used by: CIVIL + POLICE + 1983. Notes: 2026-08-07 (pass 2b).
```
#### EV-031 (block L406–L412)
```text
L411: - Tag: (X). Used by: CIVIL + POLICE + 1983. Notes: 2026-08-07 (pass 2b).
```
#### EV-032 (block L413–L418)
```text
L417: - Tag: (X). Used by: CIVIL + POLICE + 1983. Notes: 2026-08-07 (pass 2b).
```
#### EV-033 (block L419–L430)
```text
L424:   4,299,446 B) is an identical-size loose copy of THIS document (I) — the
L427:   [2026-08-19: UPGRADED (I)->(V) — sha256-identical, verified in the
L428:   preservation run; see preserved_2026-08-19/MANIFEST.md. Same document.]
L429: - Tag: (X). Used by: CIVIL + POLICE + 1983. Notes: 2026-08-07 (pass 2b).
```
#### EV-034 (block L431–L458)
```text
L444: - Tag: (V/Q) as to the forwarded receipt read at source 2026-08-08; (X) as to
L448: - Notes: 2026-08-08 registered. Kills the prior (U) belief that V6 was filed
```
#### EV-035 [1/2] (block L459–L481)
```text
L464:   excerpt of a 297-page compilation (parent compilation not yet identified).
L471:   text per API snippets (I).
L477:   headers: not yet located (L).
```
#### EV-036 [1/2] (block L482–L505)
```text
L485:   BHPD 3/29/2025 (= EV-009 content (I), byte-compare pending); pp.16–24 WF
L496: - Tag: (V) as read this session; (D) COMPLETENESS — master prompt describes
L503:   five-transfer statement lines outside the unread EV-016/017 production.
```
#### EV-037 [1/2] (block L506–L528)
```text
L515:   BeverlyHillsCA@request.justfoia.com → halsey2005@gmail.com (duplicate send
L518:   (2026-07-24, "…I think it was 12 all ignored" — his estimate, (U) as to
L520:   cityclerk/akale/mstainbrook/lwiener — located, not read in full).
L526:   address (X)" → 464 N. Rexford Drive, Beverly Hills, CA 90210 per BHPD's own
```
#### EV-038 [1/2] (block L529–L551)
```text
L543: - Tag: (V) as to on-screen content; (PK) as to phone provenance/preservation
```
#### EV-039 (block L552–L581)
```text
L553: (2024–2026)" — Halsey↔Kale reconstruction + Triangle-of-Corruption hypothesis
L554: - What: 11-page work-product/AI-assisted reconstruction of the ~2-year Halsey–
L561:   Evidence Spoliation" — L, unverified).
L562: - Tag: (I/X) — AI-derived reconstruction; its email date-stamps are Halsey's
L573:   is a Halsey-ADOPTED document and therefore a SOURCE — at minimum (U), his
L574:   account (§8.1); the (I/X) tag above states verification level only, never
L577:   ruling — what enters any packet is Halsey's call. Tests owed: date-stamps
L580:   email in the mailbox; year untested against a native.
```
#### EV-040 (block L582–L605)
```text
L591: - Tag: (I/X) — derived infographic; metrics unverified at source.
L594:   NEVER email). Corruption metrics do NOT enter the police report (firewall).
L597:   Halsey-adopted → a SOURCE, at minimum (U) (§8.1). "Do NOT enter the police
L598:   report" above is withdrawn as my phrasing; the operative rule is ADDENDUM
L601:   Halsey's. Tests owed: the day-count metrics' input years (K-01: 654 vs 289
L602:   — arithmetic verified, first-request year untested); the response-rate and
```
#### EV-035 [2/2] (block L606–L633)
```text
L621:   whether this copy is an amended petition is (X), unresolved.
L623:   "24.01.16, P's FL-100, Minor, Halsey.pdf". Duplicate id
```
#### EV-036 [2/2] (block L634–L658)
```text
L644:   "24.06.18, P's FL-141, Minor, Halsey.pdf". Duplicate id
L648: - Notes: 2026-08-19 registered. COMPUTATION (I, from EV-035 + EV-036): petition
L653:   RULE is (X) while the two DATES are (V). Halsey confirms (U) he consented
L655:   The FL-142 itself is never filed with the court (the form so states); it
```
#### EV-037 [2/2] (block L659–L727)
```text
L670:   * p.8 and p.17 (duplicate filing of the same WF statement, period 1/1/2025-
L695:     insure is NOT stated on the form — (X). **
L716:   * The prior pass's "0115" hits on pp.69/71 were FALSE POSITIVES — substring
L718:     American Express statement. Corrected here.
L719: - CROSS-FORM DISCREPANCY (I, computed): her FL-150 signed 1/7/2025 lists five
L724:   FL-142. Both are sworn. May be innocent renaming/paydown — DO NOT plead as
```
#### WP-001 (block L779–L795)
```text
L781:   email (Q); "intentionally unverified" pleading, one signature line after
L790: - Tag: (U/Q) as to the sends; AS-FILED VERSION (X) — two same-named
```
#### WP-002 (block L796–L801)
```text
L798:   2026-07-09. Tag (U). Used by: 1983.
```
#### WP-003 (block L802–L806)
```text
L804:   2026-06-10. Tag (U). Used by: 1983.
```
#### WP-004 (block L807–L812)
```text
L809:   2026-07-09. Tag (U — its internal citations claim sourcing; not re-verified
```
#### WP-005 (block L813–L817)
```text
L815:   2026-07-10. Tag (U). Used by: 1983.
```
#### WP-006 (block L818–L824)
```text
L822:   2026-07-30. Tag (U). Used by: POLICE.
```
#### WP-007 (block L825–L832)
```text
L825: WP-007 · "Google-Gemini — Deletion 100pct Match + Hacking (AI analysis)"
L826: - What: AI-generated analysis of deletion/spoliation and hacking indicators.
L828:   2026-06-12 (Google-spoliation folder). Tag (I/X — AI-derived; its
```
#### WP-008 (block L833–L837)
```text
L835:   Tag (U — derived compilation). Used by: FAMILY + CIVIL.
```
#### WP-009 (block L838–L842)
```text
L840:   Tag (U — derived graphic). Used by: CIVIL + POLICE.
```
#### WP-010 (block L843–L850)
```text
L848:   1_T2eOacZZNGi9qLfpVRn1zS0AJO8wj-x · 29,279 B. Tag (U). Used by: CIVIL.
```
#### WP-011 (block L851–L858)
```text
L856:   Tag (U). Used by: FAMILY + CIVIL.
```
#### WP-012 (block L859–L868)
```text
L865:   1–4 KB each, multiple copies). Tag (U). Used by: FAMILY + CIVIL.
```
#### WP-013 (block L869–L877)
```text
L874:   w1_6vIuKc · 35,674 B (copy 1eVzUSmidiAabnO4raxu-yjGekfubrgiy). Tag (U).
```
#### WP-014 (block L878–L883)
```text
L880:   1z3-T6RZE0ZNNUOsV8tiq6R9ElWUrriwd). Tag (U). Used by: CIVIL.
```
#### WP-015 (block L884–L889)
```text
L886:   2026-07-26. Tag (U — its verification claims are its author-session's,
```
#### WP-016 (block L890–L896)
```text
L893:   2026-07-26. Tag (U). Used by: CIVIL + POLICE + 1983.
```
#### WP-017 (block L897–L905)
```text
L897: WP-017 · "CORRECTION — Vanguard 529 recipient = Raymond Nutt / Rochester
L900:   Tag (U — "verified from statement" is the author-session's claim; the
```
#### WP-018 (block L906–L914)
```text
L909:   across ≥5 folders (ids in the 2026-08-07 sweep transcript). Tag (U).
```
#### WP-019 [1/2] (block L915–L944)
```text
L917:   whole case (VERIFIED / NEEDS-DOCUMENT / UNVERIFIED per item). Source keys:
L922: - Tag: (U as work product; but it is the fact-DISCIPLINE authority — its
L935:   KEY CORRECTIONS it forces: (#12) 2015 event = UPHOLD stock, NOT Vanguard
L936:   [Gmail 19df494cfbefd6b4; PKG 2245] — EV-015 title is a 2015 mislabel; (#15)
L938:   (Kale email) + 3/29/2025 counsel letter — EV-039's "3/29/2024" unverified;
L940:   unsourced. **CROSS-MATTER FLAG for the CIVIL + 1983 threads:** the register
L941:   supersedes several figures those activities may still carry (esp. the
```
#### EV-042 (block L1022–L1041)
```text
L1024:   ¶3 no EFS-005-CV / never authorized email service. ¶4 the 2026-02-24
L1027:   inserted into my files that I had never authored… created using my accounts
L1034: - Original: uploads c44bdef5-…_2.pdf and 6accfb51-….pdf — BYTE-IDENTICAL,
```
#### EV-045 (block L1066–L1079)
```text
L1066: EV-045 · Exhibit C — Kale / Google preservation record (SUMMARY, not source)
L1067: - What: Gmail "AI Overview" panel over a search of mail to
L1072: - Tag: **(I/X) — an AI-generated SUMMARY of emails, not the emails.** Sources
L1073:   outrank summaries; treat as a roadmap to the native messages only.
L1077:   ENDPOINTS NATIVELY and the figure becomes usable. This CORRECTS the earlier
L1078:   matters/03 instruction to discard 654 as unsourced.
```
#### EV-047 (block L1089–L1098)
```text
L1097:   letter is referenced but NOT yet located — open item.
```
#### WP-020 [1/2] (block L1111–L1121)
```text
L1114: - Tag: (U/X) work product. **NOT FILING-READY — defects recorded 2026-08-10:**
L1115:   "Anna Kralle" surname unverified (only AnnaK@ is (V)); "Matt" vs the
L1119: - Used by: none until rebuilt. Notes: rebuild from the POS signatory audit
```
#### EV-049 (block L1173–L1190)
```text
L1187:   logs in" — is (U) and is NOT in these notices; do not attribute it to
```
#### EV-051 (block L1207–L1218)
```text
L1212: - Tag: (V) as to the event. **(X) as to who did it and why — unexplained.**
```
#### EV-053 (block L1232–L1254)
```text
L1239: - Tag: **(V) as to sender/date/subject and the quoted snippet. BODY UNREAD —
```
#### EV-054 (block L1255–L1274)
```text
L1264: - Tag: (V) by header. **Bodies not yet opened — open all six before the count
```
#### EV-055 (block L1275–L1299)
```text
L1277:   Snippet (Q): "Whatever the AI is telling you, I can tell you conclusively
L1285:   that a phone call was never going to be enough.
```
#### EV-056 (block L1329–L1353)
```text
L1333:   the "Triangle of Corruption" HYPOTHESIS (police files leaked to opposing
L1335:   it. AI-assisted (Gemini), adopted and supplied by Halsey 2026-08-11.
L1340: - Tag: (U) — Halsey-adopted work product (§8). Opening sections read
```
#### EV-058 (block L1373–L1397)
```text
L1388:   reason for contacting this office" — body-open owed).
```
#### EV-059 (block L1398–L1418)
```text
L1406:   embeds a records-system screenshot (image001.png, NOT yet extracted; may
L1413:   statements (3/24 vs 3/25/2025) — state, never smooth. Halsey's 10/8/25
```
#### EV-060 (block L1419–L1431)
```text
L1428: - Tag: (V) header/snippet; body-open owed before any quote beyond snippet.
```
#### EV-061 (block L1432–L1442)
```text
L1438: - Tag: (V) header/snippet; body-open owed (Hunt #3: the chain-of-custody
```
#### EV-062 (block L1443–L1462)
```text
L1454: - Tag: (V) headers/snippets; bodies-open owed.
L1458:   `status-claim`, `refusal-context`. Also located, register-cited but not yet
```
#### EV-063 (block L1493–L1522)
```text
L1507:   567-page-document page showing the Nov 2022 emails — extraction owed).
```
#### EV-064 (block L1523–L1567)
```text
L1530: - Contemporaneous account (U — his written account, adopted and sent to law
L1546:     on-screen deletions (12 vs 15: state both, never smooth; the screenshot
L1559: - Tag: (U/Q) — his adopted contemporaneous written account, read in full at
```
#### EV-065 (block L1568–L1585)
```text
L1578: - Original: Gmail 19d9dd26f4e7242b (SENT). Body not yet opened in full.
L1579: - Tag: (V) header/subject/snippet; (U) contents as his adopted demand.
```
#### EV-066 (block L1586–L1627)
```text
L1619:   and the reported phone-number offer (U — his 3/31 statement). No
L1626:   are quoted (G5). Statutory CPRA windows still unverified at source (X).
```
#### EV-067 (block L1628–L1646)
```text
L1638:   full-body opens owed before exhibit print.
```
#### EV-068 (block L1647–L1664)
```text
L1656:   owed before exhibit print.
```
#### EV-069 (block L1665–L1682)
```text
L1672: - Original: Gmail 199db7e78dd8b1de (SENT). Body-open owed.
L1673: - Tag: (V) header/subject; (U) contents.
```
#### EV-070 (block L1683–L1701)
```text
L1684: - What: 31,157,062-byte PDF, per Halsey (U, 2026-08-12, this thread): one of
L1696: - Tag: (U) purpose/provenance per Halsey; (V) Drive metadata live-fetched
L1697:   2026-08-12. CONTENTS UNREAD (31MB — subagent extraction pass owed).
```
#### EV-071 (block L1702–L1726)
```text
L1708:   diff owed).
L1712: - Tag: (U/V) as EV-070. CONTENTS UNREAD — subagent extraction owed.
L1725:   byte-identical to what BHPD received (§7.2 fixes it permanently).
```
#### EV-073 (block L1833–L1847)
```text
L1839: - Original: Gmail 18439a5eabf63be3 (SENT). Body-open owed before exhibit.
```
#### EV-074 (block L1848–L1864)
```text
L1854:   Seroquel" now native-corroborated; A1 language rules apply — never
L1855:   "900 grams," never drug/alcohol characterization). (2) 11/6/2022 "Re:
L1861: - Tag: (V) headers/snippets at source 2026-08-12; bodies-open owed.
```
#### WP-021 (block L1886–L1905)
```text
L1891:   Caption block DEFECT: names "SHANNON MINOR, Defendant" ("In Re Matter
L1900: - Tag: (U) work product — draft pleading, never cite as proof.
```
#### EV-075 [1/2] (block L1908–L1932)
```text
L1923:   wf_0bba0c9f-b95); full-body re-open owed before exhibit print.
L1927:   12/6, 1/5, 1/8, 1/10, 2/12). Plead the list, never an adjective.
```
#### EV-076 [1/2] (block L1933–L1962)
```text
L1954:   full-body re-open owed before exhibit print.
L1961:   date remains UNSOURCED at native level — test owed.
```
#### EV-077 (block L2015–L2023)
```text
L2021:   not established by this message and is not asserted from it.
```
#### EV-078 (block L2041–L2090)
```text
L2046:   about never leaving my kids with no money, something that would never
L2071:   (=EV-079) · "Shannon_Crime_Analysis.pdf" · "AI Executive Summary_AI_
L2081: - Original: Gmail 199a442bb459fce9 (SENT). Tag: (U/Q) — his adopted
```
#### EV-079 (block L2091–L2119)
```text
L2103: - Tag: (V) read in full at source 2026-08-12; (U) as Halsey-adopted analysis.
L2108:   (11/13/2022 "Please go get Grace") ABSENT.** **DEFECT RECORDED, LOUDLY AND
L2116:   individually across BOTH accounts and cites the verified subset; it never
L2118:   remain untested pending secondary-account access.
```
#### EV-080 (block L2120–L2138)
```text
L2120: EV-080 · THE $255,000 CORRECTION — a SECOND Joyce Flaherty destination account, MUFG Union Bank x0703 (favorable (V) finding his own counsel missed)
L2129:   against EV-016/017 owed before the figure is final in the packet.
L2131:   MUFG Union Bank has never been subpoenaed) + CIVIL + 1983.
L2136:   documents + signatories). Register #7's "$242,000" is superseded as an
```
#### EV-081 (block L2209–L2222)
```text
L2209: EV-081 · "Shannon Text Messages.pdf" — THE TEXT LAYER, 111 MB (highest-value unread artifact in the matter)
L2210: - What: 111,071,942-byte PDF of Shannon Minor text messages. NEW — never
L2212: - Tag: (X) contents unread — Drive id + byte size recorded (tamper tripwire).
```
#### EV-082 (block L2223–L2231)
```text
L2226: - Tag: (X) contents unread — id + byte size recorded.
```
#### EV-083 (block L2232–L2256)
```text
L2248: - Tag: (V) as to the excerpt's on-page text read this session; (X) as to the
```
#### EV-084 (block L2257–L2290)
```text
L2257: EV-084 · "Shannon Calculated Attempt To Collect Insurance.pdf" + "Shannon Creating Suicide Scenario For Insurance.pdf" — the insurance-motive compilations (DERIVED)
L2275: - Tag: **(U/I) DERIVED — Halsey-adopted analysis, NOT the originals.** Under
L2280: - Used by: POLICE + CIVIL + 1983 (as roadmap + his adopted account).
```
#### EV-085 (block L2325–L2339)
```text
L2331: - Tag: (V) as to the text extracted this session. **PROVENANCE CAVEAT,
L2332:   MANDATORY ON ANY USE: it is NOT byte- or hash-verified against the 93 MB
L2334:   compressed derivative, or the passage is re-derived from the original.
```
#### EV-086 (block L2340–L2353)
```text
L2346: - PROOF THAT MATERIAL SITS IN THE UNREAD HALF: probes `no money` and
L2348:   the captured 100 pages. The unread half contains money-denial and
L2350: - Tag: (V) pages 1-100; (X) pages 101-214 — unread, cause identified.
```
#### EV-087 (block L2440–L2461)
```text
L2452:   Ids UNREAD (the full exports): `1lYhOFHXU9jbKBg_GVw_Jp7aFctaBf-o0`
```
#### EV-088 (block L2462–L2490)
```text
L2462: EV-088 · "CONFIDENTIAL FORENSIC AUDIT & PUBLIC CORRUPTION REPORT" (1/8/2026) — READ IN FULL, AND IT HAS THREE CHECKABLE DEFECTS
L2471: - **DEFECT 1 — Exhibit A asserts a deletion that did not occur.** It states
L2477:   stated: post-audit Google recovery (EV-049/050), or the assertion was never
L2479: - **DEFECT 2 — the statistic does not measure what it claims.** "P = 1 /
L2483: - **DEFECT 3 — wrong case number on the cover.** "CASE REF: BHPD Case
L2486: - Tag: (V) as to its contents, read in full. **(X) as to Exhibit A's
L2487:   deletion claim — CONTRADICTED at source.**
```
#### EV-092 (block L2587–L2628)
```text
L2602: - Tag: (Q) as to text; **(X) as to every speaker — see below**.
L2604:   **ATTRIBUTION — ALL 656 ROWS ARE `UNDETERMINED` (§17.6, held absolutely).**
L2623:   (b) **`read_file_content` on an image id returns a string BYTE-IDENTICAL to
```
#### EV-094 (block L2740–L2759)
```text
L2751:   still owed before "two policies" is stated as a fact.
```
#### EV-095 (block L2760–L2785)
```text
L2777:   movements are NOT established here and he may have stayed past her 9/6
L2778:   departure. **The collision date stays (X)** pending the Turkish traffic or
L2782:   (`1Hy03H8S7DW4FdodqeL1YGDdvh8HrOSGJ`, UNREAD), and the person the DV-100
L2784: - Tag: (V)/(Q) as to the document; (X) as to the collision date.
```
#### EV-096 (block L2801–L2867)
```text
L2816:   **person**; the screenshots are the custodian's and unauthenticated; frames
L2822:   UNVERIFIED pending Meta records.** Described that way and no better.
L2847:   is after him." Unsourced; filed beside the other unsourced figures.
L2865: - Tag: (Q) text; **(V-structural)** as to the sending account; **(X)** as to
```
#### WP-019 [2/2] (block L3012–L3035)
```text
L3023:   2026-03-27.pdf. Tag (U/Q — his filing; court-file conformed copy not
```
#### WP-020 [2/2] (block L3036–L3058)
```text
L3039:   written consent to electronic service... never affirmatively authorized
L3048:   2026-03-27.pdf. Tag (U/Q). Used by: FAMILY (+CIVIL P036-P037 corroboration
L3054:   2026-08-19 (U) that he "consented to initial service by email ... so we
```
#### EV-100 (block L3080–L3102)
```text
L3084:   `1T_GpQaUJIsnbb1aPGpAL_xsHOstJcstt`; three byte-identical PDF copies, no
L3089: - **DEFECTS v1 MUST NOT INHERIT (each contradicted by the registered
L3091:   "Shannon was the beneficiary" as fact (UNVERIFIED); hypothetical-form
L3098:   the kids love you, we are a family and we stick together…" — native never
```
#### EV-101 (block L3103–L3118)
```text
L3116:   duplicate-recipient line) → $915,203.56 (12/31/24).
```
#### EV-102 (block L3119–L3135)
```text
L3131:   the natural-causes instruction is never trimmed out.
L3132: - Tag: (V)/(Q); native Gmail message not located (L). "page632" contributes
```
#### EV-103 (block L3136–L3158)
```text
L3154: - Tag: (Q) from the police-held piece; native NOT located (L) — hunt open.
L3155: - **Supersedes nothing; completes EV-102: 5/24 (first $4.5mm use, "happily
```
#### EV-105 (block L3217–L3251)
```text
L3233: - **THE DEVICE (PK/U, Halsey 2026-08-23, quoted as his statement):** he
L3238:   recoverable; he did not give it to Kale because (U) Kale "empirically
L3239:   reduced my evidence when provided and never once increased it."
L3248:   claim is (PK/U) until recovery; the placeholders, times, and sender-side
L3250: - Tag: (V) image; (R) structure; (PK/U) content claim.
```
#### EV-106 (block L3252–L3267)
```text
L3264:   appeal in process (U as to filing status) is stated, sourced here. The
```
#### EV-107 (block L3268–L3292)
```text
L3275:   created and inserted into my files that I had never authored… created
L3290:   are both stated, never merged, never offered as answering each other.
```
#### EV-108 (block L3368–L3405)
```text
L3380:   until early 2024; never had an assistant named Janine; does not send
L3381:   links. **The document reads as an AI-generated narrative reconstruction
L3390: - **CONSEQUENCE 2 — THE PLANNED "LANCE-MOTION OVERLAP TABLE" HAD A FALSE
L3399:   selectivity proof — never by the discarded statistic.
```

239 marked lines across 112 entries. Entries whose blocks carry none of these markers (25): EV-001, EV-002, EV-003, EV-004, EV-005, EV-038 [2/2], EV-041, EV-043, EV-044, EV-046, EV-048, EV-050, EV-052, EV-057, EV-072, EV-075 [2/2], EV-076 [2/2], EV-089, EV-090, EV-091, EV-093, EV-097, EV-098, EV-099, EV-104. For EV-001..EV-005 the tag is "(V/Q)". For EV-003 see §6 X7.

### 5b. Non-entry blocks that withdraw, supersede, correct or restrict (verbatim)

- File header: later blocks correct earlier entries:
```text
L2: # [2026-08-27] LOCATOR JOURNAL. Read first: governance/DECISIONS.md (binding) + governance/CURRENT_STATE.md (compiled now). Later blocks correct earlier entries; duplicate-id notice in the 2026-08-27 correction block at tail.
L3: Append entries at the bottom of their class. Never renumber. Rules: README.md
```
- Entry schema: WP never cited as proof:
```text
L8:     EV-### (source evidence) / WP-### (work product — NEVER cite as proof)
```
- WP section heading:
```text
L777: ## WP entries — work product (NEVER cite as proof)
```
- WP-019 [1/2] KEY CORRECTIONS:
```text
L935:   KEY CORRECTIONS it forces: (#12) 2015 event = UPHOLD stock, NOT Vanguard
L936:   [Gmail 19df494cfbefd6b4; PKG 2245] — EV-015 title is a 2015 mislabel; (#15)
L937:   DROP "$2.5M" total, theft spine = $1,134,000; (#17) report date ~3/24/2025
L938:   (Kale email) + 3/29/2025 counsel letter — EV-039's "3/29/2024" unverified;
L939:   (#25) Kale preservation refusals = FOUR not five; (#32) "654/682 days"
L940:   unsourced. **CROSS-MATTER FLAG for the CIVIL + 1983 threads:** the register
L941:   supersedes several figures those activities may still carry (esp. the
L942:   "$2.5M" total and the "2015 Vanguard" characterization) — reconcile there
L943:   too; this is the one register, one writer discipline.
```
- SUPERSEDING NOTE on gap #1 ("Gap #1's implication was WRONG"):
```text
L966: --- 2026-08-07 (pass 2) · SUPERSEDING NOTE on gap #1, appended ---
L967: Gap #1's implication was WRONG, caught by Halsey ("it took me 5 seconds to
L968: find all the Vanguard files"). The financial corpus EXISTS in Drive at
L969: scale and its spine is now registered: EV-014..EV-028 (hidden-account
L970: statements, the Bates 0001–0780 Wells Fargo subpoena production, the
L971: subpoena/notice filings, the $400K Vanguard RFO, statement exhibits, the
L972: detective evidence package) plus WP-010..WP-018 and the 529/WF collections.
L973: The bank records are IN HAND (EV-016/017), not police-only — the demand
L974: predicate in item 5 narrows to records the police gathered BEYOND the
L975: subpoenaed set, if any. What remains open, narrower:
```
- Pass 2b RECONCILIATION ADDENDUM (second run's ids "DISCARDED as ids"):
```text
L987: --- 2026-08-07 (pass 2b) · RECONCILIATION ADDENDUM, appended ---
L988: The session restart forked pass 2 into two parallel executions of the same
L989: approved plan. The run that pushed first (EV-014..028, WP-010..018, above)
L990: is the PUBLISHED register and stands untouched. The second run's
L991: independently assigned ids were never published and are DISCARDED as ids;
L992: its unique content — the completed sweep the first run's approval gate
L993: blocked — is appended as EV-029..033 and the Collections pass-2b bracket.
L994: Full dual-run narrative, id cross-map, resume tokens, and verification:
```
- CORRECTION BLOCK 2026-08-10, C-01..C-04 (tag withdrawn; verdict withdrawn; standing rule):
```text
L1124: ## CORRECTION BLOCK — 2026-08-10 · adoption, not authorship (append-only)
L1125: Governed by OPERATING_CONDITIONS §8, added this date on Halsey's instruction.
L1126: These entries' original text stands above unaltered (append-only discipline);
L1127: where it conflicts with this block, **THIS BLOCK CONTROLS.**
L1128: 
L1129: **C-01 · EV-045 (Exhibit C — Kale/Google) — TAG SUPERSEDED.**
L1130: - Original tag, now withdrawn: "**(I/X)** — an AI-generated SUMMARY of emails,
L1131:   not the emails… treat as a roadmap to the native messages only." The header
L1132:   line "(SUMMARY, not source)" is likewise withdrawn.
L1133: - **Corrected tag: (U) — Halsey's adopted, filed exhibit.** It was submitted to
L1134:   the court as **Exhibit C** to his declaration. He stands behind it. It is a
L1135:   source, and it is citable as his account of the preservation record.
L1136: - Grounds: the tag disqualified it for being AI-produced. That is not an
L1137:   evidentiary category (§8.1). What I actually had against it was that it is a
L1138:   SUMMARY — true of any summary, by anyone (§8.4).
L1139: - What genuinely remains, stated correctly: the native Kale emails are still
L1140:   worth obtaining, because an opponent will compare exhibit to underlying
L1141:   record and because they settle the count conflict below. That is a strength
L1142:   task, not a defect. **The 654-day figure is VERIFIED arithmetic** on the
L1143:   exhibit's own two dates (F-20) and needs no apology.
L1144: 
L1145: **C-02 · The four-vs-five conflict is NOT an AI problem — restated.**
L1146: EV-042 ¶9 (sworn) says "at least five separate occasions." Fact register #25
L1147: says four [Gmail 19c31c2994519631, "Fourth Formal Request"]. EV-045 says "at
L1148: least four times." The conflict is between **Halsey's own sworn filing and his
L1149: own register** — it exists whatever produced Exhibit C, and would exist if a
L1150: paralegal had typed it. Plead neither count until the native emails resolve
L1151: it. Nothing about this reflects on EV-045's status as a source.
L1152: 
L1153: **C-03 · WP-020 (violations infographic) — VERDICT WITHDRAWN, defects kept.**
L1154: - Withdrawn: my categorical "**NOT FILING-READY**" and "Used by: none until
L1155:   rebuilt." That was my call to make and it was not mine (§8.6).
L1156: - **Kept, because they are checkable and he would want them caught:** "Anna
L1157:   Kralle" surname is unverified (only AnnaK@ is (V)); the record shows
L1158:   "Matthew" Sirriyeh, not "Matt"; the 57/43 split states no denominator; the
L1159:   bar heights disagree with the chart's own axis; the firm shows ≥5 staff on
L1160:   its own mail. A wrong surname in a filed exhibit is the F-01 failure family
L1161:   — that is why these stay on the record.
L1162: - **Corrected status: (U) work product, Halsey-adopted. Usable at his
L1163:   direction.** Fix the surname and the denominator before it goes anywhere,
L1164:   and the rebuild from the POS signatory audit (CANON OPEN-6) makes it
L1165:   stronger — it is not a precondition to its existing as a source.
L1166: 
L1167: **C-04 · STANDING RULE for this index.** No future entry is tagged (X), "not a
L1168: source," or "roadmap only" on the ground that an AI, calculator, dashboard, or
L1169: assistant produced it. Where verification is incomplete, write exactly what is
L1170: unverified and against which record — never a status label that reads as
L1171: disqualification. (X) keeps its narrow meaning only: OPERATING_CONDITIONS §7.4.
```
- CONVERSION BLOCK 2026-08-10 (prohibitions withdrawn; K-01..K-09; standing rule):
```text
L1302: ## CONVERSION BLOCK — 2026-08-10 · prohibitions become annotations (append-only)
L1303: Governed by OPERATING_CONDITIONS §10. Everywhere in this repo I wrote "do not
L1304: plead," "not pleadable," "fenced," "gated," or "does not go in this packet,"
L1305: **that was a submission ruling I had no standing to make.** Those words are
L1306: withdrawn wherever they appear. The items below are IN THE RECORD. Each carries
L1307: its tested status and the specific test still owed. **The decision to use any
L1308: of them is Halsey's.**
L1309: 
L1310: | # | Item | Status | Test that settles it | What I found |
L1311: |---|---|---|---|---|
L1312: | K-01 | **"654 days"** (EV-045 / F-20 / F-21) | Arithmetic VERIFIED (2024-03-29 → 2026-01-12 = 654 exactly). Input year UNTESTED. | Read the first preservation request's date header, with its year, from the native email. | Case's other "March 29" is the 3/29/2025 counsel letter; BHPD reporting ≈3/24/2025; a Sent subject search for preserve/preservation/legal hold returned 16 threads, none in 2024. **If the year is 2025 the figure is 289.** Both figures are in the record; neither is deleted. |
L1313: | K-02 | **"Sept & Oct 2022 locking me out"** (his 1/8/2026 email to BHPD, F-22) | The STATEMENT stands as his adopted, sent statement to law enforcement. The 2022 lockout is UNCORROBORATED. | Search 2022 for recovery notices in the backup account and any other address; check whether a 2022 episode exists that this mailbox would not show. | In THIS mailbox, 2022-07-01→2023-07-15 has no recovery notices; the notice sequence is 2023. A real, unexplained 2022-09-14 password change DOES exist (EV-051). |
L1314: | K-03 | **$1.3M → $500–600K drop** vs the **$1,134,000** spine | Both figures IN. Their relationship UNTESTED. | Pull the statements spanning the drop plus two prior months; reconcile line by line. | Not yet run. Different arithmetic, so they may be distinct events, overlapping, or the same — unknown, not excluded. |
L1315: | K-04 | **"She probably didn't do it the month before"** | Halsey's own stated read, IN as his read. | The same statements as K-03 — the prior two months answer it directly. | Not yet run. |
L1316: | K-05 | **The February account shutdown** | IN as his account. Year and account UNIDENTIFIED. | Halsey names the year and institution, or a statement/closure letter is pulled. | "After I survived" points to the Sept 17 2023 event, which would suggest Feb 2024 — my inference only, never his statement. |
L1317: | K-06 | **Preservation-request COUNT** | RESOLVED IN HIS FAVOUR. | Open the six threads in EV-054, confirm each is distinct. | The 1/10/2026 "Fourth Formal Request" is not the last (2/12/2026 follows). At least five written. The sworn "at least five" is CORRECT. |
L1318: | K-07 | **EV-053 Google Legal refusal** | IN. Header, sender, date, subject and the quoted line all verified. Body not yet opened. | One successful get_message on 19af06ba182f7aa6 (the call returned "service unavailable" 2026-08-10). | The quoted line is the operative one: "Google only takes steps to preserve data upon being properly served with valid legal process." |
L1319: | K-08 | **WP-020 infographic** | IN as his adopted work product (already converted at C-03). | Verify the "Anna Kralle" surname and the 57/43 denominator. | Only AnnaK@ is verified; record shows "Matthew" Sirriyeh. Two checkable fixes, not a verdict. |
L1320: | K-09 | **A recording of the Kale call** | Not an evidence item — an OPEN REQUEST. | The BHPD records demand (matters/04). | Nothing to withdraw here: asking for a record is the correct form, and "no recordings retained" is itself a finding. |
L1321: 
L1322: **STANDING RULE FOR THIS INDEX (replaces C-04's framing, keeps its substance):**
L1323: Every item enters. The Tag line records what has been TESTED and against what
L1324: — never whether the item is permitted. No entry is ever refused, removed, or
L1325: labelled unusable because of how it was produced or because a test is still
L1326: owed. Where I believe something is wrong, I say so once, in the Notes, with the
L1327: evidence — as a finding for Halsey to weigh, not a ruling.
```
- EV-056 ANNOTATION item 1 (page count was wrong):
```text
L1463: --- EV-056 ANNOTATION — 2026-08-12 (append-only; full-extraction pass complete) ---
L1464: Full per-section extraction committed:
L1465: matters/04/report_2026-08/15_EV056_FULL_EXTRACTION.md. Corrections/finds:
L1466: 1. PAGE COUNT: the mirrored PDF is 34 pages, not the 68 recorded at intake
L1467:    (sha256 unchanged and re-verified this session — the count, not the file,
L1468:    was wrong). Binding anomaly: the chronology's reading order is pp.1-4 →
L1469:    p.17 → pp.5-7 (p.17 misbound inside the "Three Emails" section).
```
- DEFECT BLOCK — four fabricated-form quotes in EV-011:
```text
L2139: --- DEFECT BLOCK — 2026-08-12 · FOUR FABRICATED-FORM QUOTES IN EV-011 (loud, once, with the evidence) ---
L2140: Extraction of EV-011 ("POLICE REPORT — Analysis of Evidence, Aug 2025
L2141: update", Drive 1Ddy18LylKHbe5gjkeIhzFIOVOVhKAJUO, read in full 2026-08-12,
L2142: 93,802 chars) found **four passages formatted as direct quotations of
L2143: Shannon Minor that the document's own surrounding text shows are NOT
L2144: quotations.** Worst example, at line 1237 of the extraction, presented in
L2145: quote form: "maybe you should just kill yourself, then at least we'd have
L2146: money from insurance" — the document's actual framing is **"If indeed she
L2147: said things along the lines of…"**. Another is preceded by the author's own
L2148: words: **"we don't have a direct quote of that in the record provided."**
L2149: All four are quarantined in file 21_ §9.
L2150: **WHY THIS IS RECORDED AT THE TOP OF THE REGISTER AND NOT SOFTENED:** an
L2151: investigator who quotes that line as Shannon's words would be making a
L2152: material misstatement, traceable to a document Halsey submitted. That is the
L2153: F-01/F-02 failure family and it is exactly what would destroy the packet's
L2154: credibility with a new chief — the same structural risk as the §7.6
L2155: Exhibit-F finding.
L2156: **FORM (OP.COND. §10):** this is a FINDING, not a submission ruling. The
L2157: item · tested: yes, against the document's own surrounding text · test owed:
L2158: none for the defect itself; the underlying question (did she say anything of
L2159: the kind?) is answered only by the preserved phone (EV-038 / R-9) and the
L2160: native message record · what the test showed: the four quotes have no
L2161: quoted source in the document. Halsey decides what is submitted; if EV-011
L2162: goes anywhere, it needs a cover sheet identifying these four passages as the
L2163: author's hypotheticals. Nothing in EV-011 is otherwise disqualified — its
L2164: sourced material stands.
```
- EVIDENTIARY-WEAKNESS NOTES:
```text
L2166: --- EVIDENTIARY-WEAKNESS NOTES — 2026-08-12 (append-only) ---
L2167: 1. **EV-010 is misnamed.** Titled "Sent to Police — 500 Emails & iMessages
L2168:    Timeline," its actual content is an ANALYSIS of EV-071 plus the
L2169:    Provinziano letter plus ~76% Wells Fargo statement OCR. Searches for
L2170:    From:/To:/Subject:/Sent:/iMessage return ZERO. **There is no message
L2171:    corpus inside it.** Every message quote in it is a quotation-within-an-
L2172:    advocacy-document, not a native. The 500-message corpus is therefore
L2173:    still UNLOCATED as a native set — it is a hunt target, and its absence
L2174:    explains why the text-layer evidence keeps coming up short.
L2175: 2. **The Grace-crisis texts are UNDATED in the corpus as compiled** — no
L2176:    timestamps. Quoting them as dated events would be the F-01 failure; the
L2177:    preserved phone (R-9) is what dates them.
L2178: 3. **"Advance on inheritance" appears NOWHERE in EV-010/011** ("inheritance"
L2179:    and "advance" both zero hits). Its only source remains V6 ¶20's
L2180:    description of the sworn 2/24/2025 discovery response — the document
L2181:    itself is still owed (decision-queue item).
L2182: 4. **The "Loan Repayment" memo has a documented antecedent, stated with its
L2183:    limit:** Joyce sent Shannon $50,000 (11/06 + 11/16/2022, two $25,000
L2184:    transfers) BEFORE the refund; the "Loan Repayment" transfer out of his
L2185:    account was $150,000 — **three times the advance**, and drawn on his
L2186:    separate property. Both halves go to investigators together.
L2187: 5. Counsel-letter defects re-confirmed: Exhibit B typo "**x2118**" for x2218
L2188:    (an investigator pulling x2118 finds nothing — flag on the face of any
L2189:    citation); "federal" vs "California 2010" tax-refund characterization
L2190:    conflict. Also logged and NOT a real discrepancy: an OCR artifact showing
L2191:    the same $700,000 reference number as 11/28 on one statement page and
L2192:    11/23 on another — recorded so it is not later "discovered" as a conflict.
```
- EV-081 CORRECTION (blocker "recorded WRONGLY"):
```text
L2291: --- EV-081 CORRECTION — 2026-08-12 (append-only; supersedes the blocker stated at registration) ---
L2292: **The reason EV-081 is unread was recorded WRONGLY by me.** I wrote that the
L2293: 10 MB MCP download cap and the drive.google.com egress denial were the
L2294: blockers. Extraction pass (file 26_) establishes the real cause:
L2295: **"Shannon Text Messages.pdf" HAS NO TEXT LAYER AND DRIVE HAS NEVER OCR'd IT.**
L2296: No text-based channel can reach content that does not exist.
L2297: Evidence for the finding, run rather than assumed:
L2298: 1. `read_file_content` returned `{"fileContent":""}` — no error, no
L2299:    truncation warning — on **all five** byte-identical copies (the earlier
L2300:    inventory recorded 2; there are FIVE, across four folders).
L2301: 2. CONTROL: the same tool returned 96,417 characters from an unrelated
L2302:    2.98 MB PDF. The tool works.
L2303: 3. Drive's own index returns ~5,003-char content snippets for comparable
L2304:    files — including 1.27 MB **PNGs** at ~1,285 chars, so Drive DOES OCR
L2305:    images in this corpus. This file returns **0**.
L2306: 4. DECISIVE PROBE: `fullText contains 'you'` — **no hit.** In a
L2307:    text-message corpus that is dispositive.
L2308: **TRAP RECORDED SO NO SESSION FALLS INTO IT:** `fullText` also matches the
L2309: TITLE. Probing `text` or `Shannon` RETURNS this file — off the filename
L2310: "Shannon **Text** Messages.pdf", not off any message. Without that control
L2311: those read as hits. 65 substantive probes: zero snippets.
L2312: **WHAT WAS REFUSED, CORRECTLY:** no ledger rows were invented, and quotes
L2313: were NOT harvested from "Updated Shannon Crime Analysis Text Messages.docx"
L2314: (readable, matches many probes) — that is DERIVED analysis, and presenting
L2315: its quotes under an EV-081 locator would launder secondary commentary into
L2316: the evidence record under a false citation.
L2317: **REMEDIATION (now a concrete task, not a vague blocker):** download outside
L2318: this runtime → split into <10 MB parts → OCR → upload the parts as a
L2319: DERIVATIVE, preserving the 111,071,942-byte original untouched as the tamper
L2320: tripwire. **RENDER PAGES AS IMAGES rather than flat-OCR text where possible**
L2321: — the sender-side markings (bubble alignment/colour) that OPERATING_
L2322: CONDITIONS §17.6 attribution depends on are destroyed by flat OCR.
L2323: EV-081 STATUS: **UNREAD — no channel available in this runtime can read it.**
```
- METHOD CORRECTION (supersedes the extraction premise):
```text
L2354: --- METHOD CORRECTION — 2026-08-12 (binding; supersedes the extraction premise) ---
L2355: **`contentSnippet` DOES NOT REACH PAST THE TRUNCATION.** It is a FIXED
L2356: ~5,003-character window off the HEAD of a document, byte-identical no matter
L2357: which phrase is searched. Consequence: `fullText` probes can establish
L2358: PRESENCE/ABSENCE of a phrase in Drive's index, but they CANNOT yield
L2359: verbatim text from deep in a document. Any plan that assumed snippet-based
L2360: deep retrieval (including my own, written earlier today) is wrong on that
L2361: point. What probes ARE good for: proving that unread material exists —
L2362: exactly how EV-086's unread half was demonstrated.
```
- SPEAKER DISCIPLINE (all 109 rows UNDETERMINED):
```text
L2364: --- SPEAKER DISCIPLINE APPLIED — 2026-08-12 ---
L2365: **Every one of the 109 ledger rows is tagged UNDETERMINED.** The export
L2366: renders both sides as unlabelled paragraphs: no sender field, no alignment
L2367: surviving conversion. The recurring "Messages - Shannon Minor" is a THREAD
L2368: HEADER and was not used to attribute anything (§17.6). Content cues make the
L2369: alternation legible to a human reader, but that is inference and it was kept
L2370: out of the speaker column. **No line from this corpus goes to an
L2371: investigator as a named person's words until the side is established from
L2372: the images.**
```
- SECOND 111 MB FILE: open question, then RESOLVED as "one document filed twice":
```text
L2397: --- SECOND 111 MB FILE, DIFFERENT ID — 2026-08-12 ---
L2398: A file also titled "Shannon Text Messages.pdf" exists at Drive id
L2399: `1ikRSLdaUWGE05M003ixxExDZsW5dJqiY` (111 MB) — **a DIFFERENT id from EV-081
L2400: (`1K5akFNK4ptlGF5N1dZP1haphrg8gwFas`)**. Whether these are the same bytes
L2401: under two ids, or two different documents, is UNTESTED. Both are entirely
L2402: unindexed and neither has ever been examined. Task: compare byte sizes and
L2403: resolve before either is cited.
… [L2404–L2577 not reproduced here]
L2578: --- THE SECOND 111 MB FILE — RESOLVED 2026-08-12 ---
L2579: Both "Shannon Text Messages.pdf" files are **exactly 111,071,942 bytes**,
L2580: uploaded **40 seconds apart** on 2026-06-05, into different folders:
L2581: `1K5akFNK4ptlGF5N1dZP1haphrg8gwFas` → "AA Jell Cell For Lance";
L2582: `1ikRSLdaUWGE05M003ixxExDZsW5dJqiY` → "FORENSIC EVIDENCE".
L2583: **Finding: one document filed twice, not two documents.** Limit stated:
L2584: identical byte count is strong but is not a hash, and neither copy has a text
L2585: layer, so neither has been read.
```
- C-07 truncated Drive folder ids:
```text
L2405: --- CORRECTION C-07 · TRUNCATED DRIVE FOLDER IDS (my error) — 2026-08-12 ---
L2406: **What was wrong.** File 20_ABUSE_CORPUS_INVENTORY records the WhatsApp
L2407: screenshot folder as `1-14wNOUvTP5lQeLyFSIa9yZn4DG` in the parent column of
L2408: ~45 rows. That string is **28 characters**. Drive folder ids in this corpus
L2409: are **33 characters**. The id was truncated in the table I built it from and
L2410: I propagated it without checking its length. Any query using it fails or
L2411: silently returns nothing — which is the worst failure mode available here,
L2412: because an empty result reads as "the folder is empty" rather than "the id
L2413: is malformed."
```
- C-08 EV-079 dates for entries #3/#4:
```text
L2539: --- CORRECTION C-08 · EV-079 DATES FOR ENTRIES #3/#4 — 2026-08-12 ---
L2540: EV-079 dates the Carol Minetree messages **#3 Nov 5, 2022 1:47 PM** and
L2541: **#4 Nov 5, 2022 4:03 PM**. **Both the pre-intrusion export (EV-087) and the
L2542: live account date the thread Nov 6, 2022.** The ABSENCE finding is unaffected
L2543: and is now independently verified (EV-091). **The DATES are not confirmed and
L2544: must not be pleaded as EV-079 states them** until the original is obtained
L2545: from Carol Minetree. F-01 family: a checkable date that is wrong costs more
L2546: than the point it was meant to carry.
```
- EV-092 ATTRIBUTION — all 656 rows UNDETERMINED:
```text
L2604:   **ATTRIBUTION — ALL 656 ROWS ARE `UNDETERMINED` (§17.6, held absolutely).**
L2605:   A `✓` delivery-receipt glyph does appear in the OCR, and in WhatsApp renders
L2606:   only on outgoing messages. **It was NOT used as a side marker**, for four
L2607:   documented reasons: Drive's OCR flattens the two-column bubble layout into
L2608:   one stream with timestamps demonstrably transposed against their bodies; the
L2609:   glyph OCRs inconsistently as ✓/✔/v/Q/p/D/♡/y or drops entirely; a correctly
L2610:   read glyph still cannot be bound to a specific adjacent message; and bubble
L2611:   alignment and colour — the only reliable indicators — do not survive an OCR
L2612:   channel at all. It is logged as `[✓ nearby]`, an investigative pointer,
L2613:   expressly not an attribution. **No line goes to an investigator as a named
L2614:   person's words until the side is fixed from the images or the handset.**
```
- C-09 the DA did respond ("THAT IS FALSE"):
```text
L2868: --- CORRECTION C-09 · THE DA DID RESPOND — our own record was wrong — 2026-08-12 ---
L2869: **File 12_ (OBLIGATIONS LEDGER, Completion Pass 2) states: "Last DA message on
L2870: record remains 1/12/2026." THAT IS FALSE.** A sweep
L2871: `in:anywhere from:da.lacounty.gov` returns **nine threads with at least SIX
L2872: substantive DA responses**, two from **named DA staff**, through **3/19/2026**:
L2873: 1/8/2026 (`19b9fe124c63613a`) · 1/12/2026 (`19bb307ee4795b75`) · **1/12/2026
L2874: AWise@da.lacounty.gov** (`19bb3ad9899c0a6d`, JSID: "JSID does not generally
L2875: initiate criminal investigations") · 1/15/2026 (`19bc3db9c2a11195`) ·
L2876: 1/22/2026 (`19be735cadc9e828`) · 1/30/2026 (`19c102e73a5cbca7`, "Please
L2877: contact JSID at (213) 974-3888") · **3/19/2026 jcastano@** (`19d07358d5ac4260`).
L2878: **WHAT SURVIVES:** the post-**4/17/2026** silence through all three EV-065
L2879: deadlines (5/1, 5/17, 6/16/2026) — that sweep returned zero and is unaffected.
L2880: **WHAT MUST NEVER BE SAID AGAIN: "the DA never responded."** One reply
L2881: produced by the other side would have cost the packet its credibility on
L2882: everything else in it. Correct framing: **form responses and one substantive
L2883: statement through March 2026, then silence after 4/17/2026 through every
L2884: deadline in the formal demand.**
```
- C-10 EV-036 [1/2] is 54 pages:
```text
L3061: --- CORRECTION C-10 · EV-036 IS 54 PAGES — hash-verified same file ---
L3062: sha256 of report_2026-08/39e87acb-First_50_Pages.pdf =
L3063: 60c1e6b5f6e76ac9e55e76568f561989298b40b0d3058670bb7af6ac7ffcad62 —
L3064: IDENTICAL to the 99_UPLOAD_HASHES registration. Page tree /Count 54. EV-036's
L3065: "24-page PDF… lacks the image section entirely" mis-described this same
L3066: file: pp.31–54 are present. **54/51/24 collapses to 54-vs-51**; [PKG line N]
L3067: freeze holds until the ~51-page line-numbered copy is located. pp.13–54
L3068: extracted to 36a_F50_PP13-54_TEXT.md; pp.16–18 image-only.
```
- C-11 EV-099 entry #5 date:
```text
L3070: --- CORRECTION C-11 · EV-099 ENTRY #5 IS MAY 23, 2023 — and it is her reply
L3071: to the polygraph demand ---
L3072: The "zero cash / Our marriage is over / putting us on the street" email,
L3073: estimated "~6/1/2023" in EV-099, is dated **May 23, 2023** on the face of
L3074: the police-held image [EV-036 p.46], where it appears as Shannon's direct
L3075: reply to Halsey's (Q) "I want to have a lie detector t[est]…" and "Get the
L3076: $250k back from your mom." Absence-from-live-Gmail verification unaffected
L3077: (the sweep was date-agnostic). Sequence preserved on one page: polygraph
L3078: demand → "Our marriage is over… zero cash." Fourteen days before The Plan.
```
- EV-100 "DEFECTS v1 MUST NOT INHERIT":
```text
L3089: - **DEFECTS v1 MUST NOT INHERIT (each contradicted by the registered
L3090:   record):** "$5 million policy" as fact (EV-093: $2,000,000, owner HALSEY);
L3091:   "Shannon was the beneficiary" as fact (UNVERIFIED); hypothetical-form
L3092:   passages reading as quotes ("If, for instance, a text from Shannon said,
L3093:   'Maybe you should just do it…'"; "she did, in fact, deny an autopsy and
L3094:   had him cremated, if that occurred") — EV-011/F-02 family; undated "or
L3095:   else Grace would die" assertions (F-01); and **NO Incident Group Three**
L3096:   (no deletions/Google/Kale/DA/Marsy's) — the why-supplement core.
```
- CORRECTION BLOCKS 2026-08-27 (D-1 supersedes candidate counts) and 2026-08-27b (duplicate ids):
```text
L3433: ---
L3434: 
L3435: ## CORRECTION BLOCK — 2026-08-27 · the decisions gate + duplicate ids (append-only)
L3436: - Per governance/DECISIONS.md **D-1**: every "candidate sixth/seventh demand"
L3437:   phrasing in this index and its notes is **SUPERSEDED**. The asserted
L3438:   preservation-demand count is FIVE (his ruling; EV-054 criteria). Located
L3439:   demand-like documents beyond the five (EV-069; the EV-075 demand set;
L3440:   Gmail 199db7e78dd8b1de) remain library documents under D-6 and enter no
L3441:   count absent his express reclassification.
L3442: - **DUPLICATE-ID NOTICE:** "EV-075" and "EV-076" were each assigned to TWO
L3443:   different entries (the Apr–Sep 2025 demand/deletion-window sets AND the
L3444:   July-2023 exchange/message entries). Until the owning thread renumbers by
L3445:   append, citations to these four entries must use TITLE + MESSAGE ID, not
L3446:   the bare EV number. (Allocation lessons 2026-08-07 / 2026-08-12.)
L3447: 
L3448: ## CORRECTION BLOCK — 2026-08-27b · ELEVEN duplicate ids (audit A/C; supersedes the two-id notice above)
L3449: Independent audit measured 137 entry headers over 129 unique ids. The
L3450: following ids each name TWO DIFFERENT documents: **EV-035 · EV-036 · EV-037 ·
L3451: EV-038 · EV-042 · EV-075 · EV-076 · EV-079 · EV-081 · WP-019 · WP-020.**
L3452: Roughly 211 citations reference the previously unacknowledged ones, and
L3453: preserved PDFs on disk are named by the SECOND assignment — so a bare-id
L3454: citation can silently resolve to the wrong exhibit. RULES, effective now:
L3455: (1) cite these eleven by TITLE + message id / hash, never bare id; (2) the
L3456: owning threads renumber the second assignments BY APPEND (new id, old entry
L3457: cross-noted — nothing rewritten); (3) before any NEW id is assigned, grep the
L3458: full index for it (the max()+1 allocator caused this five separate times);
L3459: (4) any on-disk mirror named by a colliding id gets a README line in its
L3460: directory stating which assignment it is.
```

### 5c. Compact index by category (verbatim lines)

- AI-derived, in the index's own words: EV-039:
```text
L553: (2024–2026)" — Halsey↔Kale reconstruction + Triangle-of-Corruption hypothesis
L554: - What: 11-page work-product/AI-assisted reconstruction of the ~2-year Halsey–
L555:   Det. Kale email history, plus the leak/"Scalpel"/insider-knowledge/Spiegel-
L556:   collusion theory, Marsy's dashboard metrics, and a 1-in-10B statistic.
… [L557–L561 not reproduced here]
L562: - Tag: (I/X) — AI-derived reconstruction; its email date-stamps are Halsey's
L563:   characterizations, NOT re-sourced to native Gmail this session. Underlying
L564:   Kale emails must be pulled before any date/quote ships.
```
- AI-derived: EV-045 (C-01 later withdrew the tag as a disqualifier, L1129-1138; AGENT_RULES #6 class remains AI-LEAD):
```text
L1066: EV-045 · Exhibit C — Kale / Google preservation record (SUMMARY, not source)
L1067: - What: Gmail "AI Overview" panel over a search of mail to
… [L1068–L1071 not reproduced here]
L1072: - Tag: **(I/X) — an AI-generated SUMMARY of emails, not the emails.** Sources
L1073:   outrank summaries; treat as a roadmap to the native messages only.
```
- AI-derived: EV-056 (AI-assisted, Gemini):
```text
L1335:   it. AI-assisted (Gemini), adopted and supplied by Halsey 2026-08-11.
```
- AI-derived: WP-007:
```text
L825: WP-007 · "Google-Gemini — Deletion 100pct Match + Hacking (AI analysis)"
L826: - What: AI-generated analysis of deletion/spoliation and hacking indicators.
… [L827–L827 not reproduced here]
L828:   2026-06-12 (Google-spoliation folder). Tag (I/X — AI-derived; its
L829:   underlying artifacts must be sourced independently before anything it says
L830:   is used). Used by: CIVIL + POLICE + 1983 (analysis-support only).
```
- AI use stated in a title: EV-028:
```text
L376: EV-028 · Evidence package for the detective — "…USED_BY_AI_TO_MAKE_ALEX_JOB_
L377: EASY_Bank_Statements._Messaging_11_01_2022_To_12_30_2024_Excludes_First_
L378: Hacking_And_Vanguard_512Pages"
```
- AI-generated reading of the challenged Exhibit F (inside EV-108):
```text
L3381:   links. **The document reads as an AI-generated narrative reconstruction
L3382:   with the wrong correspondent name attached — fully consistent BOTH with
L3383:   the court's fabrication finding AND with Halsey's on-record "narrative
L3384:   summary… was a mistake" explanation. v1 states both, adopts neither.**
```
- AI-titled attachments delivered to BHPD with EV-078 (not separately registered):
```text
L2071:   (=EV-079) · "Shannon_Crime_Analysis.pdf" · "AI Executive Summary_AI_
L2072:   Analysis_Of_All_Evidence.pdf" · "Executive Summary_AI_Analysis_of_All_
L2073:   Evidence_Kale.pdf" · "Transfer of Halsey Minor Funds to Shannons Mother
… [L2074–L2078 not reproduced here]
L2079:   Internet Innovation Timeline 2.pdf" · "OpenAI 003 Report Generated on
L2080:   Halsey Minor.pdf".
```
- Duplicate ids (8 with two headers; 08-27b lists 11): see §1 Census and §6 X1:
```text
L3442: - **DUPLICATE-ID NOTICE:** "EV-075" and "EV-076" were each assigned to TWO
L3443:   different entries (the Apr–Sep 2025 demand/deletion-window sets AND the
L3444:   July-2023 exchange/message entries). Until the owning thread renumbers by
L3445:   append, citations to these four entries must use TITLE + MESSAGE ID, not
L3446:   the bare EV number. (Allocation lessons 2026-08-07 / 2026-08-12.)
L3447: 
L3448: ## CORRECTION BLOCK — 2026-08-27b · ELEVEN duplicate ids (audit A/C; supersedes the two-id notice above)
L3449: Independent audit measured 137 entry headers over 129 unique ids. The
L3450: following ids each name TWO DIFFERENT documents: **EV-035 · EV-036 · EV-037 ·
L3451: EV-038 · EV-042 · EV-075 · EV-076 · EV-079 · EV-081 · WP-019 · WP-020.**
```
- Same document registered twice or more: EV-023 = EV-033:
```text
L423: - CROSS-REF: EV-023's "2024.pdf" (1WNXPVaKd9af-RYUSdgWMnoxDLjx7rFKi,
L424:   4,299,446 B) is an identical-size loose copy of THIS document (I) — the
L425:   "confirm institution/period" note there resolves accordingly on first
L426:   read.
L427:   [2026-08-19: UPGRADED (I)->(V) — sha256-identical, verified in the
L428:   preservation run; see preserved_2026-08-19/MANIFEST.md. Same document.]
```
- Same document: EV-101's Drive id is listed as an EV-033 copy:
```text
L422:   1zyk-4TL5iK6j4AmCbIAY7HgtsTw-XP6g · 1sneI6QWCf7lBdJgC3KFaYu5PbsG6LGo0.
… [L423–L3103 not reproduced here]
L3104: - What: "2024.pdf", Drive `1zyk-4TL5iK6j4AmCbIAY7HgtsTw-XP6g` (4,299,446 B),
```
- Same document: EV-081 under two Drive ids:
```text
L2579: Both "Shannon Text Messages.pdf" files are **exactly 111,071,942 bytes**,
L2580: uploaded **40 seconds apart** on 2026-06-05, into different folders:
L2581: `1K5akFNK4ptlGF5N1dZP1haphrg8gwFas` → "AA Jell Cell For Lance";
L2582: `1ikRSLdaUWGE05M003ixxExDZsW5dJqiY` → "FORENSIC EVIDENCE".
L2583: **Finding: one document filed twice, not two documents.** Limit stated:
L2584: identical byte count is strong but is not a hash, and neither copy has a text
L2585: layer, so neither has been read.
```
- Same document: EV-083 is page 100 of EV-086; EV-085 is the compressed twin of EV-082:
```text
L2326: - What: compressed twin of the 93 MB iMessage export. Drive id
L2327:   `1Ey5As…` (full id in file 27_). **11.6 MB — under the cap and WITH a text
… [L2328–L2340 not reproduced here]
L2341: - What: the 214-page iMessage transcript. **EV-083 ("IMessages. Not sure
L2342:   dates. Not many.pdf") is character-for-character PAGE 100 of it** — the
L2343:   parent question is closed. Pages 1-100 captured via EV-085. **Pages
```
- Same document: EV-069's message 199db7e78dd8b1de is also EV-075 [1/2] item (2):
```text
L1920: - Original: Gmail 1999df6b5ce0fbce · 199db7e78dd8b1de (=EV-069) ·
```
- Same content (I): EV-036 [1/2] pp.13–15 = EV-009:
```text
L485:   BHPD 3/29/2025 (= EV-009 content (I), byte-compare pending); pp.16–24 WF
L486:   statements — x2218 (Shannon+Halsey, 619 Trenton Dr BH 90210) Nov+Dec 2022
L487:   pages with all five transfers and refs; x0890 (Shannon+Joyce, 350 S
```
- Copies the index calls the same document (I) or byte-identical: EV-010, EV-020, EV-029, EV-042 uploads, EV-088, EV-100:
```text
L159: - Copies, identical byte size 24,470,497 (I — same document inferred from
L160:   exact size match; contents not byte-diffed):
… [L161–L255 not reproduced here]
L256: - Copies, identical byte size 4,069,611 (I — same document by exact size):
… [L257–L388 not reproduced here]
L389: - What: consolidated annual statement PDF for the 529 plan accounts; one
L390:   document copied into each account's year tree (I — inferred from
L391:   byte-identical size across all four accounts).
… [L392–L1033 not reproduced here]
L1034: - Original: uploads c44bdef5-…_2.pdf and 6accfb51-….pdf — BYTE-IDENTICAL,
L1035:   7,318,891 B each · sha256
… [L1036–L2464 not reproduced here]
L2465:   leak. Drive `1GUx4KFVuaE1OvXdMkBBRo4i53hcFPzFR` (193,440 B); same text also
L2466:   at `1o28AfWU4R54gaQKyk0P-OrNsjdJ4aULa` (129,187 B). Closing section
… [L2467–L3083 not reproduced here]
L3084:   `1T_GpQaUJIsnbb1aPGpAL_xsHOstJcstt`; three byte-identical PDF copies, no
L3085:   version conflict). **READ 100% 2026-08-23** (97,288 chars).
```
- Two different documents under one name: EV-021 and EV-022:
```text
L270: - **RECONCILIATION FLAG:** files with the SAME TITLE but 241,717 B exist
L271:   (122PTqRytZElsaDS2Ffr2KA0lfoHATlNa · 1xAoNlSBE6q7PS1psMwT41NkMxnHi1Pic ·
L272:   19WT4QY6R-rKtvIOZsPTMgg7SSk5jQmCm · 145TAxmAcIYrv__MA3EwtM_Rx0cMafHr1 ·
L273:   1DMhc03gb_OjUcC1h_cCQsjPlvzazPkhb). Two byte families = two DIFFERENT
L274:   documents under one name. Determine which is the true export before any
L275:   filing use.
… [L276–L283 not reproduced here]
L284:   Two near-identical byte families — 3-byte delta; treat as two versions
L285:   until diffed.
```
- Withdrawn: C-01 tag on EV-045; C-03 verdict on WP-020 [1/2]:
```text
L1130: - Original tag, now withdrawn: "**(I/X)** — an AI-generated SUMMARY of emails,
L1131:   not the emails… treat as a roadmap to the native messages only." The header
L1132:   line "(SUMMARY, not source)" is likewise withdrawn.
… [L1133–L1153 not reproduced here]
L1154: - Withdrawn: my categorical "**NOT FILING-READY**" and "Used by: none until
L1155:   rebuilt." That was my call to make and it was not mine (§8.6).
```
- Withdrawn: EV-040 "Do NOT enter the police report":
```text
L597:   Halsey-adopted → a SOURCE, at minimum (U) (§8.1). "Do NOT enter the police
L598:   report" above is withdrawn as my phrasing; the operative rule is ADDENDUM
```
- Withdrawn: CONVERSION BLOCK prohibitions:
```text
L1303: Governed by OPERATING_CONDITIONS §10. Everywhere in this repo I wrote "do not
L1304: plead," "not pleadable," "fenced," "gated," or "does not go in this packet,"
L1305: **that was a submission ruling I had no standing to make.** Those words are
L1306: withdrawn wherever they appear. The items below are IN THE RECORD. Each carries
```
- Superseded: 2026-08-27 D-1 (candidate counts) and 2026-08-27b (two-id notice):
```text
L3436: - Per governance/DECISIONS.md **D-1**: every "candidate sixth/seventh demand"
L3437:   phrasing in this index and its notes is **SUPERSEDED**. The asserted
L3438:   preservation-demand count is FIVE (his ruling; EV-054 criteria). Located
… [L3439–L3447 not reproduced here]
L3448: ## CORRECTION BLOCK — 2026-08-27b · ELEVEN duplicate ids (audit A/C; supersedes the two-id notice above)
```
- "Never cite" / do-not-use statements: WP schema and heading; WP-021:
```text
L8:     EV-### (source evidence) / WP-### (work product — NEVER cite as proof)
… [L9–L776 not reproduced here]
L777: ## WP entries — work product (NEVER cite as proof)
… [L778–L1899 not reproduced here]
L1900: - Tag: (U) work product — draft pleading, never cite as proof.
```
- Do-not-use: EV-013 sealed:
```text
L203: - Notes: 2026-08-07 registered. **SEALED — never quote or attach publicly;
L204:   confirm seal status before ANY use.** The 7/28 filing email (WP-001)
L205:   separately instructs: "Please do not attach the prenuptial agreement."
```
- Do-not-use: EV-010 "Never conflate them":
```text
L168: - Notes: 2026-08-07 registered. **WARNING — title collision:** the fourth
L169:   copy's "Exhibit F" title is NOT the "Exhibit F" the court found fabricated
L170:   in EV-003 (that was six emails signed "Lance"). Never conflate them; verify
L171:   exhibit history at source before using the "Exhibit F" title anywhere.
```
- Do-not-use: EV-042 "Not citable as a count until resolved"; C-02 "Plead neither count":
```text
L1039: - Notes: 2026-08-10. ¶9's "five" CONFLICTS with register #25's "four" — see
L1040:   EV-045 and the audit note §7.1. Not citable as a count until resolved.
… [L1041–L1149 not reproduced here]
L1150: paralegal had typed it. Plead neither count until the native emails resolve
```
- Do-not-use: EV-037 [2/2] "DO NOT plead as concealment":
```text
L724:   FL-142. Both are sworn. May be innocent renaming/paydown — DO NOT plead as
L725:   concealment until reconciled at source.
```
- Do-not-use: C-08 "must not be pleaded as EV-079 states them":
```text
L2543: and is now independently verified (EV-091). **The DATES are not confirmed and
L2544: must not be pleaded as EV-079 states them** until the original is obtained
L2545: from Carol Minetree. F-01 family: a checkable date that is wrong costs more
```
- Do-not-use: EV-093 "$4.5 million":
```text
L2733: - **CONSEQUENCE (F-21 family, and larger than 654 days): "$4.5 million" may
L2734:   not be stated as the policy's value in any work product.** It may be quoted
```
- Do-not-use: C-09 "MUST NEVER BE SAID AGAIN":
```text
L2880: **WHAT MUST NEVER BE SAID AGAIN: "the DA never responded."** One reply
```
- Do-not-use: SPEAKER DISCIPLINE / EV-092 attribution:
```text
L2370: out of the speaker column. **No line from this corpus goes to an
L2371: investigator as a named person's words until the side is established from
L2372: the images.**
… [L2373–L2612 not reproduced here]
L2613:   expressly not an attribution. **No line goes to an investigator as a named
L2614:   person's words until the side is fixed from the images or the handset.**
```
- Do-not-use: EV-053 / EV-055 body-read requirements (later satisfied at L1249-1253 / L1286-1291):
```text
L1241:   2026-08-10.** Read and re-register before it is quoted in any filing.
… [L1242–L1280 not reproduced here]
L1281:   decisive noun is cut off. Read the full body before any use.**
```
- Do-not-use: EV-085 provenance caveat:
```text
L2331: - Tag: (V) as to the text extracted this session. **PROVENANCE CAVEAT,
L2332:   MANDATORY ON ANY USE: it is NOT byte- or hash-verified against the 93 MB
L2333:   original (EV-082).** Any evidentiary use either discloses that it is a
L2334:   compressed derivative, or the passage is re-derived from the original.
```
- Do-not-use: 08-27b citation rule:
```text
L3455: (1) cite these eleven by TITLE + message id / hash, never bare id; (2) the
```

## 6. Index-internal contradictions and unreconciled tensions (each with the verbatim lines)

### X1 — "ELEVEN duplicate ids" vs the file's own headers
The 2026-08-27b block counts "137 entry headers over 129 unique ids", which is 8 duplicated ids, but lists ELEVEN. The census finds exactly 8 ids with two entry headers. EV-042, EV-079 and EV-081 each have one header (L1022, L2091, L2209). The other lines that begin with those ids are prose (L1146, L2323, L2540). This file contains no second EV-042, EV-079 or EV-081 entry.
```text
L3448: ## CORRECTION BLOCK — 2026-08-27b · ELEVEN duplicate ids (audit A/C; supersedes the two-id notice above)
L3449: Independent audit measured 137 entry headers over 129 unique ids. The
L3450: following ids each name TWO DIFFERENT documents: **EV-035 · EV-036 · EV-037 ·
L3451: EV-038 · EV-042 · EV-075 · EV-076 · EV-079 · EV-081 · WP-019 · WP-020.**
L1022: EV-042 · Declaration of Respondent in Support of Brief — executed 2026-03-27
… [L1023–L1145 not reproduced here]
L1146: EV-042 ¶9 (sworn) says "at least five separate occasions." Fact register #25
… [L1147–L2090 not reproduced here]
L2091: EV-079 · "Comparison of Shannon Minor's Emails in PDF vs Gmail (July 2022 – August 2023)" — THE DELETION DOCUMENT (delivered to BHPD 10/2/2025)
… [L2092–L2208 not reproduced here]
L2209: EV-081 · "Shannon Text Messages.pdf" — THE TEXT LAYER, 111 MB (highest-value unread artifact in the matter)
… [L2210–L2322 not reproduced here]
L2323: EV-081 STATUS: **UNREAD — no channel available in this runtime can read it.**
… [L2324–L2539 not reproduced here]
L2540: EV-079 dates the Carol Minetree messages **#3 Nov 5, 2022 1:47 PM** and
```

### X2 — the same filed brief and declaration registered three times; EV-107's "sworn twice"
EV-042 records sha256 e22c423b526081bc… (L1035-1036). EV-107 records "sha256 e22c423b5260…" for the same-titled 3/27/2026 declaration (L3270-3271), yet says the five-count is "sworn twice (EV-042 ¶9 + this ¶9)" and calls itself "the second sworn five-count". On disk, the WP-020 [2/2] preserved PDF and the EV-107 mirror both hash to EV-042's full sha256 (§7). Likewise EV-041 (L1015-1016), WP-019 [2/2] and EV-106 (L3254) are one brief. The same filed documents therefore sit both under EV and under the WP heading "NEVER cite as proof" (L777). The descriptions also differ: EV-042 "15pp sworn declaration" (L1023); EV-107 "3-page sworn declaration + Exhibits A/B/C" (L3269).
```text
L1022: EV-042 · Declaration of Respondent in Support of Brief — executed 2026-03-27
L1023: - What: 15pp sworn declaration, executed at Cancún under penalty of perjury.
… [L1024–L1033 not reproduced here]
L1034: - Original: uploads c44bdef5-…_2.pdf and 6accfb51-….pdf — BYTE-IDENTICAL,
L1035:   7,318,891 B each · sha256
L1036:   e22c423b526081bc7f67889871b792880f13cbe7217ac5dd0a6cdd38ea69d451.
… [L1037–L3267 not reproduced here]
L3268: EV-107 · DECLARATION OF RESPONDENT, 3/27/2026 (sworn) — the second sworn five-count, and the bundled-delivery record
L3269: - What: 3-page sworn declaration + Exhibits A/B/C (image-bound), read IN
L3270:   FULL 2026-08-23 (decrypted; AES). Mirror: uploads_2026-08-23/EV-107_… ·
L3271:   sha256 e22c423b5260…
… [L3272–L3282 not reproduced here]
L3283: - **CONSEQUENCE FOR THE COUNT:** the five-request figure is now **sworn
L3284:   twice** (EV-042 ¶9 + this ¶9). The four-vs-five discipline holds — no
L3285:   count pleaded until natives resolve it — but the packet may state "sworn
L3286:   on two occasions as at least five" as exactly that.
L1015: - Original: local upload ef4b2d75-Brief.pdf · 147,896 B · sha256
L1016:   ebdf5204f88e9af20990115707fa4a41ba6e09fd48e22fc6d689924981193815.
… [L1017–L3251 not reproduced here]
L3252: EV-106 · RESPONDENT'S BRIEF, 3/27/2026 — the service brief; the appellate-preservation source
L3253: - What: 5-page filed brief (24STFL00432), read IN FULL 2026-08-23. Mirror:
L3254:   uploads_2026-08-23/EV-106_… · sha256 ebdf5204f88e…
L3012: WP-019 · Respondent's Brief re service/notice, filed ~3/27/2026 (24STFL00432)
… [L3013–L3021 not reproduced here]
L3022: - Preserved: preserved_2026-08-19/WP-019_Respondents_Brief_re_service_
L3023:   2026-03-27.pdf. Tag (U/Q — his filing; court-file conformed copy not
… [L3024–L3035 not reproduced here]
L3036: WP-020 · Declaration of Respondent in support of Brief + Exhibits A-C
… [L3037–L3046 not reproduced here]
L3047: - Preserved: preserved_2026-08-19/WP-020_Declaration_re_Brief_ExA-C_
L3048:   2026-03-27.pdf. Tag (U/Q). Used by: FAMILY (+CIVIL P036-P037 corroboration
L777: ## WP entries — work product (NEVER cite as proof)
```

### X3 — EV-035 [2/2] header date vs its own file stamp
The header says "filed 2026-01-16… (see date below)". The transcribed file stamp reads 1/16/2024. EV-036 [2/2]'s 154-day computation uses 1/16/2024.
```text
L606: EV-035 · FL-100 Petition for Dissolution — Shannon Minor, filed 2026-01-16… (see date below)
… [L607–L608 not reproduced here]
L609: - Key contents (Q, transcribed exactly): file stamp "Electronically FILED by
L610:   Superior Court of California, County of Los Angeles 1/16/2024 9:23 AM David
L611:   W. Slayton, Executive Officer/Clerk of Court, By J. Esplana, Deputy Clerk
L612:   24STFL00432"; "Assigned for all purposes to: Ryan D. White, (Department,
… [L613–L647 not reproduced here]
L648: - Notes: 2026-08-19 registered. COMPUTATION (I, from EV-035 + EV-036): petition
L649:   filed 1/16/2024; preliminary disclosure served 6/18/2024 = 154 days; a
L650:   60-day service requirement would have expired 3/16/2024, making service 94
```

### X4 — "Anna Kralle"
EV-036 [2/2] (registered 2026-08-19, read at source) says the FL-141 was "Declared under penalty of perjury by Anna Kralle". WP-020 [1/2], C-03 and K-08 (2026-08-10) say the surname is unverified. The index never reconciles the two.
```text
L642:   form. Declared under penalty of perjury by Anna Kralle, June 18, 2024.
… [L643–L1114 not reproduced here]
L1115:   "Anna Kralle" surname unverified (only AnnaK@ is (V)); "Matt" vs the
… [L1116–L1155 not reproduced here]
L1156: - **Kept, because they are checkable and he would want them caught:** "Anna
L1157:   Kralle" surname is unverified (only AnnaK@ is (V)); the record shows
… [L1158–L1318 not reproduced here]
L1319: | K-08 | **WP-020 infographic** | IN as his adopted work product (already converted at C-03). | Verify the "Anna Kralle" surname and the 57/43 denominator. | Only AnnaK@ is verified; record shows "Matthew" Sirriyeh. Two checkable fixes, not a verdict. |
```

### X5 — consent to email service
EV-036 [2/2]: "Halsey confirms (U) he consented to service by email". The sworn declaration ¶3 and the brief say he never authorized email service. The index itself calls these reconcilable by scope (L3053-3057), and the POSTURE block records that he "was then required to give up email-service rights".
```text
L653:   RULE is (X) while the two DATES are (V). Halsey confirms (U) he consented
L654:   to service by email, so the email service method is not in dispute.
… [L655–L1011 not reproduced here]
L1012:   was not proper (Mullane/Jones/Peralta); no retroactive validation; no
L1013:   unconsented email as sole formal service. Conclusion ¶4 EXPRESSLY PRESERVES
… [L1014–L1023 not reproduced here]
L1024:   ¶3 no EFS-005-CV / never authorized email service. ¶4 the 2026-02-24
… [L1025–L3037 not reproduced here]
L3038:   ¶3 "I have not filed Judicial Council form EFS-005-CV or any other
L3039:   written consent to electronic service... never affirmatively authorized
L3040:   ... email as formal service of motion papers"; ¶¶4-6 bundled delivery
… [L3041–L3052 not reproduced here]
L3053:   locators). CONSISTENCY FLAG for future filings: Halsey stated in-session
L3054:   2026-08-19 (U) that he "consented to initial service by email ... so we
L3055:   could exchange documents" — reconcilable with ¶3 (scope: informal
L3056:   exchange vs formal e-service, no EFS-005-CV) but every future filing
L3057:   should state the consent scope identically to avoid impeachment.
… [L3058–L3271 not reproduced here]
L3272: - ¶3: no e-service consent ever filed (no EFS-005-CV). ¶¶4-6: the 2/24/2026
… [L3273–L3413 not reproduced here]
L3414: clock" though in Mexico; that he was then required to give up email-service
L3415: rights after the 5-page brief he demanded (EV-106) exposed the problem; and
```

### X6 — State Bar complaint number
EV-046 is a submission receipt dated 2026-04-20 and gives no complaint number. The POSTURE block attaches "complaint no. 24-O-18793 (a 2024-origin number)" to it. The index does not reconcile this. READING_NOTES also holds other readers' notes named D1_statebar-24-O-18793-closing-2024-07-24 and D2_statebar-26-O-13820-closing-2026-05-06; I did not read them.
```text
L1080: EV-046 · California State Bar — submission receipt, 2026-04-20 15:43:57Z
L1081: - What: complaint@calbar.ca.gov → Halsey, "Successful submission of Attorney
L1082:   Misconduct Complaint." Complaint against Lance Spiegel, Bar No. 51625.
L1083: - Original: Gmail msg 19dab900c339a76b.
L1084: - Tag: (V) — INSTITUTIONAL: authenticated by the State Bar's own send, not by
L1085:   Halsey's mailbox (OPERATING_CONDITIONS §7.4).
L1086: - Used by: FAMILY + CIVIL + POLICE (case history only — addendum §3).
L1087: - Notes: 2026-08-10. Filed ONE DAY before the 4/21/2026 hearing.
… [L1088–L3421 not reproduced here]
L3422: §473(d)); EV-046 is the State Bar's 4/20/2026 submission receipt for a
L3423: complaint against Lance Spiegel (Bar No. 51625), **one day before** the
L3424: 4/21/2026 order, complaint no. 24-O-18793 (a 2024-origin number).
```

### X7 — EV-003 tagged before it was read
EV-003 has carried "Tag: (V/Q)" since 2026-08-07. The §7.6 GATE (2026-08-23) says "EV-003 READ IN FULL (first time; 3-page minute order)".
```text
L99: - Tag: (V/Q) — CANON §3.2(3).
… [L100–L3188 not reproduced here]
L3189: **EV-003 READ IN FULL** (first time; 3-page minute order). The order's own
```

### X8 — the 11/11/2022 email
EV-065 (Halsey's adopted 4/17/2026 letter, (U)) says "Spiegel specifically demanded the November 11, 2022 email — the exact email that had been surgically deleted on August 4, 2025". The index records that thread as INTACT live (EV-065 annotation 5; EV-088 DEFECT 1; EV-098) and the 8/4/2025 date as "UNSOURCED at native level". It states "Both facts stand", unreconciled. No document in the index shows where Spiegel made the demand. EV-108 says the §271 motion "contains NO list of Shannon emails".
```text
L1781: 4. DELETION-DATE CLAIM (the causation gap's candidate answer, MASTER FIX
L1782:    PLAN): "Spiegel specifically demanded the November 11, 2022 email — the
L1783:    exact email that had been surgically deleted on August 4, 2025." Also:
L1784:    "Thirty emails from late November 2022, in which Shannon Minor
… [L1785–L1788 not reproduced here]
L1789: 5. **CROSS-VECTOR, RECORDED WITHOUT SMOOTHING (F-02): EV-067 — the
L1790:    11/10-11/2022 WF deposit-hold thread (18461348b9fe0954 /
L1791:    18467dd2c7361b33 family, Shannon's "Yes! Large number has a 10 day
L1792:    hold") — was FOUND LIVE in the mailbox 2026-08-12** by this thread's
L1793:    search. The adopted 4/17/26 claim says "the November 11, 2022 email"
L1794:    was deleted 8/4/2025. Both facts stand. Possible reconciliations (all
L1795:    untested): different 11/11/22 message (his 1/8/26 email to Kale calls
L1796:    it the email "confirming receipt of the tax refund"); restoration;
L1797:    thread-vs-message deletion. TEST: identify from Spiegel's motion +
… [L1798–L1959 not reproduced here]
L1960:   preservable" hedge). Complaint3's specific "August 4, 2025" deletion
L1961:   date remains UNSOURCED at native level — test owed.
… [L1962–L2470 not reproduced here]
L2471: - **DEFECT 1 — Exhibit A asserts a deletion that did not occur.** It states
L2472:   the 11/11/2022 "Yes! Large number has a 10 day hold" email is "DELETED
L2473:   (Surgically removed from server)." **Tested live 2026-08-12: thread
L2474:   `18461348b9fe0954` is INTACT, all five messages** — `18461348b9fe0954`,
L2475:   `18467dbd3ea6fa47`, `18467dd2c7361b33`, `1846822a40fdff6d`,
L2476:   `1846823e63d233ca`. It is also the basis of EV-067. Innocent readings
… [L2477–L2926 not reproduced here]
L2927: - **WHAT THE DISPUTE WAS ABOUT** (`19c27f6dc533be58`, 2/4/2026, Q): "I am
L2928:   specifically talking about the **November 11, 2022 email confirming receipt
L2929:   of the tax refund**" — **the exact email EV-088's Exhibit A calls
L2930:   "surgically removed," and which is PRESENT in the live account today.**
… [L2931–L3349 not reproduced here]
L3350: (`19b9f646568c79a0`): "the critical tax-refund email was **surgically
L3351: removed from my account after I gave it to you**, not that it never
L3352: existed." The Wells Fargo thread is PRESENT live today (30_ §4) — the
L3353: recovered/restored question (D-P1) is now dated to a live dispute window.
… [L3354–L3389 not reproduced here]
L3390: - **CONSEQUENCE 2 — THE PLANNED "LANCE-MOTION OVERLAP TABLE" HAD A FALSE
L3391:   PREMISE AND IS REPLACED.** This motion challenges the Spiegel log only —
L3392:   it contains NO list of Shannon emails. The documentable overlap is
```

### X9 — "do not plead" wording after its withdrawal
The CONVERSION BLOCK (2026-08-10) withdraws such wording "wherever they appear". Later entries use it again: EV-037 [2/2] (2026-08-19), C-08 (2026-08-12), EV-107 (2026-08-23). C-02, written the same day, also uses it.
```text
L1303: Governed by OPERATING_CONDITIONS §10. Everywhere in this repo I wrote "do not
L1304: plead," "not pleadable," "fenced," "gated," or "does not go in this packet,"
L1305: **that was a submission ruling I had no standing to make.** Those words are
L1306: withdrawn wherever they appear. The items below are IN THE RECORD. Each carries
L724:   FL-142. Both are sworn. May be innocent renaming/paydown — DO NOT plead as
L725:   concealment until reconciled at source.
… [L726–L1149 not reproduced here]
L1150: paralegal had typed it. Plead neither count until the native emails resolve
… [L1151–L2542 not reproduced here]
L2543: and is now independently verified (EV-091). **The DATES are not confirmed and
L2544: must not be pleaded as EV-079 states them** until the original is obtained
… [L2545–L3283 not reproduced here]
L3284:   twice** (EV-042 ¶9 + this ¶9). The four-vs-five discipline holds — no
L3285:   count pleaded until natives resolve it — but the packet may state "sworn
```

### X10 — observation, not cross-referenced: EV-011 and EV-100
Both PDFs are recorded at 296,498 B under different Drive ids. The index does not link them. Extraction character counts differ (93,802 vs 97,288).
```text
L175: - Original: Drive 1Ddy18LylKHbe5gjkeIhzFIOVOVhKAJUO · 296,498 B · 2026-06-12.
… [L176–L2139 not reproduced here]
L2140: Extraction of EV-011 ("POLICE REPORT — Analysis of Evidence, Aug 2025
L2141: update", Drive 1Ddy18LylKHbe5gjkeIhzFIOVOVhKAJUO, read in full 2026-08-12,
L2142: 93,802 chars) found **four passages formatted as direct quotations of
… [L2143–L3080 not reproduced here]
L3081: - What: "POLICE REPORT_Revised Analysis of Evidence Supporting Allegations
L3082:   in the Minor Case (Updated with August 2025 Evidence)" — Drive
L3083:   `1LmPSjyZPuFJSmW-GJRBFm5zWd2hnaQq3` (PDF 296,498 B; DOCX
L3084:   `1T_GpQaUJIsnbb1aPGpAL_xsHOstJcstt`; three byte-identical PDF copies, no
L3085:   version conflict). **READ 100% 2026-08-23** (97,288 chars).
```

Resolved inside the index, recorded for completeness:
- The four-vs-five preservation-request conflict: C-02 → EV-054 → K-06 → Kale chronology item 1 → D-1 "The asserted preservation-demand count is FIVE" (L1145-1151, L1267-1273, L1317, L3298-3306, L3436-3441).
- EV-036 [1/2] page count: C-10 corrects "24-page" to 54 (L3061-3068).
- EV-056 page count: corrected from 68 to 34 (L1466-1468).

## 7. Reader's checks outside the index (factual; read-only)

1. sha256 of the duplicate-registered files (computed now):
```text
ebdf5204f88e9af20990115707fa4a41ba6e09fd48e22fc6d689924981193815    147,896 B  WP-019 [2/2] preserved copy  governance/evidence/preserved_2026-08-19/WP-019_Respondents_Brief_re_service_2026-03-27.pdf
ebdf5204f88e9af20990115707fa4a41ba6e09fd48e22fc6d689924981193815    147,896 B  EV-106 mirror  governance/matters/04_criminal_bhpd_2025-14983/report_2026-08/uploads_2026-08-23/EV-106_Respondents_Brief_2026-03-27.pdf
e22c423b526081bc7f67889871b792880f13cbe7217ac5dd0a6cdd38ea69d451  7,318,891 B  WP-020 [2/2] preserved copy  governance/evidence/preserved_2026-08-19/WP-020_Declaration_re_Brief_ExA-C_2026-03-27.pdf
e22c423b526081bc7f67889871b792880f13cbe7217ac5dd0a6cdd38ea69d451  7,318,891 B  EV-107 mirror  governance/matters/04_criminal_bhpd_2025-14983/report_2026-08/uploads_2026-08-23/EV-107_Declaration_Re_Brief_with_Exhibits_2026-03-27.pdf
e34ed12bbb633354fe3490b8d868f60ecbd3fd84addfb862050cbe1997cda46d  4,299,446 B  EV-023 preserved copy  governance/evidence/preserved_2026-08-19/EV-023_vanguard_2024_full_year.pdf
e34ed12bbb633354fe3490b8d868f60ecbd3fd84addfb862050cbe1997cda46d  4,299,446 B  EV-033 preserved copy  governance/evidence/preserved_2026-08-19/EV-033_vanguard_529_annual_2024.pdf
```
   EV-041's recorded sha256 (L1015-1016) is ebdf5204f88e9af20990115707fa4a41ba6e09fd48e22fc6d689924981193815. EV-042's (L1035-1036) is e22c423b526081bc7f67889871b792880f13cbe7217ac5dd0a6cdd38ea69d451.

2. governance/evidence/preserved_2026-08-19/ contents vs the entries' recorded byte sizes (listing only; PDFs not opened; MANIFEST.md not read):
```text
  176,163 B  EV-001_minute_order_4-21-2026_quash.pdf  — matches entry size
  103,267 B  EV-002_minute_order_4-21-2026_service.pdf  — matches entry size
  107,381 B  EV-003_minute_order_4-21-2026_271.pdf  — matches entry size
   92,864 B  EV-004_minute_order_4-21-2026_RFO.pdf  — matches entry size
   94,262 B  EV-005_minute_order_3-2-2026.pdf  — matches entry size
  212,698 B  EV-014_hidden_vanguard_2024.pdf  — matches entry size
  171,655 B  EV-015_vanguard_2015_transfer_titled.pdf  — matches entry size
1,514,921 B  EV-018_notice_to_consumer_WF_subpoena.pdf  — matches entry size
  871,049 B  EV-019_SUBP-025_wells_fargo.pdf  — matches entry size
4,069,611 B  EV-020_RFO_400k_vanguard_2025-12-29.pdf  — matches entry size
  237,485 B  EV-021_vanguard_2024-03-31_statement.pdf  — matches entry size
4,299,446 B  EV-023_vanguard_2024_full_year.pdf  — matches entry size
  302,873 B  EV-024_exhibit_B_WF_x2218.pdf  — matches entry size
  339,090 B  EV-025_exhibit_C_WF_x0890.pdf  — matches entry size
1,385,626 B  EV-026_WF_x2218_2022.pdf  — matches entry size
  216,360 B  EV-027_WF_x2218_2022-12_2023-02.pdf  — matches entry size
2,872,554 B  EV-029_vanguard_529_annual_2020.pdf  — matches entry size
2,800,902 B  EV-030_vanguard_529_annual_2021.pdf  — matches entry size
3,260,191 B  EV-031_vanguard_529_annual_2022.pdf  — matches entry size
4,216,049 B  EV-032_vanguard_529_annual_2023.pdf  — matches entry size
4,299,446 B  EV-033_vanguard_529_annual_2024.pdf  — matches entry size
  506,941 B  EV-035_FL-100_petition_filed_1-16-2024.pdf  — matches entry size [second assignment (FL-100)]
  207,592 B  EV-036_FL-141_P_disclosure_service_6-18-2024.pdf  — matches entry size [second assignment (FL-141)]
4,231,887 B  EV-037_P_FL-142_SAD_2025-02-24.pdf  — matches entry size [second assignment (FL-142)]
  191,561 B  EV-038_LASC_case_summary_26STCV25125_printed_2026-08-18.pdf  — matches entry size [second assignment (LASC register)]
    6,863 B  MANIFEST.md  — not read
  332,582 B  P_FL-144_waiver_FDD_8-22-2024.pdf  — NO entry in EVIDENCE_INDEX.md
  750,129 B  P_FL-150_income_expense_1-8-2025.pdf  — NO entry in EVIDENCE_INDEX.md
2,428,682 B  R_FL-142_SAD_2-7-2025.pdf  — NO entry in EVIDENCE_INDEX.md
  147,896 B  WP-019_Respondents_Brief_re_service_2026-03-27.pdf  — matches entry size [second assignment; size = EV-041]
7,318,891 B  WP-020_Declaration_re_Brief_ExA-C_2026-03-27.pdf  — matches entry size [second assignment; size = EV-042]
```
   The files for colliding ids are named by the second assignment, as L3452-3454 states. Three preserved PDFs whose file names name disclosure forms have no index entry: P_FL-144_waiver_FDD_8-22-2024.pdf, P_FL-150_income_expense_1-8-2025.pdf and R_FL-142_SAD_2-7-2025.pdf. I did not open them.

3. The map /home/user/spiegel-thread/INVENTORY/ev_index_extract.tsv (137 rows) agrees with the census on every id and header line. Its dates were not relied on (see §1).

--- end of notes ---
