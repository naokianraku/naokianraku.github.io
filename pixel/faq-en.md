---
title: FAQ (Pixel Watch & Android)
---

# FAQ — MaxRecover Timer for Pixel Watch & Android

**Last updated / 最終更新:** 2026-06-11
**Contact / 連絡先:** maxsaunatimer@gmail.com

> 🌐 言語 / Language: **English** / [🇯🇵 日本語](faq-ja.html)

> 🐛 Report bugs & suggestions: **[Feedback form](../feedback.html)**

---

### 1. Subscription & Billing

**Q. How much is Premium?**
Check the current price for your region in Google Play (Subscriptions). A yearly
plan is also available at roughly **20% off** vs paying monthly. New
subscribers get a 30-day free trial.

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
the movement-quality (Flow) score, the **end-location map with the nearby-venue
picker**, the **basic Analytics** (Afterglow-over-time, by-mode average, and the
period summary), sharing the heart-rate graph as **text**, watch-settings
editing, and the Force-English toggle. The **free overview cards** in the
**Analytics** tab (current / longest streak and total count, the **Best Sessions
TOP 10**, the visit-frequency calendar heatmap, and the Sauna Map of your
visited venues) are also free, as are the **Sleep score** and the **resting-HR
reference line** when you connect Health Connect.

**Q. Is watch ↔ phone sync Premium?**
No. Finished sessions transfer from the Pixel Watch to your Android phone
automatically over the Wearable Data Layer, for everyone. The optional Google
Drive cloud sync (see "How does cloud sync / backup work?" below) is also
**free** — there is nothing to gate behind Premium here.

**Q. What happens when the free trial ends?**
Your subscription auto-renews at the regular price. You can cancel at any time
during the trial — if you cancel at least 24 hours before the trial ends, you
are not charged.

**Q. How do I cancel?**
Open the Google Play Store → tap your profile → **Payments & subscriptions** →
**Subscriptions** → MaxRecover Premium → Cancel subscription. After canceling,
you keep Premium features until the current billing period ends.

**Q. Does canceling delete my data?**
No. Your sessions, history, and settings all stay (they are stored locally on
each device). Only the Premium features (recovery curves and slope
lines, the advanced Analytics, the PDF report, CSV import/export, the HR-graph
image share / save, the β experimental value, the Premium app icon, ad-free)
revert to the free tier.

**Q. I paid but Premium isn't active on a new device.**
Open Settings and tap **Restore purchase** to re-check your Google Play
entitlement.

**Q. Refunds?**
Google handles all refund requests for Google Play purchases. Use your Google
Play order history at [play.google.com](https://play.google.com).

### 2. Data and Privacy

**Q. What data do you collect?**
The developer does not collect, receive, or store any of your data. There is no
server and no account. All session data, heart-rate data, and locations stay
on your devices and are **not** sent to the developer.

**Q. Where is my data stored?**
By default, locally on your Android phone and your Pixel Watch (local JSON
files). When the two are paired, finished sessions transfer Watch → Phone
directly over the Wearable Data Layer (Bluetooth / Wi-Fi). Watch settings sync
bidirectionally, so you can edit watch settings from the phone. There is **no**
developer server and **no** login to the developer. **Optionally**, you can turn
on **Cloud sync (Google Drive)** to back up a snapshot of your sessions to
**your own** Google Drive — see "How does cloud sync / backup work?" below.
Cloud sync is **off** until you sign in and tap Sync.

**Q. How does cloud sync / backup work?**
Cloud sync is **optional and free**. In **Settings → Cloud sync (Google Drive)**
you tap **Sync with Google Drive**: the app signs you in with Google and uses
the `drive.appdata` permission to store and retrieve a snapshot of your sessions
in **your own** Google Drive — in its app-private, hidden "App Data" folder
under your Google account. The purpose is to back up your sessions and move them
between devices; sync is **two-way and merges by session**. Importantly, **the
developer still operates no server and stores nothing**: your data goes to your
own Google Drive, not to the developer, and the developer cannot access it. It
stays **off** until you sign in / tap Sync — if you do not use it, your data
stays on your devices (Watch ↔ Phone over the Wearable Data Layer) exactly as
before. You can **delete** the synced data from your own Google Drive at any
time, and **revoke** the app's access whenever you like in your Google Account
permissions (or from Settings).

**Q. What if I delete the app?**
Data is stored on-device by default, so deleting the app removes its local data.
The free way to back up is **Cloud sync (Google Drive)** — once enabled, your
sessions are stored in your own Google Drive and can be re-synced after
reinstalling. Premium members can also use **CSV export** (Settings → Data
import/export) as a manual backup and re-import after reinstalling.

**Q. Where does the heart rate come from?**
The app reads heart rate live from the Pixel Watch's optical sensor via Wear OS
Health Services during a session (while the session screen is on). On an
emulator without a real sensor, it falls back to mock heart-rate data.
**Optionally**, if you connect **Health Connect** (Settings → Health Connect,
with your permission), the app can also read your **Resting heart rate** and
draw it as a reference line on the session HR chart, and **write each finished
session back** to Health Connect as an exercise + heart-rate record so other
apps can use it. Health Connect is entirely optional — if you do not connect
it, the app works exactly as before with no health-data integration.

**Q. What is the Sleep score / Next-day status?**
If you connect **Health Connect** and you have **sleep data** recorded there,
the session detail can show a **Next-day status** section for the night **after**
a session: a reference **Sleep score** (free) and your average respiratory rate
for that night, read from Health Connect. These are reference values only and
require both Health Connect to be connected and sleep data to be present — if
either is missing, the section simply does not appear.

**Q. Does the free version share my data with advertisers?**
The free version shows an AdMob banner ad. Ad-network data handling follows
Google's policies and your device's privacy settings (Android advertising-ID
controls under system Settings → Privacy → Ads, and the Google UMP / GDPR
consent prompt where applicable). Premium removes ads. See the Privacy Policy
for details.

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
The timer works on the Android phone alone, but heart-rate measurement and the
Afterglow Score require a Pixel Watch (or other Wear OS smartwatch).

**Q. How do I control the timer with wet hands during a session?**
Use the **rotary crown**: rotate **up** to advance to the next phase, rotate
**down** to pause. To resume, rotate **up** again. **During a running session the
screen does not respond to touch** (to prevent wet-hand misfires) — the crown is
the only control. **While paused**, an on-screen menu appears with **Resume / Go
back one phase / End**. If you prefer touch controls, turn on **Settings → Watch
settings → "Show control buttons"** to also show Next/Pause buttons during a
running session. There is also an optional **"Double-tap body to advance"** gesture
(beta, OFF by default). Phase times are **haptic alerts only** — the app does not
auto-advance, so you choose when to move on.

**Q. Can I use the system "Water Lock" during a session?**
**It's best not to.** Wear OS Water Lock is exited by **turning the crown**, so
while it's on the crown can't change phase or pause either. The app **already
ignores screen touch during a session** (to prevent wet-hand / splash mis-taps), so
Water Lock isn't needed — leave it off and just use the crown.

**Q. Does recording keep running in the background during a session?**
While a session screen is on, the watch keeps the display awake and runs a
**foreground service with an ongoing notification**, so the timer and heart-rate
measurement keep running for the duration of the session. (Fully screen-off
background recording is still being finalized and verified on real hardware.)

**Q. Can I interact with the heart-rate chart?**
Yes — the HR chart is interactive. **Tap a point** to see a value card showing
the bpm, the elapsed time, and the phase at that point. **Pinch to zoom** in up
to 20×, **drag to scroll** along the timeline, and **double-tap to reset** the
view.

**Q. Can I add moving-average lines or hide the preparation phase on the chart?**
Yes. In **Settings → Display** you can toggle two trailing moving-average
overlays on the HR chart — a **60-second** average and a **10-minute** average —
each independently. There is also a **"Hide preparation phase from chart"**
toggle that re-bases the X axis so 0:00 is your sauna entry. All three default
to **OFF**.

**Q. What's the difference between Standard and Simple mode?**
Standard mode tracks distinct phases (sauna → cold water → cool-down) per set,
with per-set times and HR thresholds, plus an optional Preparation phase and an
optional "Other/extra" phase. Simple mode runs as one continuous session and
estimates sets automatically (no manual phases).

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
**visit-frequency calendar heatmap**, and a **Sauna Map** that plots all of your
visited venues on one map. These are all free and live in the app (no Premium and
no PDF required).

**Q. How do I delete a single session?**
In the **History** tab, **left-swipe** the session row to reveal a **trash
button**, then **tap the trash button** to delete just that one session. There is
no confirmation dialog — deletion is immediate. This left-swipe is the only
per-session delete.

**Q. How do I generate a PDF report?**
Premium feature. From the **Analytics** tab, generate the report and share it via
the Android share sheet. An A4-portrait, 3-page report is produced:
- **Page 1**: sessions summary, Afterglow trend, heart-rate trend, and recovery
  data (HRR1 / HRR3 / HRR5, plus recovery details)
- **Page 2**: recovery-curve small multiples (latest 11 sessions) plus a
  session-average overlay
- **Page 3**: **Best Sessions TOP 5**, a recent-sessions table, and a
  visit-frequency heatmap

The Best Sessions ranking and the visit/calendar heatmap are **also available
free in the Analytics tab** (TOP 10 there); the PDF still includes its own
versions as part of the exported report.

**Q. What is in the Analytics tab?**
The Analytics tab is **partly free**. **Free:** Afterglow-over-time, average
Afterglow by mode, the period summary, and the free overview cards (current /
longest streak and total count, Best Sessions TOP 10, the visit-frequency
heatmap, and the Sauna Map). **Premium:** the HRR trend (1/3/5), the
recovery-slope trend, average Afterglow by set count / by session length,
set-position HRR, a recovery-curve overlay, the recovery summary (avg HRR1/3/5,
best set position, best HRR1, recovery completeness, time-to-bottom,
front-loading), and the PDF report button. A period filter (All / 30 days /
7 days) is available to everyone.

**Q. Can I save or share the heart-rate graph image?**
**Free:** the **Share** button on the heart-rate chart shares **text only**
(basic info). **Premium:** "Save graph to Photos" + "Share graph" share detailed
text **plus a PNG image** of the HR chart; you can choose "Info + HR graph" or
"HR graph only". Saved images go to your device's own Photos
(Pictures/MaxRecoverTimer) — nothing is uploaded.

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
switches your home-screen app icon to the Premium logo.

**Q. The self-rating ★ I entered on the watch — where does it show?**
In the session detail header, e.g. "Standard • 2 sets • 58min • ★5".

**Q. How does the venue / map work?**
**Free.** If Location permission is granted, the app captures the session **end**
location once when the session ends, shows it on a Google Map in the session
detail, and lists nearby sauna / bath facility candidates. The candidates come
from a Google Places search **plus your own past-visited venues within about
500 m**. Tap a candidate to set the venue. There is no continuous GPS tracking.
Each session can also have a 1–5 star rating.

### 4. Troubleshooting

**Q. Watch session data isn't reaching my Android phone.**
Open the MaxRecover app on both devices, keep them nearby with Bluetooth (or
Wi-Fi) on, and relaunch both apps. The watch resends pending sessions
automatically over the Wearable Data Layer once they reconnect.

**Q. Heart rate isn't showing on the watch.**
Make sure the watch is worn snugly and that you granted the **Body Sensors**
(heart rate) permission when the app first launched. If that permission is
denied, the app falls back to demo / mock data instead of your real heart rate.

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

**Q. The resting-HR line, Sleep score, or Next-day status isn't showing.**
These come from **Health Connect**. Make sure you connected it in **Settings →
Health Connect** and granted the relevant read permissions, and that the data
exists there (a recorded resting heart rate, and sleep data for the night after
the session). If Health Connect is not connected, or the data is missing, those
items simply do not appear and the rest of the app is unaffected.

### 5. Other

**Q. Can I switch the app to English?**
Yes. The app is available in Japanese and English. Open Settings and turn on
the **Force English** toggle to force the English UI regardless of your system
language.

**Q. Can I use this for medical purposes?**
No. The Afterglow Score, heart-rate values, HRR, the Sleep score, and all other
figures are reference information only. They are not medical metrics and must
not be used for diagnosis or treatment decisions. Consult a physician if you
have concerns.

**Q. What is the recommended use?**
Personal wellness tracking. Use saunas at your own risk and follow your local
sauna's rules. Avoid alcohol before and during sauna use.

**Q. How do I contact support?**
Email **maxsaunatimer@gmail.com**. Please include your Android / Wear OS
versions and a brief description of the issue.

**Q. Where can I find the Privacy Policy and Terms of Use?**
[Privacy Policy](privacy-policy.html) / [Terms of Use](terms-of-use.html).

---

## 関連 / See also

- [Guide / 取扱説明書](guide.html)
- [FAQ / よくある質問](faq.html)
- [Privacy Policy / プライバシーポリシー](privacy-policy.html)
- [Terms of Use / 利用規約](terms-of-use.html)
