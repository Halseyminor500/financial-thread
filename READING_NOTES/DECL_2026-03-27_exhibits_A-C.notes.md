# Reading notes — Declaration re Brief (LASC 24STFL00432), executed 2026-03-27 — Exhibits A–C (pp. 4–15)

- **Source:** `/home/user/financial-thread/documents/2026-03-27_declaration-re-brief_24STFL00432.pdf` @ financial-thread main `63d0aeeb` (commit as supplied in the brief; NOT verified — no git was run)
- **sha256:** `e22c423b526081bc7f67889871b792880f13cbe7217ac5dd0a6cdd38ea69d451` (7,318,891 bytes)
- **PDF metadata:** Title "Declaration Re Brief with Exhibits A-C.pdf"; Author "Katherine Schwenke"; Creator/Producer "Acrobat Sign"; CreationDate 2026-03-27 21:58:49 UTC; ModDate 2026-03-27 22:15:26 UTC; 15 pages, letter size.
- **Pages examined:** 4–15 (pp. 1–3 = declaration text, read separately, not re-read here).
- **Method:** `pdftoppm -r 300` render of pp. 4–15. The embedded images were extracted with `pdfimages -png` and the strips reassembled at native resolution: p5 = 24 strips @300 ppi; p6 = 152 strips @~474 ppi; pp8–10 = 100 strips each @300 ppi; p11 = 33 strips @600 ppi; p13 = 34 strips @~331 ppi. pp14–15 are vector pages plus a small logo image. Crops and zooms were made with PIL and viewed with the Read tool. Raw pixel values were dumped for the disputed digits. Disputed glyphs were tested two ways: (a) normalized cross-correlation (NCC) against rendered candidate strings in Liberation Sans, FreeSans and DejaVu, after first checking the method on known digits; (b) for the 6-vs-8 question, against exemplars cut from the same label ("9" turned 180° = "6") and against a waist-pinch edge test, itself checked on synthetic glyphs. The text layer of pp4–15 holds only the three slip-sheet captions.
- **Reader:** Opus subagent. Class: court filing (exhibits). One AI item inside Exhibit C (p13 "AI Overview") is marked **AI-LEAD** below.
- **"Read in full" status:**
  - pp4, 7, 12 (slip sheets): read in full.
  - pp8, 9, 10, 11: read in full (every printed word; handwriting as noted).
  - p14: read in full.
  - p15: read in full. It is page "1/7" of a printout, and only that one page is in the exhibit.
  - p13: read in full except the last line, which the source cuts off.
  - **pp5–6 (photographs): NOT read in full.** Items not finished are marked "not examined" or "[?]" in the table.

## Per page

| Page | What it shows |
|---|---|
| 4 | Slip sheet: **EXHIBIT “A”** |
| 5 | Photo (Ex. A): a long stone counter. From the near end: **4 white envelopes**, then **1 orange/kraft padded envelope** carrying a yellow sticky note, then **at least 5 stacks of loose printed paper** and one small white item at the far end (contents not legible). Chairs at left, water bottle at right. |
| 6 | Photo (Ex. A): close-up on a wooden table. **Orange/kraft envelope** (USPS Retail label at top right, law-firm return address at top left). On it, at least one **white envelope** (partial "Retail" label; partial rotated return address). On top, a **white sheet held by a binder clip** with a **handwritten Spanish receipt note**, a name/initials, and the **"ENTREGADO" stamp**. Faint printed text under or through the note sheet is not legible. |
| 7 | Slip sheet: **EXHIBIT “B”** |
| 8 | "DECLARATION OF BUILDING MANAGER REGARDING RECEIPT OF MAIL" — caption plus English text ¶¶1–8. ¶8 breaks off at "(Punta Del". The ENTREGADO stamp is printed over ¶8. |
| 9 | Execution block (dated 17 March 2026), signature, handwritten name and job title, ENTREGADO stamp. |
| 10 | End of English ¶8 ("Mar Cancun S.A. de C.V.) next to my signature…"), perjury clause, full Spanish text ¶¶1–8, Spanish perjury clause, signature, ENTREGADO stamp. *(As filed, p9's execution block sits between the broken sentence on p8 and its continuation on p10.)* |
| 11 | "DECLARATION OF Julia Mironova" (English), ¶¶1–7, perjury clause, executed 17 March 2026, signature. |
| 12 | Slip sheet: **EXHIBIT “C”** |
| 13 | Screenshot of a Gmail search showing Gmail's **"AI Overview"** panel — **AI-LEAD**. |
| 14 | Gmail printout: "Delivery Status Notification (Failure)" from google-legal-support@google.com, Fri, Dec 5, 2025. |
| 15 | Gmail printout, page 1/7: "Preservation and Recovery of Evidence – Fourth Formal Request", Fri, Jan 9, 2026. |

## ENVELOPE TABLE

The labels read are USPS **"Retail"** postage labels: USPS eagle logo, a short barcode with "00495" under it, then text lines. No meter strip, no Stamps.com label, no round or wavy postmark cancellation, no Correos de México mark and no tracking-number barcode label could be read on any item.

| # | Page / position | Return address (as printed) | Addressee (as written) | Carrier / postage | Amount | Every date legible on it | Other marks |
|---|---|---|---|---|---|---|---|
| 1 | p5, nearest white envelope | "Young, Spiegel & Hosp, LLP. / 301 N. Canon Dr., Suite 300 / Beverly Hills, CA 90210" (printed, upper left) | Handwritten: "Halsey Minor / 602 Punta Del Mar / Kukulcan Boulevard / Zona Hotelera / 77500 Cancún, QRO, Mexico" | USPS Retail label: "U.S. POSTAGE PAID / FCMI LE / BEVERLY HILLS, CA 90210" | **$3.15** | **"JAN 05, 202[?]"**. "JAN 05" confirmed: day "05" won 50/50 settings against 06/08/03/30/25/15/09. Final year digit is **6 or 8, unresolved** (font test leaned 8, 37:10, but see the method caveat under #7). | Barcode number "00495"; serial "S2324K502949-03" (won against 502849: 33:10, last glyph 45:3). A faint rotated strip along the left edge was **not transcribed**. |
| 2 | p5, 2nd white envelope | not examined (printed address box visible; crops not viewed) | not examined | USPS Retail label: "U.S. POSTAGE PAID / FCMI LE / BEVERLY HILLS, CA 90210" | **$13.00** (won 50/50 against $15.00/$18.00/$13.60/$16.00) | **"DEC 30, 2025"** (best reading). "DEC" confirmed (50/50 against OCT/NOV/JAN/FEB). "30" and the final "5" are the best fit (28/50 against "30, 2023" 10, "31, 2025" 7, "20, 2025" 5) but **not certain**. | "00495" (as seen); serial "S232[?]K50[?][?]41-[?]" (not resolved) |
| 3 | p5, 3rd white envelope | not examined | not examined | USPS Retail label ("U.S. POSTAGE PAID / FCM[?] LE / BEVERLY HILLS, CA 9021[?]") | "$3.[?]5" — looks like $3.15; the template test did not decide ($3.75 35, $3.15 8, $3.16 7) | Date line present but **illegible** [?] | serial illegible |
| 4 | p5, 4th white envelope | not examined | not examined | label present (Retail type) | **not examined / not resolved** | **not examined** | — |
| 5 | p5, orange/kraft padded envelope (5th item) | not examined | not examined | small label at left plus label at right | **not resolved** (blurred) | **not examined** | Yellow sticky note (text not resolved). The images cannot show whether this is the same envelope as #7. |
| 6 | p5, far end | — | — | — | — | — | At least 5 stacks of loose printed paper and 1 small white item. **Not identifiable** as envelopes; contents not legible. |
| 7 | **p6**, orange/kraft envelope (top of photo) | "Young, Spiegel & Hosp, LLP. / 301 N. Canon Dr., Suite 300 / Beverly Hills, CA 90210" (printed, upper left) | not visible (covered by the papers on top) | USPS Retail label. The "U.S. POSTAGE PAID / class / city" lines are cut off by the top edge of the photo. | **$29.70** | **"JAN 30, 202[?]"**. See the "2026-01-30" finding below. | "00495"; serial "[S2324K]502949-03" (the bracketed part is faint) |
| 8 | p6, white envelope(s) under the note sheet | partial, rotated 90°: "Yo[?]" / "30[?]" | not visible | partial "Retail" label edge | not visible | none visible | — |

### Mark dated 2026-01-30 — exactly where

- The only Jan-30 mark in Exhibit A is the **date line of the USPS Retail label on the orange/kraft envelope photographed on p6** (envelope #7). It is the top line of the photo, just left of "$29.70". In the native p6 image it sits at x≈2620–2790, y≈0–22.
- Reading: **"JAN 30, 202[?]"**.
  - "JAN": won 50/50 settings against JUN/JUL/DEC/FEB/MAR/MAY.
  - "30": won 50/50 against 20/28/26/29/39/80. The same method was first checked on this "30" (50/0 against 36/38).
  - "202": legible.
  - **The 4th digit is either "6" or "8" and I could not resolve it at this resolution** (digit ≈14.5 px tall, blur σ≈1.2 px).
- Evidence on the 4th digit:
  - At high zoom it looks like an "8". Dark ink runs continuously down the right side of the upper part.
  - But there is no left-side waist pinch: measured −0.76 px. Known "0"s measure −0.66 / −1.18, a "6" built from this label's own "9" measures −0.66, and synthetic "8"s at the same blur measure +0.04 to +0.25.
  - Against the label's own "9"s turned to "6" (tight boxes), "6" scored higher: 0.855 vs 0.654 and 0.735 vs 0.576. With looser boxes the result was mixed.
  - Rendered-font matching split: "2028" led 31 vs "2026" 14 on the whole string, while "2026" led 28 vs 17 on the last glyph.
  - **Report as "JAN 30, 202[6 or 8 — unresolved]".** No numeric "01/30/2026" or "JAN 30 2026" appears anywhere else in pp4–15.

## FRONT DESK / RECEIPT RECORDS

### A. Handwritten note on the clipped sheet (p6, Exhibit A) — verbatim, line breaks as written

> Yo Francisco Javier Franco morales recibi el correo.
> del Señor Halsey Minor el día 24 de Febrero sin
> Ricibir ninguna Nota solo el correo Por Parte del Personal
> de correoS de Mexico

- Below the note: handwritten name "Francisco Javier / Franco morales." followed by a stylised initials/signature mark (**not legible**).
- Line 3: the first letter of "Ricibir" looks overwritten (R over r). The last letter of "Nota" could also be read "o".
- **No year is written.** No date other than "24 de Febrero".
- *Literal English translation (mine):* "I Francisco Javier Franco Morales received the mail. of Mr. Halsey Minor on the day 24 of February without receiving any note, only the mail, on the part of the staff of Correos de México [Mexican postal service]."

### B. "ENTREGADO" stamp (identical on p6 note, p8, p9, p10)

> PUNTA DEL MAR CANCUN / S.A DE C.V. / PMC160822IT5 / **ENTREGADO** / [script logo] Punta del mar

- *Translation:* "ENTREGADO" = "DELIVERED".
- **The stamp carries no date.**
- **No building log or register is shown anywhere in Exhibits A–C.**

### C. Exhibit B (1) — Building manager declaration (pp8–10)

**Caption (p8):**
"Final Document for Submission / SUPERIOR COURT OF THE STATE OF CALIFORNIA / COUNTY OF LOS ANGELES / CASE NO. / NÚM. DE CASO: 24STFL00432 / CASE NAME / NOMBRE DEL CASO: Shannon Minor v. Halsey Minor / DECLARATION OF BUILDING MANAGER REGARDING RECEIPT OF MAIL / (DECLARACIÓN DE LA GERENCIA DEL EDIFICIO SOBRE LA RECEPCIÓN DE CORRESPONDENCIA) / (Special Appearance / Comparecencia Especial) / ENGLISH TEXT / I, [handwritten: María Fernanda Sánchez Pérez], declare as follows:"

**English text, verbatim:**
- **¶1** "I am an adult over the age of 18. I am the Manager at the residential apartment building located at: Punta Del Mar, Kukulcan Boulevard, Hotel Zone, 77500 Cancún, Quintana Roo, Mexico. In my capacity as Manager, I hold ultimate accountability for the building's operations, I oversee the front desk staff, and I manage the official receipt of mail for our residents."
- **¶2** "On **February 24, 2024**, our front desk received a single, unusual delivery of mail from the Mexican Postal Service directed to the resident, Halsey Minor."
- **¶3** "I am fully aware of my employees' actions and the events that occur in this building, and I have verified these facts directly with my staff. Specifically, the postal worker dropped off exactly ten (10) different envelopes/packages all at the exact same time. The sender listed on these packages was Lance Spiegel / opposing counsel's law firm in the United States."
- **¶4** "The Mexican postal worker simply dropped the packages at the front desk and left. The postal worker did not ask my staff to sign for them, did not ask the resident to sign for them, and did not collect any official return receipt or signature whatsoever."
- **¶5** "My staff and I observed that the postmarks on these packages were from much earlier dates, including early December 2023, despite them all arriving in a single batch on February 24, 2024."
- **¶6** "Upon receiving this large, un-receipted delivery, my staff called the resident's unit to inform them packages had arrived."
- **¶7** "Shortly after, the resident's girlfriend, [handwritten: Julia Mironova], came downstairs to the front desk. My staff handed the entire batch of ten (10) sealed packages directly to her under my authority."
- **¶8** "Because I hold accountability for this property, I am the same individual who previously signed and stamped an initial written statement confirming this exact delivery. I am now executing this formal declaration and affixing the official stamp of our building (Punta Del [p10:] Mar Cancun S.A. de C.V.) next to my signature below to authenticate my identity, my managerial authority, and the absolute truth of these facts."
- **Perjury clause** "I declare under penalty of perjury under the laws of the State of California, United States of America, and the laws of the United Mexican States, that the foregoing is true and correct."

**Execution block (p9):**
"Executed on this 17th day of March, 2026, at Cancún, Quintana Roo, Mexico. (Firmado este día 17 de Marzo de 2026, en Cancún, Quintana Roo, México.) / Signature of Declarant / Firma de la Gerencia [signature] / Printed Name / Nombre en letra de molde: [handwritten: María Fernanda Sánchez Pérez] / Job Title / Cargo: Building Manager (Gerente del Edificio) / [handwritten: **Asistente Administrativo**] / (Place Official Building Stamp Here / Coloque el Sello Oficial del Edificio Aquí)" + stamp.

- *Translation of the handwritten job title:* "Administrative Assistant". It is written under the printed "Building Manager (Gerente del Edificio)".

**Spanish text (p10)** follows the English paragraph for paragraph. Key paragraphs verbatim:
- **¶2** "El **24 de febrero de 2024\***, nuestra recepción recibió una entrega única e inusual de correspondencia por parte del Servicio Postal Mexicano dirigida al residente, Halsey Minor.\*"
  - The asterisks appear after "2024" and after "Minor.". No footnote text is visible.
- **¶5** "Mi personal y yo observamos que los matasellos en estos paquetes tenían fechas mucho más antiguas, incluyendo principios de diciembre de 2023, a pesar de que todos llegaron en un solo lote el 24 de febrero de 2024."
- **¶7** "Poco después, la novia del residente, [handwritten: Julia Mironova], bajó a la recepción. Mi personal le entregó el lote completo de diez (10) paquetes sellados directamente a ella bajo mi autoridad."
- **¶8** ends "(Punta Del Mar Cancun S.A. de C.V.) junto a mi firma a continuación para autenticar mi identidad, mi autoridad gerencial y la absoluta veracidad de estos hechos."
- Closing: "Declaro bajo pena de perjurio, según las leyes del Estado de California, Estados Unidos de América, y las leyes de los Estados Unidos Mexicanos, que lo anterior es verdadero y correcto. / SIGNATURE AND BUILDING STAMP / FIRMA Y SELLO DEL EDIFICIO" + cursive signature + stamp.
- *(Literal translations of the Spanish ¶2/¶5/¶7 match the declaration's own English ¶2/¶5/¶7 above.)*

### D. Exhibit B (2) — Julia Mironova declaration (p11), verbatim

"DECLARATION OF Julia Mironova / I, / Julia Mironova, declare as follows:"
- **¶1** "I am an adult over the age of 18. I reside with Respondent, Halsey Minor, at the apartment building located at Punta Del Mar, Kukulcan Boulevard, Hotel Zone, 77500 Cancún, Quintana Roo, Mexico. I have personal knowledge of the facts set forth herein."
- **¶2** "On **February 24, 2024**, the front desk staff of our apartment building called our unit to inform us that a large delivery of packages had arrived."
- **¶3** "I went downstairs to the front desk. The staff handed me exactly 10 separate packages/envelopes. All of the packages were addressed to Respondent, Halsey Minor, and bore return addresses from Lance Spiegel or his law firm."
- **¶4** "The building staff informed me that the Mexican mail carrier had just dropped them all off at once and left without asking anyone to sign for them."
- **¶5** "I observed that all 10 packages were completely sealed and unopened when the staff handed them to me."
- **¶6** "I immediately carried the 10 sealed packages upstairs to our apartment and handed them directly to Halsey Minor. At the time I handed them to him, they were still completely sealed and unopened."
- **¶7** "I did not sign any postal receipt or legal acknowledgment of service for these documents, nor was I asked to do so by any postal worker or building staff member."
- **Closing** "I declare under penalty of perjury under the laws of the State of California that the foregoing is true and correct. Executed on this 17th day of March, 2026, at Cancún, Quintana Roo, Mexico. [handwritten signature, not transcribed], Declarant"

**Note (what the documents say):**
- Both Exhibit B declarations date the delivery **"February 24, 2024"**. The building manager's also refers to postmarks of **"early December 2023"**.
- No "2026" delivery date appears in Exhibit B. The p6 note gives "24 de Febrero" with no year.
- The legible label dates in Ex. A are DEC 30, 2025 (#2), JAN 05, 202[?] (#1) and JAN 30, 202[?] (#7). **No December-2023 postmark is legible on any photographed item.**

## Exhibit C — documents shown (verbatim headers only)

1. **p13 — [AI-LEAD]** Gmail web screenshot.
   - Search box: "to:akale@beverlyhills.org google looking for him to contacy google".
   - Message row: "Alex Kale" / "akale@beverlyhills.org".
   - Panel headed **"AI Overview"**, beginning "Based on the provided emails, you have repeatedly urged Detective Alex Kale (akale@beverlyhills.org) to contact Google regarding your case:".
   - Bullets name "March 29, 2024", "654 days" and "January 12, 2026".
   - Gmail AI output. **Not evidence; class AI-LEAD.** The last line is cut off.
2. **p14** — Gmail printout.
   - "H M <halsey2005@gmail.com>" / **"Delivery Status Notification (Failure)"** / "google-legal-support@google.com <google-legal-support@google.com>" / "Fri, Dec 5, 2025 at 4:29 PM" / "To: halsey2005@gmail.com".
   - The body refers to "your letter dated 12/04/2025" and is signed "Google Legal Support".
3. **p15** — Gmail printout, page "1/7".
   - Browser header: "3/27/26, 4:17 PM  Gmail - Preservation and Recovery of Evidence – Fourth Formal Request".
   - Subject: **"Preservation and Recovery of Evidence – Fourth Formal Request"**, "3 messages".
   - "halsey2005@gmail.com <halsey2005@gmail.com>  Fri, Jan 9, 2026 at 10:48 PM / Reply-To: halsey@minorventures.com".
   - "To: Alex Kale <akale@beverlyhills.org>, 12-Sharona Nazarian <snazarian@beverlyhills.org>, David Dimond <ddimond@beverlyhills.org>, Sharona Nazarian <Sharona@sharonanazarian.com>, MayorandCityCouncil@beverlyhills.org, Citymanager@beverlyhills.org, lwiener@beverlyhills.org, Nancy Hunt-Coffey <nhuntcoffey@beverlyhills.org>, Elisabeth Albanese <ealbanese@beverlyhills.org>, ccoulter@beverlyhills.org, Chief@bhpd.gov".
   - Body opens "IN RESPONSE / Officer Kale".
   - Footer URL "https://mail.google.com/mail/u/0/?ik=181a6111b0&view=pt&search=all&permthid=thread-a:r8239279416516239409&simpl=msg-a:r-1451902251932348276&simp…  1/7".
   - Pages 2–7 are **not included**.

## WHAT IS NOT SHOWN

- **No proof of service (POS)** and no document stating a mailing date appears anywhere in Exhibits A–C.
- **The contents of the envelopes are not identified.** The loose paper stacks on p5 and the printed text under the p6 note are not legible.
- No tracking-number barcode label, USPS round or wavy cancellation, meter strip, Correos de México postmark or customs form is legible on any item.
- No building log or register. Neither the stamp nor the handwritten note carries a year.
- The declarations say "ten (10)" items. The photos show 5 envelopes on p5 (plus loose papers) and envelopes #7–#8 on p6. **A count of ten cannot be checked from the photos**, and the photos cannot show whether #5 and #7 are the same envelope.
- Not examined in this pass (left unresolved rather than guessed):
  - addressee and return blocks of #2–#5;
  - labels of #4 and #5, and the date line of #3;
  - the sticky note on #5;
  - the left-edge strip on #1.
