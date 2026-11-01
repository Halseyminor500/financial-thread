# COLLISION GATE — which existing routines would see a Spiegel filing and its replies

Read 2026-11-01 ~02:15 UTC from the account's enabled scheduled tasks (list_triggers, read-only;
nothing was changed). Charter WALL 6. **This file is the gate every draft must pass before it is
offered for filing.**

## The routines that read mail (enabled as of 2026-11-01)

| Scheduled task (id) | Schedule | Mail it reads | What it DOES with what it finds |
|---|---|---|---|
| **Case mail read, 6 am and 9 pm** (`trig_01VqB7TRQy8jAEG22S3viy6z`, Front 4 session) | 05:55 and 20:55 Cancún daily | `from:` provinziano.com, jlsnyderlaw@gmail.com, **beverlyhills.org, da.lacounty.gov, lacounty.gov, doj.ca.gov, usdoj.gov, fbi.gov, ic3.gov, post.ca.gov, courts.ca.gov, justfoia.com** (in:anywhere, incl. Trash); also restores Trash from those domains | Reads in full; writes `INBOUND_*.md` into the Front 4 (Shannon) tracker; updates `TRACKER_open_requests.md`; writes a D-73 verdict to `VERDICTS.json` (feeds the public site); **drafts and SENDS a response in Halsey's voice without approval (D-80)**; places each agency answer on the AG PIU #1564601 file; tells the federal threads about any federal message |
| **Court & legal inbox monitor — 24STFL00432** (`trig_015FsbYwqGh22MHb2EoYYvdr`) | 00:51 and 12:51 UTC | LASC + e-filing vendors, **anything from Spiegel / ysfamilylaw.com**, beverlyhills.org (Kalé, Coulter, Subin, Rivas), da.lacounty.gov | Reports to Halsey; **creates Drive docs "MINOR CASE — DOCKET ALERT [date]"** for deadlines |
| **Justice Meter mail check (record only)** (`trig_01SiUW2cQGJkeuQXXDcNkhiZ`) + **morning update** (`trig_01WYvEqsVbzEpe18LLMjACiU`) | 06:05 / 06:50 Los Angeles daily | agency replies per `site-2026/aglive/DAILY.md` | Records agency answers and **publishes the halseyminor.com site** (gh-pages) |
| **BHPD 2025-14983 — investigator question box** (`trig_01SSyWBgTmUF72rnJ7AMHMjY`) | hourly | the investigator artifact's questions | **Posts answers to BHPD investigator questions without approval** from the Shannon report |
| **Front 4 — federal filing follow-up** (`trig_016ZAN32ymjwi3nxLaiSgoEN`) | every 6 h | ic3.gov, tips.fbi.gov, eFOIPA | Records federal filing dates in Front 4 DEADLINES.md |
| 523 letters: Monday/Tuesday evening checks (one-shot, 3–4 Nov) | — | da.lacounty.gov, beverlyhills.org, doj.ca.gov | Reports to Halsey; sends nothing |

Not in any routine's sender list found: **calbar.ca.gov** (State Bar).

## Destination → who would see it

| If a Spiegel item goes to … | Replies would be caught by | Consequence if nothing is decided first |
|---|---|---|
| Beverly Hills PD (beverlyhills.org) | Case mail read; 24STFL00432 monitor; Justice Meter; investigator box (if the same detective asks) | Reply filed into the **Shannon** BHPD 2025-14983 tracker, verdict published, an auto-reply sent in your voice, copied to the AG file — the Spiegel matter enters the Shannon work and the public site (contrary to D-76 "leave out Lance") |
| LA County DA (da.lacounty.gov) | Case mail read; 24STFL00432 monitor; 523 checks | Same as above |
| CA AG / DOJ (doj.ca.gov) | Case mail read | Same; placed on PIU #1564601 |
| FBI / USDOJ (fbi.gov, usdoj.gov, ic3.gov) | Case mail read; federal follow-up | Handed to the federal threads (D-81) |
| LASC (courts.ca.gov) — a motion in 24STFL00432 | Case mail read; 24STFL00432 monitor | Court notices land in both; that is expected for a court filing |
| State Bar (calbar.ca.gov) | **none found** | Lowest collision — but see the State Bar's own court-first requirement |

## What Halsey must decide before ANY Spiegel item is filed (worksheet items W-C1..W-C3)

- **W-C1 — Separate reply channel.** File from an address/route the existing routines do not read
  (e.g., in person, by mail with a postal return address, or a separate mailbox), or
- **W-C2 — Carve-out.** Instruct the Front 4 session (yourself, by your own hand — this thread never
  writes to it) to exclude replies that concern Spiegel from `Case mail read` and the Justice Meter, and
  never to auto-answer them; or
- **W-C3 — Accept the overlap** knowingly.

Until one is chosen, no draft from this thread is marked ready to file.
