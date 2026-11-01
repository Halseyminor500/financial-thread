# Jurisdiction and crime-report intake — what the official sources say

**VERIFIED AT SOURCE — as of 2026-11-01** · topic file `jurisdiction_and_intake` · answers items 1–7 of the clerk brief for hypotheticals P1–P4 · research support only, not legal advice · **no opinion is recorded on whether any hypothetical occurred**

Source classes used below: **OFFICIAL** = government page, data service or published document read as bytes through curl; **OFFICIAL-VIA-CONNECTOR** = government page whose origin refused automated access, text taken from the Exa connector (entries say so); **PARTY-TERMS** = a private party's published contract text (not law, not a regulator statement); **THIRD-PARTY** = unauthenticated copy hosted by someone else; **AI-LEAD** = prose produced by a search tool, used only to find URLs and never quoted as evidence (AGENT_RULES rule 6).

## Result at a glance

| # | Question | Status | What the sources say (details and exact words in the numbered entries) |
|---|---|---|---|
| 1 | Police agency for 301 N. Canon Dr., Beverly Hills and for 111 N. Hill St., Los Angeles | **VERIFIED** | BHPD (City of Beverly Hills, 464 N. Rexford Dr.): the City's own address locator lists 301 N CANON DR and the City's boundary line encloses it (my computation, entry 1.4). LAPD Central Division / Central Bureau, Reporting District 122, for 111 N. Hill St. (City of Los Angeles GIS, entry 1.5). LAPD's address-lookup form was **not** submitted. |
| 2 | LA County DA statement of how crimes are reported | **VERIFIED via connector** (origin blocks bots) | "All crimes should be reported to the police agency in the area where the crime occurred", plus a short list of circumstances in which the DA takes reports, including "criminal conduct by members of the judicial system" (2.1). The words quoted in the brief ("must be reported to the police for a proper investigation") were **not** found verbatim on the DA pages read. |
| 3 | Venue: PEN 781 and PEN 118 place language | **VERIFIED** | PEN 781, 118 and adjacent PEN 27, 777, 778, 778a, 784.7 read from the Legislature's data and cross-checked against the live leginfo pages (3.1–3.6); PEN 502(j) (P2) quoted in 3.5. |
| 4 | State Bar rule for complaints involving matters pending in court | **PARTIAL** | No calbar.ca.gov page or PDF fetched contains the words "must defer to the decisions of the courts". Closest published statements are quoted (4.1–4.5); the wording appears only in a third-party-hosted, unauthenticated excerpt (4.7). |
| 5 | Regulator of Ally Bank and its complaint route | **VERIFIED** (FDIC data) | FDIC BankFind data: state charter, main office Utah, Fed member, primary federal regulator FED, insured by DIF, CFPB flag 1 (5.1–5.2); complaint routes quoted (5.3–5.6). No source retrieved says an account restriction is, or is not, a police matter (5.8). |
| 6 | USPIS mail fraud (federal, note only) | **VERIFIED** | "Any fraud that uses the U.S. Mail … is mail fraud." The old postalinspectors.uspis.gov URL now lands on a not-found page (6.1–6.4). |
| 7 | LAPD / BHPD reporting routes; victim abroad | **VERIFIED as to what the pages say** | Phone and online routes quoted. No LAPD or BHPD page retrieved addresses a victim located abroad; the only residence-related lines are identity-theft lines and LAPD's "courtesy report" rule (7.1–7.5). |

## How this file was produced (read first)

1. **Rules and scope.** Read `/home/user/spiegel-thread/INVENTORY/AGENT_RULES.md` first (read-only; write only in the named folder; contact no one; no web forms; quote verbatim; mark AI output AI-LEAD; state only what the document says). This is the only file written in the project. Raw downloads and scripts were kept in the session scratchpad. No git command was run.
2. **Search tools.** WebSearch and Exa search outputs were used only to discover URLs. Their prose is AI-LEAD and none of it is quoted as evidence. Every quotation below comes from a page, data service or document fetched afterwards, except the one search-result sentence in 4.7, which is flagged there.
3. **How quotations were made.** curl through the session proxy (CA bundle `/root/.ccr/ca-bundle.crt`) → raw bytes saved → visible text extracted by script (HTML) or `pdftotext -layout` (PDF) → each quotation cut **by script** from that text by start and end phrase, so nothing was retyped, and then re-checked as a substring of the source text. Rendering: whitespace collapsed to single spaces; the space that tag boundaries introduce before , . ; : ) and after ( was removed; curly quotes and apostrophes are as in the source; bullets in PDFs show as •; footnote markers are not included. JSON/YAML fragments are shown in code blocks with whitespace collapsed only. Entries that rest on a connector's text say so, and that text was copied from the connector output into a scratch file before extraction (it was not byte-compared with the origin HTML).
4. **Blocked or failed routes (not circumvented).** `da.lacounty.gov` and `public.gis.lacounty.gov`: HTTP 403 Imperva/Incapsula bot challenge to curl (02:57:16Z, 03:03:35Z). `leginfo.legislature.ca.gov`: HTTP 403 Cloudflare challenge to curl (02:57:23Z). `www.ffiec.gov` National Information Center page for Ally Bank: HTTP 403 CAPTCHA page (03:09:26Z). `gis.beverlyhills.org/VBH/`: HTTP 403 (03:01:27Z). `cdn.ripoffreport.com` copy of an OCTC letter: HTTP 403 (03:16:08Z). `www.beverlyhills.org/gis`: connection reset by the origin (03:22:15Z; proxy log: tunnel closed mid-exchange, no policy denial). A State Bar PDF URL returned by a search (`.../2025-10/Filing-Complaint-Against-Attorney.pdf`) returned HTTP 404 (03:05:54Z). The first Exa connector (`mcp__Exa__web_fetch_exa`) returned HTTP 402, credits exceeded (03:05:15Z). The second connector (`mcp__Exa_a17196c7__*`, account label TRUTH) worked and supplied the DA text and the live leginfo cross-checks.
5. **Forms and contacts.** No form was submitted and no one was contacted. In particular: the LAPD "Find Your Local Police Station" address lookup (a POST form), the LAPD Community Online Reporting (Coplogic) flow, the BHPD forms, and every regulator complaint form were **not** used. Only GET requests (and HEAD and byte-range GET requests for the Legislature ZIP) to public pages and public GIS/data services (ArcGIS REST query URLs, Census geocoder, FDIC API) were made.
6. **Statute text.** The leginfo HTML pages are behind a Cloudflare challenge to curl, so the statute text was read from the Legislature's own bulk-data publication `https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` (HTTP range reads; Last-Modified Mon, 26 Oct 2026 04:26:08 GMT; every entry passed its ZIP CRC-32; same method as `LAW/INDEX.md`), and the seven sections reproduced in 3.1–3.4 (PEN 781, 118, 27, 777, 778, 778a, 784.7) were then compared paragraph by paragraph with the live leginfo page text returned by the second Exa connector (all matched exactly); for PEN 502 the bulk-data record has the same SHA-256 as the earlier file records and the live page's subdivision (j) was compared by eye; PEN 782, 783, 784 and 790 were not compared (Appendix B).
7. **Not every word was read.** Web pages: I read the main content of each cited page, not navigation or footers. Long documents were searched and only the cited passages read: State Bar Rules of Procedure (10,009 text lines; read Rule 5.21), State Bar SB 211 report (4,724 lines; read the passages around "defer"), LAPD Manual Volume 5 (2,037 lines; read 030.05, 030.25, 030.63, 030.65 and the DR-number note), BHPD Policy Manual (37,834 lines; read policies 100 in part, 322 and 330 in part), Ally Deposit Agreement (2,237 lines; read the passages quoted and their neighbours), FDIC property dictionary (read the 15 field blocks quoted or named). Each such entry repeats this limit.

## Item 1 — Which police agency serves 301 N. Canon Dr., Beverly Hills and 111 N. Hill St., Los Angeles

### 1A. Beverly Hills Police Department (BHPD) and the City of Beverly Hills

#### 1.1 · BHPD address and non-emergency number (City of Beverly Hills website) — OFFICIAL
- **URL fetched:** <https://www.beverlyhills.org/548/Police-Department> · HTTP 200 · **2026-11-01T03:00:48Z** · label `bh_pd`
- **Verbatim:**
  > Beverly Hills Police Department 464 N. Rexford Drive Beverly Hills, CA 90210 Emergencies: 9-1-1 Non-emergencies: 310-550-4951

- **Verbatim (same page, "Online Services" menu list):**
  > Online Services Fingerprinting Lost & Found Pay / Contest Parking Citations Permit Information Charitable Solicitation Parade & Assembly Permits Private Security Registration Form Property Release Request Public Records Requests PRA Request Form PRA Video Request Form Security Assessment Request Special Alert Registry Traffic Collision Reports Vacation Watch Request Form

- **Establishes:** The City's website gives BHPD's address as 464 N. Rexford Drive, Beverly Hills, CA 90210 and a non-emergency number of 310-550-4951; the quoted Online Services menu has no item named for a "crime report" or "police report" (it has Lost & Found and Traffic Collision Reports).
- **Read:** main content of the page; navigation not read.

#### 1.2 · BHPD is the City's municipal police department; facility address — OFFICIAL
- **URL fetched:** <https://www.beverlyhills.org/561/Department-History> · HTTP 200 · **2026-11-01T03:15:08Z** · label `bh_history`
- **Verbatim:**
  > On August 1, 1927, the Beverly Hills Police Department was formed as a municipal organization

  > The current police facility is located across the street from City Hall at 464 N Rexford Drive.

- **Establishes:** The City's website says BHPD was formed as a municipal organization (1927) and that its current police facility is at 464 N Rexford Drive.

#### 1.3 · City FAQ on the non-emergency line — OFFICIAL
- **URL fetched:** <https://www.beverlyhills.org/Faq.aspx?QID=331> (final: <https://www.beverlyhills.org/m/faq?cat=44#question-331>) · HTTP 200 · **2026-11-01T03:00:58Z** · label `bh_faq331`
- **Verbatim:**
  > Please call the Non-Emergency Line at 310-550-4951. This number is specifically for the Beverly Hills area.

- **Establishes:** The City says the 310-550-4951 line is specifically for the Beverly Hills area.

#### 1.4 · 301 N. Canon Dr. is inside the City of Beverly Hills limits — OFFICIAL (City GIS) plus U.S. Census Bureau

No city-run "is this address inside the City" lookup page was found. The City's own public ArcGIS REST server (`https://gis.beverlyhills.org/arcgis/rest/services`, copyright text "City of Beverly Hills, CA") was queried instead, by GET only.

**1.4a · The City's address locator returns the address.**
- **URL fetched:** <https://gis.beverlyhills.org/arcgis/rest/services/Comb_Loc101p/GeocodeServer/findAddressCandidates?SingleLine=301+N+Canon+Dr&outFields=*&f=pjson> · HTTP 200 · **2026-11-01T03:01:57Z** · label `gis_bh_geocode_301`
- **Verbatim (JSON as returned, first of the matching candidates):**
  ```
  "spatialReference": { "wkid": 102645, "latestWkid": 2229,
  "address": "301 N CANON DR", "location": { "x": 6440470.5364149138, "y": 1847879.96459122 }
  "Loc_name": "SiteAddressPo1"
  "Match_addr": "301 N CANON DR", "Addr_type": "PointAddress"
  ```
- The response lists 10 candidates; four of them are `"address": "301 N CANON DR"` with `Loc_name` `SiteAddressPo1` and `Addr_type` `PointAddress`, at State Plane coordinates (wkid 102645) (6440470.536, 1847879.965), (6440473.607, 1847879.899), (6440474.041, 1847881.635), (6440475.174, 1847879.418).
- **Establishes:** The City of Beverly Hills' own GIS locator holds 301 N CANON DR as four point-address records.

**1.4b · The City's published City Boundary line encloses those points (my computation).**
- **URL fetched:** <https://gis.beverlyhills.org/arcgis/rest/services/CBH_Boundary/MapServer?f=pjson> · HTTP 200 · **2026-11-01T03:01:46Z** · label `gis_bh_boundary_meta` · service metadata
- **Verbatim (separate JSON fragments of the service metadata, as returned):**
  ```
  "Title": "Beverly Hills City Boundary Line"
  "copyrightText": "City of Beverly Hills, CA"
  "name": "City Boundary"
  "Subject": "REST for VBH public main. For authorized CBH GIS app use only.For informational purposes only. No warranties expressed nor implied"
  ```
- **URL fetched:** <https://gis.beverlyhills.org/arcgis/rest/services/VBH_for_CS_Public_CE2/MapServer?f=pjson> · HTTP 200 · **2026-11-01T03:02:08Z** · label `gis_bh_vbh_meta` · second City service, layer list
  ```
  "id": 3, "name": "City Boundary"
  ```
- **URL fetched:** <https://gis.beverlyhills.org/arcgis/rest/services/VBH_for_CS_Public_CE2/MapServer/3/query?where=1%3D1&outFields=*&returnGeometry=true&outSR=102645&f=json> · HTTP 200 · **2026-11-01T03:02:40Z** · label `gis_bh_boundary_geom` · geometry of layer VBH_for_CS_Public_CE2/MapServer/3 (City Boundary)
- **Verbatim (separate JSON fragments of that response):**
  ```
  "geometryType":"esriGeometryPolyline"
  "LENGTH":86932.903
  ```
- **URL fetched:** <https://gis.beverlyhills.org/arcgis/rest/services/CBH_Boundary/MapServer/0/query?where=1%3D1&outFields=*&returnGeometry=true&outSR=102645&f=json> · HTTP 200 · **2026-11-01T03:22:14Z** · label `gis_bh_boundary2_geom` · geometry of layer CBH_Boundary/MapServer/0; same geometry type, same vertices, `SHAPE.STLength()` 86932.90372736879
- **What I computed (not an attribute the City returned):** both City services return the same single closed line of 997 vertices (identical vertex lists). An even-odd point-in-polygon test places all four `301 N CANON DR` `SiteAddressPo1` points **inside** that line. Controls from the same locator: 455 N REXFORD DR (City Hall address) inside; 464 N REXFORD DR (BHPD address) inside; 8687 MELROSE AVE outside; a walk west from the 301 point along constant y crosses the line between 5,000 and 5,500 coordinate units, so the test does discriminate.
- **Limit stated by the source:** the quoted `Subject` text says "For informational purposes only. No warranties expressed nor implied".
- **Establishes:** The City's published boundary line, as published, encloses the City locator's points for 301 N CANON DR.

**1.4c · The City's parcel and zoning layers at the same point.**
- **URL fetched:** <https://gis.beverlyhills.org/arcgis/rest/services/VBH_for_CS_Public_CE2/MapServer/2/query?geometry=6440470.536414914,1847879.96459122&geometryType=esriGeometryPoint&inSR=102645&spatialRel=esriSpatialRelIntersects&outFields=*&returnGeometry=false&f=pjson> · HTTP 200 · **2026-11-01T03:02:26Z** · label `gis_bh_parcel_q` · VBH_for_CS_Public_CE2/MapServer/2 (Parcels) point query
  ```
  "AIN": "4343012019"
  "PARCELADDRESS": "321 N CANON DR"
  ```
- **URL fetched:** <https://gis.beverlyhills.org/arcgis/rest/services/Zoning/MapServer/2/query?geometry=6440470.536414914,1847879.96459122&geometryType=esriGeometryPoint&inSR=102645&spatialRel=esriSpatialRelIntersects&outFields=*&returnGeometry=false&f=pjson> · HTTP 200 · **2026-11-01T03:02:25Z** · label `gis_bh_zoning_q` · Zoning/MapServer/2 (ZONING) point query
  ```
  "ZONE": "C-3"
  ```
- **Establishes:** At the locator's point the City's Parcels layer returns AIN 4343012019 whose PARCELADDRESS is 321 N CANON DR (not 301), and its Zoning layer returns ZONE C-3; I did not determine why the parcel address differs from 301.

**1.4d · U.S. Census Bureau geocoder (independent, federal).**
- **URL fetched:** <https://geocoding.geo.census.gov/geocoder/geographies/onelineaddress?address=301+N+Canon+Dr%2C+Beverly+Hills%2C+CA+90210&benchmark=Public_AR_Current&vintage=Current_Current&layers=all&format=json> · HTTP 200 · **2026-11-01T03:03:22Z** · label `census_301`
  ```
  "matchedAddress":"301 N CANON DR, BEVERLY HILLS, CA, 90210"
  "GEOID":"0606308"
  "NAME":"Beverly Hills city"
  ```
- **Establishes:** The Census Bureau's address geocoder assigns 301 N CANON DR, BEVERLY HILLS, CA, 90210 to incorporated place "Beverly Hills city" (GEOID 0606308) in the Incorporated Places layer.

**1.4e · The City's own description of its GIS (links the REST server above to the City).**
- **URL fetched:** <https://www.beverlyhills.org/971/Maps-GIS> (final: <https://beverlyhills.org/759/Interactive-Maps-GIS>) · HTTP 200 · **2026-11-01T03:39:19Z** · label `bh_maps` · City page "Interactive Maps (GIS)"
- **Verbatim:**
  > The City of Beverly Hills offers the following Geographic Information System (GIS) Services for residents, businesses, and visitors:

  > The system (a.k.a. Virtual Beverly Hills), is being expanded to offer more geo-enabled citizen engagement facilitating services.

- **Anchor as extracted from the page's HTML (text → href):** `interactive mapping websites and downloadable maps → https://gis.beverlyhills.org/vbhapps/` (fetched 2026-11-01T03:39:32Z, label `bh_vbhapps`; it is a script-driven map viewer whose content cannot be read as text, so it was not used).
- **Verbatim (separate JSON fragment of the metadata of the service queried in 1.4b–1.4c):**
  ```
  REST for Virtual Beverly Hills for Public Facing City Smart Application.
  ```
- **Establishes:** The City says it offers GIS services under the name Virtual Beverly Hills, and the City's REST service queried above describes itself as "REST for Virtual Beverly Hills" (City of Beverly Hills IT/GIS).

### 1B. Los Angeles Police Department (LAPD) and 111 N. Hill St.

**1.5a · The address resolves to a point inside "Los Angeles city" (Census geocoder).**
- **URL fetched:** <https://geocoding.geo.census.gov/geocoder/geographies/onelineaddress?address=111+N+Hill+St%2C+Los+Angeles%2C+CA+90012&benchmark=Public_AR_Current&vintage=Current_Current&layers=all&format=json> · HTTP 200 · **2026-11-01T03:03:23Z** · label `census_111`
  ```
  "matchedAddress":"111 N HILL ST, LOS ANGELES, CA, 90012"
  "coordinates":{"x":-118.246496192834,"y":34.054523799954}
  "NAME":"Los Angeles city"
  ```
- **Establishes:** The Census Bureau geocoder resolves 111 N HILL ST, LOS ANGELES, CA, 90012 to longitude -118.246496192834, latitude 34.054523799954, in incorporated place "Los Angeles city".

**1.5b · City of Los Angeles GIS ("LAHub" LAPD service) — the LAPD Division at that point.**
- **URL fetched:** <https://maps.lacity.org/lahub/rest/services/LAPD/MapServer?f=pjson> · HTTP 200 · **2026-11-01T03:03:42Z** · label `gis_lapd_meta` · layer list of `https://maps.lacity.org/lahub/rest/services/LAPD/MapServer`
  ```
  "id": 3, "name": "LAPD Divisions"
  ```
- **URL fetched:** <https://maps.lacity.org/lahub/rest/services/LAPD/MapServer/3/query?geometry=-118.246496192834,34.054523799954&geometryType=esriGeometryPoint&inSR=4326&spatialRel=esriSpatialRelIntersects&outFields=*&returnGeometry=false&f=pjson> · HTTP 200 · **2026-11-01T03:03:49Z** · label `gis_lapd_q3` · layer 3 point query; layers 2 and 4 (`gis_lapd_q2`, `gis_lapd_q4`) returned the identical record
- **Verbatim (JSON as returned):**
  ```
  "OBJECTID": 633, "REPDIST": 122, "PREC": 1, "APREC": "CENTRAL", "BUREAU": "CENTRAL BUREAU", "BASICCAR": "1A1", "TOOLTIP": "Bureau: CENTRAL BUREAU\\nDistrict: 122\\nDivision: CENTRAL"
  ```
- (The doubled backslash in `TOOLTIP` is in the service's JSON as returned.)
- **Establishes:** At the point for 111 N Hill St, the City of Los Angeles' LAPD service returns Bureau CENTRAL BUREAU, Reporting District 122, Division CENTRAL (field `APREC` = CENTRAL).

**1.5c · City of Los Angeles GIS — the Central station record.**
- **URL fetched:** <https://maps.lacity.org/lahub/rest/services/LAPD/MapServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&f=pjson> · HTTP 200 · **2026-11-01T03:03:51Z** · label `gis_lapd_stations` · layer 0 (LAPD Stations) attribute query
  ```
  "Division": "CENTRAL", "Location": "251 E. 6TH ST.", "Precinct": 1, "TOOLTIP": "CENTRAL Community Police Station\\nStation Number: 1\\nAddress: 251 E. 6TH ST."
  ```
- **Establishes:** The same City GIS lists the CENTRAL Community Police Station, station number 1, at 251 E. 6TH ST.

**1.5d · LAPD's own Central Community Police Station page.**
- **URL fetched:** <https://www.lapdonline.org/lapd-contact/central-bureau/central-community-police-station/> · HTTP 200 · **2026-11-01T02:59:07Z** · label `lapd_central`
- **Verbatim:**
  > Serving the Following Communities: Bunker Hill/Historic Core, Central City East, Chinatown, Civic Center, Downtown Los Angeles, Fashion District, Jewelry District, Little Tokyo, Solano Canyon, South Park-Entertainment, Toy District, Old Bank District, Artists Lofts, Financial District

  > Under the Jurisdiction of: Central Bureau

  > 251 E. 6th Street Los Angeles, CA 90014 213-486-6606 Voice 213-485-9819 TDD/TTY

  > The Central Community Police Station is staffed by approximately 200 sworn and civilian members of the Los Angeles Police Department and is responsible for all police operations in downtown Los Angeles.

- **Establishes:** LAPD's page lists "Civic Center" among the communities the Central station serves, gives the station address (251 E. 6th Street, Los Angeles, CA 90014), places it under Central Bureau, and says it is responsible for all police operations in downtown Los Angeles.
- **Read:** main content of the page. The page does not name 111 N. Hill St.; the address-level result is 1.5b.

**1.5e · LAPD's "Find Your Local Police Station" page (lookup form NOT submitted).**
- **URL fetched:** <https://www.lapdonline.org/find-your-local-police-station/> · HTTP 200 · **2026-11-01T02:59:17Z** · label `lapd_find`
- **Verbatim:**
  > Enter your address below to locate the police station within your community.

- **Anchor as extracted from the page's HTML (text → href):** `Civic Center → https://www.lapdonline.org/lapd-contact/central-bureau/central-community-police-station/`
- **Establishes:** LAPD's page invites an address lookup (a POST form, not submitted here per the no-forms rule) and its community list links "Civic Center" to the Central Community Police Station page.

## Item 2 — The Los Angeles County District Attorney's published statements on how crimes are reported

All `da.lacounty.gov` pages below were refused to curl (HTTP 403 Incapsula challenge, 02:57:16Z) and were read through the second Exa connector, which returned the page text. Timestamps are `date -u` readings: for 2.5–2.8 they are sequential readings taken immediately before and after the connector call (the call falls between them); the FAQ call (2.1–2.4) was issued in the same batch as its clock readings, so its time is approximate. The FAQ and Overview pages were also returned by earlier connector calls (about 03:04Z and 03:05Z) with the same wording (compared by eye).

#### 2.1 · DA Office FAQs — "How do I report a crime?" — OFFICIAL-VIA-CONNECTOR
- **URL fetched:** <https://da.lacounty.gov/about/office-faqs> · **about 2026-11-01T03:15:40Z** (clock readings in the same call batch)
- **Verbatim:**
  > How do I report a crime? All crimes should be reported to the police agency in the area where the crime occurred. If you need to report an emergency, call 911. In certain limited circumstances, the District Attorney's Office takes crime reports for cases such as public corruption, criminal conduct by members of the judicial system, fraud cases in excess of $725,000 and real estate fraud.

- **Establishes:** The DA's FAQ says all crimes should be reported to the police agency in the area where the crime occurred, and lists limited circumstances (public corruption, criminal conduct by members of the judicial system, fraud over a stated dollar amount, real estate fraud) in which the DA's Office takes crime reports.
- **Note on the brief's quotation:** the words "all crimes must be reported to the police for a proper investigation" were searched for in the DA pages read here and were not found verbatim; the FAQ wording is the quotation above.

#### 2.2 · DA Office FAQs — who decides charges — OFFICIAL-VIA-CONNECTOR
- **URL fetched:** <https://da.lacounty.gov/about/office-faqs> · about 2026-11-01T03:15:40Z
- **Verbatim:**
  > Who decides what charges to file, and how do they make that decision? A deputy district attorney reviews cases brought to the District Attorney's Office by local law enforcement agencies. The reports are reviewed in light of current law and whether the case presented by the agency can be proven in court beyond a reasonable doubt.

- **Establishes:** The DA's FAQ says a deputy district attorney reviews cases brought to the DA's Office by local law enforcement agencies.

#### 2.3 · DA Office FAQs — attorney misconduct; Justice System Integrity Division (JSID) — OFFICIAL-VIA-CONNECTOR
- **URL fetched:** <https://da.lacounty.gov/about/office-faqs> · about 2026-11-01T03:15:40Z
- **Verbatim:**
  > Where do I make a complaint about alleged misconduct by an attorney or a person acting as an attorney? The State Bar of California investigates complaints and disciplines attorneys who violate State Bar rules. For information on how to file a complaint, visit www.calbar.ca.gov or call the Attorney Complaint Hotline at (800) 843-9053.

  (the next paragraph on the page, in the same answer:)

  > The District Attorney's Justice System Integrity Division (JSID) investigates and prosecutes criminal conduct by persons who work within the justice system in Los Angeles County, including attorneys, judges, court employees and law enforcement personnel. To contact JSID, call (213) 974-3888.

- **Establishes:** The DA's FAQ refers attorney-misconduct complaints to the State Bar and states that JSID investigates and prosecutes criminal conduct by persons who work within the justice system in Los Angeles County, "including attorneys, judges, court employees and law enforcement personnel", with a phone contact.

#### 2.4 · DA Office FAQs — the DA's jurisdiction — OFFICIAL-VIA-CONNECTOR
- **URL fetched:** <https://da.lacounty.gov/about/office-faqs> · about 2026-11-01T03:15:40Z
- **Verbatim:**
  > What is the District Attorney's jurisdiction? The Los Angeles County District Attorney's Office prosecutes felony crimes throughout Los Angeles County and misdemeanor crimes in unincorporated areas of the county and in all cities except Burbank, Hawthorne, Hermosa Beach, Inglewood, Long Beach, Los Angeles, Pasadena, Redondo Beach, Santa Monica and Torrance.

- **Establishes:** The DA's FAQ lists the cities (Los Angeles included; Beverly Hills not listed) in which the DA does not prosecute misdemeanors.

#### 2.5 · DA Office Overview — how cases come to the DA; Bureau of Investigation — OFFICIAL-VIA-CONNECTOR
- **URL fetched:** <https://da.lacounty.gov/about/office-overview> · **2026-11-01T03:15:46Z–03:15:52Z** (clock readings before and after the connector call)
- **Verbatim:**
  > Deputy district attorneys are prosecutors who represent the people of the State of California. They review investigations conducted by law enforcement agencies and decide whether there is sufficient evidence to file criminal charges. They also decide what charge or charges, if any, are appropriate based on the evidence presented. Prosecutors handle court proceedings, including trials, that may follow the filing of criminal charges.

  > The Los Angeles County District Attorney’s Office maintains a staff of nearly 300 sworn peace officers, known as DA investigators, who conduct some of the most unique, sensitive and complex criminal investigations in law enforcement.

  > DA investigators function primarily to provide prosecution support to deputy district attorneys. They locate and process witnesses and conduct supplemental pretrial investigations to help strengthen the prosecution’s case. In some cases, such as those involving public corruption, they conduct their own independent investigations.

  > The Bureau of Investigation is the county’s fourth largest law enforcement agency. Its staff also assists other law enforcement agencies with vehicular and electronic surveillance, undercover operations and photographic services.

- **Establishes:** The DA's Overview says deputy DAs review investigations conducted by law enforcement agencies and decide whether to file charges; DA investigators function primarily as prosecution support and, in some cases such as public corruption, conduct independent investigations; the Bureau of Investigation is described as the county's fourth largest law enforcement agency.

#### 2.6 · DA "Where to Report Fraud" — OFFICIAL-VIA-CONNECTOR
- **URL fetched:** <https://da.lacounty.gov/contact/forms/fraud-report> · 2026-11-01T03:15:46Z–03:15:52Z
- **Verbatim:**
  > Local Law Enforcement Contact the law enforcement agency that serves the location where the person accused of a crime conducts business/criminal activity or where the victim resides.

- **Establishes:** The DA's page directs fraud reports to the law enforcement agency serving the place where the accused conducts business/criminal activity or where the victim resides, and links LAPD's and the Sheriff's station finders (also listed: California Attorney General, FBI).

#### 2.7 · DA "Forms" page — OFFICIAL-VIA-CONNECTOR
- **URL fetched:** <https://da.lacounty.gov/contact/forms> · 2026-11-01T03:15:46Z–03:15:52Z
- **Verbatim:**
  > In certain, limited circumstances, the Los Angeles County District Attorney's Office takes crime reports for cases such as consumer fraud and real estate fraud.

  > If the loss amount in your case exceeds $750,000.00

- **Establishes:** The DA's Forms page repeats that the DA takes crime reports only in certain, limited circumstances and states a white-collar-fraud loss threshold of USD 750,000, while the FAQ (2.1) states USD 725,000; the two DA pages differ.

#### 2.8 · DA directory entry for JSID — OFFICIAL-VIA-CONNECTOR
- **URL fetched:** <https://da.lacounty.gov/contact/office-directory/justice-system-integrity-division> · 2026-11-01T03:15:46Z–03:15:52Z
- **Verbatim:**
  > Justice System Integrity Division 211 West Temple Street Suite 1200 Los Angeles, CA 90012 Phone: (213) 974-3888

- **Establishes:** The DA's directory lists JSID at 211 West Temple Street Suite 1200 with phone (213) 974-3888.

## Item 3 — Penal Code venue and place language

#### 3.1 · Penal Code § 781 — offense committed in part in one jurisdictional territory and in part in another — OFFICIAL

- **Canonical page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=781> — curl: HTTP 403 Cloudflare challenge; live text via the second Exa connector, bracket 03:20:04Z–03:20:12Z, matched the bulk data paragraph by paragraph (machine-compared).
- **Bulk data:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> entry `LAW_SECTION_TBL_102882.lob` read **2026-11-01T03:11:46Z** · ZIP CRC-32 OK · XML record SHA-256 `bafc0e43cbb9f20858186cb628614e995f9a09bfd68468a05ccd01c862aef762` · version id `id_f6957fd0-6e92-11e3-8818-ebf46b809fe7` · active flag Y
- **Official location:** PART 2. OF CRIMINAL PROCEDURE [681. - 1620.] > TITLE 3. ADDITIONAL PROVISIONS REGARDING CRIMINAL PROCEDURE [777. - 883.] > CHAPTER 1. Of the Local Jurisdiction of Public Offenses [777. - 795.]
- **Official history note:** "Amended by Stats. 2013, Ch. 59, Sec. 2. (SB 514) Effective January 1, 2014."
- **Verbatim (complete section):**
  > Except as provided in Section 923, when a public offense is committed in part in one jurisdictional territory and in part in another jurisdictional territory, or the acts or effects thereof constituting or requisite to the consummation of the offense occur in two or more jurisdictional territories, the jurisdiction for the offense is in any competent court within either jurisdictional territory.

- **Establishes:** PEN 781 gives jurisdiction for an offense committed in part in one jurisdictional territory and in part in another, or whose acts or effects requisite to consummation occur in two or more territories, to "any competent court within either jurisdictional territory", "[e]xcept as provided in Section 923".
- The section's text refers only to the court in which the offense is triable; it does not mention law-enforcement agencies or reports.

#### 3.2 · Perjury place language: PEN 118 and PEN 27(b) — OFFICIAL

- **Canonical page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=118> — curl: HTTP 403 Cloudflare challenge; live text via the second Exa connector, bracket 03:20:17Z–03:20:24Z, matched the bulk data paragraph by paragraph (machine-compared).
- **Bulk data:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> entry `LAW_SECTION_TBL_69289.lob` read **2026-11-01T03:11:45Z** · ZIP CRC-32 OK · XML record SHA-256 `14cada31a67a532c5ec84e487188b81c3b2166dc7340b56c2f72718d795b78cb` · version id `id_6530331d-2920-11d9-9844-b32bb8dfae52` · active flag Y
- **Official location:** PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 7. OF CRIMES AGAINST PUBLIC JUSTICE [92. - 186.36.] > CHAPTER 5. Perjury and Subornation of Perjury [118. - 131.]
- **Official history note:** "Amended by Stats. 1990, Ch. 950, Sec. 2."
- **Verbatim (the place sentence of PEN 118(a)):**
  > This subdivision is applicable whether the statement, or the testimony, declaration, deposition, or certification is made or subscribed within or without the State of California.

- The full section text (oath and penalty-of-perjury wording) is in `LAW/VERIFIED_AT_SOURCE_2026-11-01_PC_perjury_false_evidence.md`; all three paragraphs of PEN 118 read here were matched verbatim to that file.

**PEN 27** (same method)
- **Canonical page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=27> — curl: HTTP 403 Cloudflare challenge; live text via the second Exa connector, bracket 03:20:04Z–03:20:12Z, matched the bulk data paragraph by paragraph (machine-compared).
- **Bulk data:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> entry `LAW_SECTION_TBL_67112.lob` read **2026-11-01T03:11:45Z** · ZIP CRC-32 OK · XML record SHA-256 `bf35a32496fe706ded8bf81d0ec7d7cba62ca39caa559b85661bdbdefa74d6db` · version id `id_650d1a3d-2920-11d9-9844-b32bb8dfae52` · active flag Y
- **Official location:** PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 1. OF PERSONS LIABLE TO PUNISHMENT FOR CRIME [25. - 29.8.]
- **Official history note:** "Amended by Stats. 1993, Ch. 611, Sec. 2. Effective October 1, 1993."
- **Verbatim (subdivision (b)):**
  > (b) Perjury, in violation of Section 118, is punishable also when committed outside of California to the extent provided in Section 118.

- **Verbatim (subdivision (a)(1), also retrieved as an adjacent provision):**
  > (1) All persons who commit, in whole or in part, any crime within this state.

- **Establishes:** PEN 118 states that its subdivision (a) applies whether the statement is made or subscribed within or without California, and PEN 27(b) states that perjury under Section 118 is punishable also when committed outside California to the extent provided in Section 118.
- No perjury-specific venue (county) provision appears in PEN 118 or PEN 27(b); the general venue sections follow (3.3). PEN 27(a)(1) (quoted above): persons who commit, "in whole or in part, any crime within this state" are liable to punishment under the laws of this state.

#### 3.3 · Adjacent sections retrieved because they address offenses with parts in different places (PEN 27(a)(1) is quoted in 3.2) — OFFICIAL

**PEN 777**
- **Canonical page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=777> — curl: HTTP 403 Cloudflare challenge; live text via the second Exa connector, bracket 03:20:17Z–03:20:24Z, matched the bulk data paragraph by paragraph (machine-compared).
- **Bulk data:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> entry `LAW_SECTION_TBL_102824.lob` read **2026-11-01T03:11:45Z** · ZIP CRC-32 OK · XML record SHA-256 `38885d873d7a0b737e43c9959071320d6c272e2cec7eb44a44d080e4365cd10a` · version id `id_6963f1ae-2920-11d9-9844-b32bb8dfae52` · active flag Y
- **Official location:** PART 2. OF CRIMINAL PROCEDURE [681. - 1620.] > TITLE 3. ADDITIONAL PROVISIONS REGARDING CRIMINAL PROCEDURE [777. - 883.] > CHAPTER 1. Of the Local Jurisdiction of Public Offenses [777. - 795.]
- **Official history note:** "Amended by Stats. 1951, Ch. 1674."
- **Verbatim:**
  > Every person is liable to punishment by the laws of this State, for a public offense committed by him therein, except where it is by law cognizable exclusively in the courts of the United States; and except as otherwise provided by law the jurisdiction of every public offense is in any competent court within the jurisdictional territory of which it is committed.

**PEN 778**
- **Canonical page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=778> — curl: HTTP 403 Cloudflare challenge; live text via the second Exa connector, bracket 03:20:17Z–03:20:24Z, matched the bulk data paragraph by paragraph (machine-compared).
- **Bulk data:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> entry `LAW_SECTION_TBL_102880.lob` read **2026-11-01T03:11:45Z** · ZIP CRC-32 OK · XML record SHA-256 `a0a52ebc0ac265bd148dcb59c3d0da16dd03ba036b0b961aeb7a0b7b8250d064` · version id `id_69657854-2920-11d9-9844-b32bb8dfae52` · active flag Y
- **Official location:** PART 2. OF CRIMINAL PROCEDURE [681. - 1620.] > TITLE 3. ADDITIONAL PROVISIONS REGARDING CRIMINAL PROCEDURE [777. - 883.] > CHAPTER 1. Of the Local Jurisdiction of Public Offenses [777. - 795.]
- **Official history note:** "Amended by Stats. 1951, Ch. 1674."
- **Verbatim:**
  > When the commission of a public offense, commenced without the State, is consummated within its boundaries by a defendant, himself outside the State, through the intervention of an innocent or guilty agent or any other means proceeding directly from said defendant, he is liable to punishment therefor in this State in any competent court within the jurisdictional territory of which the offense is consummated.

**PEN 778a(a)**
- **Canonical page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=778a> — curl: HTTP 403 Cloudflare challenge; live text via the second Exa connector, bracket 03:20:04Z–03:20:12Z, matched the bulk data paragraph by paragraph (machine-compared).
- **Bulk data:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> entry `LAW_SECTION_TBL_102881.lob` read **2026-11-01T03:11:46Z** · ZIP CRC-32 OK · XML record SHA-256 `53d505accf9aa13497bb35f96b346d30970c3399dc6ef47b7373da50ebc7e588` · version id `id_69657856-2920-11d9-9844-b32bb8dfae52` · active flag Y
- **Official location:** PART 2. OF CRIMINAL PROCEDURE [681. - 1620.] > TITLE 3. ADDITIONAL PROVISIONS REGARDING CRIMINAL PROCEDURE [777. - 883.] > CHAPTER 1. Of the Local Jurisdiction of Public Offenses [777. - 795.]
- **Official history note:** "Amended by Stats. 2001, Ch. 854, Sec. 39. Effective January 1, 2002."
- **Verbatim:**
  > (a) Whenever a person, with intent to commit a crime, does any act within this state in execution or part execution of that intent, which culminates in the commission of a crime, either within or without this state, the person is punishable for that crime in this state in the same manner as if the crime had been committed entirely within this state.

- **Establishes:** PEN 777: general rule that jurisdiction is in any competent court within the territory where the offense is committed; PEN 778: offense commenced outside the State and consummated within it; PEN 778a(a): act within the state in part execution of the intent, with the crime culminating within or without the state.

#### 3.4 · PEN 784.7 (queried in the brief with a question mark) — OFFICIAL

- **Canonical page:** <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=784.7> — curl: HTTP 403 Cloudflare challenge; live text via the second Exa connector, bracket 03:20:17Z–03:20:24Z, matched the bulk data paragraph by paragraph (machine-compared).
- **Bulk data:** <https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip> entry `LAW_SECTION_TBL_61583.lob` read **2026-11-01T03:11:47Z** · ZIP CRC-32 OK · XML record SHA-256 `180b308574bc47c6659be929a692e09b9fa51fa4f0753f13203335748957c773` · version id `id_e6a3e3ed-8257-11ee-bcfe-9f16e66157a6` · active flag Y
- **Official location:** PART 2. OF CRIMINAL PROCEDURE [681. - 1620.] > TITLE 3. ADDITIONAL PROVISIONS REGARDING CRIMINAL PROCEDURE [777. - 883.] > CHAPTER 1. Of the Local Jurisdiction of Public Offenses [777. - 795.]
- **Official history note:** "Amended by Stats. 2023, Ch. 666, Sec. 1. (AB 806) Effective January 1, 2024."
- **Verbatim (the lead clause of each subdivision; the rest of the section concerns hearings under Section 954 and written agreement of district attorneys):**
  > (a) If more than one violation of Section 220, except assault with intent to commit mayhem, 261, 264.1, 269, 286, 287, 288, 288.5, 288.7, or 289 or former Section 262 or 288a occurs in more than one jurisdictional territory

  > (b) If more than one violation of Section 243.4, 261.5, 273a, 273.5, 646.9, or any crime of domestic violence as defined in subdivision (b) of Section 13700 occurs in more than one jurisdictional territory

  > (c) If more than one violation of Section 236.1, 266h, or 266i occurs in more than one jurisdictional territory

- **Machine check of the whole section text:** Sections 118, 132, 134 and 502 do not appear in it (118: False, 132: False, 134: False, 502: False).
- **Establishes:** PEN 784.7 applies by its terms to repeated violations of the Penal Code sections it names (listed above); Sections 118, 132, 134 and 502 are not among them.
- Retrieved but not reproduced (not requested or not on point by their text): PEN 782 (boundary within 500 yards), 783 (vessels, trains, vehicles, aircraft), 784 (kidnapping, inveigling), 790 (murder, manslaughter); entries in Appendix B. PEN 779 and 780 returned no row in the data.

#### 3.5 · P2 — PEN 502 subdivision (j): the venue words — OFFICIAL

- **Read first (as instructed):** `/home/user/spiegel-thread/LAW/VERIFIED_AT_SOURCE_2026-11-01_PC_computer_502.md`. Subdivision (j) is at its line 151 and restated in its ELEMENTS item 7.
- **Independent re-check:** `pubinfo_2025.zip` entry `LAW_SECTION_TBL_61669.lob` read 2026-11-01T03:24:22Z, CRC-32 OK, XML record SHA-256 `6eef3b31611b417549b70d4d1a2b4c5449ef42ed75e42b6e2ebaef32fc3e214e` (identical to the SHA-256 recorded in that earlier file); live page <https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=502> via the second Exa connector, bracket 03:24:25Z–03:24:31Z: subdivision (j) identical.
- **Official location:** PART 1. OF CRIMES AND PUNISHMENTS [25. - 680.4.] > TITLE 13. OF CRIMES AGAINST PROPERTY [450. - 593g.] > CHAPTER 5. Larceny [484. - 502.9.] (from `LAW/VERIFIED_AT_SOURCE_2026-11-01_PC_computer_502.md`)
- **Official history note:** "Amended by Stats. 2019, Ch. 16, Sec. 1. (AB 814) Effective January 1, 2020."
- **Verbatim (subdivision (j), complete):**
  > (j) For purposes of bringing a civil or a criminal action under this section, a person who causes, by any means, the access of a computer, computer system, or computer network in one jurisdiction from another jurisdiction is deemed to have personally accessed the computer, computer system, or computer network in each jurisdiction.

- **Machine check of the whole section text:** the words "venue", "jurisdictional" and "territor…" occur 0, 0 and 0 times; "jurisdiction" occurs 3 times, all in subdivision (j).
- **Establishes:** The only venue-type wording in PEN 502 is subdivision (j): a person who causes, by any means, the access of a computer, computer system, or computer network in one jurisdiction from another jurisdiction "is deemed to have personally accessed" it "in each jurisdiction", for purposes of a civil or criminal action under the section.

#### 3.6 · Currency of the statute text — OFFICIAL

- Snapshot: `pubinfo_2025.zip`, Last-Modified Mon, 26 Oct 2026 04:26:08 GMT, entries dated 2026-10-25. Newer incremental files `pubinfo_Mon` (27 Oct), `pubinfo_Wed` (29 Oct), `pubinfo_Thu` (30 Oct) and `pubinfo_Fri` (24 Oct, older) were downloaded on 2026-11-01 at about 03:19Z and contain no `LAW_*` table (entries: `BILL_ANALYSIS_TBL`, `BILL_HISTORY_TBL`, `BILL_TBL`).
- Bill scan: all 2,254 chaptered bill versions in `BILL_VERSION_TBL` (990 dated 2025, 1,263 dated 2026, 1 dated 2024) were range-read (CRC-32 OK for all; 0 failures) and searched for "Section(s) … of the Penal Code is/are amended/added/repealed". **No bill names PEN 27, 777, 778, 778a, 781, 784.7, 118, 126, 127, 132, 134, 135, 182, 502, 518, 519, 523 or 524.** Positive control: the same pattern matched 168 Penal Code statements in 67 other bills. Limit: this scan finds bills that use the standard amending sentence; it does not read bill digests.

## Item 4 — The State Bar of California on complaints involving matters pending in, or decided by, a court

**Not found:** the words "must defer to the decisions of the courts" (from the brief's 2026 closing letter) do not appear in any calbar.ca.gov page or PDF fetched for this item (the pages and PDFs below were searched by script for "defer", "pending", "abate" and "decisions of the court"). What the State Bar does publish on the subject is quoted in 4.1–4.5.

#### 4.1 · "Want To File a Complaint" — what the State Bar can and cannot do — OFFICIAL
- **URL fetched:** <https://www.calbar.ca.gov/basic-page/want-file-complaint> (final: <https://www.calbar.ca.gov/public/file-complaints-claims/want-file-complaint>) · HTTP 200 · **2026-11-01T03:05:52Z** · label `cb_want` · the `/basic-page/...` URL redirects to this page
- **Verbatim (items under "The State Bar cannot"):**
  > Reverse a court decision or settlement or ask a court to reverse an earlier decision or settlement

  > Act as your advocate in a dispute or litigation

- **Verbatim (item under "The State Bar can"):**
  > Refer criminal conduct to law enforcement

- **Verbatim (same page):**
  > If your issue is a fee dispute, poor legal strategy, or a case outcome that you disagree with, it probably does not qualify as attorney misconduct.

- **Establishes:** The State Bar's page says it cannot reverse a court decision or settlement or ask a court to reverse one, and cannot act as an advocate in a dispute or litigation; it can refer criminal conduct to law enforcement.
- **Read:** the page's main content.

#### 4.2 · State Bar "Frequently Asked Questions: Complaints & Claims" — OFFICIAL
- **URL fetched:** <https://www.calbar.ca.gov/frequently-asked-questions-complaints-claims> · HTTP 200 · **2026-11-01T03:05:54Z** · label `cb_faq`
- **Verbatim:**
  > The State Bar’s Office of Chief Trial Counsel handles complaints about unethical attorney conduct from several different sources, including clients, family and friends of clients, courts, opposing counsel, members of the public or other third parties, and anonymous submissions.

  > If criminal conduct is suspected, the State Bar may also refer the matter to a law enforcement agency for investigation and potential prosecution.

- **Establishes:** The State Bar FAQ says OCTC takes complaints from several sources including courts, and that when criminal conduct is suspected the State Bar may refer the matter to a law enforcement agency.

#### 4.3 · Rules of Procedure of the State Bar, rule 5.21(C)(3) — OFFICIAL
- **URL fetched:** <https://www.calbar.ca.gov/sites/default/files/portals/0/documents/rules/Rules-of-Procedure.pdf> · HTTP 200 · **2026-11-01T03:05:59Z** · label `cb_rop` · PDF; title page reads as quoted below
- **Verbatim (title page):**
  > Rules of Procedure of the State Bar of California January 1, 2026

- **Verbatim (rule heading):**
  > Rule 5.21 Limitations Period (A) Time Limit for Complaint.

- **Verbatim (rule 5.21(C), lead-in and paragraph (3)):**
  > (C) Tolling. The time limit for the filing of an initial pleading under section (A) above is tolled:

  > (3) while civil, criminal, or administrative investigations or proceedings based on the same acts or circumstances as the violation, including but not limited to proceedings seeking to determine whether a violation has occurred, the scope of the violation, the harm resulting from the violation, or any actions to be taken to remediate the violation, including efforts to collect funds owed as the result of the violation, are pending with any governmental agency, court, or tribunal;

- **Establishes:** Rule 5.21(C)(3) tolls the time limit for filing disciplinary charges while civil, criminal or administrative investigations or proceedings based on the same acts are pending with any governmental agency, court, or tribunal.
- **Read:** rule 5.21 only; the 10,009-line PDF was otherwise searched, not read.

#### 4.4 · State Bar report "Senate Bill 211 Case Processing Standards Proposal" (2022) — OFFICIAL, dated
- **URL fetched:** <https://www.calbar.ca.gov/sites/default/files/portals/0/documents/reports/Senate-Bill-211-Case-Processing-Standards-Proposal.pdf> · HTTP 200 · **2026-11-01T03:05:57Z** · label `cb_sb211_pdf` · PDF
- **Verbatim (title page):**
  > Senate Bill 211 Case Processing Standards Proposal October 28, 2022 Revised November 4, 2022

- **Verbatim (page 8):**
  > The case processing times reported in this section exclude the time when investigations are deferred pending civil or criminal litigation addressing similar issues. This “time in deferral” is also excluded from the proposed case processing standards. As is discussed in Part Three, this accords with practices in three states reviewed by the State Bar and provides OCTC with the necessary prosecutorial discretion to await a resolution of issues by a civil or criminal court when there is a substantial overlap with issues posed by a disciplinary complaint.

  > This practice also serves to avoid potential differences in the resolution of issues in different forums and interference with law enforcement investigation and prosecution of criminal matters, and it provides appropriate deference to civil or criminal court resolution of issues.

- **Verbatim (page 32):**
  > OCTC currently defers further review and investigation of some complaints based on pending criminal or civil litigation involving similar material allegations.

- **Establishes:** A State Bar report to the Legislature dated October 28, 2022 (revised November 4, 2022) says OCTC currently defers further review and investigation of some complaints based on pending criminal or civil litigation involving similar material allegations, and describes that as prosecutorial discretion and deference to civil or criminal court resolution of issues.
- **Limit:** a 2022 document; whether OCTC's 2026 practice is unchanged is not stated by any source retrieved. The passages around "defer" were read; the whole 4,724-line PDF was not.

#### 4.5 · State Bar online complaint page and complaint form — OFFICIAL
- **URL fetched:** <https://apps.calbar.ca.gov/complaint/> · HTTP 200 · **2026-11-01T03:05:58Z** · label `cb_online` · online complaint page
- **Verbatim:**
  > The State Bar is not a court that can provide civil remedies to you.

- **URL fetched:** <https://www.calbar.ca.gov/sites/default/files/2025-09/Attorney_Misconduct_Complaint.pdf> · HTTP 200 · **2026-11-01T03:05:56Z** · label `cb_form_pdf` · PDF form
- **Verbatim:**
  > If your complaint involves a court case, please provide information (if known) in this section.

- **Establishes:** The State Bar says it is not a court that can provide civil remedies, and its complaint form asks for related court-case information.

#### 4.6 · Search result for the brief's exact words on calbar.ca.gov — OFFICIAL (negative result)
- Scripted search of the extracted text of `cb_want`, `cb_faq`, `cb_online`, `cb_after`, `cb_second`, `cb_form_pdf`, `cb_sb211_pdf`, `cb_rop` for the patterns "defer to the decision", "decision(s) of the court(s)" and "must defer": **0 matches for "defer to the decision" and for "must defer" in every document**, and one incidental match for "decision of the court" in `cb_rop` (a rule on withdrawing a request for review in the State Bar Court, unrelated) (labels in Appendix A). A WebSearch restricted to calbar.ca.gov and statebarcourt.ca.gov also returned no page containing the words (AI-LEAD; not quoted).
- **Establishes:** No calbar.ca.gov page or PDF fetched states the brief's quoted words.

#### 4.7 · The same words in a third-party-hosted excerpt of an OCTC letter — THIRD-PARTY, unauthenticated
- **Where seen:** an Exa connector search highlight (about 03:06Z) of a PDF letter on a third-party complaint-posting site, `cdn.ripoffreport.com/95x70/docs_o/r1537258-ynwvte-wsroilqod6`, dated May 2025, addressed to a complainant other than the brief's, concerning a different matter. My direct fetch of that host returned HTTP 403 at 03:16:08Z. Names are omitted here. Authenticity not verified.
- **Verbatim (the sentence, as shown in the highlight):**
  > However, the State Bar cannot intervene on your behalf, cannot rule upon the merits of your contentions, and must defer to the decisions of the courts on these points.

- **Establishes:** Wording identical to the brief's phrase appears in an unauthenticated third-party-hosted letter attributed to OCTC (May 2025); it is not a State Bar publication.

## Item 5 — P4: who supervises Ally Bank, and the complaint routes

#### 5.1 · FDIC BankFind data record for Ally Bank — OFFICIAL
- **URL fetched:** <https://api.fdic.gov/banks/institutions?filters=CERT%3A57803&limit=1> · HTTP 200 · **2026-11-01T03:07:38Z** · label `fdic_ally_full` · FDIC public API behind BankFind: `institutions?filters=CERT:57803`; a first query by name, `NAME:"Ally Bank"`, at 2026-11-01T02:57:17Z (label `p_bankfind`) returned total 1, the same CERT
- **Verbatim (JSON fragments as returned; the record has about 150 fields, these are the ones relied on):**
  ```
  "NAME":"Ally Bank"
  "CERT":57803
  "CITY":"Sandy"
  "STNAME":"Utah"
  "STALP":"UT"
  "BKCLASS":"SM"
  "CHRTAGNT":"STATE"
  "REGAGNT":"FED"
  "INSAGNT1":"DIF"
  "CFPBFLAG":1
  "CFPBEFFDTE":"2011-07-21"
  "FED_RSSD":"3284070"
  "ACTIVE":1
  "REPDTE":"06/30/2026"
  "NAMEHCR":"ALLY FINANCIAL INC"
  "index":{"name":"institutions_20261030090007","createTimestamp":"2026-10-30T11:58:49Z"}
  ```
- **Establishes:** FDIC's data lists Ally Bank (CERT 57803, Sandy, Utah; active; Federal Reserve ID 3284070) with chartering agent STATE, institution class SM, primary regulator code FED, primary insurer DIF and CFPB flag 1, as of the 2026-06-30 report date, in a data index created 2026-10-30.

#### 5.2 · FDIC's own definitions of those codes — OFFICIAL
- **URL fetched:** <https://api.fdic.gov/banks/docs/institution_properties.yaml> · HTTP 200 · **2026-11-01T03:07:48Z** · label `fdic_props` · YAML data dictionary for the same API
- **Verbatim:**
  > SM - Commercial bank, state charter, Fed member, and supervised by the Federal Reserve Bank (FRB)

  > A code indicating the federal regulatory agency that provides primary supervision over an institution. OCC=Office of the Comptroller of Currency; FDIC=Federal Deposit Insurance Corporation; OTS=Office of Thrift Supervision; STATE=State; FED=Federal Reserve.

  > State (includes U.S. Territories) - Chartering authority for institutions that are not chartered by the OCC or OTS

  > Indicates secondary supervision by CFPB ('0' - not supervised by CFPB, '1'- secondarily supervised by CFPB)

  > The state abbreviation of the location of the institution's main office.

- **Establishes:** Per FDIC's dictionary, class SM is a state-chartered commercial bank, Fed member, supervised by the Federal Reserve Bank; REGAGNT FED means Federal Reserve; chartering agent State means chartered by a state rather than the OCC or OTS; the main-office state is Utah; CFPBFLAG 1 means secondary supervision by CFPB. (The dictionary does not name the state regulator; the Utah DFI page in 5.6 does for Utah state banks.)
- **Read:** the 15 field blocks quoted or named; not the whole 94,832-byte file. The record's `REGAGENT2` field is the empty string while `CFPBFLAG` is 1; I did not reconcile that with the dictionary's formula for the flag.

#### 5.3 · Federal Reserve — complaint route — OFFICIAL
- **URL fetched:** <https://www.federalreserveconsumerhelp.gov/> · HTTP 200 · **2026-11-01T03:08:26Z** · label `fr_frch` · Federal Reserve Consumer Help home page
- **Verbatim:**
  > Filing your complaint directly with your bank’s regulator is the most efficient way to have your concerns addressed. Use the FDIC’s BankFind tool to discover who supervises your bank and file your complaint directly with that agency for a faster response.

  > If you are still unsure of the correct agency to submit your concerns to, you may file your complaint here and we’ll refer it for you or provide information on how to file a complaint with the appropriate agency.

- **URL fetched:** <https://www.federalreserve.gov/faqs/credit_12666.htm> · HTTP 200 · **2026-11-01T03:08:26Z** · label `fr_faq` · Board FAQ page
- **Verbatim:**
  > Although the Federal Reserve looks into every complaint that involves banks it regulates, it does not have the authority to resolve every problem. There are several federal agencies who handle complaints about banks and other financial institutions, so the Federal Reserve may connect you with or forward your complaint to another federal regulator.

  > Last Update: August 02, 2013

- **Establishes:** Federal Reserve Consumer Help says to find the bank's supervisor with FDIC's BankFind and file with that agency, or to file with Federal Reserve Consumer Help for referral; the Board's FAQ (last updated August 2013, as the page shows) says the Fed looks into every complaint involving banks it regulates but cannot resolve every problem.

#### 5.4 · FDIC — complaint route and scam-victim guidance — OFFICIAL
- **URL fetched:** <https://www.fdic.gov/consumer-resource-center/consumer-complaint-process> · HTTP 200 · **2026-11-01T03:08:28Z** · label `fdic_cp` · Consumer Complaint Process page
- **Verbatim:**
  > Last Updated: August 14, 2025

  > While the FDIC may insure the funds at your bank, the FDIC may not be your bank’s federal regulator. It’s important you contact the correct regulator.

  > You can find out which agency regulates your bank on BankFind. There are four different federal banking regulators.

  > If your concerns involve a bank outside of the FDIC’s direct supervisory oversight, we will refer your correspondence to the appropriate regulatory agency.

  > What do you do if you are a scam victim? Report the incident to the Federal Trade commission (FTC)

  > If you received any correspondence via the Internet, you should report the incident to the Internet Crime Complaint Center (ICCC) at www.ic3.gov. The ICCC is a central repository for complaints related to Internet fraud, developed by the Federal Bureau of Investigation and the National White Collar Crime Center. Complaints filed via this website may be referred to law enforcement/regulatory agencies for possible investigation.

- **Establishes:** FDIC says it may insure a bank's funds without being its federal regulator, refers complaints about banks outside its direct supervision to the appropriate regulator, and tells scam victims to report to the FTC and, for internet correspondence, to IC3.

#### 5.5 · CFPB — complaint route and scam guidance — OFFICIAL
- **URL fetched:** <https://www.consumerfinance.gov/complaint/> · HTTP 200 · **2026-11-01T03:08:30Z** · label `cfpb_complaint`
- **Verbatim:**
  > We’ll share your complaint with the company so it can review and respond to the issues you’ve described.

  > If you suspect a scam, there are a few important steps you should take right away. Contact your local police or sheriff’s office to report the scam.

- **Establishes:** CFPB says it shares a complaint with the company for response, and, on suspected scams, tells consumers to contact their local police or sheriff's office.

#### 5.6 · Utah Department of Financial Institutions — OFFICIAL
- **URL fetched:** <https://dfi.utah.gov/resources/helpful-links/file-a-complaint/> · HTTP 200 · **2026-11-01T03:08:29Z** · label `utah_dfi`
- **Verbatim:**
  > The DFI does not regulate all financial institutions in Utah.

  > State Banks Utah DFI and other options may apply. Please call us at 801-538-8830 before submitting a complaint

- **Establishes:** Utah DFI says it does not regulate all financial institutions in Utah and that for State Banks "Utah DFI and other options may apply" (call first). Whether Ally Bank appears on the DFI's institution list was not checked (its lookup tool was not used).

#### 5.7 · Ally Bank Deposit agreement and disclosures — PARTY-TERMS (private contract text; not law, not a regulator statement)
- **URL fetched:** <https://www.ally.com/content/dam/pdf/bank/ally-bank-deposit-agreement.pdf> · HTTP 200 · **2026-11-01T03:09:35Z** · label `ally_dep_pdf` · the `/docs/bank/deposit-agreement/` URL redirects to this PDF
- **Verbatim:**
  > Deposit agreement and disclosures Effective October 10, 2026

  > The laws and regulations of the United States and (to the extent not preempted) the State of Utah will govern all our actions relating to your account and the terms of this Agreement.

  > In certain circumstances, as described below, we may delay, decline, cancel or reverse transactions, or otherwise restrict or freeze some or all of the funds in your account. These circumstances are for your protection and ours, and may include: if we suspect that any transaction may involve illegal activity or may be fraudulent, if we suspect you may be the victim of a fraud, scam or financial exploitation, even if you have authorized the transaction, or if we believe that doing so is necessary to avoid loss or reduce risk. You agree that we will have no liability to you for any action we take under this paragraph, and that we may take such action without prior notice to you, except as prohibited by law.

  > We have discretion to react in ways we believe are appropriate, including restricting or closing your account or asking a court to take custody of funds, in any of the following situations: • Third parties make claims on your account • We receive conflicting instructions from joint owners or authorized signers • We become involved in or concerned about a dispute between you and a joint owner or authorized signer

  > If a legal process (such as an attachment, garnishment, levy or other state or federal legal process) is brought against your account, we may limit or prevent withdrawals or transfers from your account until the legal process is satisfied or dismissed.

- **Establishes:** Ally's own published terms (effective October 10, 2026) say Utah law governs to the extent not preempted and list as circumstances in which it may restrict or freeze funds: suspected illegal activity or fraud, suspected scam victimization, third-party claims on the account, and legal process such as attachment, garnishment or levy.
- **Read:** the clauses quoted and their neighbours (about 115 of 2,237 text lines).

#### 5.8 · What the sources do and do not say about "civil/regulatory vs police" — note
- The brief's characterization (civil/regulatory, not a police matter unless a court order or fraud is shown) is **not stated in those terms by any source retrieved**.
- What the sources say, in the quotations above: the regulators' pages describe complaint routes (5.3–5.6); FDIC's page tells scam victims to report to the FTC and IC3 (5.4) and CFPB's page tells consumers who suspect a scam to contact local police or the sheriff (5.5); Ally's own terms list suspected illegal activity or fraud, third-party claims and legal process among the circumstances in which it may restrict or freeze funds (5.7).
- No source retrieved says whether a bank's restriction of a customer's accounts is, or is not, a matter for the police, and none addresses a bank referring a customer by telephone to an attorney's office.

## Item 6 — U.S. Postal Inspection Service (federal; noted only)

USPIS is a federal agency. Nothing below assesses whether P1 fits any federal statute.

#### 6.1 · "Mail Fraud" definition — OFFICIAL
- **URL fetched:** <https://www.uspis.gov/tips-prevention/mail-fraud> · HTTP 200 · **2026-11-01T03:10:16Z** · label `us_mailfraud` · `https://postalinspectors.uspis.gov/` (the host named in the brief) redirects (301) to `https://www.uspis.gov/`; this page is the current mail-fraud page
- **Verbatim:**
  > Any fraud that uses the U.S. Mail™—whether it originates in the mail, by phone, or online—is mail fraud.

- **Establishes:** USPIS defines mail fraud as any fraud that uses the U.S. Mail, whether it originates in the mail, by phone, or online.

#### 6.2 · "What We Do" — OFFICIAL
- **URL fetched:** <https://www.uspis.gov/about/what-we-do> · HTTP 200 · **2026-11-01T03:10:17Z** · label `us_whatwedo`
- **Verbatim:**
  > The Postal Inspection Service enforces over 200 federal statutes related to crimes that involve the postal system, its employees, and its customers.

  > Our jurisdiction is worldwide.

- **Establishes:** USPIS says it enforces over 200 federal statutes related to crimes that involve the postal system, its employees, and its customers, and that its jurisdiction is worldwide.

#### 6.3 · "Report a Crime" page — OFFICIAL
- **URL fetched:** <https://www.uspis.gov/report> · HTTP 200 · **2026-11-01T03:10:18Z** · label `us_report`
- **Verbatim:**
  > Our Investigation starts with your report

  > Report suspected fraud and scams related to the U.S. Mail™, including: • sweepstakes scams • lottery scams • online auctions • chain letters • investments • romance scams

  > Or call USPIS: 1-877-876-2455

- **Establishes:** USPIS's report page lists mail fraud among reportable crimes (types listed) and gives 1-877-876-2455.

#### 6.4 · Old mail-fraud URL on postalinspectors.uspis.gov — OFFICIAL (negative)
- **URL fetched:** <https://postalinspectors.uspis.gov/investigations/MailFraud/MailFraud.aspx> (final: <https://www.uspis.gov/investigations/MailFraud/MailFraud.aspx>) · HTTP 200 · **2026-11-01T03:10:19Z** · label `us_old_mailfraud` · `.../investigations/MailFraud/MailFraud.aspx`, redirected to the www.uspis.gov path shown
- **Verbatim:**
  > This suspected page is at large. Postal Inspectors are on the lookout for a page that matches your description.

- **Establishes:** The old URL no longer serves the mail-fraud definition (HTTP 200 but a not-found page); the definition is at <https://www.uspis.gov/tips-prevention/mail-fraud> (6.1).

## Item 7 — LAPD and BHPD crime-reporting routes, and whether a victim abroad is addressed

#### 7.1 · LAPD "File A Police Report" page — OFFICIAL
- **URL fetched:** <https://www.lapdonline.org/file-a-police-report/> · HTTP 200 · **2026-11-01T02:59:29Z** · label `lapd_file`
- **Verbatim (types listed as reportable online):**
  > Types of Crime Reports That Can Be Filed Online: Harassing Phone Calls: Any person who repeatedly, with the intent to annoy, telephones or makes contact by means of an electronic communication. For example, immediate hang-ups, obscene language, emails, text messages with no known suspects. Lost Property: Personal property that was unintentionally left by its true owner. For example, property left behind at an unknown location or left behind with no attempt to retrieve it. Vandalism: Any person who maliciously damages, destroys or defaces the property of another person. For example, knocking over a mailbox, spray painting a wall, or throwing a rock through a window. Theft: Personal property taken from a publicly accessible location. For example, a package is taken from your porch; or, you left your wallet behind in a restaurant, but when you attempted to go back to retrieve it, the wallet was no longer there. Theft from Vehicle: Theft from an unlocked or locked vehicle. Minor Traffic Collisions: Minor injuries and you have exchanged information Hit and Run: Damage caused by another vehicle in which the driver should have left information or fled the scene without stopping to provide information. VICE Tips: Tips may be reported filer may remain anonymous. Narcotics Tips: Tips may be reported filer may remain anonymous. Identity Theft: Crime location should be reported as the filer’s home residence address (regardless of where the crime is believed to have occurred), and reported to the filer’s local law enforcement agency for investigation. Hate Incident: A hate incident is any non-criminal act, including words, directed against a person(s) based on that person’s actual or perceived protected characteristics. Hate incidents do not violate criminal law statutes. Hate incidents are generally protected free speech under the First Amendment of the U.S. Constitution.

- **Verbatim (eligibility criteria):**
  > IS COMMUNITY ONLINE REPORTING RIGHT FOR YOU? Your incident must meet the following criteria: The incident is not an emergency. The incident occurred within the City of Los Angeles. You must be at least 18 years old. No one was injured as a result of this incident. There are no known suspects. The incident did not occur on the state highway. No firearms were involved in the incident. You must have internet access and an email address.

- **Verbatim (phone routes):**
  > If your incident did not meet the criteria for online reporting, please dial 1-877-ASK-LAPD (Toll Free) (1-877-275-5273) (Voice and TDD/TTY) for Non-Emergency Police Response.

  > Filers can also call 424-359-4636, to receive a text message with a link to file an online report from a mobile device.

  > IF THIS IS AN EMERGENCY OR CRIME IN PROGRESS, PLEASE CALL 911.

- **Verbatim (follow-up and station lookup):**
  > Supplemental Reports cannot be filed online. To add any additional information, please wait until you have received your final report with a LAPD report number and call your local police station to speak with the detective assigned to your case.

- **Establishes:** LAPD offers a Community Online Reporting Service for the listed types when the eight quoted criteria are met (among them: the incident occurred within the City of Los Angeles, there are no known suspects, and the reporter is 18 or older with internet access and an email address); otherwise it directs the reporter to 1-877-ASK-LAPD (and offers a text-message link via 424-359-4636).
- **Machine checks of the page text:** none of the terms 'perjur', 'forg', 'ante-dat', 'computer', 'hack', 'bank', 'account', 'mail fraud' occurs in the quoted list of online types. Words in the pattern `abroad|foreign|internation|mexic|out of state|outside (the) city/state/country|non-resident|live outside|home residence|victim … resid…` occur 1 time(s) on the whole page, namely in the identity-theft line: "Identity Theft: Crime location should be reported as the filer’s home residence address (regardless of where the crime is believed to have occurred), and reported to the filer’s local law enforcement agency for investigation."
- **Read:** the whole page's main content (183 extracted lines). The form itself (Coplogic) was not opened.

#### 7.2 · LAPD Central Community Police Station — phone directory — OFFICIAL
- **URL fetched:** <https://www.lapdonline.org/lapd-contact/central-bureau/central-community-police-station/> · HTTP 200 · **2026-11-01T02:59:07Z** · label `lapd_central`
- **Verbatim:**
  > Non-emergency To report any non-emergency crime 1-877-ASK-LAPD Central Area Front Desk General inquiries and information 213-486-6606

- **Establishes:** LAPD's Central station page lists 1-877-ASK-LAPD for reporting any non-emergency crime and a Front Desk number labelled "General inquiries and information"; no retrieved LAPD page states in terms that a crime report can be made in person at a station.

#### 7.3 · LAPD Department Manual, Volume 5, sections 030.05, 030.25, 030.65 — OFFICIAL, dated
- **URL fetched:** <https://lapdonlinestrgeacc.blob.core.usgovcloudapi.net/lapdonlinemedia/VOLUME_5_Q3_2025_Updates_from_4_1_25_to_9_30_25_.pdf> · HTTP 200 · **2026-11-01T03:14:12Z** · label `lapd_manual5` · PDF on LAPD's media host
- **Verbatim (page header):**
  > Los Angeles Police Department Manual Quarter 3 – 2025 Volume 5

- **Verbatim (030.05, courtesy reports):**
  > Courtesy Reports. Courtesy reports shall only be completed when the following conditions exist: • The person reporting is a Los Angeles City resident; and, • Exigent circumstances exist (e.g., there is an active mutual aid task force in operation; travel distance to the concerned jurisdiction is extreme); and, • The concerned jurisdiction does not complete a telephonic report; and, • Prior approval is obtained from a supervisor or detective. Note: Courtesy reports shall not be taken telephonically.

- **Verbatim (030.25):**
  > 030.25 DETERMINING AREA OF OCCURRENCE. The area of occurrence is the Area in which the incident occurred, except:

- **Verbatim (030.65):**
  > 030.65 COURTESY REPORTS. A DR number shall be obtained and used on all reports where the location of occurrence is outside the jurisdiction of the Los Angeles Police Department.

- **Establishes:** Under LAPD's manual, courtesy reports (reports of incidents outside LAPD's jurisdiction) are completed only when the reporter is an LA City resident, exigent circumstances exist, the concerned jurisdiction does not take a telephonic report and a supervisor or detective approves; courtesy reports are not taken telephonically.
- **Limit:** the document is the Quarter 3 – 2025 update (file name: updates from 4/1/25 to 9/30/25); whether a later edition supersedes it was not checked. Read: sections named above only.

#### 7.4 · BHPD — City pages and Policy Manual — OFFICIAL
- **URL fetched:** <https://www.beverlyhills.org/597/Calling-the-Police> · HTTP 200 · **2026-11-01T03:00:56Z** · label `bh_calling` · "Calling the Police"
- **Verbatim:**
  > Calls for general police services such as parking problems, construction or loud parties should be reported on the non-emergency telephone line at 310-550-4951 or 310-550-4952.

  > You do not have to identify yourself when you are reporting a crime, unless you are the victim of the crime.

- **URL fetched:** <https://www.beverlyhills.org/705/Property> · HTTP 200 · **2026-11-01T02:59:03Z** · label `bh_property` · "Property"
- **Verbatim:**
  > You may call non-emergency dispatch at 310-550-4951 to file a police report for lost or stolen property.

- **URL fetched:** <https://www.beverlyhills.org/sitemap> · HTTP 200 · **2026-11-01T03:38:54Z** · label `bh_sitemap` · City site map, Police Department section
- **Verbatim (the section's Contact Us and Crime Information pages; the Online Services pages are quoted in 1.1):**
  > Contact Us Anonymous Tip Calling the Police Comments, Complaints & Commendations Evidence Submission Portal Get Involved Crime Information Anonymous Tips Cold Case Missing Persons CrimeMapping.com Crime Statistics Interactive Crime Map Megan's Law Information

- **Machine check of the whole site-map text:** none of the phrases 'file a', 'online report', 'crime report', 'police report', 'report a crime' occurs; the site map's service list also contains "Report a Concern" (`/139/Report-a-Concern`, which redirects to the City's general askBH request form at `beverlyhills.comcate.com`, fetched 2026-11-01T03:39:21Z as `bh_concern`; its text is script-driven and was not examined).
- **URL fetched:** <https://www.beverlyhills.org/DocumentCenter/View/3557/Department-Policy-Manual-PDF> (final: <https://www.beverlyhills.org/DocumentCenter/View/3557/Department-Policy-Manual?bidId=>) · HTTP 200 · **2026-11-01T03:14:29Z** · label `bh_policy_manual` · BHPD Department Policy Manual (Lexipol), PDF at `https://www.beverlyhills.org/DocumentCenter/View/3557/Department-Policy-Manual-PDF`; PDF creation date shown by `pdfinfo`: Fri Jul 24 00:41:36 2026 UTC
- **Verbatim (footer of the page carrying policy 322.2.1 and 322.2.7):**
  > Copyright Lexipol, LLC 2026/07/24, All Rights Reserved. Report Preparation - 198 Published with permission by Beverly Hills Police Department

- **Verbatim (policy 322.2.1):**
  > 322.2.1 CRIMINAL ACTIVITY When an officer responds to a call for service and determines a crime has occurred, the member shall document the incident regardless of whether a victim desires prosecution.

- **Verbatim (policy 322.2.7):**
  > 322.2.7 ALTERNATE REPORTING FOR VICTIMS Reports that may be submitted by the public via online or other self-completed reporting processes include: 1. Lost property. 2. Misdemeanor thefts of property, other than firearms or materials that threaten public safety, when there is no suspect information, serial number or ability to trace the item. 1. Misdemeanor thefts of cellular telephones may be reported even though they have a serial number. 3. Misdemeanor vandalism with no suspect information and no hate crime implications. 4. Vehicle burglaries with no suspect information or evidence. 5. Stolen vehicle attempts with no suspect information or evidence. 6. Annoying telephone calls with no suspect information. 7. Identity theft without an identifiable suspect. 8. Online or email fraud solicitations without an identifiable suspect and if the financial loss classifies the crime as a misdemeanor. 9. Hit-and-run vehicle collisions with no suspect or suspect vehicle. 10. Supplemental property lists.

  > Members may refer victims to online victim assistance programs (e.g., Federal Communications Commission (FCC) website for identity theft, Internet Crime Complaint Center (IC3) website for computer crimes).

- **Verbatim (policy 330.2(a), identity theft):**
  > For incidents of identity theft occurring outside this jurisdiction, officers should observe the following: 1. For any victim not residing within this jurisdiction, the officer may either take a courtesy report to be forwarded to the victim’s residence agency or the victim should be encouraged to promptly report the identity theft to the law enforcement agency where he or she resides.

- **Establishes:** BHPD's pages give 310-550-4951 (and 4952) for non-emergency reports by phone, including lost or stolen property, and the City's site map lists no page named for filing a crime or police report; BHPD's policy manual lists report types that may be submitted by the public "via online or other self-completed reporting processes" (without naming a web address), and, for identity theft only, says an officer "may either take a courtesy report to be forwarded to the victim's residence agency or the victim should be encouraged to promptly report" to the agency where the victim resides.
- **Read:** policies 322 (report preparation) and 330 (identity theft) and the start of 100; the 37,834-line manual was otherwise searched, not read.

#### 7.5 · Whether a non-resident victim, or one abroad, may report by phone or online — what the pages say
- **LAPD online/phone page (7.1):** the eight eligibility criteria are quoted in 7.1; none refers to where the reporter lives or is located; the only residence-related wording on the page is the identity-theft line in 7.1; the page does not mention reporters outside the United States.
- **BH pages searched by script** (`bh_pd`, `bh_calling`, `bh_faq331`, `bh_property`, `bh_online`, `bh_contact`, `bh_crimeinfo`, `bh_records`) for the same word pattern: no matches. The BH pages quoted in 1.1–1.3 and 7.4 do not address a victim who lives outside Beverly Hills or outside the United States; the only non-resident wording found is policy 330.2(a) (identity theft), quoted in 7.4.
- **LAPD manual (7.3):** the courtesy-report conditions quoted there (LA City resident; not taken telephonically) concern incidents outside LAPD's jurisdiction.
- **Toll-free number:** LAPD's page labels 1-877-ASK-LAPD "Toll Free"; no retrieved page says whether it can be dialled from outside the United States.
- **Establishes:** None of the LAPD or BHPD pages retrieved states whether a victim who lives abroad (here, Cancún, Mexico) may report by phone or online.

#### 7.6 · P2 supplement — Los Angeles County Sheriff's Department (the brief gives only "Los Angeles County" for the suspected actor) — OFFICIAL
- **URL fetched:** <https://lasd.org/victims/> · HTTP 200 · **2026-11-01T03:13:38Z** · label `lasd_victims` · "Victim Resources and Crime Prevention"
- **Verbatim:**
  > Victims can report crime by calling 911 if it is an emergency, contact your local Sheriff’s Station or police department, or remain anonymous by calling Los Angeles-Crime Stoppers at 800-222-TIPS or by visiting lacrimestoppers.org.

  > If you wish to report a non-emergent crime involving the internet please call your local Sheriff’s station, law enforcement agency or the LASD Fraud & Cyber Crime Bureau (562) 374-2601.

  > FBI Internet Crime Complaint Center – Victims should report their incident there as well if it involves the Internet.

- **Establishes:** LASD's page says victims report crime to 911 (emergency), their local Sheriff's station or police department, and that non-emergent internet crimes can be reported to the local Sheriff's station, law enforcement agency or LASD's Fraud & Cyber Crime Bureau at (562) 374-2601; it also names the FBI's Internet Crime Complaint Center (federal).

## Final table — pattern → agency per the sources → the exact source line

Entry numbers refer to the entries above. "Agency" cells record only what the sources say; they are not a recommendation, and no opinion is recorded on whether any hypothetical occurred. Where the sources do not resolve a point, the cell says so.

| Pattern (hypothetical, as given in the brief) | Agency or agencies the sources identify | Exact source line(s) |
|---|---|---|
| **P1** — proof of service signed at the law office at 301 N. Canon Dr., Beverly Hills, declaring a December 2025 mailing; postage label on the envelope delivered in Cancún dated Jan. 30, 2026; filed at LASC Stanley Mosk, 111 N. Hill St. (Dept. 23). Statutes listed in the brief: PEN 118, 132, 134; BPC 6128(a). | Place of signing, 301 N. Canon Dr.: **Beverly Hills Police Department** (City of Beverly Hills), 464 N. Rexford Dr. [1.1–1.4]. Place of filing, 111 N. Hill St.: **LAPD, Central Division** (Central Bureau, Reporting District 122), station 251 E. 6th St. [1.5]. Named on the DA's page for conduct of attorneys and court personnel: **DA Justice System Integrity Division** [2.3]; attorney discipline: **State Bar OCTC** (not a law-enforcement agency) [4.1]. Court in which an offense in two territories may be tried: any competent court in either [3.1]. Federal, note only: **USPIS** (mail) [6.1]. The sources do not say which of the two police agencies takes a report about an act that spans both places. | "Beverly Hills Police Department 464 N. Rexford Drive Beverly Hills, CA 90210" [1.1a]<br>`"Match_addr": "301 N CANON DR", "Addr_type": "PointAddress"` [1.4a] and the City boundary line encloses the point (my computation) [1.4b]<br>`"APREC": "CENTRAL", "BUREAU": "CENTRAL BUREAU"` [1.5b]<br>"All crimes should be reported to the police agency in the area where the crime occurred." [2.1]<br>"investigates and prosecutes criminal conduct by persons who work within the justice system in Los Angeles County, including attorneys, judges, court employees and law enforcement personnel." [2.3b]<br>"the jurisdiction for the offense is in any competent court within either jurisdictional territory." [3.1]<br>"Any fraud that uses the U.S. Mail™—whether it originates in the mail, by phone, or online—is mail fraud." [6.1] |
| **P2** — unauthorized access to, and deletion of messages in, a Google Workspace account whose owner lives in Cancún, Mexico; suspected actor in Los Angeles County (PEN 502). | The sources identify the police agency by where the crime occurred [2.1]; the brief gives the actor's location only as Los Angeles County. **LAPD** if inside the City of Los Angeles (Division by address), **BHPD** if inside Beverly Hills, otherwise "your local Sheriff's Station or police department" (**LASD**) [Item 1, 7.6]. LASD's **Fraud & Cyber Crime Bureau** is named for non-emergent internet crimes [7.6]. PEN 502(j) treats access of a computer in one jurisdiction from another jurisdiction as access in each jurisdiction [3.5]. No retrieved source identifies an agency in Mexico or a route for a victim located abroad [7.5]. Federal, note only: **FBI IC3**, named on LASD's and FDIC's pages [7.6, 5.4]. | "is deemed to have personally accessed the computer, computer system, or computer network in each jurisdiction." (PEN 502(j)) [3.5]<br>"All crimes should be reported to the police agency in the area where the crime occurred." [2.1]<br>"If you wish to report a non-emergent crime involving the internet please call your local Sheriff’s station, law enforcement agency or the LASD Fraud & Cyber Crime Bureau (562) 374-2601." [7.6]<br>"FBI Internet Crime Complaint Center – Victims should report their incident there as well if it involves the Internet." [7.6] |
| **P3** — sworn declaration filed in LASC family court alleged to be knowingly false (PEN 118). | The brief names no courthouse. The sources identify the police agency by the place where the crime occurred [2.1]: for a filing at 111 N. Hill St., **LAPD Central Division** [1.5]; for the place where the declaration was signed, the agency serving that address (not given in the brief). PEN 118(a) applies within or without California, and PEN 27(b) says perjury under Section 118 is punishable also when committed outside California to the extent provided in Section 118 [3.2]. The DA's page describes **JSID** for attorneys, judges, court employees and law enforcement personnel [2.3] and lists limited circumstances in which the DA takes reports [2.1]. **State Bar OCTC** (attorney conduct) says it cannot reverse a court decision [4.1]; its rule 5.21(C)(3) tolls the filing time limit while related court proceedings are pending [4.3], and a 2022 report says it defers some complaints while related litigation is pending [4.4]. | "All crimes should be reported to the police agency in the area where the crime occurred." [2.1]<br>"This subdivision is applicable whether the statement, or the testimony, declaration, deposition, or certification is made or subscribed within or without the State of California." [3.2]<br>"(b) Perjury, in violation of Section 118, is punishable also when committed outside of California to the extent provided in Section 118." [3.2]<br>"investigates and prosecutes criminal conduct by persons who work within the justice system in Los Angeles County, including attorneys, judges, court employees and law enforcement personnel." [2.3b]<br>"Reverse a court decision or settlement or ask a court to reverse an earlier decision or settlement" [4.1]<br>"OCTC currently defers further review and investigation of some complaints based on pending criminal or civil litigation involving similar material allegations." [4.4, a 2022 report] |
| **P4** — Ally Bank (online bank, no California branch) restricting a customer's accounts and referring the customer by phone to an attorney's office. | Regulators in the sources' complaint routes (not police): **Federal Reserve** (primary-regulator code FED; Federal Reserve Consumer Help) [5.1–5.3]; **CFPB** (secondary-supervision flag 1) [5.1, 5.5]; **Utah DFI** for state banks [5.6]; **FDIC** is the insurer and refers complaints about banks it does not supervise [5.4]. Police: no retrieved source identifies a police agency for a bank's restriction of accounts as such; the FDIC and CFPB pages direct scam victims to the FTC, IC3 and local police or sheriff [5.4, 5.5, 5.8]. | `"REGAGNT":"FED"` [5.1]<br>"SM - Commercial bank, state charter, Fed member, and supervised by the Federal Reserve Bank (FRB)" [5.2]<br>"Use the FDIC’s BankFind tool to discover who supervises your bank" [5.3]<br>"the FDIC may not be your bank’s federal regulator." [5.4]<br>"State Banks Utah DFI and other options may apply. Please call us at 801-538-8830 before submitting a complaint" [5.6]<br>"Contact your local police or sheriff’s office to report the scam." [5.5] |

## Not verified, not found, or limited

1. **DA wording in the brief.** "all crimes must be reported to the police for a proper investigation" was not found verbatim on the DA pages read (2.1). The 2026-03-02 letter itself was not available to me.
2. **State Bar wording in the brief.** "must defer to the decisions of the courts" is on no calbar.ca.gov page or PDF fetched (4.6); it appears only in a third-party, unauthenticated excerpt (4.7). The 2022 report (4.4) is the State Bar's published statement on deferral; its current practice was not confirmed.
3. **LAPD address lookup.** Not submitted (no-forms rule). The Division for 111 N. Hill St. comes from the City of Los Angeles GIS and LAPD's station page, not from LAPD's lookup result.
4. **Courthouse reports.** Whether a report about a filing at the Stanley Mosk Courthouse is taken by LAPD or by the Sheriff's court-security unit was not researched.
5. **Beverly Hills city limits.** No city-run lookup page found; the conclusion rests on the City's GIS boundary line and locator (my point-in-polygon computation) and the Census geocoder. The City's parcel layer labels the parcel at the point "321 N CANON DR"; the difference from 301 was not resolved. The City's page `/gis` could not be fetched (connection reset); its "Interactive Maps (GIS)" page (1.4e) was fetched, but the map viewer it links to is script-driven and could not be read.
6. **BHPD online or in-person reporting.** No BHPD page retrieved describes a general online crime-report form or an in-person walk-in procedure, and the City's site map lists none (7.4); the policy manual lists report types the public may submit "via online or other self-completed reporting processes" without a web address (7.4).
7. **Victim abroad.** No LAPD or BHPD page retrieved addresses a victim located abroad (7.5).
8. **Statutes.** No opinion is recorded on whether PEN 781, 777, 778, 778a, 27, 118 or 502 applies to any hypothetical. PEN 782, 783, 784 and 790 were retrieved but not reproduced. Pending 2026 legislation was checked only by the scan described in 3.6 (standard amending sentence for the named sections), not by reading bill digests.
9. **Ally Bank.** The FFIEC National Information Center page was blocked (CAPTCHA); FDIC's human-readable BankFind page is a script-driven page and was not read (the API behind it was); whether Ally appears on Utah DFI's institution list was not checked; the record's `REGAGENT2` is empty while `CFPBFLAG` is 1 (5.2).
10. **USPIS.** No text of 18 U.S.C. § 1341 was retrieved (not asked); nothing is recorded on whether P1 fits.
11. **Connector-sourced text.** DA page text and the live leginfo comparisons rest on the Exa connector's returned text, bracketed by `date -u` readings, not on the origin HTML bytes.
12. **Dated documents.** LAPD Manual Volume 5 is the Q3 2025 update; the Federal Reserve FAQ page shows "Last Update: August 02, 2013"; the State Bar SB 211 report is dated 2022. Newer editions were not looked for.

## Appendix A — Fetch log (every curl fetch cited above)

All fetches: `curl -sS -L` through the session proxy with a descriptive User-Agent; times are the UTC clock reading taken just before each request. SHA-256 is of the bytes received.

| label | requested URL | final URL if different | HTTP | fetched (UTC) | bytes | SHA-256 |
|---|---|---|---|---|---|---|
| `ally_dep_pdf` | `https://www.ally.com/content/dam/pdf/bank/ally-bank-deposit-agreement.pdf` |  | 200 | 2026-11-01T03:09:35Z | 370385 | `f5ee0895117e1ff1b2d5f6dceac7edccf78670eaea1ec34c24a3ed58f4b99406` |
| `bh_calling` | `https://www.beverlyhills.org/597/Calling-the-Police` |  | 200 | 2026-11-01T03:00:56Z | 100238 | `f68145e0ff3b9e3be4bb006b826cb80a8fbe9a14b93b1ead4b15f9d387cf571c` |
| `bh_concern` | `https://www.beverlyhills.org/139/Report-a-Concern` | `https://beverlyhills.comcate.com/en/submitRequest` | 200 | 2026-11-01T03:39:21Z | 27187 | `d1c2e58b1d5c5f649860fe144c847027a0cec097c405255cc2742b4d12938e39` |
| `bh_contact` | `https://www.beverlyhills.org/595/Contact-Us` |  | 200 | 2026-11-01T03:00:57Z | 99961 | `2e8181aba0d4e0a9cdd90fe14d2d416c018058337c322698991a3bac91100ce1` |
| `bh_crimeinfo` | `https://www.beverlyhills.org/604/Crime-Information` |  | 200 | 2026-11-01T03:01:00Z | 109830 | `7ad1bd6014b1f84d9c455a941d1bd88a731e69de57db7a7e8f864b7c70b29a78` |
| `bh_faq331` | `https://www.beverlyhills.org/Faq.aspx?QID=331` | `https://www.beverlyhills.org/m/faq?cat=44#question-331` | 200 | 2026-11-01T03:00:58Z | 112993 | `f45a50b63acfa08988be428f940c28dfd5b99ed7f1cf592c628f46adcacdda41` |
| `bh_history` | `https://www.beverlyhills.org/561/Department-History` |  | 200 | 2026-11-01T03:15:08Z | 127443 | `ed4779fcf501e5bb05f3a51bea9f2c3e8499de86d4bc980f5519315e35dbb94b` |
| `bh_maps` | `https://www.beverlyhills.org/971/Maps-GIS` | `https://beverlyhills.org/759/Interactive-Maps-GIS` | 200 | 2026-11-01T03:39:19Z | 102703 | `c07f1d87cf0e16445237ea562e8b053aa27b6b7370466633ad10a60009ebba2e` |
| `bh_online` | `https://www.beverlyhills.org/653/Online-Services` |  | 200 | 2026-11-01T02:59:01Z | 106068 | `7b7767cb506ed83fce710ae809c88e4cef4ff5f02f1ecb5c9eff5778f62d6b4e` |
| `bh_pd` | `https://www.beverlyhills.org/548/Police-Department` |  | 200 | 2026-11-01T03:00:48Z | 153144 | `2541ad8e897f42d5a46d04961e31cc58ee2e731dae29345eed258697071d8d72` |
| `bh_policy_manual` | `https://www.beverlyhills.org/DocumentCenter/View/3557/Department-Policy-Manual-PDF` | `https://www.beverlyhills.org/DocumentCenter/View/3557/Department-Policy-Manual?bidId=` | 200 | 2026-11-01T03:14:29Z | 14262004 | `5b7b5e40bdc3fff72ceee1975164a9bbb881d229f8a94fa446504929b0894d16` |
| `bh_property` | `https://www.beverlyhills.org/705/Property` |  | 200 | 2026-11-01T02:59:03Z | 102448 | `23756f0ff973eb401e9af26958d13b816f77c8699d655bf9761f25afa30c2c70` |
| `bh_records` | `https://www.beverlyhills.org/707/Records-Bureau` |  | 200 | 2026-11-01T02:59:04Z | 112097 | `a9f5ecfa4d7f64495f322a793f97ab49228085c308803406b30fce7af8217bb1` |
| `bh_sitemap` | `https://www.beverlyhills.org/sitemap` |  | 200 | 2026-11-01T03:38:54Z | 561618 | `ea3e5c2647e0466d65b3fcd7be434ac28c3f721d968cbec1afd2b0849ab2b60b` |
| `bh_vbhapps` | `https://gis.beverlyhills.org/vbhapps/` |  | 200 | 2026-11-01T03:39:32Z | 2904 | `6c5ac3e11c200e3fb292dce39bca22b8c2c270347c73f6e657c045c1636ef573` |
| `cb_after` | `https://www.calbar.ca.gov/public/file-complaints-claims/file-attorney-complaint/after-you-file-attorney-misconduct-complaint` |  | 200 | 2026-11-01T03:07:20Z | 427694 | `abdd245ff9e14979f8f5f018816c015f5caa35f0b540a3014b4ddf52fed89dd8` |
| `cb_faq` | `https://www.calbar.ca.gov/frequently-asked-questions-complaints-claims` |  | 200 | 2026-11-01T03:05:54Z | 442944 | `18d01d71ff01790664b55ce44e141591918ead1e39e757916921acfb925faa74` |
| `cb_form_pdf` | `https://www.calbar.ca.gov/sites/default/files/2025-09/Attorney_Misconduct_Complaint.pdf` |  | 200 | 2026-11-01T03:05:56Z | 879924 | `52e907e35b45c4c876b52b18604463508601207fe33b7ef6046fcb1f4c5e1bd7` |
| `cb_online` | `https://apps.calbar.ca.gov/complaint/` |  | 200 | 2026-11-01T03:05:58Z | 679933 | `52dddc288c42c7508aa602f095c422f57e6480325e9431f026ceeef87028650b` |
| `cb_rop` | `https://www.calbar.ca.gov/sites/default/files/portals/0/documents/rules/Rules-of-Procedure.pdf` |  | 200 | 2026-11-01T03:05:59Z | 6623484 | `81b13a78d0c37b309fbc52a0b251adff6ccd43c1665b700943b8911d359c88be` |
| `cb_sb211_pdf` | `https://www.calbar.ca.gov/sites/default/files/portals/0/documents/reports/Senate-Bill-211-Case-Processing-Standards-Proposal.pdf` |  | 200 | 2026-11-01T03:05:57Z | 1517282 | `6512dfcac83036cc9d74f7310c750b97b0007e599c2c45180790530fd12109d9` |
| `cb_second` | `https://www.calbar.ca.gov/public/file-complaints-claims/request-complaint-review` |  | 200 | 2026-11-01T03:05:58Z | 432871 | `3edd7da50d2ce3e7b1bfd202670bfe18aff139a24b7510e443bd5287af7290a2` |
| `cb_want` | `https://www.calbar.ca.gov/basic-page/want-file-complaint` | `https://www.calbar.ca.gov/public/file-complaints-claims/want-file-complaint` | 200 | 2026-11-01T03:05:52Z | 458981 | `9c7008986c78e477f787b2906ab16b334121f071de83e00ef3532d99c7fdbcef` |
| `census_111` | `https://geocoding.geo.census.gov/geocoder/geographies/onelineaddress?address=111+N+Hill+St%2C+Los+Angeles%2C+CA+90012&benchmark=Public_AR_Current&vintage=Current_Current&layers=all&format=json` |  | 200 | 2026-11-01T03:03:23Z | 8429 | `e5f2a56ff2d9dbfa1cd23d84c58441b835cb9fc1e7e66ac71ef7cf5ce99bf9ab` |
| `census_301` | `https://geocoding.geo.census.gov/geocoder/geographies/onelineaddress?address=301+N+Canon+Dr%2C+Beverly+Hills%2C+CA+90210&benchmark=Public_AR_Current&vintage=Current_Current&layers=all&format=json` |  | 200 | 2026-11-01T03:03:22Z | 8411 | `5e4e7b0d6498281eaaf73dc04711ebdba591cea0dba2278ebab7e8b310ef3fe7` |
| `cfpb_complaint` | `https://www.consumerfinance.gov/complaint/` |  | 200 | 2026-11-01T03:08:30Z | 167793 | `7a78e5ae01723132e4d004e163e7fcae06d9b4ea7fb04f5778b5769e1f10d532` |
| `fdic_ally_full` | `https://api.fdic.gov/banks/institutions?filters=CERT%3A57803&limit=1` |  | 200 | 2026-11-01T03:07:38Z | 2524 | `3de9143c14a3db2fc6404fc98f2d7465eb8f2a1e75d40661e564a85bf25cc870` |
| `fdic_cp` | `https://www.fdic.gov/consumer-resource-center/consumer-complaint-process` |  | 200 | 2026-11-01T03:08:28Z | 84259 | `1095050995bd032bc88c7dbbec382dfa3f2c1bea929c4ae69ef12af547c358bf` |
| `fdic_props` | `https://api.fdic.gov/banks/docs/institution_properties.yaml` |  | 200 | 2026-11-01T03:07:48Z | 94832 | `6ed1763c66a9e240904a45712b23d825c0f31beaadb6cd0213fc1bf00b2af1b9` |
| `fr_faq` | `https://www.federalreserve.gov/faqs/credit_12666.htm` |  | 200 | 2026-11-01T03:08:26Z | 86455 | `951d32ae9ba18ab64005cac9e21bdd0282b3f09ceecb78ed8e708840dbc3156e` |
| `fr_frch` | `https://www.federalreserveconsumerhelp.gov/` |  | 200 | 2026-11-01T03:08:26Z | 17448 | `2d3aac18f092c70c12e6b9c792fdd0ab03f804ebd66c5ed44c358bbc810e0b2e` |
| `gis_bh_boundary2_geom` | `https://gis.beverlyhills.org/arcgis/rest/services/CBH_Boundary/MapServer/0/query?where=1%3D1&outFields=*&returnGeometry=true&outSR=102645&f=json` |  | 200 | 2026-11-01T03:22:14Z | 40261 | `2545ba319d88d222aa29e1fe3b36fdeaaf4e59ccc9f0fa87351185b9a407c2bd` |
| `gis_bh_boundary_geom` | `https://gis.beverlyhills.org/arcgis/rest/services/VBH_for_CS_Public_CE2/MapServer/3/query?where=1%3D1&outFields=*&returnGeometry=true&outSR=102645&f=json` |  | 200 | 2026-11-01T03:02:40Z | 40436 | `246c2f465a23c73a18be4549d25c46158507e52184d29af0ba6316142db08e96` |
| `gis_bh_boundary_meta` | `https://gis.beverlyhills.org/arcgis/rest/services/CBH_Boundary/MapServer?f=pjson` |  | 200 | 2026-11-01T03:01:46Z | 2455 | `af8751f4bee860bee1c400f2d182978d02a5beda0463944a434984354346f34a` |
| `gis_bh_geocode_301` | `https://gis.beverlyhills.org/arcgis/rest/services/Comb_Loc101p/GeocodeServer/findAddressCandidates?SingleLine=301+N+Canon+Dr&outFields=*&f=pjson` |  | 200 | 2026-11-01T03:01:57Z | 10055 | `8cc4d24f13a9569f41a1b344ee61fe54fbc5646664fd5a46b94456ee062a487d` |
| `gis_bh_parcel_q` | `https://gis.beverlyhills.org/arcgis/rest/services/VBH_for_CS_Public_CE2/MapServer/2/query?geometry=6440470.536414914,1847879.96459122&geometryType=esriGeometryPoint&inSR=102645&spatialRel=esriSpatialRelIntersects&outFields=*&returnGeometry=false&f=pjson` |  | 200 | 2026-11-01T03:02:26Z | 1085 | `302c7f1d44a6eb06999ac40f94a38e19b64484ce29e26cdf4256acd14f4e626c` |
| `gis_bh_vbh_meta` | `https://gis.beverlyhills.org/arcgis/rest/services/VBH_for_CS_Public_CE2/MapServer?f=pjson` |  | 200 | 2026-11-01T03:02:08Z | 3925 | `13a61ac46b7e2d2164e10f1f0b1e71690a08ad71a88908fd8d5fd91a98e3df20` |
| `gis_bh_zoning_q` | `https://gis.beverlyhills.org/arcgis/rest/services/Zoning/MapServer/2/query?geometry=6440470.536414914,1847879.96459122&geometryType=esriGeometryPoint&inSR=102645&spatialRel=esriSpatialRelIntersects&outFields=*&returnGeometry=false&f=pjson` |  | 200 | 2026-11-01T03:02:25Z | 3068 | `585f013424eba6aac0d077e4f881772f2fe4e48b15792250409c5fe37c6b7382` |
| `gis_lapd_meta` | `https://maps.lacity.org/lahub/rest/services/LAPD/MapServer?f=pjson` |  | 200 | 2026-11-01T03:03:42Z | 4125 | `a961605e71db52bf04f0185f5decad6289e58b3f88cd1444e1f20ff809a86356` |
| `gis_lapd_q2` | `https://maps.lacity.org/lahub/rest/services/LAPD/MapServer/2/query?geometry=-118.246496192834,34.054523799954&geometryType=esriGeometryPoint&inSR=4326&spatialRel=esriSpatialRelIntersects&outFields=*&returnGeometry=false&f=pjson` |  | 200 | 2026-11-01T03:03:49Z | 1165 | `f0deb37acd1f15f0c9225a73cbdfa3c53741f14bb2cde506cf24e60808ec3a43` |
| `gis_lapd_q3` | `https://maps.lacity.org/lahub/rest/services/LAPD/MapServer/3/query?geometry=-118.246496192834,34.054523799954&geometryType=esriGeometryPoint&inSR=4326&spatialRel=esriSpatialRelIntersects&outFields=*&returnGeometry=false&f=pjson` |  | 200 | 2026-11-01T03:03:49Z | 1165 | `f0deb37acd1f15f0c9225a73cbdfa3c53741f14bb2cde506cf24e60808ec3a43` |
| `gis_lapd_q4` | `https://maps.lacity.org/lahub/rest/services/LAPD/MapServer/4/query?geometry=-118.246496192834,34.054523799954&geometryType=esriGeometryPoint&inSR=4326&spatialRel=esriSpatialRelIntersects&outFields=*&returnGeometry=false&f=pjson` |  | 200 | 2026-11-01T03:03:50Z | 1165 | `f0deb37acd1f15f0c9225a73cbdfa3c53741f14bb2cde506cf24e60808ec3a43` |
| `gis_lapd_stations` | `https://maps.lacity.org/lahub/rest/services/LAPD/MapServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&f=pjson` |  | 200 | 2026-11-01T03:03:51Z | 6302 | `91866ed22b59fd68b49f0a268d4712b10dda2d8a2757bc06271313bc4a819b7d` |
| `lapd_central` | `https://www.lapdonline.org/lapd-contact/central-bureau/central-community-police-station/` |  | 200 | 2026-11-01T02:59:07Z | 99516 | `40d9769cf82bd5ccdc65cbfe688f5613c5a29af30492aa0fc60b2009fc6bcaa6` |
| `lapd_file` | `https://www.lapdonline.org/file-a-police-report/` |  | 200 | 2026-11-01T02:59:29Z | 82034 | `c607ac40ddf112a554674851fd4cfafa1c5f44eee8a5329dd7f2f7fbe02f5c2e` |
| `lapd_find` | `https://www.lapdonline.org/find-your-local-police-station/` |  | 200 | 2026-11-01T02:59:17Z | 121109 | `8a77ba3d4e41466ca1d5d8a64a11ce98b295658655a576d88e7fb8eb6006a31d` |
| `lapd_manual5` | `https://lapdonlinestrgeacc.blob.core.usgovcloudapi.net/lapdonlinemedia/VOLUME_5_Q3_2025_Updates_from_4_1_25_to_9_30_25_.pdf` |  | 200 | 2026-11-01T03:14:12Z | 770376 | `5613efcc5f6275bc7baa1003a3644c46f6da8353db0954b99911a7f938bcb6f7` |
| `lasd_victims` | `https://lasd.org/victims/` |  | 200 | 2026-11-01T03:13:38Z | 215869 | `340f58a3e89314bdd9e86bddc00977290c5dce1ccb8dccd81f84777cfa007240` |
| `p_bankfind` | `https://banks.data.fdic.gov/api/institutions?filters=NAME%3A%22Ally%20Bank%22&fields=NAME%2CCERT%2CSTALP%2CCHARTER%2CREGAGNT%2CFED_RSSD&limit=5` | `https://api.fdic.gov/banks/institutions?filters=NAME%3A%22Ally%20Bank%22&fields=NAME%2CCERT%2CSTALP%2CCHARTER%2CREGAGNT%2CFED_RSSD&limit=5` | 200 | 2026-11-01T02:57:17Z | 378 | `eb615da58a6fcfc89ae2b0b9b28b384632b922a9416cef3f9bdbe69c68397720` |
| `us_mailfraud` | `https://www.uspis.gov/tips-prevention/mail-fraud` |  | 200 | 2026-11-01T03:10:16Z | 61119 | `ba4100631eb3bf4d9cdee93de41bd9a035731f72e98e9fdd03ba856ebd1a7399` |
| `us_old_mailfraud` | `https://postalinspectors.uspis.gov/investigations/MailFraud/MailFraud.aspx` | `https://www.uspis.gov/investigations/MailFraud/MailFraud.aspx` | 200 | 2026-11-01T03:10:19Z | 50379 | `e758f54c9b5d7303c76b1b9d37b8c79156e2bb8008ad04ce371c8f586b0823f1` |
| `us_report` | `https://www.uspis.gov/report` |  | 200 | 2026-11-01T03:10:18Z | 59682 | `492d9332e943bc2f48c657b2bb7b28edd64eb08d3ee88e268d83f0cd729648fe` |
| `us_whatwedo` | `https://www.uspis.gov/about/what-we-do` |  | 200 | 2026-11-01T03:10:17Z | 66082 | `b22c619d6ad51dd41c5de0aeeb80669a335d5f548163b90a587e01fa48795094` |
| `utah_dfi` | `https://dfi.utah.gov/resources/helpful-links/file-a-complaint/` |  | 200 | 2026-11-01T03:08:29Z | 32072 | `cc7901a78d77cfb911dd0c81715c4413bcfdae28a801607509b58a5064fd75a9` |

### Blocked or failed fetches (not circumvented)

| label | URL | HTTP | fetched (UTC) | what it was |
|---|---|---|---|---|
| `p_da` | `https://da.lacounty.gov/` | 403 | 2026-11-01T02:57:16Z | Imperva/Incapsula bot challenge (da.lacounty.gov) |
| `gis_laco_root` | `https://public.gis.lacounty.gov/public/rest/services?f=pjson` | 403 | 2026-11-01T03:03:35Z | Imperva/Incapsula bot challenge (public.gis.lacounty.gov) |
| `p_leginfo` | `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=781` | 403 | 2026-11-01T02:57:23Z | Cloudflare challenge (leginfo) |
| `gis_bh_vbh` | `https://gis.beverlyhills.org/VBH/` | 403 | 2026-11-01T03:01:27Z | IIS 403 (Beverly Hills GIS viewer path) |
| `ffiec_npw` | `https://www.ffiec.gov/npw/Institution/Profile/3284070` | 403 | 2026-11-01T03:09:26Z | CAPTCHA page (FFIEC NIC profile for Ally Bank) |
| `ext_octc_letter` | `https://cdn.ripoffreport.com/95x70/docs_o/r1537258-ynwvte-wsroilqod6` | 403 | 2026-11-01T03:16:08Z | 403 from a third-party host |
| `cb_process_pdf` | `https://www.calbar.ca.gov/sites/default/files/2025-10/Filing-Complaint-Against-Attorney.pdf` | 404 | 2026-11-01T03:05:54Z | 404 for a stale search-result URL |
| `bh_gis_page` | `https://www.beverlyhills.org/gis` | 000 | 2026-11-01T03:22:15Z | connection reset by origin; no body |

Also fetched, not cited by label: the Legislature download index (`pubinfo_index`, 2026-11-01T03:19:41Z) and the incremental ZIPs listed in Appendix B.

## Appendix B — Legislature bulk-data entries read (`pubinfo_2025.zip`)

`https://downloads.leginfo.legislature.ca.gov/pubinfo_2025.zip` · HEAD 200 · Content-Length 1292052065 · Last-Modified Mon, 26 Oct 2026 04:26:08 GMT · Accept-Ranges bytes · central directory 205,148 entries (Zip64) read by range request; every entry read passed its ZIP CRC-32.

| purpose | ZIP entry | read (UTC) | compressed bytes | uncompressed bytes | CRC-32 | ZIP entry date |
|---|---|---|---|---|---|---|
| section index (162,526 rows) | `LAW_SECTION_TBL.dat` | 2026-11-01T03:11:41Z | 6,058,294 | 43,276,148 | OK | 2026-10-25 21:22:54 |
| official headings | `LAW_TOC_TBL.dat` | 2026-11-01T03:12:54Z | 951,130 | 5,329,533 | OK | 2026-10-25 21:23:06 |
| PEN 118 | `LAW_SECTION_TBL_69289.lob` | 2026-11-01T03:11:45Z | 564 | 1,273 | OK | 2026-10-25 21:22:22 |
| PEN 27 | `LAW_SECTION_TBL_67112.lob` | 2026-11-01T03:11:45Z | 444 | 982 | OK | 2026-10-25 21:22:20 |
| PEN 777 | `LAW_SECTION_TBL_102824.lob` | 2026-11-01T03:11:45Z | 275 | 460 | OK | 2026-10-25 21:22:34 |
| PEN 778 | `LAW_SECTION_TBL_102880.lob` | 2026-11-01T03:11:45Z | 297 | 507 | OK | 2026-10-25 21:22:34 |
| PEN 778a | `LAW_SECTION_TBL_102881.lob` | 2026-11-01T03:11:46Z | 386 | 916 | OK | 2026-10-25 21:22:34 |
| PEN 781 | `LAW_SECTION_TBL_102882.lob` | 2026-11-01T03:11:46Z | 260 | 494 | OK | 2026-10-25 21:22:34 |
| PEN 782 (not reproduced) | `LAW_SECTION_TBL_102883.lob` | 2026-11-01T03:11:46Z | 198 | 317 | OK | 2026-10-25 21:22:34 |
| PEN 783 (not reproduced) | `LAW_SECTION_TBL_102884.lob` | 2026-11-01T03:11:46Z | 342 | 677 | OK | 2026-10-25 21:22:34 |
| PEN 784 (not reproduced) | `LAW_SECTION_TBL_102934.lob` | 2026-11-01T03:11:46Z | 533 | 1,103 | OK | 2026-10-25 21:22:34 |
| PEN 784.7 | `LAW_SECTION_TBL_61583.lob` | 2026-11-01T03:11:47Z | 761 | 2,893 | OK | 2026-10-25 21:22:18 |
| PEN 790 (not reproduced) | `LAW_SECTION_TBL_103092.lob` | 2026-11-01T03:11:47Z | 692 | 1,681 | OK | 2026-10-25 21:22:34 |
| PEN 502 (independent re-read) | `LAW_SECTION_TBL_61669.lob` | 2026-11-01T03:24:22Z | 4,937 | 19,701 | OK | 2026-10-25 21:22:18 |
| bill index | `BILL_TBL.dat` | 2026-11-01T03:16:41Z | 100,933 | 954,316 | OK | 2026-10-25 21:21:14 |
| bill versions index | `BILL_VERSION_TBL.dat` | 2026-11-01T03:16:41Z | 756,287 | 4,512,719 | OK | 2026-10-25 21:21:46 |
| 2,254 chaptered bill texts | `BILL_VERSION_TBL_*.lob` (one per chaptered version) | 2026-11-01T03:17:10Z–03:18:12Z (scan 1) and again (control scan) | — | — | OK for all (0 failures) | — |

Live-page cross-checks (second Exa connector, `date -u` brackets): PEN 781, 27, 778a — 03:20:04Z–03:20:12Z; PEN 118, 777, 778, 784.7 — 03:20:17Z–03:20:24Z; PEN 502 — 03:24:25Z–03:24:31Z. For the first seven, the live paragraph text equalled the bulk-data paragraph text exactly (machine-compared); for PEN 502 the whole section text was returned and subdivision (j) is identical to the bulk data and to the earlier verified file.

Incremental files checked: `pubinfo_Mon.zip`, `pubinfo_Wed.zip`, `pubinfo_Thu.zip`, `pubinfo_Fri.zip` — no `LAW_*` entry (HTTP Last-Modified 27, 29, 30, 24 Oct 2026).

## Appendix C — Exa connector calls whose text is quoted

| purpose | URLs | UTC |
|---|---|---|
| DA FAQ (2.1–2.4) | `https://da.lacounty.gov/about/office-faqs` | about 03:15:40Z (also about 03:04Z) |
| DA Overview, Where to Report Fraud, Forms, JSID directory (2.5–2.8) | `https://da.lacounty.gov/about/office-overview`, `.../contact/forms/fraud-report`, `.../contact/forms`, `.../contact/office-directory/justice-system-integrity-division` | 03:15:46Z–03:15:52Z (these pages were also returned by earlier calls at about 03:05Z) |
| Live leginfo PEN 781, 27, 778a | `https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=…` | 03:20:04Z–03:20:12Z |
| Live leginfo PEN 118, 777, 778, 784.7 | same pattern | 03:20:17Z–03:20:24Z |
| Live leginfo PEN 502 | same pattern | 03:24:25Z–03:24:31Z |
| OCTC-letter sentence (4.7) | search highlight only; origin host returned HTTP 403 to curl at 03:16:08Z | about 03:06Z |

Raw downloads, extracted text and the scripts that produced this file are in the session scratchpad (outside the project); no file other than this one was written in the project.
