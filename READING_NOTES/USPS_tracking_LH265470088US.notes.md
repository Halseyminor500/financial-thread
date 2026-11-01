# Reading notes — Tracking history for LH265470088US (number on the customs form of the Cancún envelope): USPS page blocked, Correos de México history read

- **Reader:** Claude Sonnet 5.5 subagent, read-only. I read `INVENTORY/AGENT_RULES.md` first. No git was run. Nothing was submitted except the public tracking query (§2, rows 8 and 9). No one was contacted. No scratch files: command output was kept on stdout, and this notes file is the only file I wrote.
- **Class of the source read:** government postal tracking web page (Correos de México), public record. Not AI output; no AI-LEAD material was used. The one AI-mediated fetch tool (WebFetch) returned only an HTTP 403, so nothing from it is used here.
- **Headline:**
  1. The USPS tracking page could **not** be read. `tools.usps.com` answered with an "Access Denied" page (HTTP 403; the response carries an `akamai-grn` header). I did not try to get around it.
  2. The Correos de México tracking page, which the brief names as the fallback, returned **11 events** for `LH265470088US`. It showed no CAPTCHA and no login.
  3. The earliest event is dated **30/01/2026**. The page writes dates day/month/year, so that is the same calendar date as the form's `01/30/2026`.
  4. The event reading **"Entrega"** is dated **26/02/2026**. The event dated 24/02/2026 reads "Con mensajero para entrega".

## 1. Facts as given in the brief (I did not verify these)

Customs form on an envelope photographed in Cancún: "Date of Mailing: 01/30/2026"; tracking number "LH 265 470 088 US"; First-Class Package International Service, $29.70; mailed from 00495 Beverly Hills, CA 90210; delivered to the addressee's building 2026-02-24 per the recipient's declaration.

## 2. Every request I made

Plain requests only: `curl` through the session proxy with curl's default User-Agent and no cookies, or the named fetch tools. No header spoofing, no browser automation, no CAPTCHA handling. UTC times come from the session clock (`date -u`). "≈" means the tool returned no time of its own and the call was issued in the same batch as the time shown.

| # | UTC (2026-11-01) | Tool | Target | Result |
|---|---|---|---|---|
| 1 | 03:36:50Z | curl GET | `https://tools.usps.com/go/TrackConfirmAction?tLabels=LH265470088US` | HTTP/2 **403**, `content-type: text/html`, `content-length: 398`, `akamai-grn: 0.a4423917.1793504210.65e81b12`. The body is an "Access Denied" page (§2.1). No tracking data. |
| 2 | 03:37:37Z | curl GET to the proxy's own local status endpoint (not an outbound request) | `$HTTPS_PROXY/__agentproxy/status` | `recentRelayFailures` lists no failure for `tools.usps.com`. So the 403 in row 1 was not produced by the egress proxy. |
| 3 | ≈03:37:37Z | WebFetch | same USPS URL | "The server returned HTTP 403 Forbidden." / "The response body was not retrieved." |
| 4 | 03:37:37.365Z (stamp inside the error) | `mcp__Exa__web_fetch_exa` | same USPS URL | Error 402: "You have exceeded your credits limit. Please top up to keep using Exa at dashboard.exa.ai". No page content. |
| 5 | ≈03:37:55Z | `mcp__Exa_a17196c7__web_fetch_exa` | same USPS URL | "Error fetching URL(s): https://tools.usps.com/go/TrackConfirmAction?tLabels=LH265470088US: CRAWL_EMPTY_CONTENT". No page content. |
| 6 | 03:37:55Z; two further reads between 03:37:56Z and 03:39:16Z (untimed); one just before each of rows 8 and 9 | curl GET (5 in all) | `https://www.correosdemexico.gob.mx/SSLServicios/SeguimientoEnvio/Seguimiento.aspx` | HTTP 200 form page, title "Seguimiento de Envíos". Details in §2.2. |
| 7 | between 03:37:56Z and 03:39:16Z (untimed) | curl GET | `https://www.correosdemexico.gob.mx/SSLServicios/SeguimientoEnvio/Contenido/Funciones.js` (a script the form page references) | HTTP 404 page: "404: archivo o directorio no encontrado." |
| 8 | 03:39:17Z to 03:39:18Z | curl POST (the tracking query) | `https://www.correosdemexico.gob.mx/SSLServicios/SeguimientoEnvio/Seguimiento.aspx` | HTTP 200, 11 events (§3). |
| 9 | 03:40:28Z to 03:40:29Z | curl POST (the same query, repeated once) | same | HTTP 200, same 11 events. Repeated only to see the "Recibió" value untruncated and the real response headers (my first display filter had cut long values). |

### 2.1 Body of the USPS response (row 1), verbatim, read in full (398 bytes)

```
<HTML><HEAD>
<TITLE>Access Denied</TITLE>
</HEAD><BODY>
<H1>Access Denied</H1>
 
You don't have permission to access "http&#58;&#47;&#47;tools&#46;usps&#46;com&#47;go&#47;TrackConfirmAction&#63;" on this server.<P>
Reference&#32;&#35;18&#46;a4423917&#46;1793504210&#46;65e81b12
<P>https&#58;&#47;&#47;errors&#46;edgesuite&#46;net&#47;18&#46;a4423917&#46;1793504210&#46;65e81b12</P>
</BODY>
</HTML>
```

This is neither a CAPTCHA nor a login page. It is a flat denial, and nothing on it can be completed by a visitor. The page does not say why access was denied.

### 2.2 The Correos de México form (rows 6, 8, 9)

- Fields on the form page: text input `Guia` (`maxlength="13"`, placeholder "Número de guía", label "Ingrese el número de guía:"); select `Periodo` (label "Ejercicio:", options 2026 [pre-selected], 2025, 2024); buttons "LIMPIAR" (`Limpia`) and "BUSCAR" (`Busqueda`); hidden `__VIEWSTATE`, `__VIEWSTATEGENERATOR`, `__EVENTVALIDATION`.
- I searched the form page's HTML for `captcha`, `recaptcha`, `g-recaptcha`, `hcaptcha`, `turnstile`, `cf-challenge`, `data-sitekey` and "código de seguridad": no matches. There is no login element. The tracking query returned results directly.
- What I sent in each POST (the fields the BUSCAR button posts, with the three state values copied from the form page I had just fetched): `__EVENTTARGET=Busqueda`, `__EVENTARGUMENT=` (empty), `__VIEWSTATE`, `__VIEWSTATEGENERATOR=6CB5246A`, `__EVENTVALIDATION`, `Guia=LH265470088US`, `Periodo=2026`. The served HTML contained no `__EVENTTARGET` field, so I set it to `Busqueda`, the target named in the BUSCAR button's `onclick`.

### 2.3 Not done, and why

- **USPS JSON endpoint: not tried.** The brief offers it if the page "may need JavaScript". The response here was an edge access denial, not a JavaScript requirement, and trying other USPS endpoints would have meant routing around that denial.
- No WebSearch, no third-party tracking site, no browser automation, no User-Agent change, no cookies.
- `Periodo` 2025 and 2024 were not queried (the brief gives a 2026 mailing date).

## 3. The record read

- **URL:** `https://www.correosdemexico.gob.mx/SSLServicios/SeguimientoEnvio/Seguimiento.aspx`. The result is the response to a form POST, so there is no per-number link.
- **Query:** `Guia` = `LH265470088US`; `Periodo` ("Ejercicio") = `2026`.
- **Read at (UTC):** 2026-11-01T03:39:18Z (row 8, primary) and 2026-11-01T03:40:29Z (row 9, confirmation; response headers `HTTP/1.1 200 OK`, `Server: Microsoft-IIS/8.5`, `Date: Sun, 01 Nov 2026 03:40:29 GMT`). Dates, times, places and statuses were identical on both reads (compared row by row).
- **The page's own stamps:** "Fecha de Consulta: 31/10/2026 09:39:18 p. m." (row 8) and "Fecha de Consulta: 31/10/2026 09:40:29 p. m." (row 9). Set against the row 9 `Date` header (03:40:29 GMT), the page clock reads 6 hours behind GMT. The page states no time zone for the event times.
- **"Total de eventos : 11"** (span `NumeroEventos`).

Events, verbatim, in the page's order. Heading above the table on the page: "Datos de seguimiento". Column headers: Fecha | Hora | Origen | Evento | (blank). The first column below, `#`, is the number the page prints in white text in a fifth column. Accented letters were stored as HTML entities in the page source (for example `Am&#233;rica`) and are decoded here. Rows 4 and 5 have two spaces after the comma, exactly as in the source.

```
# | Fecha | Hora | Origen | Evento
1 | 30/01/2026 | 12:14:00 | Estados Unidos de América | Deposito del Cliente en el país de origen
2 | 01/02/2026 | 01:37:00 | Estados Unidos de América | En zona de intercambio int. hacia el país destino, previo Aduana
3 | 10/02/2026 | 08:18:00 | Oficina de Cambio México | Arribo a Zona Intercambio México, en espera de ingreso a la Aduana
4 | 10/02/2026 | 12:29:00 | Oficina Operativa BJ ORD IMP,  CDMX | En tránsito hacia destino
5 | 10/02/2026 | 14:40:00 | Oficina Operativa BJ REG IMP,  CDMX | En tránsito hacia destino
6 | 16/02/2026 | 16:04:00 | Centro de Clasificación Internacional 23 | Recepción en Oficina de Correos
7 | 16/02/2026 | 17:24:00 | Centro de Clasificación Internacional 23 | En tránsito hacia destino
8 | 23/02/2026 | 13:43:00 | Centro Operativo de Reparto Benito Juárez Cancún, Q. Roo. | Recepción en Oficina de Correos
9 | 23/02/2026 | 13:49:00 | Centro Operativo de Reparto Benito Juárez Cancún, Q. Roo. | 1er visita al domicilio para entrega, no se encontró al destinatario
10 | 24/02/2026 | 09:31:00 | Centro Operativo de Reparto Benito Juárez Cancún, Q. Roo. | Con mensajero para entrega
11 | 26/02/2026 | 12:04:00 | Centro Operativo de Reparto Benito Juárez Cancún, Q. Roo. | Entrega
```

- Row 11 is the only row drawn with a background colour (`bgcolor="#B9D577"`) and with bold, centred text.
- **Delivery field.** Above the events table the page shows a block with the label "Recibió :" and a read-only text input. Its raw tag: `<input name="PersonaRecibe" type="text" value="SALOMON R" readonly="readonly" id="PersonaRecibe" class="TextoEntrega" />`. Value: `SALOMON R`.
- **Page note** (span `lblMenAdico`), verbatim: "Te recordamos que el envío buscado es un producto Ordinario el cual no tiene rastreo, por lo que la respuesta en nuestro Centro de Atención, será la misma que se presenta en esta página."
- Result spans that are empty on the page: `lblLeyenda`, `lblMensaje`, `lbl_msj`.
- **Not in the page text I read:** any USPS office name, city or ZIP; a postage amount; a weight; a sender; an addressee; a service name. Rows 1 and 2 name only "Estados Unidos de América".
- **To look at it yourself:** open the URL above, type `LH265470088US` into "Número de guía", leave "Ejercicio" at 2026, and press BUSCAR.

## 4. Comparison with the brief's facts (comparison only; no inference drawn)

**(a) Acceptance date against "Date of Mailing: 01/30/2026".**
- The earliest event (#1) is `30/01/2026`, `12:14:00`, `Estados Unidos de América`, "Deposito del Cliente en el país de origen".
- The page's date format is day/month/year: the page's own stamp reads "31/10/2026", and no month 30 or 31 exists. So `30/01/2026` is 30 January 2026, which is `01/30/2026` in US order. **The dates match.**
- Limits on that match: (i) it is Correos de México's record of the item, not a USPS scan, and the USPS page was unreadable; (ii) the event text is "Deposito del Cliente en el país de origen", and the words "accepted" or "aceptación" do not appear; (iii) the page names no USPS facility, city or ZIP, so "00495 Beverly Hills, CA 90210" is neither confirmed nor contradicted; (iv) no time zone is given for 12:14:00.

**(b) Delivery against "delivered to the addressee's building 2026-02-24 per the recipient's declaration".**
- #9, 23/02/2026 13:49:00: "1er visita al domicilio para entrega, no se encontró al destinatario".
- #10, 24/02/2026 09:31:00: "Con mensajero para entrega".
- #11, 26/02/2026 12:04:00: "Entrega"; "Recibió :" field reads `SALOMON R`.
- No event dated 24/02/2026 reads "Entrega". The event that reads "Entrega" is dated 26/02/2026. I draw no conclusion from this about the declaration or about why the dates differ.

**(c) Service wording.** The page note calls the item "un producto Ordinario el cual no tiene rastreo". The brief's service is "First-Class Package International Service". The page names no service of its own. I draw no conclusion.

## 5. Limits

- The USPS page remains unread. Everything in §3 is Correos de México data.
- **What I read in full:** the 398-byte USPS denial body; in row 8, the whole results region of the page (from the `lblLeyenda` span through `</main>`); in row 9, the response headers, the `PersonaRecibe` tag, every row of the events table and the spans `FechaConsulta`, `NumeroEventos`, `lblLeyenda`, `lblMensaje`, `lblMenAdico`, `lbl_msj`; the form page's markup.
- **What I did not read as text:** the opaque hidden fields (`__VIEWSTATE`, `__EVENTVALIDATION`; my display cut them to 30 characters), the external scripts (`jquery.min.js`, `bootstrap.min.js`, `gobmx.js`, `encuestas.js`) and the images.
- Only `Periodo` = 2026 was queried.
- This note is a reader's transcript, which is AI work and so not evidence in itself. An evidentiary capture would need a person to save the live page.
