---
title: Quick Guide (Pixel Watch & Android)
---

# Quick Guide — MaxRecovery Timer for Pixel Watch & Android

**Last updated / 最終更新:** (set on release / 公開時に設定)

> 🌐 言語 / Language: **English** / [🇯🇵 日本語](guide-ja.html)

> 🐛 Report bugs & suggestions: **[Feedback form](../feedback.html)**

---

### 1. Setup

- Install **MaxRecovery Timer** (formerly MaxSauna Timer) from **Google Play** on
  your Android phone.
- Pair your **Pixel Watch** first using the **Pixel Watch / Wear OS** app, then
  install the **MaxRecovery Timer** watch app to the watch (via the phone's Play
  Store / Wear OS app).
- The first time you open the watch app, read **"Before you start"** and tap
  **"Agree & continue"**.
- **Permissions are explained and requested when you first start a session.**
  When you tap "Start Standard" (or "Start Simple") on the watch, a **"Before you
  start"** screen lists what the app needs and why:
  - **Heart rate** — to record your heart rate during the session.
  - **Notifications** — to show the running session on the watch face.
  - **Location (optional)** — to record where the session ended.

  Tap **"Allow and start"** to grant them and start, or **"Start without"** to
  start anyway (anything you don't allow is not used; if you don't allow heart
  rate, the session is timed without heart rate). The screen doesn't appear once
  everything it needs is granted. Location is asked only once; to change it later,
  go to the watch's **Settings → Apps → MaxRecovery Timer → Permissions**. In the
  watch's settings the heart-rate permission is called "Heart rate" ("Sensors" on
  earlier watch software). Location is read once at the end of each session, saved
  with that session, and used only to tag the venue and show it on the map.
- When paired, finished sessions transfer from the **watch to the phone
  automatically** over the Wearable Data Layer (Bluetooth / Wi-Fi). The watch
  keeps each session and resends it until the phone confirms it was received.
  Watch settings sync both ways, so you can edit them from the phone (if you change
  settings on both, **the newer change to each item is kept**). By default there
  is **no cloud account / login**; data stays locally on each device.
- **Keep both the watch app and the phone app up to date.** An older phone app
  may not be able to receive long sessions (the watch home screen tells you; see
  section 4).
- **Cloud sync (optional, FREE):** **Settings → Cloud sync (Google Drive) →
  "Sync with Google Drive"** to back up your sessions to **your own** Google
  Drive and move them between devices. It is **off until you sign in / tap
  Sync**, and the developer operates **no server and stores nothing** — your
  data goes to your own Drive's app-private folder, not to the developer. See
  the Cloud sync section below.

### 2. Start a session

1. Open **MaxRecovery Timer** on your **Pixel Watch** (the home screen title is
   "MaxRecovery").
2. Choose **Standard** or **Simple** mode (set in phone Settings → Watch settings).
3. Tap **Start Standard** (or **Start Simple**). The first time, the "Before you
   start" screen appears (see section 1).

The watch app is shown in English or Japanese (see "Languages" in section 5).

### 3. During the session — hands-free

Once started, you don't need to touch the screen. **During a running session the
screen does not respond to touch** (to prevent wet-hand mis-taps) — you operate with
the **rotary crown** (except for the buttons you get with "Show control buttons" and
similar options). It works the same on every watch:

- **Rotate the crown UP** = advance to the next phase. This is the recommended
  hands-free action.
- **One turn, one phase** — once a turn advances a phase, the rest of that turn is
  ignored (so a long turn can't skip two phases). To advance again, stop turning
  and wait **at least 1 second** — a second Next within 1 second (from the crown, a
  button or any other input) is ignored.
- **Rotate the crown DOWN** = pause. To resume, **rotate the crown UP** again (or
  tap **Resume** in the pause menu).
- **While paused**, an on-screen touch menu appears: **Resume / Back / End**.
- **Go back one phase** — if you advanced by mistake, rotate the crown DOWN to pause,
  then tap **Back** in the pause menu and confirm with **Go back** ("Go back one
  phase?"; the current phase's record is discarded). You return to the previous
  phase and its **previous elapsed time is carried over** (it does not reset to
  zero). You **stay paused** afterwards — rotate the crown UP or tap **Resume** to
  continue.
- **Wrist turn** is disabled during a session by default (so it can't bring up the
  end confirmation by accident; it doesn't pause or close confirmations or alerts
  either). If you turn on the experimental "Wrist turn to pause (beta)" on the watch,
  you can pause and resume by turning your wrist (see the last item in this list).
  Turn gestures on/off and change hint frequency in the watch's system settings
  (Gestures → Hand gestures or similar; names can differ by watch software version).
- **On-screen Next / Pause buttons** during a running session appear **only if you turn
  on Settings → Watch settings → "Show control buttons"** (off by default). If you
  turn on the experimental "Use Double pinch (beta)" on the watch (see the last item
  in this list), **Next** is always shown (Pause only when the setting is on).
- **Crown rotation** — Settings → Watch settings lets you choose how far you must
  turn the crown to act (**Light / Standard / More / Most**), to avoid accidental
  triggers from incidental contact.
- **Double-tap the watch body (beta, off by default)** — Settings → Watch settings →
  "Double-tap to advance (beta)" uses the accelerometer so a quick **double-tap**
  advances to the next phase hands-free. It's turned off while "Use Double pinch
  (beta)" is on for the watch and double pinch is available (so one move can't
  advance twice). Experimental and may misfire (it can also react to the finger
  movement of a double pinch); keep it off if you see unwanted advances, and use
  **Back** to undo.
- **Swipe right** to open the end confirmation ("End session?"; it closes by itself
  after 5 seconds and the session keeps running). Tap **Cancel** (or **turn the
  crown**) to close it, or tap **End** to finish. The screen shows
  "Turn the crown to cancel".
- **The crown closes confirmations and warnings** — while a confirmation (end, go
  back, final-set choice) or a warning is open, turning the crown (either way)
  **cancels** the confirmation, **continues** on the inactivity warning, and presses
  **OK** on the low-HR warning and on "Heart rate unavailable". It doesn't change
  phase or pause. **End, Go back and One more set are tap-only.** On the rating
  screen, while saving, and on the "Unfinished session" prompt, turning the crown
  does nothing.
  - If a confirmation or warning opens, or closes by itself (for example when it
    times out), while you are turning the crown, that turn stops there (so you don't
    dismiss a warning you haven't seen, or advance or pause after it closes). Stop
    turning, then turn again.
  - For 1 second after the crown closes one, Next is ignored.
- **Don't use the system "Water Lock" during a session** — Wear OS Water Lock is
  exited by **turning the crown**, so while it is on the crown can't change phase or
  pause either. During a session the app **already ignores screen touch** (to prevent
  mis-taps, except for the buttons above), so Water Lock isn't needed — just keep
  using the crown.
- **Double pinch (beta, off by default; Pixel Watch 3 and later, Wear OS 7)** — it's
  off by default because it's experimental. To try it, on the watch go to the
  MaxRecovery home → **Settings → Options → "Use Double pinch (beta)"** and turn it
  on. The option only appears on Pixel Watch 3 and later when hand gestures (double
  pinch) are turned on in the watch's own system settings. When it's on, a **Next**
  button (**Next set** in Simple mode) is shown at the bottom of the screen while
  running; tapping your thumb and index finger together twice does the same as that
  button (next phase; at the end of the final set it opens the **One more set / End /
  Cancel** screen). On a confirmation (end, go back, final-set choice) it
  **cancels**, on the rating screen it **saves**, on the inactivity warning it
  **continues**, and on a heart-rate alert it **dismisses**. It does nothing while
  paused or saving. If it doesn't respond well, the crown works as usual. If you turn
  hand gestures off in the watch's system settings, double pinch isn't used even
  with this option on, and the usual controls come back. Note: the Next button can
  also react to wet fingers or water drops.
  While the option is off, the app doesn't accept double pinch (it won't close a
  confirmation or save a rating). However, if "Double-tap to advance (beta)" is on,
  the finger movement of a pinch may be picked up and advance to the next phase.
- **Wrist turn to pause (beta, off by default; Pixel Watch 3 and later, Wear OS 7)** —
  it's off by default because it's experimental. To try it, on the watch go to the
  MaxRecovery home → **Settings → Options → "Wrist turn to pause (beta)"** and turn it
  on. The option only appears on Pixel Watch 3 and later when wrist turn is turned on
  in the watch's own system settings.
  When it's on, **turning your wrist (a quick turn outward and back) pauses** a running
  session, and **turning it again resumes** (the screen and notification are the same
  as when you pause or resume with the crown or the pause menu). On a confirmation
  (end, go back, final-set choice) it **cancels**. It doesn't close heart-rate alerts
  or the inactivity warning (so a movement such as wiping off sweat can't dismiss an
  alert you haven't seen — use the crown or tap). It does nothing on the rating
  screen, while saving, or on the "Unfinished session" prompt. So that one movement
  can't pause and then resume, a wrist turn within **1 second** of the previous wrist
  turn, or of pausing/resuming with the crown or a button, is ignored. If it doesn't
  respond well, the crown works as usual. If you turn wrist turn off in the watch's
  system settings, it isn't used even with this option on.
  While the option is off, the app ignores wrist turns during a session (no pause, no
  end confirmation, and it doesn't close confirmations or alerts). Outside a session
  (home, settings, history and so on), wrist turn stays the system's Back either way.

The watch displays the current phase, elapsed time, heart rate, and your recent
HR peak / bottom (last 5 minutes). Configured phase times act as **haptic
alerts** — the app does not auto-advance. If heart rate can't be read, the heart-rate
field shows "—" or "♡×" and a **"Heart rate unavailable"** notice appears (it closes
after 10 seconds, or when you turn the crown or tap **OK**); the timer keeps running
(see the FAQ).

**Background recording:** the session runs in a **foreground service with an ongoing
notification**, and heart rate is read with the watch's workout feature (Health
Services). While a session runs, an **ongoing-activity icon** appears on the watch
face and the notification shows the current phase (e.g. "Sauna 1/3") and
"Measuring". The session keeps running if you go back to the watch face or the
screen turns off; tap the icon or the notification to return to the session screen.
While the session screen is shown, the display is **kept on** by default. However,
**without the Heart rate permission** the foreground service can't run, so
recording may stop when the screen turns off (the watch tells you). Also, when the
workout feature can't be used (for example while another app is recording a
workout), heart rate may stop while the screen is off. Keeping the session screen
open during a session is recommended.

### 4. End the session

- **Standard mode:** moving past the last phase of the final set shows **"What
  next?"** with **One more set / End / Cancel**. It closes by itself after 8 seconds
  and the session keeps running (you can also close it with **Cancel** or by turning
  the crown).
- **Simple mode:** pause and tap **End**.
- In either mode you can also end from the pause menu (**End**) or from the
  right-swipe end confirmation.
- The app **auto-ends after 60 minutes** with no input (you get a warning first;
  tap **Continue** or turn the crown to keep going).
- After ending, rate the session 1–5 stars on the **"Nice work!"** screen and tap
  **Save** (or **Skip**).
- The finished session is transferred to your phone automatically over the
  Wearable Data Layer. The watch keeps it and resends it until the phone confirms
  it was received.
  - If there is still no confirmation after 1 hour, the watch history marks the
    session **"Not on phone yet"**. Bring the phone close and open both apps.
  - If the watch home screen says **"Update the phone app to receive N
    session(s)."**, update the phone app to the latest version (an older phone app
    can't receive long sessions). The sessions arrive automatically after the
    update.

### 5. Review on your Android phone

- **Home tab (ホーム)** — shows the latest session's full analysis directly (no
  tap needed): the detail header with self-rating (e.g. "Standard • 2 sets •
  58min • ★5"), heart-rate chart with phase bands, Afterglow Score, set-level
  breakdown, the **Detailed data** card (Max / Min / Avg HR, HR drop, HRR1 /
  HRR3 / HRR5), personal z-score / vs-previous, movement quality, and (Premium)
  the β score & recovery curve.
- **Sessions without heart rate** — sessions where the watch couldn't read your
  heart rate (heart rate permission off, no readings received, etc.) are marked
  **"No heart-rate data (reason)"**. They count toward visits, total time, streaks,
  the heatmap and the recent-sessions list, but are not used for the Afterglow
  Score, personal comparisons, recovery curves, trends or the PDF report.
- **Interactive heart-rate chart** — the HR chart is fully interactive:
  - **Tap a point** to show a value card (bpm, elapsed time, and the phase at
    that moment).
  - **Pinch to zoom** in up to **20×**.
  - **Drag to scroll** along the timeline.
  - **Double-tap to reset** the view.
- **Chart display options (Settings → Display)** — optional overlays and views
  for the HR chart, all **default OFF**:
  - **"Show 60s moving average"** — a trailing 60 s moving-average line.
  - **"Show 10min moving average"** — a trailing 10 min moving-average line.
  - **"Hide prep phase from chart"** — re-bases the X axis so it starts at
    **sauna entry (0:00)**.
  - If you connect Health Connect, your **Resting heart rate** can also appear
    as a reference line on the chart (see Health Connect below).
- **History tab (履歴)** — now just the **list of past sessions**. **Tap a row**
  to open that session's analysis (same screen as Home), including the
  **end-location map (FREE)** and venue-name entry (see the next item).
  **Left-swipe a row** to reveal a **trash button**, then **tap it** to delete that
  single session (no confirmation dialog — deletion is immediate; this is the only
  per-session delete). If you use Google Drive sync, the session is also removed
  from the cloud and your other devices at the next sync (see 5a).
- **Venue name (FREE)** — tap "**+ Add venue name**" (or the venue name, once
  set) in the session-detail header to type or edit it. This works even for
  sessions without a location. For sessions with a location, you can also set
  it from the **Venue / end location** card:
  - **Your past venues (within 500 m)** — names you entered before are listed
    first. **One tap sets the venue**, with no Google search. For a venue you
    have visited before, this is all you need.
  - **"Find nearby venues (N left today)"** — searches Google Maps for nearby
    venues **only when you tap it** (never automatically) and lists the
    suggestions with the **Google Maps logo**.
  - **Tap a suggestion** to open the venue-name dialog. The text field starts
    empty, and the suggested name is shown outside it for reference. Type the
    name you want to keep and save (under Google's terms, suggested names are
    never saved as-is).
  - Searches are limited to **5 per day per device** (Premium included; the
    count resets when your device's date changes). If you reach the limit or
    search is unavailable (when the app-wide search limit is reached, the time
    it resumes is shown), type the name in with **"Enter venue name"**.
- **Recovery curve slope lines (Premium)** — on the recovery-curve chart the app
  overlays a straight **slope line** for each set, with a **"Show slope lines"**
  toggle and dashed **1-min / 3-min** guide lines. A per-set legend shows the
  slope (bpm/min), R², and lag (seconds).
- **Save / share graph** — from a session's detail you can share the heart-rate
  chart. **FREE:** a **Share** button shares **text only** (basic info).
  **PREMIUM:** **Save graph to Photos** + **Share graph** shares detailed text
  **plus a PNG of the HR chart**; choose **"Info + HR graph"** or **"HR graph
  only"**. Saved images (`MaxRecovery_<date-time>.png`) go to your device's own
  Photos (Pictures/MaxRecoveryTimer) — nothing is uploaded. **Images saved with
  earlier versions stay in Pictures/MaxSaunaTimer** (they are not moved).
- **Next-day status (with Health Connect)** — if connected, for the night
  **after** a session the app shows a reference **Sleep score (FREE)** and your
  **average respiratory rate**.
- **Analytics tab (分析)** — **partly free**. FREE: the overview cards moved here
  from History — **Streaks & count** (current / longest streak + total count),
  **Best Sessions TOP 10** (by Afterglow score), the **visit-frequency calendar
  heatmap**, and the **Venue Map** — plus afterglow over time, average by mode,
  and the period summary. Premium: HRR trend (1/3/5), the recovery-slope trend,
  averages by set count / session length, set-position HRR, a recovery-curve
  overlay, and a recovery summary. The period filter (All / 30 days / 7 days) is
  available to everyone.
- **PDF report (Premium)** — generated from the Analytics tab and shared via the
  Android share sheet (file name `MaxRecovery_Report_<start>_<end>.pdf`). A4
  portrait, 3 pages, including **Best Sessions** and a **visit-frequency heatmap**
  (these are also available in-app for free, in the Analytics tab).
- **Settings → Data import/export (CSV)** — CSV import/export (Premium) for offline
  backup or analysis. Exported files are named `maxrecovery_*.csv` (sessions),
  `maxrecovery_sets_*.csv`, `maxrecovery_phases_*.csv` and
  `maxrecovery_hr_samples_*.csv`; files exported by earlier versions
  (`max_sauna_*.csv`) can still be imported. Exporting **set-aside history files**
  (copies of history that couldn't be read) works without Premium (see the FAQ).
- **Settings → Cloud sync (Google Drive)** — back up to your own Drive, FREE,
  optional (see the Cloud sync section below).

**Free vs Premium:** the personal z-score / vs-previous, the movement-quality
(Flow) score, the **Detailed data** card, the end-location map / venue-name
entry (nearby-venue search up to 5 times a day), the **basic Analytics** (afterglow-over-time, by-mode, summary), cloud sync
(Google Drive), the overview cards (streaks / Best Sessions / heatmap / Venue
Map), the Sleep score, and the resting-HR reference line are all **FREE**;
sharing the HR graph as **text** is also free. The β score, the recovery curve
(with slope / R² / lag), the **advanced Analytics**, the PDF report, the
**HR-chart image** in share + Save-to-Photos, and CSV import/export are
**Premium**. Without Premium, banner ads appear on Home / History / Analytics and
the session-detail screen (no ads on Settings); **Premium removes all ads**.
Premium also unlocks a **Premium app icon** (Settings → Premium → "Use Premium
app icon").

**Getting Premium:** open **Settings → Premium → "Upgrade to Premium"** (or **"See
Premium"** on the locked recovery curve, advanced Analytics or CSV import/export) to
reach the Premium screen, then choose the
**Monthly plan** or the **Yearly plan**. Prices are loaded from Google Play and shown
in your local currency. First-time Premium subscribers get a free period (such as
**"Premium: first month free"**; Google Play decides eligibility). When the free
period ends, the subscription renews automatically at the plan's price. Cancel in
Google Play → Subscriptions (while subscribed, "Manage subscription (cancel,
payment)" on the Premium screen opens it too). See "Subscription & Billing" in the
FAQ.

**Languages:** the phone app (including the shared graph image and the PDF report)
and the watch app are available in English and Japanese. The phone app follows the
phone's language setting, and the watch app follows the watch's own language setting
(on both, languages other than Japanese show English). Turn on **Settings → Display →
"Force English"** on the phone to show both the phone and the watch in English
regardless of their language settings (if you switch it while a session is running on
the watch, the watch changes after the session ends).

### 5a. Cloud sync (optional, FREE)

Cloud sync is **optional** and **off until you turn it on**. If you do not use
it, your data stays on your devices (Watch ↔ Phone over the Wearable Data Layer)
exactly as before.

- Turn it on under **Settings → Cloud sync (Google Drive) → "Sync with Google
  Drive"**. You sign in with Google and grant the **app-data (`drive.appdata`)**
  permission. Syncing happens when you tap this button (it does not sync
  automatically).
- It stores and retrieves a **snapshot of your sessions in your own Google
  Drive's app-private folder** (the hidden "App Data" area under your Google
  account), so you can **back up your sessions and move them between devices**.
- Sync is **two-way** and **merges by session**.
- **Sync protects your cloud data:** if the cloud data can't be fetched or read, or
  if saving would reduce the number of sessions in the cloud, the app **stops without
  changing the cloud** and tells you why. "Synced" is shown only after the save
  succeeds.
- **Deletions sync too:** a single-session delete and "Delete all received data" are
  applied to **the cloud and your other synced devices** at the next sync. Deleted
  sessions don't come back from a watch resend or from sync. To bring them back,
  restore them explicitly with CSV import (Premium); the restore reaches your other
  devices at the next sync.
- **If you sync two or more devices, update the app on all of them before
  syncing.** Older versions can't read the deletion records, so a deleted session
  stays on such a device (it won't come back to devices on the latest version).
- **The developer operates no server and stores nothing.** Your data goes to
  **your own** Google Drive, not to the developer; the developer **cannot
  access it**.
- You can **delete the synced data** from your own Google Drive at any time, and
  **revoke the app's access** anytime by deleting its connection in **Google
  Account → Security → "Your connections to third-party apps & services"** (the
  app itself has no disconnect setting).

### 6. Health Connect (optional)

Health Connect is **optional** and only used **with your permission**. If you do
not connect it, the app works exactly as before, with no health-data
integration.

- **Reads Resting heart rate** and shows it as a reference line on the session
  HR chart.
- For the night **after** a session, **reads your Sleep** (shown as a reference
  **Sleep score**, free) and your **average respiratory rate**, in the
  **Next-day status** section.
- Tap **Settings → Health Connect → "Export sessions to Health Connect"** to
  **write your sessions** to Health Connect as **exercise + heart-rate
  records**, so other apps can use them (export is manual, not automatic).
  - **Exporting again never creates duplicates** (records of the same session are
    replaced).
  - Sessions recorded without heart rate are exported as exercise only.
  - The exercise record is named after the venue; without a venue name it is named
    **"MaxRecovery"**.
  - **Records exported by earlier versions** keep the name **"Sauna"** and may be
    duplicated when you export again. Tap **"Clean up duplicates from earlier
    exports"**: for the time ranges of the sessions on your phone, the exercise and
    heart-rate records this app exported earlier are deleted and exported again
    (data from other apps is not affected; records of sessions you deleted from the
    phone stay as they are).
- Connect and export under **Settings → Health Connect**; revoke permissions in
  Health Connect (your device's system settings on Android 14 and later, or the
  Health Connect app on earlier versions).

### 7. Tips

- Wear your watch snugly for stable heart-rate readings.
- To advance several phases in a row, wait **at least 1 second** between inputs.
- **Tap a point** on the HR chart to read its exact bpm / time / phase, and
  **pinch to zoom** into the part you care about.
- Turn on the **moving averages** and **"Hide prep phase from chart"** under
  **Settings → Display** to read the curve more clearly.
- Add the **venue name** in a session's detail (typed in; for a venue you have
  visited before, one tap from your past venues within ~500 m — free) to power
  the Venue Map, the visit heatmap, and the PDF report.
- Add a **1–5 star rating** to each session (entered on the watch; it then shows
  in the detail header).
- Check the **Analytics tab** for your streaks, Best Sessions and visit heatmap —
  all free.
- The Afterglow Score and the Sleep score are **reference values**, not medical
  metrics.

### 8. Recording flow — a 3-set example

An example of recording **3 sets of Sauna → Cold bath → Cool-down** at a venue with a
set time limit (e.g. 60–90 minutes).

**Setup before you arrive**:
- Use **Standard mode** (phone Settings → Watch settings).
- Enable **"Start with prep time"** in Settings → Watch settings.

**At the venue**:
1. When your time at the venue starts (entry / locker), tap **Start Standard** on
   the watch to start the session. The session enters the **Prep** phase — use this
   time for changing clothes and washing.
2. When you start the **1st sauna**, **rotate the crown UP** → advances to the
   **Sauna** phase.
3. When entering the **cold water** (cold bath, lake, pool), rotate the crown
   **UP** → advances to **Cold bath**.
4. When you sit or lie down to rest, rotate the crown **UP** → advances to
   **Cool-down**.
5. When entering the sauna for the **next set**, rotate the crown **UP** again →
   starts set 2's Sauna.
6. Repeat 2–5 until the 3rd cool-down ends, then **advance past the final phase**
   and choose **End** on the "What next?" screen (or use **End** in the pause menu).
   You can also **rotate the crown DOWN to pause** at any time.

Total crown UP turns per 3-set session: **~9** (3 sauna + 3 cold bath + 3
cool-down). The first UP turn (Prep → Sauna) counts in this total. Wait at least 1
second between turns.

---

## 用語対応表 / Terminology

アプリ画面と本取説で同じ機能を指す用語の対応です（English はウォッチの英語表示）。
Terms in the app and in this guide that refer to the same thing (English = the watch's English UI).

| 日本語（アプリ表記） | English (app) | 説明 / Notes |
|---|---|---|
| クラウン（リューズ） | Crown | ウォッチ側面の回転リューズ。本取説の「リューズ」＝アプリの「クラウン」 / The rotating side button |
| ダブルピンチ | Double pinch | Pixel Watch 3 以降・実験（ウォッチの設定「ダブルピンチを使う（実験）」を ON にしたときだけ。既定オフ）。計測中は「次へ」と同じ / Pixel Watch 3+, beta (only when "Use Double pinch (beta)" is on in the watch app's settings; off by default); same as Next while running |
| 手首ターン | Wrist turn | Pixel Watch 3 以降・実験（ウォッチの設定「手首ターンで一時停止（実験）」を ON にしたときだけ。既定オフ）。計測中は一時停止／再開、確認画面はキャンセル。オフのときはセッション中は無効 / Pixel Watch 3+, beta (only when "Wrist turn to pause (beta)" is on in the watch app's settings; off by default): pauses/resumes in a session and cancels confirmations. When off, disabled in a session |
| 標準モード（開始ボタン「標準モード開始」） | Standard (Start Standard) | サウナ→水風呂→外気浴を繰り返す / The full sauna → cold bath → cool-down cycle |
| シンプルモード（開始ボタン「シンプルモード開始」） | Simple (Start Simple) | サウナのみを繰り返す簡易計測 / Sauna-only simple timing |
| 準備時間（設定「準備時間から開始」）→ 準備フェーズ（表示「準備」） | Start with prep time → Prep | ON にすると最初に入る、着替え等の時間 / Optional first phase before the sauna |
| サウナ | Sauna | 温まるフェーズ / The heat phase |
| 水風呂 | Cold bath | 冷水のフェーズ / The cold-water phase |
| 外気浴 | Cool-down | 休憩・外気浴のフェーズ / The outdoor-rest phase |
| その他フェーズ（休憩 / お風呂 / 給水 / シャワー / ストレッチ） | Extra phase (Rest / Hot bath / Hydration / Shower / Stretch) | 外気浴の後に入る任意の第4フェーズ。名称を選択可 / Optional 4th phase after cool-down; name is selectable |
| クラウン回転量（少なめ / 標準 / 多め / 最多） | Crown rotation (Light / Standard / More / Most) | フェーズ移行に必要な回転量 / How far to turn the crown to act |
| スマホ未転送 | Not on phone yet | スマホの受信確認がまだの記録 / Not yet confirmed as received by the phone |

**「休憩」など第4フェーズを使いたいときは / To add a "rest" 4th phase:** 設定 →
ウォッチ設定で **「その他フェーズを使う」** を ON にすると、外気浴の後に第4フェーズが
入り、名称を **休憩・お風呂・給水・シャワー・ストレッチ** から選べます。
Turn on **"Use extra phase"** in Settings → Watch settings to insert a 4th phase after
cool-down, with a selectable name (Rest / Hot bath / Hydration / Shower / Stretch).

---

## 関連 / See also

- [FAQ / よくある質問](faq.html)
- [Privacy Policy / プライバシーポリシー](privacy-policy.html)
- [Terms of Use / 利用規約](terms-of-use.html)

**Support / お問い合わせ:** anraku.tech@gmail.com
