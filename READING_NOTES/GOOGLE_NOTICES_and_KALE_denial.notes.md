# GOOGLE NOTICES (EV-049–052), GOOGLE LEGAL (EV-053), KALÉ DENIAL (EV-063), 11/11/2022 THREAD (EV-065 claim)

Reading date: 2026-11-01. Behavior (a). Halsey Minor is the victim and reporting party.
Method: Gmail read-only (get_message / get_thread PLAIN_TEXT; search_threads). Nothing was labelled, moved, trashed, sent or otherwise modified. No git run.
Quotes are verbatim from the native messages. Bracketed text is mine.

---

## 1. Google account notices

All of the following: **From `no-reply@accounts.google.com`**, **To `halsey2005@gmail.com`**, account concerned = **halsey2005@gmail.com**. Each body read in full. Attachments: none listed (inline Google logo only). Each closes "You received this email to let you know about important changes to your Google Account and services."

### EV-049 — four "Critical security alert" notices (identical bodies apart from link tokens)

| # | Date (UTC) | Msg id | Labels |
|---|---|---|---|
| 1 | 2023-09-07 18:08:46Z | 18a70d512865b590 | UNREAD, CATEGORY_UPDATES, INBOX |
| 2 | 2023-09-09 11:55:00Z | 18a79cb99e316376 | UNREAD, CATEGORY_UPDATES, INBOX |
| 3 | 2023-10-10 07:50:54Z | 18b1891454bc580d | UNREAD, CATEGORY_UPDATES, INBOX |
| 4 | 2023-10-21 08:16:44Z | 18b514edd2a06abe | UNREAD, CATEGORY_UPDATES, INBOX |

Subject: "Critical security alert". Every security sentence (verbatim, same in all four):
- "We’ll send a link to sign in to your account in 30 days"
- "Google received a request to recover your account *halsey2005@gmail.com*."
- "If you didn’t make this request, you can cancel it."
- "In *30 days*, we’ll email *halsey@liveplanet.net* with a link to sign in to your account."
- "You can check the status of your request at any time."

Names an actor? **No.** None of the notices says who made the recovery request, from what device, or from where.

### EV-050 — recovery completed, 2023-11-20; recovery email verified 2023-11-28

- 18bed8e553245b27 · 2023-11-20 16:26:45Z · Subject "Security alert" · labels CATEGORY_UPDATES, INBOX.
  "Your password was changed" · "The password for your Google account halsey2005@gmail.com was changed. If you didn't change it, you should recover your account." · "You can also see security activity at https://myaccount.google.com/notifications"
- 18bed8e4a4bb39c1 · 2023-11-20 16:26:46Z · Subject "Your Google Account was recovered successfully" · labels Label_83, CATEGORY_UPDATES.
  "Account recovered successfully" · "Welcome back to your account" · "If you suspect you were locked out of your account because of changes made by someone else, you should review & protect your account."
- 18bed8e4a8de5817 · 2023-11-20 16:26:46Z · Subject "Security alert" · labels CATEGORY_UPDATES, INBOX.
  "A new sign-in on Android" · "We noticed a new sign-in to your Google Account on a Android device. If this was you, you don’t need to do anything. If not, we’ll help you secure your account."
- 18c15583f81d5464 · 2023-11-28 09:52:31Z · Subject "Recovery email verified for your Google Account" · labels UNREAD, Label_83, CATEGORY_UPDATES.
  "The recovery email halsey@liveplanet.net was verified for your account."
- Forward 19625f47de243ed8 (index: 2025-04-11): NOT read this pass.

Names an actor? **No.** The 11/20 text uses the conditional "someone else" only.

### EV-051 — password change 2022-09-14

- 1833ca16271d09ea · 2022-09-14 15:32:29Z · Subject "Security alert" · labels CATEGORY_UPDATES, INBOX.
  "Your password was changed" · "The password for your Google account halsey2005@gmail.com was changed. If you didn't change it, you should recover your account." · "You can also see security activity at https://myaccount.google.com/notifications"
- The SaneBox (15:34:42Z) and Airmail (15:37:41Z) access grants the index mentions: NOT read this pass (no ids in index).

Names an actor? **No.**

### EV-052 — Halsey's 2025-10-16 preservation letter to Google, and the bounce (not a Google account notice; Halsey's own letter)

- 199ec75f75e16cd7 · 2025-10-16 09:59:37Z · From halsey2005@gmail.com · To legal-support@google.com, halsey2005@gmail.com · Subject "Preservation Request – Gmail Account halsey2005@gmail.com " · labels Label_124, IMPORTANT, Label_132, SENT, INBOX. Read in full.
  His words (his adopted account, not Google's): "In the timeframe between April 2025 and September 2025, my Gmail account was the target of a sophisticated unauthorized breach." · "numerous emails (including entire conversation threads) were permanently deleted from my mailbox without my knowledge or consent." · requests preservation of emails "permanently deleted from halsey2005@gmail.com between approximately April 1, 2025 and September 1, 2025" and "records of any unusual login sessions (IP addresses, device information, etc.)". The letter names no perpetrator: "Such logs can help identify the perpetrator of the hack".
- 199ec76298c0a6ff · 2025-10-16 09:59:50Z · From mailer-daemon@googlemail.com · Subject "Delivery Status Notification (Failure)" · attachment icon.png.
  "Your message wasn't delivered to legal-support@google.com because the address couldn't be found, or is unable to receive mail." · "Status: 5.1.3"

Names an actor? **No.**

---

## 2. EV-053 — Google Legal's "valid legal process" reply

- **19af06ba182f7aa6** · **2025-12-05 21:29:36Z** · From **google-legal-support@google.com** · To halsey2005@gmail.com · Subject "Re: URGENT: Evidence Preservation Request – Criminal Investigation – Account Halsey2005@gmail.com" · labels Label_124, IMPORTANT, Label_132, Label_53, CATEGORY_PERSONAL · no attachments. Read in full:
  > "Dear Halsey McLean Minor:
  > Google's Legal department is in receipt of your letter dated 12/04/2025. Google only takes steps to preserve data upon being properly served with valid legal process. You may wish to request preservation after serving Google with valid legal process.
  > To learn more about serving Google with a civil subpoena or other legal process that requests user data, please see our help center article at https://support.google.com/faqs/answer/6151275?hl=en.
  > Thank you for your compliance with this policy.
  > Regards,
  > Google Legal Support"
- Thread 19aeb71fdbbceb23 (4 messages, all read): (i) 19aeb813a9016750 · 2025-12-04 22:35:05Z · mailer-daemon · **"Delivery Status Notification (Failure)"** · bounce of mayorandcitycouncil@beverlyhills.com ("returned Null MX"); (ii) the Google Legal reply above; (iii) 19af167fed51179c · 2025-12-06 02:05:15Z · Halsey forward "FYI. Action: Make Record" to akale@beverlyhills.org and ten City addresses; (iv) 19af1682da9e15a2 · 2025-12-06 02:05:27Z (= Fri 12/5 18:05 PST) · mailer-daemon DSN, nhuntcoffey@beverlyhills.org "BLOCK-SEND-ER".
- **Exhibit C p14 reconciliation (fact only):** p14's printout header reads "Delivery Status Notification (Failure)" over the google-legal-support Fri Dec 5, 2025 4:29 PM message (DECL_2026-03-27_exhibits_A-C.notes.md L141-143). The native message 19af06ba182f7aa6 sits in thread 19aeb71fdbbceb23, whose first message carries the subject "Delivery Status Notification (Failure)". No DSN in that thread or in the 12/4–12/6 search reports a failure to any Google address. Halsey's 12/04/2025 letter itself was NOT returned in the thread or by search (`"Evidence Preservation Request" after:2025/12/03 before:2025/12/07`; `in:anywhere … preservation OR legal-support OR google-legal-support`).
- Related, same day: 19aeb814db96053b · 2025-12-04 22:35:10Z · lis-noreply@google.com · Subject "[5-5346000040263]": "This is an automatic response to let you know that Google Emergency Records has received your emergency request." (His 22:48:19Z reply 19aeb8d557da367f quotes a pasted text with "[google +2]"/"[reddit +1]" citation markers, which look like AI output; it is not Google's words.)

Names an actor? **No.** Google states a policy; it names no one who accessed the account.

---

## 3. EV-063 — Det. Kalé (akale@beverlyhills.org), thread 19b9f7b82104dd6f

19bb38cf19aec75b is a message id; its thread is 19b9f7b82104dd6f (18 messages per header; 17 returned). All three Kalé messages were read in full. Halsey's own messages were read only where Kalé's replies quote them (1/11 and 1/12 22:24Z, 1/13 5:32 PM PT); his other messages were seen by snippet only.

**(a) 19bb38cf19aec75b · 2026-01-12 18:51:48Z** · To halsey@minorventures.com · cc halsey2005@gmail.com · "RE: Fwd:" · attachments image001.png, image002.png, image003.png (not opened). Kalé's sentences on Google / preservation / hold:
- "I am sorry you think I am part of some elaborate corruption scheme to hide/destroy evidence. I can assure you this is not the case, as I would not know how to be a part of a “Scalpel-like hacking” operation."
- "Like I said – we still have that original 567-page document you sent us. That document has not been compromised at all."
- "Regarding the Gmail emails you spoke about from November of 2022 – we have that page of the document showing the emails between you and Shannon, as seen below:"
- **"In the case you think someone hacked your Gmail account and now you no longer have access to that original email, I have submitted a preservation request to Google for those emails (assuming they are still preservable). The request was made for two accounts: Halsey2005@gmail.com and Shannonminor@gmail.com."**

**(b) 19bb480c18e327b1 · 2026-01-12 23:17:56Z** · To halsey2005@gmail.com:
- "I was simply updating you on the case status regarding the preservation letter to Google."
- "My work on this case has included multiple interviews of involved witnesses and serving a search warrant for the related bank statements."

**(c) 19bba42b48bd3355 · 2026-01-14 02:08:06Z** · To halsey2005@gmail.com: "You did not really answer my one question - but I will continue working the case and let you know when I have submitted it to the DA’s Office for filing consideration." (Nothing on Google, a hold, the firm or Spiegel.)

**Kalé says nothing about Spiegel, Lance, or the firm (YS Family Law) in any of the three messages.** He uses the word "hold" nowhere. Those names appear only in Halsey's quoted text.

Names an actor for account access? **No.** "someone hacked" is conditional ("In the case you think…").

---

## 4. The 11/11/2022 email (EV-065's "surgically deleted on August 4, 2025")

- Searches `after:2022/11/10 before:2022/11/13 from:halsey2005@gmail.com` and `… to:shannonminor@gmail.com` (includeTrash) each returned 1 thread: **18461348b9fe0954**.
- **It is present in the mailbox now. All 5 messages were returned. None is labelled TRASH:**
  - 18461348b9fe0954 · 2022-11-10 11:02:23Z · alerts@notify.wellsfargo.com → halsey2005 · "Wells Fargo deposit hold alert" · IMPORTANT, CATEGORY_UPDATES, INBOX
  - 18467dbd3ea6fa47 · 2022-11-11 18:02:50Z · halsey2005 → shannonminor@gmail.com · "Fwd: Wells Fargo deposit hold alert" · body "?" + forward · **SENT**
  - 18467dd2c7361b33 · 2022-11-11 18:04:12Z · shannonminor@gmail.com → halsey@minorventures.com · "Re: …" · "Yes! Large number has a 10 day hold" · IMPORTANT, CATEGORY_PERSONAL, INBOX
  - 1846822a40fdff6d · 2022-11-11 19:20:11Z · halsey2005 → shannonminor · "From the government!" · **SENT**
  - 1846823e63d233ca · 2022-11-11 19:21:15Z · shannonminor → halsey@minorventures.com · "Yes" · IMPORTANT, CATEGORY_PERSONAL, INBOX
- I did not alter it. These documents do not show whether any message was ever deleted and restored.

**2025-08-04 window:** `in:anywhere after:2025/08/03 before:2025/08/06` (METADATA_ONLY, includeTrash): **resultCountEstimate 449 threads**. The first page held 50; the tool returned no page token, so I could not enumerate an exact count. **No Google security notice was found in the window.** `from:no-reply@accounts.google.com` returned **0**. `from:google` returned 6 threads (calendar-notification ×4, voice ×2). `"security alert" OR "sign-in"` returned 13 threads, none from Google.

---

## 5. WHAT THESE DOCUMENTS SHOW / DO NOT SHOW (PC 502(c): "Knowingly … without permission"; actor = "any person")

| Doc | Actor named | Dates fixed | Operative words |
|---|---|---|---|
| EV-049 ×4 | none | 2023-09-07, 09-09, 10-10, 10-21 | "Google received a request to recover your account" |
| EV-050 | none | 2023-11-20 16:26:45–46Z; 2023-11-28 | "Welcome back to your account"; "changes made by someone else" (conditional) |
| EV-051 | none | 2022-09-14 15:32:29Z | "The password … was changed. If you didn't change it…" |
| EV-052 | none (Halsey as author) | 2025-10-16; bounce +13 s | his "unauthorized breach" Apr–Sep 2025 |
| EV-053 | none | 2025-12-05 21:29:36Z | "Google only takes steps to preserve data upon being properly served with valid legal process." |
| EV-063 | Kalé (as requester only) | 2026-01-12, 01-14 | "I have submitted a preservation request to Google" |
| 18461348b9fe0954 | — | 2022-11-10/11 | present, 5 messages, not TRASH |

**No document read here names any person as the one who accessed, altered or deleted anything in Halsey's accounts.** They give dates of Google account events and of preservation requests. None identifies who caused an access or event, or any lack of permission by a named person.

Not read this pass: forward 19625f47de243ed8; SaneBox/Airmail 2022-09-14 grants; Kalé's image attachments; the help-center page; Halsey's 12/04/2025 letter (not located).
