# COURT OF APPEAL docket check (appeal from LASC 24STFL00432) — reading notes

- **Reader:** Sonnet 5.5 subagent (claude-sonnet-5-5), 2026-11-01, work window 03:32Z–03:43Z UTC. First read `/home/user/spiegel-thread/INVENTORY/AGENT_RULES.md` in full (7 rules).
- **Class:** the appellate docket was **NOT reached**, so this file holds **no COURT-class docket content**. It is a log of attempts and null results, plus local-lead checks (DATA from earlier readers' notes; not evidence).
- **Rules kept:** web read-only. The only query aimed at the court's case-search host was the public case-search GET for the trial-court case number (§2, rows 6-8): it was blocked or timed out and never answered. No other form, e-mail or account action; no one contacted; no git; nothing on halseyminor.com opened; no AI-generated page used (§6). Only file written in the project: this one. Scratch curl output is in the session scratchpad (§7).
- **Quotation rule:** quoted text is verbatim from the tool output. Times are UTC. Search tools return no per-call time stamp, so for them I give the window between my own `date -u` readings.

---

## 1. Bottom line

| Item | Result |
|---|---|
| Second District case number (B-number) | **NOT FOUND** |
| Docket entries read | **none (0)** |
| Order dismissing the appeal | not seen. **Not ruled out.** |
| Motion to vacate the dismissal / reinstate | not seen. Not ruled out. |
| Remittitur | not seen. Not ruled out. |
| Current status "in the docket's words" | **UNKNOWN. The docket was not reachable by any route the brief allows.** |

The dates in the brief (NOA 6/18/2026; Notice of Default mailed 7/7/2026; Clerk's Notice of Non-Compliance filed 8/10/2026, forwarded "for consideration to dismiss") are not re-verified against the court here. Nothing I read says what happened after 8/10/2026. I draw no inference from the null results below.

---

## 2. Route 1 — California Courts appellate case search (https://appellatecases.courtinfo.ca.gov/), Second District

| # | UTC | Tool | URL | Result (verbatim) |
|---|---|---|---|---|
| 1 | 03:33:16Z-03:33:17Z | curl via proxy | `https://appellatecases.courtinfo.ca.gov/` | `HTTP/2 403`; headers `cf-mitigated: challenge`, `server: cloudflare`, `cf-ray: a537d64d7a097e51-IAD`; body `<title>Just a moment...</title>` (5,389 bytes). |
| 2 | ~03:33:42Z-03:33:45Z (parallel batch; my `date -u` in the batch printed 03:33:44Z) | WebFetch | `https://appellatecases.courtinfo.ca.gov/search.cfm?dist=2` | "The server returned HTTP 403 Forbidden. The response body was not retrieved." |
| 3 | same batch; the error's own stamp is 03:33:42.567Z | `mcp__Exa__web_fetch_exa` (default Exa connector) | same | "web_fetch_exa error (402): You have exceeded your credits limit. Please top up to keep using Exa at dashboard.exa.ai" |
| 4 | same batch | `mcp__Exa_a17196c7__web_fetch_exa` (second Exa connector) | same | Returned only the blank form page text (below). The tool does not say whether the copy was live or cached. |
| 5 | 03:34:22Z-03:34:33Z | curl via proxy | `https://web.archive.org/web/2025/https://appellatecases.courtinfo.ca.gov/search.cfm?dist=2` (I wanted the blank form's field names) | `curl: (35) Recv failure: Connection reset by peer`. Proxy status log: `kind: ws_closed_mid_exchange`, `tunnel closed (code 1006) after 10s; 517 B sent, 39 B received`, `host: web.archive.org:443`, `ts: 2026-11-01T03:34:33.220Z`. |
| 6 | after 03:35:56Z; after 03:36:12Z; after 03:38:18Z (three attempts) | `mcp__Exa_a17196c7__web_fetch_exa` | `https://appellatecases.courtinfo.ca.gov/search/searchResults.cfm?dist=2&query_caseNumber=24STFL00432&search=number&useSession=0` | Each time: "Error fetching URL(s): [that URL]: CRAWL_LIVECRAWL_TIMEOUT" |
| 7 | 03:36:44Z-03:36:45Z | curl via proxy | same query URL as row 6 | `HTTP/2 403`; `cf-mitigated: challenge`; `server: cloudflare`; `server-timing: chlray;desc="a537db616c58d0cc"`; `<title>Just a moment...</title>` (5,838 bytes). |
| 8 | ~03:36:45Z (same batch as row 7) | WebFetch | same query URL | "The server returned HTTP 403 Forbidden. The response body was not retrieved." |
| 9 | 03:39:51Z | curl via proxy | `https://appellatecases.courtinfo.ca.gov/search.cfm?dist=2` | `HTTP/2 403`; `cf-mitigated: challenge`; `cf-ray: a537dff06e0bd6eb-IAD`; `<title>Just a moment...</title>` (5,477 bytes). |

**Row 4, the only page I fetched directly from the court's host** (blank search form; no field names, links or results came through; Exa search results also showed snippets of the site's home page and calendar page, which say nothing about this case):

> California Courts - Appellate Court Case Information | Case Search
> You may choose one of four search options to obtain appellate court case information. Each of these options will take you to a Case Summary screen once you have identified the case number of interest. The four options are:
> ### Search by Court of Appeal or Trial Court Case Number
> Party 1 (required): Party 1 v. Party 2:

**Where the query URL pattern came from.** Exa search results (row-level detail not kept) listed other cases' result pages on this host at URLs of the form `https://appellatecases.courtinfo.ca.gov/search/searchResults.cfm?dist=2&query_caseNumber=<number>&search=number&useSession=0`, headed "Search by Court of Appeal or Trial Court Case Number" with columns "Court of Appeal Case Number", "Trial Court Case Number", "Case Caption". Those pages belong to unrelated cases; I did not record their contents.

**Related read:** `https://appellate.courts.ca.gov/district-courts/2dca` (the Second District's public page), curl at 03:36:45Z: HTTP 200, 232,362 bytes, `<title>2nd District Court of Appeal | District Courts of Appeal</title>`. **Not read in full.** I grepped it for `href` values containing case/docket/appellatecases/courtinfo and found only `https://appellatecases.courtinfo.ca.gov/index.cfm` and `https://appellatecases.courtinfo.ca.gov/search.cfm?dist=2`, so that page points back to the same host.

**Stopped, per the brief ("if it needs a session or a CAPTCHA, record that and stop").** Not attempted: (a) the party-name / caption search, because I do not know the field names (the form text above carries none, and the archive copy was blocked) and every curl/WebFetch request to the host drew the challenge; (b) any way around the Cloudflare challenge (browser automation, header or user-agent spoofing, third-party reader proxies); (c) the site's e-mail notification sign-up.

---

## 3. Route 2 — web searches (no result was opened; titles and snippets only)

Search-tool narrative summaries are tool-generated text; I did not treat them as evidence and rely only on the returned titles and URLs.

| Tool and settings | Query (verbatim) | Window (UTC) | What came back |
|---|---|---|---|
| WebSearch, standard, blocked halseyminor.com | `"Marriage of Minor" California Court of Appeal Second District 2026 Halsey Minor appeal dismissed` | 03:34:40Z-03:35:56Z | 10 links. Captions seen: "IN RE: the Marriage of JESSICA and SAMMER Z. (2026)", "Marriage of Traweek" (courts.ca.gov .../2026-08-28/b336738), "In re Marriage of Jessica L." (Justia d084336), "Sterndahl v. Sterndahl" (Justia b347548), "Marriage of Johnson" (courts.ca.gov .../2026-04-13/b345460). None names Minor. |
| WebSearch, standard, blocked halseyminor.com | `"24STFL00432"` | 03:34:40Z-03:35:56Z | 10 links, all unrelated product, part-number or real-estate pages. No title carries the string. |
| WebSearch, standard, blocked halseyminor.com | `"Minor v. Minor" Second Appellate District California Court of Appeal 2026 Halsey Minor Shannon Minor family law appeal B3` | 03:36:45Z-03:38:18Z | 1 link: "Minor v. Minor" `https://law.justia.com/cases/california/court-of-appeal/2d/184/118.html`. Not opened. The path is a Cal.App.2d reporter cite (184 Cal.App.2d 118), not a B-number docket. |
| WebSearch, standard, blocked halseyminor.com | `Halsey Minor Shannon Minor divorce appeal "Court of Appeal" Los Angeles 2026` | 03:36:45Z-03:38:18Z | 10 links: Justia 2026 list, LAist voter guide, Ninth Circuit No. 21-55360 ("HALSEY MINOR V. USA", a 2022 bankruptcy-tax matter), LASC press-release PDF, Justia "In re X.A." (b350895), two trellis.law coverage pages, lacourt.ca.gov Appeals-and-Appellate, a law-firm blog, LASC Family Law Division. None is the Minor appeal. |
| WebSearch, standard, allowed domains courts.ca.gov, appellate.courts.ca.gov, law.justia.com, courtlistener.com, caselaw.findlaw.com | `"Marriage of Minor" OR "Minor v. Minor" 2026 Second Appellate District order dismissing appeal Los Angeles family` | 03:36:45Z-03:38:18Z | 10 links: Second District Forms / Local Rules & Orders / Practices & Procedures / News & Announcements pages, three Supreme Court minutes PDFs (2/11, 3/11, 4/22/2026), Justia b350895, b348185, b342515. None names Minor. (An earlier try adding casetext.com failed: "API Error: 400 The following domains are not accessible to our user agent: ['casetext.com']".) |
| WebSearch, standard, blocked halseyminor.com | `"Halsey Minor" appeal dismissed Court of Appeal Shannon Minor divorce October 2026` | 03:38:18Z-03:39:51Z | 10 links about unrelated matters (English Halsey v Milton Keynes, other states' appeals, news items). None relevant. |
| WebSearch, extended, blocked halseyminor.com | `appellatecases.courtinfo.ca.gov "MINOR v. MINOR" 2nd Appellate District "24STFL00432"` | 03:38:18Z-03:39:51Z | 1 link: the same Justia 184 Cal.App.2d 118. |
| `mcp__Exa_a17196c7__web_search_exa` | `"Marriage of Minor" Second District Court of Appeal 2026 Halsey Minor Shannon Minor appeal 24STFL00432` | 03:34:22Z-03:34:40Z | Unrelated: a 1968 Florida DCA case and similar "minor" (juvenile) hits. |
| same | `appellatecases.courtinfo.ca.gov 2nd Appellate District docket (register of actions) MINOR v. MINOR trial court case number 24STFL00432 Los Angeles County Superior Court` | 03:34:40Z-03:35:56Z | The blank search-form page, the site home page, the 2dca page, `calendar.cfm?dist=2`, a third-party explainer (californiacourt.us), and result pages for unrelated B-numbers (not recorded). **No page for this case.** |
| same | `"Minor" "Halsey" appeal dismissed "Court of Appeal" Second Appellate District 2026 default notice designate record rule 8.121` | 03:34:40Z-03:35:56Z | Other matters: Ninth Cir. 21-55360 (2022), Fla. 3d DCA Minor v. Brunetti (2010), C.D. Cal. 2021 tax opinions, CourtListener docket 2:18-cv-00731 (Halsey Minor v. Bill Laggner, filed 2018). None concerns the 2026 appeal. |
| same | `Minor v. Minor 24STFL00432 Los Angeles Superior Court family law case docket register of actions Shannon Minor Halsey Minor` | 03:36:45Z-03:38:18Z | LASC and re:SearchLA portal pages, a library guide, a UniCourt LA family-search landing page, a UniCourt page for a different 2004 San Francisco case with the same-named petitioner, an AI-branded site's page for a different LASC case (not used). **No hit for 24STFL00432 or any B-number.** |
| same | `Search Results - 2nd Appellate District Search by Party Name Minor Halsey case caption MINOR v. MINOR appellatecases.courtinfo.ca.gov` | 03:36:45Z-03:38:18Z | Form page, home page, 2dca page, calendar page, result pages for unrelated B-numbers (not recorded), and two old Justia/HallApproved "Minor" opinions (1963, 1980). **Not this case.** |
| `mcp__CourtListener__search`, type `o`, court `calctapp`, filed_after 2026-01-01 | `"Marriage of Minor"` | 03:36:45Z-03:38:18Z | query_id `dc11ccbc`: `"count": 0`. |
| `mcp__CourtListener__search`, type `o`, court `calctapp`, filed_after 2025-06-01 | `"Halsey Minor" OR "Shannon Minor" OR 24STFL00432` | 03:36:45Z-03:38:18Z | query_id `15a12bd8`: `"count": 0`. Caveat: opinions only (it cannot hold a docket entry or a non-opinion order), and I did not verify its coverage of 2026 Second District unpublished opinions. |

---

## 4. Could not reach, and why (consolidated)

1. **Appellate case search, any query:** Cloudflare managed challenge to curl (rows 1, 7, 9); WebFetch returned only "HTTP 403 Forbidden" (rows 2, 8). Not defeated, by instruction.
2. **Default Exa connector:** HTTP 402, credits exhausted (row 3).
3. **Second Exa connector on the query URL:** `CRAWL_LIVECRAWL_TIMEOUT` three times (row 6). It served only the blank form page.
4. **Wayback Machine copy of the blank form:** connection reset in the proxy tunnel (row 5).
5. **Party-name / caption search:** not attempted (§2, "Stopped").
6. **Trial-court side after 7/13/2026:** not within this brief. The newest LASC register printout in the collection is dated 7/13/2026 (§5).

---

## 5. Local-lead checks (DATA from earlier readers' notes; the underlying PDFs were not opened)

- `READING_NOTES/WRITS_2026-04-28_and_appeal_notice.notes.md`, lines 99-127 read. Its transcription of the Clerk's Notice filed 08/10/2026: "REVIEWING COURT CASE NUMBER:" (blank); "To: ... [✓] 2ND District Court of Appeal / Ronald Reagan State Building / 300 S. Spring Street / 2nd Floor, North Tower Los Angeles, CA 90013"; body "The above-entitled appeal record consisting of the following is herewith forwarded for consideration to dismiss the appeal pursuant to California Rules of Court, rule 8.842, 8.874, or 8.924." The attached 7/7/2026 Notice of Default: "COURT OF APPEAL CASE NUMBER:" blank. The caption on the notice reads "PLAINTIFF AND RESPONDENT : SHANNON MINOR"; "DEFENDANT AND APPELLANT : HALSEY MINOR". The caption the Court of Appeal uses is unknown to me.
- `READING_NOTES/DOCKET_24STFL00432.notes.md`: lines 1-40 read, plus grep hits for appeal terms (not read in full). Entries quoted: "6/18/2026 | Appeal - Notice of Appeal/Cross Appeal Filed General Appeal | Respondent"; "6/26/2026 | Appeal - Notice of Filing of Notice of Appeal | (none shown)"; "7/7/2026 | Appeal - Notice of Default Issued for NOA filed 6/18/2026. DEFAULT FOR DESIGNATION. | Respondent". Its §1 states: "Result: no register printout dated after 7/13/2026 was found on Drive."
- Grep for a whole-word `B3dddddd` number across `/home/user/spiegel-thread` (excluding `EVIDENCE_REGISTER.tsv`): no matches. In `EVIDENCE_REGISTER.tsv`: 0 whole-word matches and 0 rows containing "court of appeal", "second district" or "appellate". A looser case-insensitive match hit 2 rows, both inside Gmail message-id hex strings (`1979e2dcb382217d`, `19ae64fb3079084e`), not case numbers.
- Grep of `READING_NOTES/` for appeal terms hit 3 files: the WRITS notes (10 lines), `BEHAVIOR_g_writs_schwenke_2026.notes.md` (1 line: Schwenke's e-mail mentioning the "Notice of Non-Compliance in the appeals case"; no appellate number), and `ENVELOPE_PHOTOS_originals.notes.md` (1 line, "Non-Compliance with Marsy's Law", unrelated).
- The DOCKET notes mention AI-LEAD Google Docs (a "KEY DATES LOCKED" register and "DOCKET ALERT" docs). I did not open them.

---

## 6. AI-generated / excluded material

- Nothing on halseyminor.com was opened or cited.
- Search-tool narrative summaries (WebSearch) are tool-generated; not used as evidence.
- An AI-branded case-prediction site (aicasepredict.com) appeared in one Exa result, for a different LASC case; not used.
- Justia snippets carry the notice "Some case metadata and case summaries were written with the help of AI"; no Justia summary is relied on.
- Result pages for unrelated cases on the court's host and a UniCourt page for a different 2004 case surfaced in Exa results; their contents are unrelated and are not recorded here.

## 7. Files written outside the project (temporary curl output only; no docket content)

Under `/tmp/claude-0/-home-user/9a86eccf-071d-5c97-88ae-ef129ec55f9d/scratchpad/`: `dl_home/` (row 1), `dl_query/` (row 7), `dl_form/` (row 9), `dl_newsite/` (the 2dca page, 232,362 bytes), `dl_wayback_form/` (row 5 header only). Only Cloudflare challenge pages and the courts' own 2dca page are in them.

## 8. Ways to close the gap (not done by me)

- Someone in an ordinary browser can run the Second District "Search by Court of Appeal or Trial Court Case Number" query for `24STFL00432`, and a party/caption search for "Minor", at `https://appellatecases.courtinfo.ca.gov/search.cfm?dist=2`. I did not test whether the challenge clears in a normal browser. The page to capture is the case's docket with every entry and date, plus the case summary, saved with a date and time.
- Not searched under this brief: the appellant's own mail or e-mail for any Court of Appeal notice, and the LASC register after 7/13/2026.
