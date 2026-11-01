# Reading notes — Envelope photos (Spiegel mail delivered 24 Feb, Cancún): search for the originals behind Exhibit A of the 3/27/2026 declaration

- **Reader:** Opus subagent, read-only (Gmail: search_threads/get_thread/get_message only; Drive: search_files/get_file_metadata/download_file_content only). No git was run. Scratch: `/tmp/claude-0/-home-user/9a86eccf-071d-5c97-88ae-ef129ec55f9d/scratchpad/ph/`.
- **Class:** photographs taken by or for Respondent (party material). Not AI output.
- **Headline:** Higher-quality photos of the envelopes **were found**. They are 13 separate photos at 1920×2560, embedded in an iOS-made PDF that Halsey emailed to Katherine Schwenke on 2026-03-17. They show **each postage label up close**. **The year on the $29.70 "JAN 30" label now reads 2026**: it matches this printer's known "6"s much better than its known "8" (details in §3). The $3.15 label's year is now plainly **"JAN 05, 2026"**. A CN22 customs form on the same orange envelope reads **"Date of Mailing: 01/30/2026"**.
- **Not found:** an original of the **p6 photo** (orange envelope with the clipped Spanish note and the ENTREGADO stamp). The likeliest candidate is a Gmail attachment that has **no Drive export** (§1.3).
- **Caveat on resolution:** the found photos are about 1920 px wide, not 12-MP camera files, and they carry **no EXIF**: iOS stripped it when it built the PDF. On the orange label the year digit is about 12 px tall, roughly the same as in the filed p6 strip (≈14.5 px). The gain comes from a **different, sharper photograph** and from **same-printer exemplars** of "6" and "8" on the other labels, not from more pixels.

## 1. Sources found

### 1.1 Primary find: PDF of envelope photos

| Field | Value |
|---|---|
| Drive id | `1zNB5FyWD6EuWN3Ob6fnVEf0i_-xiZEFl` |
| Title | `2026-03-17__gmail.com__Lances Mail Dumped At Once By Mailman No Signature Me or Him.pdf` |
| Drive createdTime | 2026-08-22T10:19:08Z (archive export) |
| Bytes | 4,807,319 |
| sha256 | `6ab25e84c7b32585b27e9c2b67a0abbb42c33da6213ecf94354b16ae2599f6d0` |
| Source email | Gmail msg `19cfcf815d187364` (thread `19cfcf6a0973371b`), 2026-03-17T18:04:02Z, halsey2005@gmail.com → kat.flds@gmail.com. Subject identical to the PDF title. |
| Email body (verbatim) | "All photos of mess. I opened a few and saw fakes emails from me and stopped opening starting filing charges. He needs to go to jail. This is outrageous." |
| PDF metadata | Producer "iOS Version 26.4 (Build 23E5234a) Quartz PDFContext"; CreationDate 2026-03-17 17:57:35 UTC; 16 pages, 594×792 pt |
| Embedded images | 16 JPEG, each 1920×2560, 233 ppi. Pages 12, 15, 16 repeat pages 4, 3, 2 (identical bytes), so **13 unique photos** (pdfimages p-000 … p-013, without p-011/p-014/p-015). No EXIF in any of them. |

### 1.2 Same overview photo, sent separately

| Field | Value |
|---|---|
| Drive id | `16SIlr36WPrvZQcVzlFZXvqWX2JqjLGMs` |
| Title | `2026-03-17__gmail.com__Lances Mail Mess Dumped Same Day.pdf` |
| Bytes | 292,997 |
| sha256 | `cc7025de9c2e140374a455ac1e905912cd7c12c5b1b84295650117b4daeae42f` |
| Source email | Gmail msg `19cfcf64c6f37b30`, 2026-03-17T18:02:05Z, to kat.flds@gmail.com |
| Email body (verbatim) | "Long shot of Lances f$4ing “Service” by Mail" |
| Content | 1 page, 1 JPEG 1920×2560 (iOS PDF, created 2026-03-17 17:59:26 UTC). It is the **same image** as p-000 in §1.1: the extracted JPEG streams have identical hashes (prefix `799a3fd078966ad3`). |

### 1.3 Probable original of the p6 photo: NOT obtained

- Gmail msg `19cfdfd90e19cc55` (thread `19cfdfd7dd68a549`), 2026-03-17T22:49:39Z, halsey2005 → kat.flds@gmail.com.
- Subject and only attachment: **`IMG_4DB4E344-AE60-47F9-8851-0447C66ACED6.JPEG`** (image/jpeg). The message sizeEstimate is 3,904,894 bytes; the attachment alone is not measured.
- The Gmail tool cannot open attachments.
- **No Drive export exists.** `title contains 'IMG_4DB4E344'` returns nothing. The `2026-03-17__gmail.com__*` export set holds no JPEG. It does hold a 522-byte untitled octet-stream, `1L5qnIUBLwlogS6Jxe9R_bQlR5iQUjqc4` (`2026-03-17__gmail.com__`), which was not opened.
- Whether this JPEG is the p6 photo is **unverified**.
- **No original of the p6 orange-envelope / clipped-note photo was found in Drive.**

### 1.4 Exhibit A p5 = photo p-000

- I rendered the filed PDF (sha256 prefix `e22c423b526081bc`, matching the earlier notes) at p5 and set it beside p-000.
- Framing, envelope order, chairs and water bottle are the same: **visually the same photograph**. Not checked pixel by pixel.
- None of the 13 photos is the p6 photo. All 13 are on a stone counter; p6 is on a wooden table.

## 2. Image table

All 13 unique photos have dimensions 1920×2560 and **no EXIF** (no DateTimeOriginal, camera or GPS). The p-number is the extracted image index in Drive id `1zNB5FyWD6EuWN3Ob6fnVEf0i_-xiZEFl`.

All labels below are USPS "Retail" labels: USPS eagle, a barcode with "00495" under it, and the lines "U.S. POSTAGE PAID / [class] / BEVERLY HILLS, CA 90210 / [date]". Return/addressee text is quoted as it appears.

| p# | sha256 (first 16) | Envelope | Return address | Addressee | Postage label (verbatim) | Dates transcribed / confidence | Resolved? |
|---|---|---|---|---|---|---|---|
| p-000 | 799a3fd078966ad3 | Overview on the counter (= Ex. A p5) | — | — | Labels too small to read | — | n/a |
| p-001 | 03db7f73fa8acbf3 | White, large (Ex. A table #1) | Printed, upper left: "Young, Spiegel & Hosp, LLP. / 301 N. Canon Dr., Suite 300 / Beverly Hills, CA 90210" | Handwritten: "Halsey Minor / 602 Punta Del Mar / Kukulcan Boulevard / Zona Hotelera / 77500 Cancún, QRO, Mexico" + "Mexico" | "FCMI LE … **JAN 05, 2026** / **$3.15** / S2324K502949-03" | JAN 05, 2026: high | **Yes**: year "6" is plain |
| p-002 | 9a2158137299cb36 | White, printed From/To label | "From : YOUNG, SPIEGEL & HOSP, LLP / 301 NORTH CANNON DRIVE / SUITE 300 / BEVERLY HILLS, CA 90210" (sic "CANNON") | Printed: "To : Halsey Minor / 602 Punta Del Mar / Kukulcan Boulevard / Zona Hotelera / 77500 Cancún, QRO, Mexico" + handwritten "Mexico" | "FCMI LE … **DEC 30, 2025** / **$13.00** / S2324K500641-9" | DEC 30, 2025: high | Yes |
| p-003 | 9171ab3af798e8bc | **Orange/kraft** (Ex. A #5/#7) | Printed, upper left: "Young, Spiegel & Hosp, LLP / 301 N. Canon Dr., Suite 300 / Beverly Hills, CA 90210" | Yellow sticky label, handwritten: "Halsey Minor / 602 Punta Del Mar / Kukulcan Boulevard / Zona Hotelera / 77500 Cancun, QRO, Mexico" + "MEXICO" | "U.S. POSTAGE PAID / **FCPIS** / BEVERLY HILLS, CA 90210 / **JAN 30, 202[6]** / **$29.70** / S2324K502949-03". Also a **CN22 customs form**, transcribed in full in §4 | Label JAN 30, 202[6]: "JAN 30, 202" high; final digit = 6, moderate-to-high (§3). CN22 "01/30/202[6]": same digit shape, not tested separately | **Resolved as 6** (not certain; §3) |
| p-004 | 3b3d2e9061977cf9 | White (opened), label rotated 90° | partly visible, rotated: "YOUNG, SPIEGEL & HOSP, LLP / 301 NORTH CANON DRIVE …" (partly read) | not visible | "FCMI LE … **JAN 06, 2026** / **$13.00** / S2324K502949-03" | JAN 06, 2026: high | Yes |
| p-005 | c39fc89c4f05442f | Contents only | — | — | — | Document caption "PETITIONER'S OBJECTIONS AND REQUEST TO STRIKE DECLARATION OF RESPONDENT" (thumbnail read only; hearing-date line not zoomed) | n/a |
| p-006 | 46edbd3d4ea4a6ff | White (opened), label rotated; FL-300 under a binder clip | not legible | not visible | "FCMI LE … **FEB 02, 2026** / **$13.00** / S2324K502949-03" | FEB 02, 2026: high | Yes |
| p-007, p-008 | c2ab252a9204ec1b, 841d2359da951b1d | Contents only | — | — | — | FL-320 "RESPONSIVE DECLARATION TO REQUEST FOR ORDER", case 24STFL00432, hearing "February 3, 2026 / 8:30 a.m. / 23" (thumbnail read only; not read in full) | n/a |
| p-009 | 6423703f12aaea31 | White, handwritten address | Printed, rotated, partly torn: "Young, S[…] / 301 N. C[…] / Beverly Hills, CA 90210" | Handwritten: "Halsey Minor / 602 Punta Del Mar / Kukulcan Boulevard / Zona Hotelera / 77500 Cancún, QRO, Mexico" + "MEXICO" | "FCMI LE … **JAN 08, 2026** / **$7.55** / S2324K502949-03". **Machine cancellation**, partly under the label: "Los Ange[…]" / "THU 0[8?] […]" + wavy lines | Label JAN 08, 2026: high. Cancellation: low; only "THU 0?" legible | Label yes; cancellation no |
| p-010 | 16dc9cf484dda97a | White, printed From/To label | as p-002 | as p-002 + "Mexico" | "FCMI LE … **DEC 30, 2025** / **$13.00** / S2324K500641-9" | DEC 30, 2025: high | Yes. Tape strip and tears differ from p-002, so it looks like a different envelope, but this is not confirmed |
| p-012 | 718ac98d2981e99b | White, printed From/To label | as p-002 (header) | as p-002 + "Mexico" | "FCMI LE … **DEC 30, 2025** / **$8.65** / S2324K500641-9" | DEC 30, 2025: high | Yes |
| p-013 | 064547c771625321 | White, printed From/To label | as p-002 | as p-002 + "Mexico" | "FCMI LE … **DEC 30, 2025** / **$3.15** / S2324K500641-9" | DEC 30, 2025: high | Yes |

**Distinct labels seen:**
- $3.15 JAN 05 2026; $13.00 DEC 30 2025 (×2, or one envelope photographed twice); $29.70 JAN 30 2026; $13.00 JAN 06 2026; $13.00 FEB 02 2026; $7.55 JAN 08 2026; $8.65 DEC 30 2025; $3.15 DEC 30 2025.
- That is 9 envelopes if p-002 ≠ p-010. The declarations say ten.
- None of these photos shows a Correos de México mark.

**Other candidate images (none shows an envelope):**

| Id | Title / description | Bytes | Dimensions | EXIF | sha256 |
|---|---|---|---|---|---|
| `1CSRhRWaPXYf-Hncfwny8fyxUcKomRaEb` | `2026-02-24__gmail.com__IMG_0051.jpeg`: Vanguard 529 statement page | 372,578 | 2000×2101 | DateTimeOriginal 2026:02:13 19:53:00; no camera or GPS | `d75238…d2b1` |
| `1ESfPf24xKZ7b0g8KWf5mXduc82sj2NHj` | `image.png`, 2026-03-24, Drive root: BHPD "Marsy's Law" dashboard screenshot | 4,844,398 | 2770×9244 | none | `1b790b…f0de` |
| `1q37EGU74t0XOXx9WIV6aR-RCXBMWjWuB` | `image.png`, same type | 4,801,823 | 2061×9211 | none | `36d932…9369` |
| `1bPhongyj2MEfsE3-y3TvZd8_JC_mzZik` | `image.png`, same type | 2,412,747 | 2216×9898 | none | `ca3769…3319` |
| `1EPhPaTug4h_nrIWTFjj6fz47SDyhHiOh` | `image.png`, same type | 2,410,336 | 2212×9897 | none | `11c046…5bcc` |
| `1HlYIxmrso0TTTyqm1CC0t3Q4M_VUoDix` | `IMG_0014.PNG`: "Complete Non-Compliance with Marsy's Law" bar chart | 257,430 | 2400×1600 | none | `4ad88f…764b` |

`1-4SILBrukI8NDza6_g_oDGSBbp5a4FDS` (`image.png`, 2,412,747 bytes, the same size as `1bPh…`) was **not downloaded**.

**Not downloaded, judged non-photographic:** the 2026-03-24 PNGs in folder "CLOSED LOOP OF CORRUPTION BY GOOGLE GEMINI AI" (`1OgvJLK1rSQ-sAdVJCzNh2ZXem9rua_8N`):
- `13tfj0UM7U8F…` ("ChatGPT Image Feb 9, 2026…")
- `1qCT38u_a0zp…` (AFF2E834…)
- `1YFiUbewIB3F…` (92CC15E6…)
- `1iDR5akJttD_…` (0E78B074…)
- `1RdfKAJDaKFn…` (197CAD09…)
- `1nm1KjUMHYtd…` (B7CC5BAB…)
- `1G8diN74YtnK…` ("HELP First Hacking … Gmail.jpeg.png")

The same UUID filenames were attached to the 2026-03-09 email about Marsy's Law (msg `19cd38cc65e66272`).

## 3. The "JAN 30" year digit (orange envelope, p-003)

**Crop files** (scratch `out/`):
- `c003_label.png`: whole label
- `c003_date.png`, `c003_year.png`: date line at 6× and 12×
- `panel_year_digit.png`: side-by-side digits

**Where the glyphs are:**
- Target: native label crop `n/L003.png` box (452,145)-(460,157); in p-003 itself ≈ x1632–1640, y325–337. The digit is about 12 px tall.
- Exemplars, all from labels printed by the same office ("00495", serial prefix S2324K):
  - **known "6"**: the day digit of "JAN 06" on p-004
  - **known "6"**: the year digit of "2026" on p-004 and on p-009
  - **known "8"**: the day digit of "JAN 08" on p-009
  - control: the "0" of "30" on p-003

**Normalized cross-correlation** (each glyph resampled to 16×24) against the target:

| Exemplar | NCC |
|---|---|
| "6" (day, p-004) | **0.898** |
| "6" (year, p-004) | 0.828 |
| "6" (year, p-009) | 0.800 |
| "8" (day, p-009) | **0.704** |
| "0" control | 0.550 |

**Visual comparison** (panel):
- The target's left side runs down without a break, as in the "6"s. The known "8" pinches at the waist on both sides.
- The target's top-right terminal curls down further than in the exemplars. A label crease runs through this area, and that probably makes it look 8-like at low resolution.

**Reading:** "JAN 30, 2026". Confidence moderate-to-high.
- Every same-printer "6" scores above the "8", by 0.10–0.19.
- Not certain: the glyph is about 12 px tall, and only one "8" exemplar was available.
- Context, not used as proof: these photos existed by 2026-03-17 (PDF CreationDate and Gmail send time), and the CN22 form on the same envelope prints a mailing date of 01/30/202[6] in another font.

## 4. CN22 customs form on the orange envelope (p-003): verbatim

- **Header:** "CN22-CUSTOMS DECLARATION / Origin Post: US Postal Service / Date of Mailing: **01/30/202[6]** / Category of Item: Document / AES/ITN/Exemptions: NOEEI 30.37(y) / Detailed description of contents / DOCUMENTS"
- **Handwritten:** "0.55" (with arrows)
- **FROM:** "NATHAN GRAY / YOUNG N SPIEGEL / 301 N. CANON DR # 300 / BEVERLY HILLS, CA 90210"
- **TO:** "HALSEY MINOR / 602 PUNTA DEL MAR / KUKULCAN BOULEVARD, ZONA HOTELERA / CANCUN / QRO / 77500 / MEXICO"
- **Item lines:** Qty "20"; Wgt "1" lb "2" oz; Value "0.01"; HS Tariff "4911999802"; TOTAL 1 / 2 / 0.01
- **Other printed text:** "F"; "Not Valid As Proof-Of-Payment For U.S. Postage"; "1.1"; "PS Form 2976 (March 2015)"
- **Barcode text:** "**LH 265 470 088 US**". The S10 check digit (weights 8-6-4-2-3-5-9-7 over 26547008) comes to 8, which matches the printed final 8. A reading of "…086" would fail the check.
- This is a USPS tracking number. It was **not looked up**: no outbound action was taken.

## 5. Queries run (all read-only)

**Drive:**

| # | Query | Result |
|---|---|---|
| 1 | `mimeType contains 'image/' and createdTime > '2026-02-23T00:00:00Z' and createdTime < '2026-03-28T00:00:00Z'` | 13 files, single page (no nextPageToken): the 8 PNGs in the "CLOSED LOOP" folder and 5 `image.png` in root, all created 2026-03-24 |
| 2 | `title contains 'IMG_' and createdTime > '2026-02-23T00:00:00Z' and createdTime < '2026-04-01T00:00:00Z'` | 1 file (IMG_0014.PNG) |
| 3 | Combined `title contains 'envelope' or 'sobre' or 'Exhibit A' or 'postmark' or 'delivery'` | > 100 hits, mostly 2006–2013 archive files. Only page 1 was listed. |
| 3a | Rerun as `title contains 'envelope' and createdTime > '2026-02-23…'` | No 2026 envelope photos |
| 3b | `(sobre/postmark/Exhibit A) and createdTime > '2026-02-23…'` | Page 1 (100) filtered: no relevant images. Later pages were not read. |
| 3c | `delivery … title contains '2026'` | Only "Delivery Status Notification" PDF |
| 4 | Folders `Exhibit` / `Service` / `Envelope` | Only "A PROOF OF SERVICE", "Refusal of Service by Email History", "exhibits_attachments", "Google Services". None are envelope-photo folders; contents not listed. |
| 5 | `title contains '2026-02-24__' or '2026-02-25__'` | The only image is `IMG_0051.jpeg` (Vanguard) |
| 6 | `(title contains '2026-03-1'/'2026-02-2'/'2026-03-0'/'2026-03-2') and mimeType contains 'image/'` | No envelope photos |
| 7 | `title contains '2026-03-17__gmail.com'` | Found the two PDFs in §1.1–1.2 |
| 8 | `IMG_4DB4E344` | Nothing |
| 9 | `IMG_CD2EA195` / `FullSizeRender` / `IMG_1242` / `IMG_1047` / `IMG_0466` / `IMG_0300` | Archive or older items only. Page 1 only. |

**Gmail** (includeTrash):

| # | Query | Result |
|---|---|---|
| a | `has:attachment after:2026/02/23 before:2026/03/28 (envelope OR envelopes OR sobre OR postmark OR "front desk" OR entregado OR Franco)` | ~38 threads (first page of 50 read) |
| b | `(filename:jpg OR filename:jpeg OR filename:heic) after:2026/02/23 before:2026/03/28` | ~63 estimated; first page of 50 read, not paginated further. The only envelope-relevant hit was `IMG_4DB4E344…JPEG`. |
| c | `filename:pdf ("Lances Mail" OR Dumped) after:2026/03/16 before:2026/03/19` | The two §1 emails |

**Gmail attachments seen in candidate threads:**
- msg `19cd3583064f1189` (2026-03-09, 17.6 MB): `IMG_CD2EA195-15AF-4AF7-91E6-8110C83D4A23.jpeg`, `FullSizeRender.jpeg`, `IMG_1242.jpeg`, plus a PDF. Not opened; no Drive export found for IMG_CD2EA195. The email text concerns the hearing schedule, not envelopes.
- msg `19cfd8583251dc52`: "Mexican Testimony-1.pdf" (Drive `1bvKSnDqboO_YtKTq7kwO4bH0kFrM7Sq3`). Not opened.

## 6. Not done / limits

- p-005, p-007 and p-008 (document contents) were not read in full.
- The left-edge strip and the wavy marks on p-001 were examined: the wavy marks are a dotted cancellation-like pattern with **no legible text**. The p-001 bottom barcode strip has no human-readable text.
- The p6 original was not obtained (§1.3).
- The full-resolution camera originals (HEIC / 12 MP), if they exist, are on Halsey's phone or in iCloud, not in Drive.
- The **physical envelopes** (held by Halsey) remain the definitive check for the "JAN 30" year digit and the CN22 date. Tracking LH265470088US is another independent check, but checking it needs outbound action, which this pass did not take.
