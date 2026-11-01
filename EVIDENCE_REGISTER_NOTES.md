# EVIDENCE_REGISTER — notes (Spiegel thread, charter step 1)

Built 2026-11-01 by a subagent under INVENTORY/AGENT_RULES.md (read-only everywhere; only this file and EVIDENCE_REGISTER.tsv written; no git; scripts in the session scratchpad `reg/`, run with `python3 -I`). No Gmail or Drive call was made for this step: the register is built only from INVENTORY/ and READING_NOTES/, plus a read-only `ls` of the tracker's `preserved_2026-08-19/` and `uploads_2026-08-23/` folders to confirm the paths exist.

## 1. Row counts

**Total rows: 2,815** (SP-0001 … SP-2815). They are sorted by date, then pointer. Rows with date `unknown` (2,056) sort last.

| class | rows |
|---|---|
| WORK-PRODUCT | 836 |
| CORRESPONDENCE | 738 |
| COURT | 565 |
| SWORN | 383 |
| AI-LEAD | 133 |
| ACCOUNT | 86 |
| DUPLICATE | 74 |

| source (pointer prefix) | rows | of which |
|---|---|---|
| drive: | 2,194 | 2,004 title-match inventory rows; 116 inventory rows that READING_NOTES cite (no title match); 74 ids named in READING_NOTES that drive_inventory.tsv lacks |
| gmail: | 550 | 211 gmail_inventory.tsv rows (all included); 339 ids named in READING_NOTES that the inventory lacks |
| tracker: (@6f5d8b0) | 64 | 30 preserved_2026-08-19 files (28 EV/WP-named PDFs + P_FL-144, P_FL-150, R_FL-142; MANIFEST.md not included); 15 tracker files READING_NOTES read (incl. EVIDENCE_INDEX.md); 12 EV pointers to report_2026-08 uploads/extractions, preserved uploads and Complaint3; 7 extra EV rows on shared fallback pointers |
| finthread: (@63d0aee) | 6 | Brief and Declaration of 3/27/2026 (the Declaration pointer carries 4 rows: EV-042 and its Exhibits A–C = EV-043/044/045); Ally ECR file |
| courtlistener: | 1 | Jolie v. Superior Court, opinion 4706097 (context only) |
| ghpages: | 0 | no READING_NOTES file reads a ghpages file |

read_status: metadata-only 2,291 · not-read 394 · full 112 · partial 18.

EV/WP rows: 270 rows carry an EV-/WP- id, and they cover all 137 entries of the index (137 primary rows plus 133 set members, copies and preserved mirrors). By class: CORRESPONDENCE 121, DUPLICATE 49, WORK-PRODUCT 45, ACCOUNT 29, COURT 12, AI-LEAD 9, SWORN 5.

## 2. How each source was merged

Rows are merged on the pointer: one row per Drive id, Gmail message id or repository file. The only exceptions are three pointers that several EV entries share and that have no pointer of their own: `tracker:governance/evidence/EVIDENCE_INDEX.md` (WP-018, WP-020[1], EV-056, EV-057, EV-086, EV-089, plus the index's own row), the finthread Declaration (EV-042 to EV-045), and `39e87acb-First_50_Pages.pdf` (EV-036[1] and EV-103, p.52). The sources were applied in the order below. A later source never overwrites an earlier row; it only adds rows.

1. **EVIDENCE_INDEX (137 entries).** Class and tags come from READING_NOTES/EVIDENCE_INDEX.notes.md §2. ev_index_extract.tsv was used only to confirm ids and lines; its dates are mechanical and wrong for several rows (per the notes §1), so they were not used. Each entry's primary pointer became the EV row. Other ids that the entry names became rows with the same EV-id:
   - set members (for example the six EV-054 demands, and the EV-066 ids at index L1590–1616);
   - copies and variants;
   - the preserved_2026-08-19 and uploads_2026-08-23 mirrors.
   Ids used for two documents are written EV-xxx[1] / EV-xxx[2].
2. **READING_NOTES annotations.** Every notes file was read (list in §6). Documents that a notes file read, or that it describes with pointer and date, received hand-entered date, type, class, read_status and note. That annotation table is in the scratchpad file `reg/ann.py`.
3. **gmail_inventory.tsv (211 rows).** All rows are included as metadata-only unless a notes file read the message. Tags come from the search_bucket (C → d-eservice-consent, D → statebar, F → g-ally, G → c-service-dates) plus subject keywords. The 26 messages in the inventory's AI-LEAD name appendix are classed AI-LEAD (carrier email with AI-named attachments). gmail_work_rows.psv is the source of the TSV and was not used separately.
4. **Gmail ids named in READING_NOTES but not in the inventory (339).** A mechanical scan of all notes files found every 16-hex id beginning with "1". sha256 prefixes (those preceded by "sha256" or followed by "…") were excluded. For these ids:
   - **date** is decoded from the Gmail id (id >> 20 = internalDate in ms). The decode was checked against all 211 inventory rows: 211/211 give the same date, with a maximum error of 3 minutes.
   - **thread** is taken from the notes when they state it, else the id itself when the notes call it a thread, else `thread:unknown` (291 rows).
5. **Drive ids named in READING_NOTES.** Every 33- or 44-character Drive id in the notes was included; folders were excluded (§3). Ids that are in the inventory carry its title and size in the note.
6. **drive_inventory.tsv title matches.** These are rows whose matched_terms contains "(title)": 2,076 rows, minus 72 folders = 2,004. drive_inventory.tsv (17,617 rows) is cited here once; its other 15,541 rows stay in the inventory file.
7. **repo_file_index.tsv / ai_lead_marks.tsv.** Only the files that READING_NOTES report as read are included: EVIDENCE_INDEX.md, JURISDICTION_SPLIT, the 2026-08-10 audit note, SERVICE_VIOLATIONS_LOG, KNOWN_FALSE, CANON, 85_POLICE_REPORT_V3 (partial), 81, 81B, 81C, 63K, qa_Q61, ex_23, 24c (window only) and R7. The preserved PDFs are also included. Of the 23 ai_lead_marks rows, only 81/81B/81C were read; the other 20 (FOR_GEMINI etc.) are excluded as unread.

**Provisional fields.** Class and type for rows known only from inventory metadata (2,004 Drive title rows and the uncited Gmail rows) were assigned by title or subject keyword. Every such row's note says "class provisional from title". Drive titles with an AI token (Gemini, ChatGPT, Perplexity, Claude, standalone "AI", or the inventory's `AI?` flag) are classed AI-LEAD. Tags for rows outside the index were assigned by keyword over the subject, the title or the citing notes line. They are leads only. Date is `unknown` for inventory-only Drive rows, because Drive created/modified times are metadata, not document dates. Those times are kept in the note.

## 3. Excluded, and why

- drive_inventory rows without a title match (15,541): out of scope by the brief.
- Drive folders: the 72 title-match folder rows, and 10 folder ids named in the notes (parents/containers: 15Kwe3SX…, 17Z_tsPI…, 1Fm9plSU… (EV-087 folder), 1Jh7n2wn…, 1KwJxA9X…, 1SG9KoZg… (02_1983_Federal), 1UvJnv1p…, 1_vuyupR…, 1bd3UymI… (PDD parent), 1f-lBbjO…). Folders are containers, not documents. Exception: the EV-092 folder 1-14wNOU… is kept because it is that entry's own pointer (the screenshot corpus).
- repo_file_index files not reported read (about 1,800) and the 20 unread ai_lead_marks files.
- preserved_2026-08-19/MANIFEST.md: not a PDF, and no notes file read it.
- Truncated ids (for example "1Ey5As…" in EV-085, "190c2fad…") cannot be resolved. The entry points to the file that holds the full id.
- Web URLs (EV-057): this pointer type is not allowed, so the row points to the index entry.
- Session uploads that are not in the tracker (EV-056 6c56814d-…, EV-041/042 upload names): these rows point to the index entry or to the byte-identical finthread copy.

## 4. Ids that READING_NOTES name but the inventories lack (added as rows)

Drive (74; includes EV primaries, gdoc work product, Log A/B copies and docket copies):
1-14wNOUvTP5lQeLyFSIa9yZn4DGsXWp_ (SP-0072), 1-_ZUF3r-ivGnBBRwbzjxL8xzhPxp4h-O (SP-0049), 10T2418e4-r1St53ICmK-AQonibheJ2ZQ (SP-0812), 10rXdbzCB6x7KqQzeAerZ0408oyCtevkT (SP-0027), 11kdVWKj8IkOxLZ3FKdqJtfj6Ygapsqib (SP-0855), 122PTqRytZElsaDS2Ffr2KA0lfoHATlNa (SP-0861), 12SxdmRCBLqaRI0wDhZLbZnmVIcJuB7zv (SP-0030), 13A21iC1ltJN27HExxsNZlKJoXlZxZjvz186aomuyLKA (SP-0899), 13BwkvjbX10Wov2Idv7ICZV9SJN6Lbh50 (SP-0900), 141G5x_ygVrXIn-sUss_C-RdUDTkyEbK1 (SP-0925), 145TAxmAcIYrv__MA3EwtM_Rx0cMafHr1 (SP-0927), 15d5x6yrAHvjV45-H2wzlAVNGELpJemZf (SP-0978), 16Xiho9OW-ozxRecJkwhULmjpxg1DmV0Q (SP-1007), 17FS72fsZrTWBpxxXlOrIb_1wzRRlPRUJ (SP-0407), 19WT4QY6R-rKtvIOZsPTMgg7SSk5jQmCm (SP-1117), 1B9rS4E1aTbsjggV8sHO2f0c_7_vXTWvn (SP-0031), 1CuG6-SmmKcATPmM5x-PPhmpB0CDoj19T (SP-1221), 1DLVF3_tUYSbV41yx0Rk33jfzFuzaGEJN (SP-0032), 1DMhc03gb_OjUcC1h_cCQsjPlvzazPkhb (SP-1243), 1Ddy18LylKHbe5gjkeIhzFIOVOVhKAJUO (SP-0283), 1FjwZbbMWwuekd_ZSG77Dk_aQIPWIOfx0 (SP-1330), 1Hy03H8S7DW4FdodqeL1YGDdvh8HrOSGJ (SP-1392), 1IUm-tR81jO1d788zlS80MbuBGxXm4eHp (SP-1410), 1K5akFNK4ptlGF5N1dZP1haphrg8gwFas (SP-1458), 1LmPSjyZPuFJSmW-GJRBFm5zWd2hnaQq3 (SP-0306), 1MG5Xo-1oH33WBC3RPK2OL1KNclpnoqRy (SP-0013), 1MZr2sx6VzT9q83WqQ4kBHIBJwjd5kLyB (SP-1539), 1O-UUiIrylrXMwrI1r8-uGUmHPs3JqUQfj4-Cd_nIbJc (SP-0353), 1QDkSmtZjLFsoy5Zfcji6JjDp3inAbSNr (SP-1680), 1Qh_j4v89d2lTNUyNWzXiICxZiq6kHkWX (SP-0084), 1T_GpQaUJIsnbb1aPGpAL_xsHOstJcstt (SP-0307), 1V8i9ngoS0kh_7vwkyWaIRcSgSHX70hyO (SP-1840), 1VZUQTA965ni8Aw9PfMpsKX8rVoXXJjEN (SP-0047), 1WNXPVaKd9af-RYUSdgWMnoxDLjx7rFKi (SP-0085), 1WmYmVlTYAv7A41-HNoOGs2BrOA3arW3x (SP-1892), 1Xe-KTA3Na23U-l39oApG5ovX0jmCj_LV (SP-1917), 1YHM3akoW5NJcIkTcvPbBZlbRBYewI3Vr (SP-0086), 1ZyoLwf0fYnhRqSRomb3xq8CfXCSndfTv (SP-1997), 1_MveRC1mZ48LVx0Ae1VM4spLmVX8mFDv (SP-0053), 1_T2eOacZZNGi9qLfpVRn1zS0AJO8wj-x (SP-2012), 1a_iab_mBLny5vBE7qp58Q7kUat-HBgwR (SP-0061), 1bgsyCEf6kPFhveHvofuiHWNuA6r3geRA (SP-2079), 1cgualz4h8Fl2XhZuu0_ZVE4CjkT5nO0s (SP-0017), 1eVzUSmidiAabnO4raxu-yjGekfubrgiy (SP-2177), 1ed4vTjCji-rAlLMeiJf50-hDv1w0bHU_ (SP-0146), 1egJWcqn6XIIYOeZm7qp6WOGp3OyBJfH3 (SP-0062), 1eqvC2WTxZ_Z8KQkhJE6MMy9D--V98D2K (SP-0103), 1f1OV8FKxh8dbEIeDiEiyey6NzdkSP0I8 (SP-0104), 1gtK4-agu-Hj21P4TJLdwVccEyLiZ_ugL9Y_B7rjepHM (SP-0356), 1hdLvGPCBW1TxCjegaRuuQPq294PKMeJk (SP-0033), 1ikRSLdaUWGE05M003ixxExDZsW5dJqiY (SP-2297), 1jC10sbsKieuCP3mVaf9hv_AeCLb55rFj (SP-0110), 1jTdwcazhviJh95KBe1b36HX_cxhzntsr (SP-2322), 1kMQuWDQQ6klQhkpV3Ii7uC7pRpZNMngD (SP-0111), 1kPdz46RjYa47ES98POCRIygREl3v4vwI (SP-0409), 1kwP2WiUSOmoznNn_NjBxh7PjRFvoyLSA (SP-0051), 1lYhOFHXU9jbKBg_GVw_Jp7aFctaBf-o0 (SP-0034), 1lpWcvv4NhcPJXclzwxzFXgxHgKka4CFV (SP-0035), 1mgU2f2IZ3u_w8gzBf8nbQCptChsWFxnn (SP-2414), 1q_E3uqoQbVX8jVI-HTTRO6fXiJDjL0HP (SP-0105), 1rVCoLHWU1sOyXFuGBQTxDx37r-BgE_KXo1_kJHCd_40 (SP-0720), 1roVJs1Nhe_xUrDKXlVhdyTxCVrMpP9wg (SP-0106), 1rxYrESga2z2oeLR79GePFLOTJ7Un7urD (SP-0159), 1sDRZlPggoZ8IC9L85mZzDEZ7ybuEHvWB (SP-2584), 1sneI6QWCf7lBdJgC3KFaYu5PbsG6LGo0 (SP-0087), 1u5ZTi3uThH29M2U_nItrETnlY52cTruF (SP-2634), 1ubyf17qgYs3jpkA3v63E54zMO9HVA-EH (SP-2651), 1w1gArcnH5dypLx30ZKDozQm4yKuSpgP3eJYs6Hv8Fjk (SP-2687), 1wwlhsowkt1LQ6uUYpOTOYOBeHP4SW0mn (SP-0240), 1xAoNlSBE6q7PS1psMwT41NkMxnHi1Pic (SP-2721), 1xBEtBvzIq26wLxd-ZPcM9IavN1lAzED- (SP-0019), 1yz3o0NMDLydn_hXJz7n0enIzsHIZrQep (SP-0025), 1z3-T6RZE0ZNNUOsV8tiq6R9ElWUrriwd (SP-2767), 1zyk-4TL5iK6j4AmCbIAY7HgtsTw-XP6g (SP-0186)

Gmail (339; date decoded from id; thread often unknown):
1102e3c6199d0c39 (SP-0001), 1105784ee37d061d (SP-0002), 1107a58d57f8792d (SP-0003), 11114c6272f39a5f (SP-0004), 16413f42f96f7208 (SP-0015), 168d01b29ecf5f6b (SP-0016), 176f77bf10ac898f (SP-0021), 176f7864666df364 (SP-0022), 176f809da80fb8be (SP-0023), 1833ca16271d09ea (SP-0029), 18439a5eabf63be3 (SP-0036), 18444ef3ac32ccd3 (SP-0037), 1844d84b3e8e369f (SP-0038), 1844da95b9cb8766 (SP-0039), 1844df7371df95ec (SP-0040), 18454b35eacde372 (SP-0041), 18461348b9fe0954 (SP-0042), 18467dbd3ea6fa47 (SP-0043), 18467dd2c7361b33 (SP-0044), 1846822a40fdff6d (SP-0045), 1846823e63d233ca (SP-0046), 1850da4e115dbb45 (SP-0050), 185ea400074e635b (SP-0055), 1875c1bbb2ae4c3e (SP-0056), 1875c1ebdd8719d1 (SP-0057), 1875ccc96ec41402 (SP-0058), 1875dbd27a787aa9 (SP-0059), 1875e230f7dc3a88 (SP-0060), 189309251612ecb6 (SP-0063), 18930a9aa534c917 (SP-0064), 189312a78f6dc42c (SP-0065), 1894190f98311064 (SP-0066), 18942a1f414a6c66 (SP-0067), 18942a8d7a9560e1 (SP-0068), 189ff8e8aaeb0f47 (SP-0070), 189ffbe65b4fdf4d (SP-0071), 18a70d512865b590 (SP-0074), 18a79cb99e316376 (SP-0075), 18b1891454bc580d (SP-0078), 18b514edd2a06abe (SP-0079), 18bed8e4a4bb39c1 (SP-0080), 18bed8e4a8de5817 (SP-0081), 18bed8e553245b27 (SP-0082), 18c15583f81d5464 (SP-0083), 18cf64db45243ba9 (SP-0091), 18d13fab671da237 (SP-0094), 18d424f91222fab9 (SP-0096), 18d617333d82df9a (SP-0097), 18d64fbeb13f840e (SP-0098), 18d6598e61e8abf0 (SP-0099), 18d659c74c96f2f5 (SP-0100), 18d65a9dad2be7d3 (SP-0101), 18da4c2fe5eb3cd1 (SP-0102), 18ea11c7a1b64cd0 (SP-0108), 18ea161400dbc944 (SP-0109), 18fcbf751a4a00ae (SP-0112), 18fdf4915ea20042 (SP-0113), 18fe55caf6501974 (SP-0114), 1901d53bbcd4ab2f (SP-0115), 190329e29a9a186c (SP-0126), 190455b73e341d60 (SP-0127), 1904c5418f9e531b (SP-0128), 1904c5f9feddc769 (SP-0129), 1906e73405df236f (SP-0132), 1906e98d087775db (SP-0133), 1906f138d21142f0 (SP-0134), 19070da5c8ce171b (SP-0135), 19074db16ceb6a53 (SP-0136), 19094f2ef58d7950 (SP-0137), 190ae3d99538d18c (SP-0138), 190ae8b6b2ad2499 (SP-0139), 190c2fad1c4fd49a (SP-0140), 190c322ff4021189 (SP-0141), 190c83dfe9cb7fd1 (SP-0142), 190cbaf290e12a0f (SP-0143), 190dcf708ca9607b (SP-0144), 190e0eee763559a9 (SP-0145), 190e4dfe9a2c2743 (SP-0148), 190e656108df1d8f (SP-0150), 19123d4be19e2d44 (SP-0155), 19157ba8e41220f7 (SP-0157), 1915be1eb053053e (SP-0158), 1917bf993cc8b2d8 (SP-0160), 1928cd256a4b5bde (SP-0162), 1928d461b755d173 (SP-0163), 192aba5b76e8cd03 (SP-0164), 192e4eb48f4671cf (SP-0180), 192e4f2f43647e39 (SP-0181), 192e51c99e3757de (SP-0183), 192e52ae0b36ccc4 (SP-0184), 19340b0eb2056651 (SP-0185), 194482330a95baa0 (SP-0188), 195f3970ee2df184 (SP-0207), 195fe9941e06c382 (SP-0208), 19611abc648f91a8 (SP-0209), 19611bdcfde5c78f (SP-0210), 19625f47de243ed8 (SP-0211), 196f8888b82a1183 (SP-0246), 1973c9cdeeb8a442 (SP-0255), 1977c51ddad08b0a (SP-0261), 1979db6b2125390b (SP-0262), 1979e246622738f5 (SP-0263), 1979e2946a3346f0 (SP-0264), 1979e2cd049f87a2 (SP-0265), 1979e2dcb382217d (SP-0266), 1979e30e22e4ae99 (SP-0267), 1979e7813a178045 (SP-0269), 197a2dc47ddd607c (SP-0271), 197a3724d248ab44 (SP-0272), 197ef5895435e31b (SP-0273), 197ef5eeb73a5be8 (SP-0274), 197f0190d0a820ec (SP-0275), 1980a06eb3177ce9 (SP-0276), 1980aad41bcc7b22 (SP-0277), 1980ab73fbfe94e7 (SP-0278), 19814f71e34d448e (SP-0279), 1983aeaaaf2f91a4 (SP-0280), 1983aec0ff36fac3 (SP-0281), 1984fd6ec53551c4 (SP-0282), 198717bc1e84199f (SP-0284), 198768bdcb030829 (SP-0287), 198773659236b416 (SP-0288), 19877f1fad1c4529 (SP-0291), 1987c30b472820da (SP-0292), 1987c51a21963f01 (SP-0295), 1987c696a2db031e (SP-0296), 19881ad39b42a700 (SP-0297), 19881b493805982e (SP-0298), 198858d3a85cd7ea (SP-0299), 1989a0b964394e79 (SP-0300), 198d2853d2dd6410 (SP-0302), 198e338062a3bb85 (SP-0303), 198e7213c97e482c (SP-0304), 198f1708b4eb9340 (SP-0305), 198f6f253f2a7e0a (SP-0308), 1992ff3853ff8100 (SP-0310), 1992fffec95f776b (SP-0311), 1997a6491cd669da (SP-0326), 1998c027ef83cc88 (SP-0327), 19997c42bd4b9c64 (SP-0328), 1999df6b5ce0fbce (SP-0329), 199a442bb459fce9 (SP-0330), 199c5cbc967a9010 (SP-0331), 199c5dc7db16c037 (SP-0332), 199db7e78dd8b1de (SP-0333), 199e40b0c7a5927e (SP-0334), 199e45bc07381dc6 (SP-0335), 199e45d488541702 (SP-0336), 199ec75f75e16cd7 (SP-0337), 199ec76298c0a6ff (SP-0338), 19a0369c2de9fe45 (SP-0339), 19a09e899cab9e7c (SP-0341), 19a0d16829b0084f (SP-0342), 19a134f34cb9ada9 (SP-0343), 19a13eb82bb6d8fd (SP-0344), 19a14b7ed8e70c23 (SP-0345), 19a1c2b3c5b50a06 (SP-0346), 19a275d457ec3591 (SP-0347), 19a276eb2382abe7 (SP-0348), 19a285a5f64bb0cb (SP-0349), 19a2b9aee561a4c4 (SP-0350), 19a2ba87ce5e12d9 (SP-0351), 19a2d8a2eedbbea8 (SP-0352), 19a3715f9d26dd92 (SP-0357), 19a3c147879af74a (SP-0360), 19a3c510e55270e0 (SP-0361), 19a3c79d00dc46e7 (SP-0362), 19a3c80ea4f494ad (SP-0363), 19a4237b1d2e2fae (SP-0365), 19a42915823eea6d (SP-0366), 19a46f5cb3cf5acf (SP-0367), 19a4cb0a7fd791b2 (SP-0368), 19a53fea7063415c (SP-0369), 19a5620d5a054560 (SP-0370), 19a84d3d95de6534 (SP-0372), 19a89ddcc887bba2 (SP-0373), 19ab753ad35b7d52 (SP-0374), 19ab8474aa899682 (SP-0375), 19ab9f8d6778e159 (SP-0376), 19ae64fb3079084e (SP-0377), 19ae68bf08204bd5 (SP-0378), 19af06ba182f7aa6 (SP-0379), 19af167fed51179c (SP-0380), 19b0eaf3f049d381 (SP-0381), 19b5cbba04495f7b (SP-0383), 19b5d9d769d3fea9 (SP-0384), 19b6cc55639bdc93 (SP-0398), 19b6fc619f4bafef (SP-0399), 19b70bba0694f1d9 (SP-0400), 19b8f1dd4d7a670c (SP-0433), 19b8f6fcd6f82d0b (SP-0434), 19b8fbc478f4e54b (SP-0435), 19b8fc6fabdac16f (SP-0436), 19b90daa5f6a5300 (SP-0440), 19b9f2badaeb5eeb (SP-0449), 19b9f2e529d79fbc (SP-0450), 19b9f646568c79a0 (SP-0453), 19ba02a9c00c3b61 (SP-0459), 19ba60583051da79 (SP-0464), 19ba8ab4ac49e9ab (SP-0465), 19bb307ee4795b75 (SP-0468), 19bb3ad9899c0a6d (SP-0470), 19bbd7a38e011667 (SP-0482), 19be2c2fa4b8f5b3 (SP-0486), 19be3bbd3fa862b8 (SP-0487), 19be735cadc9e828 (SP-0489), 19c0338466026974 (SP-0492), 19c036b7d786e9b7 (SP-0493), 19c102e73a5cbca7 (SP-0494), 19c11524cb39dfe1 (SP-0495), 19c20c6b957e80c5 (SP-0497), 19c27f6dc533be58 (SP-0498), 19c2e62e339d6e4f (SP-0504), 19c31c2994519631 (SP-0505), 19c43efcecf77097 (SP-0508), 19c498713648d147 (SP-0509), 19c4f9dc9d26b93f (SP-0510), 19c5176a7213b8cc (SP-0511), 19c53b539239a231 (SP-0512), 19c5435095e084b7 (SP-0513), 19c548a31edc8c3d (SP-0514), 19c55a8607a774c5 (SP-0515), 19c55c4a64f0391e (SP-0516), 19c6e65078799f95 (SP-0523), 19c6e667b7ba8a4a (SP-0524), 19c6e8c40f8e9c2e (SP-0525), 19c7237c8e283d5a (SP-0526), 19c8c7743a00925a (SP-0529), 19c8ca6230be2d9a (SP-0530), 19c8ce40d7913f4b (SP-0531), 19c90cf4d4c1f5ae (SP-0533), 19c9262bb219c577 (SP-0538), 19c9504bcff60c82 (SP-0540), 19c95433a987386e (SP-0541), 19c954d01418d16c (SP-0542), 19c95bcbc53efa16 (SP-0543), 19c95f8dca64b8ad (SP-0544), 19c95fbc55a8d1a1 (SP-0545), 19c9daf655f3002e (SP-0546), 19ca0e9ad01a16cd (SP-0547), 19ca398af605f23a (SP-0548), 19cb05b6a5ac0151 (SP-0563), 19cb0e3ed0509547 (SP-0564), 19cba04b6a01b903 (SP-0566), 19cc9f5be1fd779c (SP-0570), 19cde109aee9e0d8 (SP-0573), 19cde873a732271b (SP-0574), 19d04381eaab4c60 (SP-0583), 19d07358d5ac4260 (SP-0586), 19d225c4bcd23b69 (SP-0589), 19d2d33646672aa2 (SP-0592), 19d30b35c8ae890e (SP-0594), 19d30e829fbc2838 (SP-0595), 19d39f76b80650dd (SP-0600), 19d3ac1d78697485 (SP-0601), 19d3fc9b6c9ad1cb (SP-0602), 19d3fff4f6f07acf (SP-0603), 19d44d1f89f62183 (SP-0607), 19d44d2223067fd1 (SP-0608), 19d44d24c905eea0 (SP-0609), 19d44d9196e48486 (SP-0610), 19d44dcafa9aa501 (SP-0611), 19d44dcbbcc2f313 (SP-0612), 19d44dcc48115c2b (SP-0613), 19d44dccfa89510f (SP-0614), 19d44dcda6a7a9ef (SP-0615), 19d44f7ee240732b (SP-0616), 19d451814251ae3a (SP-0617), 19d643ff9dda21bd (SP-0618), 19d6442dba0dabce (SP-0619), 19d6446135a29cbf (SP-0620), 19d6446ffc5f53b3 (SP-0621), 19d6447025040635 (SP-0622), 19d644707b536cd4 (SP-0623), 19d644ef6e4f09b1 (SP-0624), 19d647a2b8bd4d86 (SP-0625), 19d647a32c6b3cad (SP-0626), 19d647a41419da17 (SP-0627), 19d64912dc3b7a28 (SP-0628), 19d64940b1e9d860 (SP-0629), 19d64940cdcfe614 (SP-0630), 19d6ded69e5461e2 (SP-0631), 19d6e15bd278eb75 (SP-0632), 19d8d4651b42e71a (SP-0638), 19d92ff93fc8b4f0 (SP-0639), 19d9674a44e360f1 (SP-0640), 19d9dd26f4e7242b (SP-0641), 19dab6b5b2ffcf5f (SP-0646), 19dab6f4f0e2c0be (SP-0647), 19dab983ae3aa08a (SP-0649), 19dab9842852b961 (SP-0650), 19dac2031903beab (SP-0651), 19db16a2e288c3e7 (SP-0664), 19db1d411f18b570 (SP-0665), 19db2dc31208f02d (SP-0670), 19db5b25bb020ddc (SP-0671), 19db6286e0fd8857 (SP-0672), 19db63bd0a662f4c (SP-0673), 19db7634412cf151 (SP-0674), 19db765c797500a0 (SP-0675), 19dcf83a0d732a05 (SP-0677), 19dcf83c478a060c (SP-0678), 19ddf3205d6ca2fc (SP-0679), 19dea223e125b9fe (SP-0684), 19df494cfbefd6b4 (SP-0687), 19df520c1952a8e6 (SP-0688), 19dff18b2aa86646 (SP-0692), 19e0415c7756eb39 (SP-0694), 19e04f7c4026ee5d (SP-0695), 19e14925ef8ded90 (SP-0697), 19e1497b3af12396 (SP-0698), 19e17f7fe0f01875 (SP-0699), 19e1817fd696dccf (SP-0700), 19e23145b9b264db (SP-0701), 19e3d773b931aaea (SP-0702), 19e46e43877f04e5 (SP-0703), 19edc257f7a46da7 (SP-0707), 19f3d7ad12f99c51 (SP-0709), 19f4d4b0332101c9 (SP-0710), 19f526263dcac002 (SP-0711), 19f621d4a50fd4af (SP-0715), 19f82164c88d86aa (SP-0716), 19f870bf19d5f34f (SP-0717), 19f9ae0e20ccd355 (SP-0721), 19f9ae3bf1daad82 (SP-0722), 19fa6d6b84e641f7 (SP-0723), 19fa8a62b57f386b (SP-0724), 19faf6086bb922c5 (SP-0725), 19fb9141436502ce (SP-0727), 19fc876dc8f9a368 (SP-0730), 19fc8aa2f66c76e9 (SP-0731), 19fc8b4c1e458ada (SP-0732), 19fce1b46968673d (SP-0735), 19fd3ced6cbce4c1 (SP-0737), 19fde8b2d8fe8858 (SP-0738), 19fded0413b2d3ff (SP-0739), 19fdf0dab8975f4d (SP-0740), 1a0fd8d3c1e9ed06 (SP-0758), 1a165b0f9cabe7b9 (SP-0774)

## 5. Ambiguities resolved by judgment

1. **Class rule conflicts for tracker files.** The brief says tracker work product (v3_parts, READERS, notes) is WORK-PRODUCT, and lists 81/81B/81C/63K as AI-LEAD. Several reading notes class tracker files AI-LEAD: CANON, KNOWN_FALSE, qa_Q61 (v3_parts), SERVICE_VIOLATIONS_LOG (per BEHAVIOR), ex_23 and R7. The brief's explicit lists were applied: those files are WORK-PRODUCT, and each note records the AI-LEAD label. 81, 81B, 81C and 63K are AI-LEAD. D4 (a Drive Google Doc, not a tracker file) is AI-LEAD, per its notes.
2. **Copies of the same document.** Byte-identical or same-size copies are one primary row plus DUPLICATE rows ("copy of SP-xxxx").
   - The primary is the index's original pointer.
   - Where only a preserved copy was read, the primary's read_status reflects that read, and the note says "via preserved copy".
   - Same-size copies that are not hash-verified (EV-010, EV-020, EV-037[2], the PDD copies, the EV-003 copies, docket copies C/D/E) are also DUPLICATE, with "not hash-verified" in the note.
3. **Same-text but not byte-identical files are DUPLICATE**, with the reason in the note: EV-088's 1o28AfW… and EV-037[1]'s duplicate send 19f9ae3b…. Different formats or variants keep their own class (EV-100 DOCX, EV-028 variants, EV-022 "EXHIBIT D" family).
4. **EV-023 and EV-101 are DUPLICATE of EV-033**, per the index and the sha256 check in the notes §7. WP-019[2] and EV-106 are DUPLICATE of EV-041, and WP-020[2] and EV-107 are DUPLICATE of EV-042. Because EV-041 and EV-042 have only session-upload pointers, their primaries are the finthread copies with the same sha256.
5. **Entries outside the seven classes.** EV-013 (prenup, sealed) is CORRESPONDENCE as its carrier email. EV-057 (web organisation facts) and EV-089 (a verification finding) are WORK-PRODUCT and point to the index. EV-036[1] (a mixed police-report segment) is WORK-PRODUCT.
6. **EV-043/044/045** (Exhibits A–C) point to the Declaration file that contains them. EV-045 is AI-LEAD. No reader in this thread read the exhibit pages: DECL_2026-03-27_exhibits_A-C.notes.md is referenced by BRIEF_and_DECL but does not exist yet.
7. **read_status follows what the Spiegel-thread readers read, not what a tracker or AI file claims.** For example, the Drive files qa_Q61 says it opened are metadata-only or not-read here, with a note.
8. **Gmail dates for ids outside the inventory** are decoded from the id (validated 211/211). The thread is `unknown` unless a notes file states it.
9. **Dates for date ranges** use the range start, with the range in the note (for example EV-025, EV-026, EV-092). A year or month alone is written as `2024` or `2025-08`.
10. **Sets.** Each message or file is its own row carrying the set's EV-id. Where one id appears in two entries, the row carries the first EV-id and the note names the other (199db7e7… EV-069/EV-075[1]; 199ec75f… EV-052/EV-076[1]; 1844d84b… EV-091/EV-074; 19af167f… EV-054/EV-053 forward; 18467dd2… EV-067/EV-089).
11. **The State Bar complaint drive copies.** 1Uo94Vcg… and 1oXP4u0Q… are 86-byte shell-command exports. They are DUPLICATE (type other) of the unsigned draft 17_UTAx…, which is WORK-PRODUCT, with the content described in the note.
12. **Gmail carriers with AI-named attachments** are AI-LEAD (inventory appendix, plus 19c9262b…, 19d3fff4… and 19d401f9… per HALSEY_REFERRALS). The fact that each message was sent stays recorded in its note.
13. **Fallback pointers.** Index entries with no locator of their own point to the index file. The note gives the index line.
14. **EV-020.** The index calls it "Respondent RFO". Its Drive title reads "[P] Resp.RFO" and it is the same size as Petitioner's 12/29/2025 Response (15X2aSba…, 1bUF2pk…). The discrepancy is recorded in the note and not resolved; those two ids remain separate rows.
15. **WP-013.** Its id is wrapped across index L870–871. It was joined as 1V8i9ngoS0kh_7vwkyWaIRcSgSHX70hyO and is not in the inventory.

## 6. READING_NOTES files used (all read in full)

The files below were read in full, except EVIDENCE_INDEX.notes.md. Of that file, §1, §2, §5a and §6–§7 were read line by line. §3, §4, §5b and §5c are verbatim quotations of the index; they were scanned mechanically for identifiers rather than read line by line.

2026-08-10_service_declaration_statebar_and_kale · 63K_BAR_AND_JANINA_EXTRACT · 81B_LANCE_KEYWORD_SWEEP · 81C_LANCE_LITIGATION_CONDUCT · 81_LANCE_ARTIFACTS_EXTRACT · 85_POLICE_REPORT_V3 · BEHAVIOR_b_e_primary · BRIEF_and_DECL_2026-03-27_text · CANON · COURT_ORDERS_and_FL141 · D1 · D2 · D3 · D4 · EVIDENCE_INDEX · G1 · G2 · G3 · G4 · JOLIE_context_only · JURISDICTION_SPLIT · KNOWN_FALSE · L1_ally · MO_2026-04-21 · SERVICE_VIOLATIONS_LOG · qa_Q61 · and three that landed during the build: PDD_2024-06-17_content, HALSEY_REFERRALS_2026, DOCKET_24STFL00432.

DOCKET_24STFL00432 was not read line by line in its §4–§6 (verbatim docket transcriptions). Its §1 sources table and §7 scope were read, and all of its ids were scanned.

**Pending — add on next pass** (not present in READING_NOTES/ when this register was finished):
- DECL_2026-03-27_exhibits_A-C.notes.md
- BEHAVIOR_c_proofs_of_service.notes.md
- BEHAVIOR_f_police_contacts.notes.md
- SPIEGEL_DECLARATIONS_2025-12.notes.md

To rebuild after they land, run `python3 -I reg/build.py` from the scratchpad. It re-scans every notes file for ids; new hand annotations go in `reg/ann.py`.

---

# PASS 2 (register maintenance, 2026-11-01)

Same rules as pass 1: INVENTORY/AGENT_RULES.md obeyed (read-only everywhere; only EVIDENCE_REGISTER.tsv and this file written; no git; no Gmail or Drive call). The pass-1 schema, class rules and the judgment calls in §5 above are kept. `reg/build.py` was **not** re-run, because it renumbers every row. Pass 2 is an append script: scratchpad `reg2/pass2.py`, with hand annotations in `reg2/ann2.py`, the id scan in `reg2/scan.py` → `scan.json`, and the pass-1 register backed up at `reg2/EVIDENCE_REGISTER.pass1.bak.tsv`. To reproduce: copy the backup over the register, then run `python3 -I reg2/pass2.py`.

## P2.1 Counts

| | before | after |
|---|---|---|
| rows | 2,815 | **3,512** (new SP-2816 … SP-3512) |
| CORRESPONDENCE | 738 | 1,391 |
| WORK-PRODUCT | 836 | 837 |
| COURT | 565 | 520 |
| SWORN | 383 | 387 |
| DUPLICATE | 74 | 184 |
| AI-LEAD | 133 | 135 |
| ACCOUNT | 86 | 58 |
| read: metadata-only | 2,291 | 2,871 |
| read: not-read | 394 | 305 |
| read: full | 112 | 283 |
| read: partial | 18 | 53 |

- **New rows: 697.** 191 come from READING_NOTES (steps 1 and 3) and 506 from gmail_inventory.tsv (step 2). By class: CORRESPONDENCE 650, DUPLICATE 25, WORK-PRODUCT 9, COURT 8, ACCOUNT 3, AI-LEAD 2. By read_status: metadata-only 552, full 92, not-read 41, partial 12. They are numbered in date order among themselves, with `unknown` dates last.
- **Existing rows changed: 278.** SP-ids, EV-ids and pointer ids are unchanged; this was checked against the backup.
  - 120 were updated from the new notes: read_status raised (102), date set (39), tags merged (65), class set (20), type set (12).
  - 75 Gmail rows that pass 1 marked not-read because they were "not in gmail_inventory" are now in the inventory. They are metadata-only, with the inventory header appended to the note.
  - 76 step-3 copies became DUPLICATE, and their 6 primaries were annotated.
  - 134 pointers had `thread:unknown` (or the message's own id) replaced by the thread id that the inventory or the notes give. Another 11 new rows took their thread from writs_levy_locate.tsv.
- Notes field: each pass-2 text starts with `P2:` and the pass-1 note is kept after ` || `. Notes are clipped at 480 characters.
- **Structural checks (re-run independently):** every line has 9 columns, the 3,512 SP-ids are unique and run without gaps, and all classes, types, tags and read_status values are valid. The only pointers carried by more than one row are the three shared pass-1 fallbacks (§2).

## P2.2 Step 1: READING_NOTES not registered in pass 1

Files read in full this pass:
- DECL_2026-03-27_exhibits_A-C, BEHAVIOR_c_proofs_of_service, BEHAVIOR_f_police_contacts, BEHAVIOR_g_writs_schwenke_2026, SPIEGEL_DECLARATIONS_2025-12, WRITS_2026-04-28_and_appeal_notice, ENVELOPE_PHOTOS_originals, EXHIBIT_F_chain_emails and EXHIBIT_F_source_doc_metadata. These are the nine files newer than pass 1.
- MO_2026-04-21_compel_disclosures, G4_stip_personal_service_DVRO_2025-11-24, JOLIE_context_only, COURT_ORDERS_and_FL141 and BRIEF_and_DECL_2026-03-27_text were re-read. They add nothing new; their documents were already registered.

Every 16-hex Gmail id and every 33- or 44-character Drive id in the nine new files was scanned with the pass-1 regexes: 204 Gmail and 122 Drive ids. Each one is annotated by hand, already registered, or excluded. The script stops if any id is left unannotated.

**Excluded:**
- Folders: 13AdG4-9…, 18meu_Dv…, 1veFjTj9…, 1OgvJLK1… ("CLOSED LOOP…" folder), 1i6TqFK6…, 17Jjsm6E…, 1SUO9jGS… and 15Kwe3SX….
- The sha256 prefix 16dc9cf484dda97a (ENVELOPE image table).
- Truncated ids that cannot be resolved (13tfj0UM7U8F… and the others in the ENVELOPE §2 list).

**Named rows:**
- **EV-042 to EV-045 (shared finthread pointer):**
  - EV-042 (SP-0590) stays partial: pp.4 and 7–15 are now read, but the pp.5–6 photos are not read in full.
  - EV-043 (SP-2798) is dated 2026-03-27 and partial.
  - EV-044 (SP-2799) is dated 2026-03-17 (execution date of both Exhibit B declarations) and full.
  - EV-045 (SP-2800) is dated 2026-03-27 and full. It stays AI-LEAD; p13's last line is cut off by the source.
- **Preserved minute orders:** EV-002, EV-003, EV-004 and EV-005 (SP-0565, SP-0667, SP-0668, SP-0669) were already "full" in pass 1. EV-001 preserved (SP-0666) stays **not-read**: no notes file read it.
- **Writs** W1, W2 and W3 (SP-3373 to SP-3375) and the clerk's Notice of Non-Compliance (SP-3433) are COURT and full.
- **Envelope photos:** the envelope-photo PDF 1zNB5FyW… (SP-2776) is now dated 2026-03-17, photo, partial. The overview 16SIlr36… (SP-1004) is full.
- **Exhibit F chain:** the 18 messages are full. Thread ids that are not among the returned messages are rows marked not-read.
- **Exhibit F source doc** 1vXbXc01… (SP-0323) stays AI-LEAD and metadata-only, with the Drive metadata added to the note.

## P2.3 Step 2: Gmail inventory (874 rows; 663 new since pass 1)

- **Reconciliation of the 663 new inventory rows:** 146 were already registered in pass 1 (ids named in READING_NOTES), 11 were added in step 1 from the new notes, and 506 are new step-2 rows. All 874 inventory messages are now in the register.
- **Class** is provisional from sender and subject:
  - CORRESPONDENCE, which covers firm mail (A) and Halsey's SENT mail (E);
  - AI-LEAD for the 26 appendix messages (all already registered in pass 1) and for the monitor sender/subject pattern;
  - ACCOUNT for Google and Apple account senders.
- **Result:** all 506 new rows are CORRESPONDENCE. The new A and E rows have attachments "(not fetched)", so no name-based AI-LEAD match was possible.
- **Tags:** A gives keyword tags over subject and attachments; E gives da, police or statebar only when the subject shows it; C, D, F and G map as in pass 1.
- **read_status:** metadata-only. Where a notes file read the message, the step-1 annotation wins and the inventory header is appended to its note.

## P2.4 Step 3: writ/levy locate (court or bank documents only)

- **Added (new rows):**
  - the three 2026-08-24 writ exports;
  - the Notice of Non-Complaince export (1Rekh834…). It is not in writs_levy_locate.tsv; its source is the WRITS notes.
  - the LASD levy-file request PDF 11dNGcfS… (SP-3494, CORRESPONDENCE, unopened).
- **Updated:** the Ally SecureMessageAtt.html export (SP-2342) is now dated 2026-09-04; its note names the carrier email 1a06da14…; content still unread.
- **One primary plus DUPLICATE rows** (same title and same size; not hash-verified; all unopened):

| group | copies | primary | primary chosen as |
|---|---|---|---|
| ALLY BANK - 0001-0238.pdf | 16 | SP-1435 | earliest copy |
| ALLY FINANCIAL INC. - 0001.pdf | 16 | SP-1992 | earliest copy |
| Ally_Regulatory_Complaint_Package_2026-10-29.pdf | 2 | SP-1426 | earliest copy |
| 2024-10-31 Notice to Consumer, Ally Bank | 16 | SP-1156 | `2024-10-31__ysfamilylaw.com__` export |
| 2024-10-31 Notice to Consumer, Ally Financial Inc. | 16 | SP-2310 | `2024-10-31__ysfamilylaw.com__` export |
| 2024-10-31 Notice to Consumer, Ally Servicing LLC | 16 | SP-0844 | `2024-10-31__ysfamilylaw.com__` export |

- The three notice primaries are dated 2024-10-31, from the title and from the firm's transmittal 192e4eb4… (read in full).
- Not added: the 2010 Sotheby's items and the AI monitor rows.

## P2.5 Judgment calls

1. **EV-108.** The primary stays on the index pointer, File C 1r_5T4D4… (SP-0397), under pass-1 rule 2, even though File B 1MZDYige… (SP-0395) holds the firm's original bytes. SPIEGEL_DECL shows File C is a PDFium re-save of File B with the same text. File B, D2 1WMbJ0KT… and D2b 1DZJSg1s… are DUPLICATEs of SP-0397.
2. **15X2aSba… (SP-0386)** is now hash-verified byte-identical to File A 1bUF2pkz… (SP-0390; sha256 6f0f3b39…). It is now a DUPLICATE, and SP-0390 is SWORN and full. The EV-020 family (SP-0393 and the others, same 4,069,611 B) was not hashed by any reader, so pass-1 call 14 stays unresolved.
3. **Provisional classes corrected where a reader saw the face of the document:**
   - SP-0227, SP-0869, SP-2368, SP-2393 and SP-2683 → SWORN;
   - SP-1544 and SP-2760 → COURT;
   - SP-0932, SP-0986 and SP-2730 → CORRESPONDENCE;
   - SP-0390 → SWORN.
4. **Same-size copies are DUPLICATE with "not hash-verified"** (pass-1 rule 2):
   - 20 copies of the 16,443,000 B 4/18/2025 Supplemental Pleadings → SP-0221;
   - 4 copies of Halsey's "Spiegel, The Beverly Hills Police Department… FORMAL NO.pdf" → SP-1388;
   - the two 414,452 B "e8a95c7b…" PDFs → the Provinziano letter SP-1221 (R1, 1CuG6…). Only the size matches; the content was not checked.
   - Copies with the same text but different bytes: SP-1856 → SP-0227; 1thu8Zr7… → SP-1332; 1y5-lA6t… → SP-0221.
5. **Thread ids** that the notes name but that are not among the returned messages get their own rows marked not-read, as in pass 1, with a note.
6. **1a01fcb067325e9b** appears only in BEHAVIOR_g's §D table, for the message whose text §B gives under 1a01fc775016ae06. Both are rows; the discrepancy is not resolved.
7. **1a015ef09efeb917** is AI-LEAD: its body quotes an AI analysis and a monitor email. The BHPD "Marsy's Law" dashboard images are WORK-PRODUCT, not AI-LEAD, because no document read shows they are AI output. The note records the BEHAVIOR_f §2.5 description.
8. **The Ally regulatory package** keeps its provisional ACCOUNT class: it is unopened and its authorship is not established. The Provinziano invoices are ACCOUNT. The Square invoice notices are CORRESPONDENCE (type other).
