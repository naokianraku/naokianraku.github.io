---
title: FAQ (Pixel Watch & Android)
---

# FAQ — MaxRecovery Timer for Pixel Watch & Android

**Last updated / 最終更新:** (set on release / 公開時に設定)
**Contact / 連絡先:** anraku.tech@gmail.com

> 🌐 言語 / Language: **English** / [🇯🇵 日本語](faq-ja.html)

> 🐛 Report bugs & suggestions: **[Feedback form](../feedback.html)**

---

### 1. Subscription & Billing

**Q. How much is Premium?**
Premium is an auto-renewing subscription with a **Monthly plan** and a **Yearly
plan**. Prices are loaded from Google Play and shown on the app's Premium screen and
on the Google Play purchase screen, in your local currency. First-time Premium
subscribers get a free period (such as **"Premium: first month free"**). Google Play
decides eligibility; if you are eligible, the free period is shown on the Premium
screen and the purchase screen.

**Q. What does Premium unlock?**
Per-set **recovery curves** with the straight **slope line** for each set (the
"Show slope lines" toggle, plus per-set slope (bpm/min), R² and lag), the
**advanced Analytics** (HRR trend, recovery-slope trend, by-set-count /
by-session-length averages, set-position HRR, the recovery-curve overlay, and
the recovery summary), the **PDF report** (generated from the Analytics tab),
**CSV import/export**, the **heart-rate chart image** in share + **Save graph to
Photos**, the experimental new Afterglow value **β** (when you also turn it on in
Settings → Experimental), the **Premium app icon**, and **no banner ads**.
(The personal z-score / vs-previous comparison, the movement-quality score, the
end-location map, the free overview cards (streak / best sessions / heatmap /
map), and the basic per-session and Analytics analysis are **free** — see
below.)

**Q. What is free?**
The heart-rate chart with phase bands, the absolute Afterglow score, the
per-set breakdown, the **Detailed data** card (Max / Min / Avg HR, HR drop,
HRR1 / HRR3 / HRR5), the history list (left-swipe a row to reveal a trash button,
then tap it to delete a single session), the **personal z-score (個人比) and vs-previous (前回比)** comparisons,
the movement-quality (Flow) score, the **end-location map with venue-name
entry** (nearby-venue search up to 5 times a day), the **basic Analytics** (Afterglow-over-time, by-mode average, and the
period summary), sharing the heart-rate graph as **text**, watch-settings
editing, and the Force-English toggle. The **free overview cards** in the
**Analytics** tab (current / longest streak and total count, the **Best Sessions
TOP 10**, the visit-frequency calendar heatmap, and the Venue Map of your
visited venues) are also free, as are the **Sleep score** and the **resting-HR
reference line** when you connect Health Connect.

**Q. Is watch ↔ phone sync Premium?**
No. Finished sessions transfer from the Pixel Watch to your Android phone
automatically over the Wearable Data Layer, for everyone. The optional Google
Drive cloud sync (see "How does cloud sync / backup work?" below) is also
**free** — there is nothing to gate behind Premium here.

**Q. Where do I subscribe?**
Open **Settings → Premium → "Upgrade to Premium"**, or tap **"See Premium"** on the
locked recovery curve, advanced Analytics or CSV import/export, to reach the Premium
screen, then tap the button for the Monthly or
Yearly plan. If you're eligible for the free period, the button reads "Start … free,
then …"; otherwise it reads "Subscribe for …". The price after the free period,
automatic renewal and how to cancel are shown right next to each plan's button.

**Q. How does auto-renewal work?**
When the free period ends, your subscription automatically becomes a paid
subscription at the plan's price and renews every month (Monthly plan) or every year
(Yearly plan) until you cancel. If you cancel in Google Play before the next renewal
date, you are not charged for later periods. Cancel during the free period and you
won't be charged.

**Q. How do I switch between the Monthly and Yearly plans?**
Open **Settings → Premium → "Premium member (view or change plan)"** and tap "Switch
to yearly" or "Switch to monthly". The new plan starts right away and the new price
applies from your next billing date. (Plans can't be changed from the Google Play
Store's subscription screen.)

**Q. How do I cancel?**
Open the Google Play Store → tap your profile → **Payments & subscriptions** →
**Subscriptions** → this app's Premium (MaxRecovery Premium) → Cancel subscription.
While subscribed, **"Manage subscription (cancel, payment)"** on the app's Premium
screen opens it too. After canceling, you keep Premium features until the end of the
period you've paid for.

**Q. Does canceling delete my data?**
No. Your sessions, history, and settings all stay (they are stored locally on
each device). Only the Premium features (recovery curves and slope
lines, the advanced Analytics, the PDF report, CSV import/export, the HR-graph
image share / save, the β experimental value, the Premium app icon, ad-free)
revert to the free tier. If you used the Premium app icon, the app icon switches
back to the default once Google Play confirms that Premium has ended (if you
subscribe again and the setting is still on, the Premium icon comes back).

**Q. It says "Your subscription is on hold".**
Your subscription is on hold because of a payment problem or because it's paused,
and Premium isn't available until it's resumed. Tap **"Open Google Play (payment,
resume)"** in Settings or on the Premium screen, then update your payment method or
resume the subscription in Google Play; Premium comes back once it's active. During a
payment grace period you keep Premium, and Google Play asks you to fix your payment
method.

**Q. I paid but Premium isn't active on a new device.**
Make sure you're signed in to Google Play with the Google account you used to
subscribe, then open the Premium screen from **Settings → Premium** and tap
**Restore purchase** to re-check your Google Play entitlement.

**Q. Can I use Premium I bought on the iPhone version?**
No. Premium on the iPhone version (App Store) and on the Android version (Google
Play) are separate purchases and don't carry over to each other.

**Q. Refunds?**
Google handles all refund requests for Google Play purchases. Use your Google
Play order history at [play.google.com](https://play.google.com).

### 2. Data and Privacy

**Q. What data do you collect?**
The developer does not collect, receive, or store any of your data. There is no
server and no account. Session data, heart-rate data, and locations are stored
on your devices (and, if you use cloud sync, in your own Google Drive) and are
**not** sent to the developer. Note that showing maps and searching for nearby
venues sends the session's end location to Google. For ads in the free
version (AdMob), see the question below.

**Q. Where is my data stored?**
By default, locally on your Android phone and your Pixel Watch (local JSON
files). When the two are paired, finished sessions transfer Watch → Phone
directly over the Wearable Data Layer (Bluetooth / Wi-Fi); the watch keeps each
session and resends it until the phone confirms it was received. Watch settings sync
bidirectionally, so you can edit watch settings from the phone (if you change them
on both, the newer change to each item is kept). There is **no**
developer server and **no** login to the developer. **Optionally**, you can turn
on **Cloud sync (Google Drive)** to back up a snapshot of your sessions to
**your own** Google Drive — see "How does cloud sync / backup work?" below.
Cloud sync is **off** until you sign in and tap Sync. Note that if Android backup is
on for your phone, Android may back up a copy of the app's data to your Google
Account (see "What if I delete the app?" below).

**Q. How does cloud sync / backup work?**
Cloud sync is **optional and free**. In **Settings → Cloud sync (Google Drive)**
you tap **Sync with Google Drive**: the app signs you in with Google and uses
the `drive.appdata` permission to store and retrieve a snapshot of your sessions
in **your own** Google Drive — in its app-private, hidden "App Data" folder
under your Google account. The purpose is to back up your sessions and move them
between devices; sync is **two-way and merges by session**. Syncing happens when
you tap the button (not automatically). If the cloud data can't be fetched or read,
or if saving would reduce the number of sessions in the cloud, the app **stops
without changing the cloud** and tells you why. Deletions are synced too (see the
next question). If you sync two or more devices, update the app on all of them
before syncing. Importantly, **the
developer still operates no server and stores nothing**: your data goes to your
own Google Drive, not to the developer, and the developer cannot access it. It
stays **off** until you sign in / tap Sync — if you do not use it, your data
stays on your devices (Watch ↔ Phone over the Wearable Data Layer) exactly as
before. You can **delete** the synced data from your own Google Drive at any
time, and **revoke** the app's access whenever you like by deleting its
connection in your Google Account → Security → "Your connections to third-party
apps & services" (the app itself has no disconnect setting).

**Q. Are deleted sessions also removed from the cloud and my other devices?**
Yes. Both a single-session delete (left-swipe → trash) and **Settings → Data →
"Delete all received data"** are applied, if you use Google Drive sync, to **the
cloud and your other synced devices at the next sync**. Deleted sessions don't come
back from a watch resend or from Drive sync (the app keeps only each deleted
session's ID and the time it was deleted, to keep it from coming back). To bring
sessions back, restore them explicitly with CSV import (Premium); the restore also
reaches your other devices at the next sync. Devices running an older version of the
app can't read the deletion records, so deleted sessions stay on those devices —
update the app on all of them.

**Q. What if I delete the app?**
Data is stored on-device by default, so deleting the app removes its data from the
device. However, if **Android backup** (backup to your Google Account) is on for your
phone, Android may have backed up the app's data (such as your sessions, deletion
records and settings) automatically, so **your sessions may come back** when you
reinstall the app with the same Google Account or move to a new phone (the watch
app's data may likewise be included in the watch's backup). That backup is handled
by Google and is separate from the app's Cloud sync (the developer can't access it).
If you don't want the restored sessions, delete them from History or with
**Settings → Data → "Delete all received data"**.
The free way to keep a reliable backup is **Cloud sync (Google Drive)** — once
enabled, your sessions are stored in your own Google Drive and can be re-synced after
reinstalling. Premium members can also use CSV export in **Settings → Data
import/export (CSV)** as a manual backup and re-import after reinstalling.

**Q. Where does the heart rate come from?**
The app reads heart rate live from the Pixel Watch's optical sensor via Wear OS
Health Services (the watch's workout feature) during a session. If heart rate can't
be read (no heart rate permission, no sensor, no readings, etc.), the watch **keeps
timing without heart rate** and shows **"Heart rate unavailable"**. On the phone,
that session is marked "No heart-rate data (reason)" and is not used for scores (see
below).
**Optionally**, if you connect **Health Connect** (Settings → Health Connect,
with your permission), the app can also read your **Resting heart rate** and
draw it as a reference line on the session HR chart, and **export your
sessions** to Health Connect as exercise + heart-rate records with **"Export
sessions to Health Connect"** in Settings, so other apps can use them (export is
manual, not automatic, and exporting again never creates duplicates). Health
Connect is entirely optional — if you do not connect it, the app works exactly as
before with no health-data integration.

**Q. What is the Sleep score / Next-day status?**
If you connect **Health Connect** and you have **sleep data** recorded there,
the session detail can show a **Next-day status** section for the night **after**
a session: a reference **Sleep score** (free) and your average respiratory rate
for that night, read from Health Connect. These are reference values only and
require both Health Connect to be connected and sleep data to be present — if
either is missing, the section simply does not appear.

**Q. Does the free version share my data with advertisers?**
Without Premium, the app shows an AdMob banner ad. Ad-network data handling follows
Google's policies and your device's privacy settings (Android advertising-ID
controls under system Settings → Privacy → Ads). In the EEA, the UK and
Switzerland, the app shows Google's consent form (UMP) before ads are loaded. Where
the law requires it, such as in some US states, you can choose how your data is used
for ads (see the next question). Heart-rate, location and Health Connect data are
never used for ads or given to ad networks. Premium removes ads. See the Privacy
Policy for details.

**Q. How do I change my ad consent (privacy settings)?**
Use **Settings → Help & legal → "Ad privacy settings"**. This item appears only where
a way to change consent or opt out is required, such as the EEA, the UK, Switzerland
and some US states (it normally doesn't appear in Japan). To reset or delete your
advertising ID, use Android Settings → Privacy → Ads.

### 3. Usage & Features

**Q. What is the Afterglow Score?**
A 0–100 score estimating how quickly your parasympathetic nervous system
("rest mode") engages after a sauna session, derived from your heart-rate
recovery (HRR1 / HRR3 / HRR5). It puts a number on what Japanese sauna culture
calls "totonou". The absolute score, the personal z-score (個人比) and the
vs-previous (前回比) comparisons are all **free**; the experimental new Afterglow
value **β** is Premium (and only when you turn it on in Settings →
Experimental). Reference value only — not a medical metric.

**Q. Can I use the app without a Pixel Watch?**
No. **Timing and heart-rate measurement run in the watch app, so a Pixel Watch
(or other Wear OS smartwatch) is required.** The phone app is for reviewing and
analyzing the sessions sent from the watch.

**Q. How do I control the timer with wet hands during a session?**
Use the **rotary crown**: rotate **up** to advance to the next phase, rotate
**down** to pause. To resume, rotate **up** again. **During a running session the
screen does not respond to touch** (to prevent wet-hand misfires) — on watches
without double pinch, the crown is the only control. **On Pixel Watch 3 and later you can also double pinch (tap your
thumb and index finger together twice) to advance** (a Next button is shown while
running). **While paused**, an on-screen menu appears with **Resume / Back / End**.
If you prefer touch controls, turn on **Settings → Watch
settings → "Show control buttons"** to also show Next/Pause buttons during a
running session. There is also an optional **"Double-tap to advance"** gesture
(beta, OFF by default; for watches without double pinch). Phase times are **haptic
alerts only** — the app does not auto-advance, so you choose when to move on. When a
confirmation or warning appears, turning the crown (either way) closes it too (it
cancels a confirmation and continues on the inactivity warning, without changing
phase); End is tap-only.

**Q. The second "Next" in a row doesn't respond.**
To prevent skipping two phases by accident, **a Next within 1 second of the previous
input is ignored**, whether it comes from the crown, double pinch, the Next button or
the body double-tap. Also, the crown works as **one turn, one phase**: keeping on
turning doesn't advance a second phase. To advance again, stop and wait at least 1
second.

**Q. Turning my wrist shows "End session?".**
In the latest version, **wrist turn is disabled during a session** (Pixel Watch 3 and
later). It only closes a confirmation or heart-rate alert that is already open. If
the confirmation does appear, close it by **turning the crown** (either way), with a
double pinch, or by tapping **Cancel**; the session keeps running. Even in earlier
versions, that confirmation closes by itself after 5 seconds and the session doesn't
end unless you tap **End**. Please update the app.

**Q. Can I use the system "Water Lock" during a session?**
**It's best not to.** Wear OS Water Lock is exited by **turning the crown**, so
while it's on the crown can't change phase or pause either. The app **already
ignores screen touch during a session** (to prevent wet-hand / splash mis-taps,
except for buttons such as Next), so Water Lock isn't needed — leave it off and just
use the crown.

**Q. Does recording keep running in the background during a session?**
The session runs in a **foreground service with an ongoing notification**. While a
session runs, an ongoing-activity icon appears on the watch face, and the session
keeps running if you go back to the watch face or the screen turns off (tap the icon
or the notification to return to the session screen). While the session screen is
shown, the display is kept on by default. However, **without the Heart rate
permission** the foreground service can't run, so recording may stop when the screen
turns off (the watch tells you). Also, when the watch's workout feature can't be used
(for example while another app is recording a workout), heart rate may stop while the
screen is off. Keeping the session screen open during a session is recommended.

**Q. Can I interact with the heart-rate chart?**
Yes — the HR chart is interactive. **Tap a point** to see a value card showing
the bpm, the elapsed time, and the phase at that point. **Pinch to zoom** in up
to 20×, **drag to scroll** along the timeline, and **double-tap to reset** the
view.

**Q. Can I add moving-average lines or hide the preparation phase on the chart?**
Yes. In **Settings → Display** you can toggle two trailing moving-average
overlays on the HR chart — **"Show 60s moving average"** and **"Show 10min moving
average"** — each independently. There is also a **"Hide prep phase from chart"**
toggle that re-bases the X axis so 0:00 is your sauna entry. All three default
to **OFF**.

**Q. What's the difference between Standard and Simple mode?**
Standard mode tracks distinct phases (Sauna → Cold bath → Cool-down) per set,
with per-set times and HR thresholds, plus an optional Prep phase and an
optional extra phase. Simple mode doesn't split the cold bath and cool-down into
phases: at each set break **you move to the next set yourself** (rotate the crown
up, or use the Next set button / double pinch). There is no set limit; to finish,
pause and tap End. One sauna time and one pair of HR thresholds apply to every set,
and the Prep phase can be used too. On the phone, the per-set breakdown and the
recovery curves are found from your heart-rate peaks.

**Q. What is HRR (HRR1 / HRR3 / HRR5)?**
HRR = Heart Rate Recovery. HRR1 is your heart-rate drop 1 minute after the
peak, HRR3 at 3 minutes, HRR5 at 5 minutes. Higher means faster recovery,
which is the basis for the Afterglow Score.

**Q. What is the recovery slope?**
A Premium analytics metric (bpm/min) — the slope (β) of the linear-fitted
central portion of your recovery curve. Steeper means faster recovery.

**Q. What is the Movement Quality score?**
A score (0–100, Excellent / Good / Average / Needs work) that measures how
many heart-rate spikes occur after each sauna peak. Long walking distances
between sauna → cold water → cool-down area cause HR rebounds; fewer spikes =
better facility flow. The per-session score is **free** in the session
analysis; the detailed breakdown and the period-average (in the Premium PDF
report) are Premium.

**Q. What is in the History tab?**
The **History** tab is now just the **session list**. Tap a row to open that
session's full analysis. **Left-swipe a row to reveal a trash button, then tap it
to delete that single session** (no confirmation dialog — deletion is immediate);
this is the only per-session delete. The free
overview cards (streak, best sessions, heatmap, map) have moved to the
**Analytics** tab — see below.

**Q. Where did the streak / best / heatmap / map overview go?**
**Free.** Those overview cards moved from the History tab to the **Analytics**
tab. The app shows your **current and longest streak** plus your **total session
count**, a **Best Sessions TOP 10** ranking (by Afterglow score), a
**visit-frequency calendar heatmap**, and a **Venue Map** that plots all of your
visited venues on one map. These are all free and live in the app (no Premium and
no PDF required).

**Q. How do I delete a single session?**
In the **History** tab, **left-swipe** the session row to reveal a **trash
button**, then **tap the trash button** to delete just that one session. There is
no confirmation dialog — deletion is immediate. This left-swipe is the only
per-session delete. If you use Google Drive sync, the session is also removed from
the cloud and your other devices at the next sync.

**Q. How do I generate a PDF report?**
Premium feature. From the **Analytics** tab, generate the report and share it via
the Android share sheet (file name `MaxRecovery_Report_<start>_<end>.pdf`). An
A4-portrait, 3-page report is produced:
- **Page 1**: sessions summary, Afterglow trend, heart-rate trend, and recovery
  data (HRR1 / HRR3 / HRR5, plus recovery details)
- **Page 2**: recovery-curve small multiples (latest 11 sessions) plus a
  session-average overlay
- **Page 3**: **Best Sessions TOP 5**, a recent-sessions table, and a
  visit-frequency heatmap

Sessions without heart-rate data are not used for the score and recovery-curve
pages; they only appear in the recent-sessions table. The Best Sessions ranking and
the visit/calendar heatmap are **also available free in the Analytics tab** (TOP 10
there); the PDF still includes its own versions as part of the exported report.

**Q. What is in the Analytics tab?**
The Analytics tab is **partly free**. **Free:** Afterglow-over-time, average
Afterglow by mode, the period summary, and the free overview cards (current /
longest streak and total count, Best Sessions TOP 10, the visit-frequency
heatmap, and the Venue Map). **Premium:** the HRR trend (1/3/5), the
recovery-slope trend, average Afterglow by set count / by session length,
set-position HRR, a recovery-curve overlay, the recovery summary (avg HRR1/3/5,
best set position, best HRR1, recovery completeness, time-to-bottom,
front-loading), and the PDF report button. A period filter (All / 30 days /
7 days) is available to everyone.

**Q. Can I save or share the heart-rate graph image?**
**Free:** the **Share** button on the heart-rate chart shares **text only**
(basic info). **Premium:** "Save graph to Photos" + "Share graph" share detailed
text **plus a PNG image** of the HR chart; you can choose "Info + HR graph" or
"HR graph only". Saved images (`MaxRecovery_<date-time>.png`) go to your device's
own Photos (Pictures/MaxRecoveryTimer) — nothing is uploaded. **Images saved with
earlier versions stay in Pictures/MaxSaunaTimer** (they are not moved).

**Q. The CSV file names changed.**
With the new app name, exported files are named `maxrecovery_*.csv` (sessions),
`maxrecovery_sets_*.csv`, `maxrecovery_phases_*.csv` and
`maxrecovery_hr_samples_*.csv` (the same as the iPhone version). The columns haven't
changed, and files exported by earlier versions (`max_sauna_*.csv`) can still be
imported.

**Q. What are the recovery-curve slope lines?**
Premium feature. On the per-set recovery curve the app overlays a straight
**slope line** for each set, with a **"Show slope lines"** toggle and a per-set
legend showing the slope (bpm/min), R², and lag (seconds). Dashed 1-minute and
3-minute guide lines are also drawn.

**Q. What is the "Detailed data" card?**
**Free.** In the session detail the **Detailed data** card shows your **Max HR,
Min HR, Avg HR, HR drop (peak − min)**, and **HRR1 / HRR3 / HRR5** for that
session.

**Q. What is the experimental new Afterglow value (β)?**
β is an **experimental** new Afterglow value. It is shown only when you are
**Premium** AND you turn on **Settings → Experimental → "Show new Afterglow
value (β)"**. On the free tier it is not shown at all and the Experimental
section is hidden.

**Q. What is the Premium app icon?**
A Premium-only option. In **Settings → Premium**, "Use Premium app icon"
switches your home-screen app icon to the Premium logo. When Premium ends, the icon
switches back to the default.

**Q. The self-rating ★ I entered on the watch — where does it show?**
In the session detail header, e.g. "Standard • 2 sets • 58min • ★5".

**Q. How does the venue / map work?**
**Free.** If Location permission is granted, the app captures the session **end**
location once when the session ends and shows it on a Google Map in the session
detail. You can set the venue name in these ways:
- **Your past venues (within 500 m)**: names you entered before are listed
  first, and **one tap sets the venue** (no Google search). For a venue you
  have visited before, this is all you need.
- **"Find nearby venues"**: searches Google Maps for nearby sauna / bath
  facilities **only when you tap it** (never automatically) and lists the
  suggestions with the Google Maps logo. Tap a suggestion to open an empty
  venue-name dialog, with the suggested name shown outside the text field for
  reference. Type the name you want to keep and save.
- **Type it in**: use "Enter venue name", or "**+ Add venue name**" in the
  session-detail header. This works even for sessions without a location.

There is no continuous GPS tracking. Each session can also have a 1–5 star
rating.

**Q. Why doesn't tapping a suggestion fill in the venue name?**
Because the Google Maps Platform terms don't allow the app to store venue names
from Google's suggestions. Suggestions are shown for reference only, and the app
saves **only the venue names you type in** (the suggestion list itself is never
saved on your device; it is kept in memory for up to 30 minutes). Once you have
typed a name, it appears under "Your past venues" for nearby sessions (within
about 500 m), ready to set with one tap.

**Q. Is there a limit on nearby-venue searches?**
Yes — **5 per day per device** (Premium included). The count resets when your
device's date changes. A search that finds no suggestions still counts as one.
If you reopen a session at the same place within 30 minutes, the previous
suggestions are shown again without using a search (they can be cleared sooner,
for example when the app is fully closed). If the app-wide daily search limit is
reached, the app tells you so and shows when search will resume. Either way,
you can type the venue name in with "**Enter venue name**".

**Q. The venue names I set earlier are gone.**
Venue names picked from suggestions in earlier versions can't be stored under
Google's terms, so they are removed the first time the updated app starts (the
app tells you how many, once). You can add them again by typing. Venue names
imported from CSV are removed too, because earlier versions couldn't tell them
apart from picked suggestions — import the CSV exported from the iPhone app
again to bring them back (CSV import/export is Premium).

### 4. Troubleshooting

**Q. Watch session data isn't reaching my Android phone.**
Open the MaxRecovery Timer app on both devices, keep them nearby with Bluetooth (or
Wi-Fi) on, and relaunch both apps. The watch keeps each session until the phone
confirms it was received and resends it automatically once they reconnect (the
phone app also picks up sessions it missed when it starts). If there is still no
confirmation after 1 hour, the watch history marks the session **"Not on phone
yet"**. If the watch home screen says **"Update the phone app to receive N
session(s)."**, the phone app is too old to receive long sessions — update it from
Google Play and the sessions arrive automatically.

**Q. Heart rate isn't showing on the watch.**
Make sure the watch is worn snugly and that the Heart rate permission is allowed.
When heart rate can't be read, the heart-rate field shows "—" (the last reading is
more than 10 seconds old) or "♡×" (unavailable), and a **"Heart rate unavailable"**
notice appears. The timer keeps running and the session is recorded without heart
rate. If the permission is off, allow "Heart rate" ("Sensors" on earlier watch
software) in the watch's **Settings → Apps → MaxRecovery Timer → Permissions** (if you
declined only once, the "Before you start" screen asks again when you start a
session).

**Q. The watch says "Unfinished session".**
If the app stopped unexpectedly during a session, the session kept restarting, or
the last save was more than 60 minutes ago, the watch asks instead of resuming
automatically. Tap **Continue** to resume, **Save** to save what was recorded and
end, or **Discard** to throw that session away.

**Q. Watch battery drains during a session.**
While a session screen is on, the display is kept awake and a foreground
service runs so the timer and heart-rate keep running, which uses more battery
than an idle watch. The app auto-ends after 60 minutes with no input (it warns
first, then auto-ends) to protect the battery. There is also an optional low-HR
warning during cold water / cool-down.

**Q. The Afterglow Score didn't appear after my session.**
The score needs valid heart-rate data after the peak. If you ended the session
within 1 minute of the sauna peak, or the watch lost contact (dropouts), the
score may be missing. Sessions with too few samples are marked as unscored.
Sessions where the watch couldn't read heart rate are marked **"No heart-rate data
(reason)"** and are not used for the Afterglow Score, personal comparisons, recovery
curves, trends or the PDF report (they still count toward visits, total time and
streaks).

**Q. A red banner says the history file couldn't be read.**
Your phone's history file (or some records in it) was damaged and couldn't be read,
so the app **set it aside and kept it** instead of overwriting it. Tap **"Export the
set-aside file"** on the banner and choose where to save it. Set-aside files are also
listed under **Settings → Data import/export (CSV) → "Set-aside history files"**, and you
can export them without Premium. Attaching them when you contact support helps us
investigate. If the banner asks you to restart the app, please do so.

**Q. Health Connect has duplicate sessions / names still say "Sauna".**
The latest version never creates duplicates, however many times you export. Records
exported by earlier versions may be duplicated and keep the name "Sauna" (the latest
version names records without a venue "MaxRecovery"). Tap **Settings → Health Connect
→ "Clean up duplicates from earlier exports"**: for the time ranges of the sessions
on your phone, the exercise and heart-rate records this app exported earlier are
deleted and exported again. Data from other apps is not affected. Records of
sessions you deleted from the phone remain; delete them in Health Connect if you
don't need them.

**Q. The resting-HR line, Sleep score, or Next-day status isn't showing.**
These come from **Health Connect**. Make sure you connected it in **Settings →
Health Connect** and granted the relevant read permissions, and that the data
exists there (a recorded resting heart rate, and sleep data for the night after
the session). If Health Connect is not connected, or the data is missing, those
items simply do not appear and the rest of the app is unaffected.

### 5. Other

**Q. Can I switch the app to English?**
Yes. Both the phone app and the watch app are available in English and Japanese. The
phone app follows the phone's language setting, and the watch app follows the watch's
own language setting (on both, languages other than Japanese show English). Turn on
**Settings → Display → "Force English"** on the phone to show both the phone and the
watch in English regardless of their language settings (if you switch it while a
session is running on the watch, the watch changes after the session ends).

**Q. Can I use this for medical purposes?**
No. The Afterglow Score, heart-rate values, HRR, the Sleep score, and all other
figures are reference information only. They are not medical metrics and must
not be used for diagnosis or treatment decisions. Consult a physician if you
have concerns.

**Q. What is the recommended use?**
Personal wellness tracking. Go at a pace that suits how you feel, and follow the
venue's rules. Avoid using it after drinking alcohol. Follow the manufacturer's
guidance on where to wear your watch.

**Q. How do I contact support?**
Email **anraku.tech@gmail.com**. Please include your Android / Wear OS
versions and a brief description of the issue.

**Q. Where can I find the Privacy Policy and Terms of Use?**
[Privacy Policy](privacy-policy.html) / [Terms of Use](terms-of-use.html).

---

## 関連 / See also

- [Guide / 取扱説明書](guide.html)
- [FAQ / よくある質問](faq.html)
- [Privacy Policy / プライバシーポリシー](privacy-policy.html)
- [Terms of Use / 利用規約](terms-of-use.html)
