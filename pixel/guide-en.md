---
title: Quick Guide (Pixel Watch & Android)
---

# Quick Guide — MaxSauna Timer for Pixel Watch & Android

**Last updated / 最終更新:** 2026-06-11

> 🌐 言語 / Language: **English** / [🇯🇵 日本語](guide-ja.html)

> 🐛 Report bugs & suggestions: **[Feedback form](../feedback.html)**

---

### 1. Setup

- Install **MaxSauna Timer** from **Google Play** on your Android phone.
- Pair your **Pixel Watch** first using the **Pixel Watch / Wear OS** app, then
  install the **MaxSauna Timer** watch app to the watch (via the phone's Play
  Store / Wear OS app).
- On first launch, grant **Body Sensors** (heart rate, on the watch) and
  (optional) **Location** when prompted. Location is only used to tag the venue
  at the end of a session.
- When paired, finished sessions transfer from the **watch to the phone
  automatically** over the Wearable Data Layer (Bluetooth / Wi-Fi). Watch
  settings sync both ways, so you can edit them from the phone. By default
  there is **no cloud account / login**; data stays locally on each device.
- **Cloud sync (optional, FREE):** **Settings → Cloud sync (Google Drive) →
  "Sync with Google Drive"** to back up your sessions to **your own** Google
  Drive and move them between devices. It is **off until you sign in / tap
  Sync**, and the developer operates **no server and stores nothing** — your
  data goes to your own Drive's app-private folder, not to the developer. See
  the Cloud sync section below.

### 2. Start a session

1. Open MaxSauna on your **Pixel Watch**.
2. Choose **Standard** or **Simple** mode (set in phone Settings → Watch settings).
3. Tap **Standard** (or **Simple**) to start. *The watch buttons are shown in
   Japanese — **標準モード開始** (Standard) / **シンプルモード開始** (Simple); the
   watch UI is currently Japanese-only.*

### 3. During the session — hands-free

Once started, you don't need to touch the screen. **During a running session the
screen does not respond to touch** (to prevent wet-hand mis-taps) — you operate with
the **rotary crown**:

- **Rotate the crown UP** = advance to the next phase. This is the recommended
  hands-free action.
- **Rotate the crown DOWN** = pause. To resume, **rotate the crown UP** again (or
  tap **Resume** in the pause menu).
- **While paused**, an on-screen touch menu appears: **Resume / Go back one phase /
  End**.
- **Go back one phase** — if you advanced by mistake, rotate the crown DOWN to pause,
  then tap **Go back** in the pause menu (a confirmation appears). You return to the
  previous phase and its **previous elapsed time is carried over** (it does not reset
  to zero).
- **On-screen Next / Pause buttons** during a running session appear **only if you turn
  on Settings → Watch settings → "Show control buttons"** (off by default).
- **Crown rotation amount** — Settings → Watch settings lets you choose how far you must
  turn the crown to act (**Light / Standard / More / Most**), to avoid accidental
  triggers from incidental contact.
- **Double-tap the watch body (beta, off by default)** — Settings → Watch settings →
  "Double-tap body to advance (beta)" uses the accelerometer so a quick **double-tap**
  advances to the next phase hands-free. Experimental and may misfire; keep it off
  if you see unwanted advances, and use **Go back** to undo.

The watch displays the current phase, elapsed time, heart rate, and your recent
HR peak / bottom (last 5 minutes). Configured phase times act as **haptic
alerts** — the app does not auto-advance.

**Background recording:** while a session screen is on, the watch **keeps the
display awake** and runs a **foreground service with an ongoing notification**,
so the timer and heart rate keep running throughout the session. (Fully
screen-off background recording is still being finalized and verified on real
hardware.)

### 4. End the session

- Move past the final phase to end, or
- The app **auto-ends after 60 minutes** with no input (you get a warning
  first).
- The finished session is transferred to your phone automatically over the
  Wearable Data Layer.

### 5. Review on your Android phone

- **Home tab (ホーム)** — shows the latest session's full analysis directly (no
  tap needed): the detail header with self-rating (e.g. "Standard • 2 sets •
  58min • ★5"), heart-rate chart with phase bands, Afterglow Score, set-level
  breakdown, the **Detailed data** card (Max / Min / Avg HR, HR drop, HRR1 /
  HRR3 / HRR5), personal z-score / vs-previous, movement quality, and (Premium)
  the β score & recovery curve.
- **Interactive heart-rate chart** — the HR chart is fully interactive:
  - **Tap a point** to show a value card (bpm, elapsed time, and the phase at
    that moment).
  - **Pinch to zoom** in up to **20×**.
  - **Drag to scroll** along the timeline.
  - **Double-tap to reset** the view.
- **Chart display options (Settings → Display)** — optional overlays and views
  for the HR chart, all **default OFF**:
  - **60-second moving average** — a trailing 60 s moving-average line.
  - **10-minute moving average** — a trailing 10 min moving-average line.
  - **Hide preparation phase from chart** — re-bases the X axis so it starts at
    **sauna entry (0:00)**.
  - If you connect Health Connect, your **Resting heart rate** can also appear
    as a reference line on the chart (see Health Connect below).
- **History tab (履歴)** — now just the **list of past sessions**. **Tap a row**
  to open that session's analysis (same screen as Home), including the
  **end-location map (FREE)** with venue candidates you tap to set the venue
  (nearby Places search **and your past-visited venues within about 500 m**).
  **Left-swipe a row** to reveal a **trash button**, then **tap it** to delete that
  single session (no confirmation dialog — deletion is immediate; this is the only
  per-session delete).
- **Recovery curve slope lines (Premium)** — on the recovery-curve chart the app
  overlays a straight **slope line** for each set, with a **"Show slope lines"**
  toggle and dashed **1-min / 3-min** guide lines. A per-set legend shows the
  slope (bpm/min), R², and lag (seconds).
- **Save / share graph** — from a session's detail you can share the heart-rate
  chart. **FREE:** a **Share** button shares **text only** (basic info).
  **PREMIUM:** **Save graph to Photos** + **Share graph** shares detailed text
  **plus a PNG of the HR chart**; choose **"Info + HR graph"** or **"HR graph
  only"**. Saved images go to your device's own Photos
  (Pictures/MaxSaunaTimer) — nothing is uploaded.
- **Next-day status (with Health Connect)** — if connected, for the night
  **after** a session the app shows a reference **Sleep score (FREE)** and your
  **average respiratory rate**.
- **Analytics tab (分析)** — **partly free**. FREE: the overview cards moved here
  from History — **Streaks & count** (current / longest streak + total count),
  **Best Sessions TOP 10** (by Afterglow score), the **visit-frequency calendar
  heatmap**, and the **Sauna Map** — plus afterglow over time, average by mode,
  and the period summary. Premium: HRR trend (1/3/5), the recovery-slope trend,
  averages by set count / session length, set-position HRR, a recovery-curve
  overlay, and a recovery summary. The period filter (All / 30 days / 7 days) is
  available to everyone.
- **PDF report (Premium)** — generated from the Analytics tab and shared via the
  Android share sheet. A4 portrait, 3 pages, including **Best Sessions** and a
  **visit-frequency heatmap** (these are also available in-app for free, in the
  Analytics tab).
- **Settings → Data import/export** — CSV import/export (Premium) for offline
  backup or analysis.
- **Settings → Cloud sync (Google Drive)** — back up to your own Drive, FREE,
  optional (see the Cloud sync section below).

**Free vs Premium:** the personal z-score / vs-previous, the movement-quality
(Flow) score, the **Detailed data** card, the end-location map / venue picker,
the **basic Analytics** (afterglow-over-time, by-mode, summary), cloud sync
(Google Drive), the overview cards (streaks / Best Sessions / heatmap / Sauna
Map), the Sleep score, and the resting-HR reference line are all **FREE**;
sharing the HR graph as **text** is also free. The β score, the recovery curve
(with slope / R² / lag), the **advanced Analytics**, the PDF report, the
**HR-chart image** in share + Save-to-Photos, and CSV import/export are
**Premium**. Banner ads appear on Home / History / Analytics and the
session-detail screen on FREE (no ads on Settings); **Premium removes all ads**.
Premium also unlocks a **Premium app icon** (Settings → Premium → "Use Premium
app icon").

**Bilingual:** the entire app — every screen, the shared graph image, and the
PDF report — is fully Japanese / English. Use **Settings → Display → "Force
English"** to force English regardless of your system language.

### 5a. Cloud sync (optional, FREE)

Cloud sync is **optional** and **off until you turn it on**. If you do not use
it, your data stays on your devices (Watch ↔ Phone over the Wearable Data Layer)
exactly as before.

- Turn it on under **Settings → Cloud sync (Google Drive) → "Sync with Google
  Drive"**. You sign in with Google and grant the **app-data (`drive.appdata`)**
  permission.
- It stores and retrieves a **snapshot of your sessions in your own Google
  Drive's app-private folder** (the hidden "App Data" area under your Google
  account), so you can **back up your sessions and move them between devices**.
- Sync is **two-way** and **merges by session**.
- **The developer operates no server and stores nothing.** Your data goes to
  **your own** Google Drive, not to the developer; the developer **cannot
  access it**.
- You can **delete the synced data** from your own Google Drive at any time, and
  **revoke the app's access** anytime in your **Google Account permissions** (or
  from Settings).

### 6. Health Connect (optional)

Health Connect is **optional** and only used **with your permission**. If you do
not connect it, the app works exactly as before, with no health-data
integration.

- **Reads Resting heart rate** and shows it as a reference line on the session
  HR chart.
- For the night **after** a session, **reads your Sleep** (shown as a reference
  **Sleep score**, free) and your **average respiratory rate**, in the
  **Next-day status** section.
- **Writes each session** to Health Connect as an **exercise + heart-rate
  record**, so other apps can use it.
- Connect or manage it any time under **Settings → Health Connect**.

### 7. Tips

- Wear your watch snugly for stable heart-rate readings.
- **Tap a point** on the HR chart to read its exact bpm / time / phase, and
  **pinch to zoom** into the part you care about.
- Turn on the **moving-average overlays** and **Hide preparation phase** under
  **Settings → Display** to read the curve more clearly.
- Fill in the **venue** (from the nearby candidates or your past-visited venues
  within ~500 m — free) in a session's detail to power the Sauna Map, the
  visit heatmap, and the PDF report.
- Add a **1–5 star rating** to each session (entered on the watch; it then shows
  in the detail header).
- Check the **Analytics tab** for your streaks, Best Sessions and visit heatmap —
  all free.
- The Afterglow Score and the Sleep score are **reference values**, not medical
  metrics.

### 8. Typical workflow — time-limited sauna venues

A recommended flow for time-limited sauna venues (e.g. 60–90 min facilities)
doing **3 sets of sauna → cold plunge → cool-down**.

**Setup before you arrive**:
- Use **Standard mode** (phone Settings → Watch settings).
- Enable **"Use Pre-sauna phase"** in Settings → Watch settings.

**At the venue**:
1. When the venue starts your timer (entry tag / locker), tap **Standard**
   (**標準モード開始** on the watch) to start the session. The session enters the **Preparation**
   phase — use this time for changing clothes and body wash.
2. Just before entering the sauna for the **1st time**, **rotate the crown UP**
   → advances to the **Sauna** phase.
3. When entering the **cold water** (cold plunge, lake, pool), rotate the crown
   **UP** → advances to **Cold plunge**.
4. When sitting / lying on the chair or beach chair, rotate the crown **UP** →
   advances to **Cool down**.
5. When entering the sauna for the **next set**, rotate the crown **UP** again →
   starts set 2's Sauna.
6. Repeat 2–5 until the 3rd cool-down ends, then **advance past the final phase
   (or use the on-screen End)** to finish. You can also **rotate the crown DOWN
   to pause** at any time.

Total crown UP turns per 3-set session: **~9** (3 sauna + 3 plunge + 3
cool-down). The first UP turn (preparation → sauna) counts in this total.

---

## 用語対応表 / Terminology

アプリ画面と本取説で同じ機能を指す用語の対応です。
Terms in the app and in this guide that refer to the same thing.

| 日本語（アプリ表記） | English (app) | 説明 / Notes |
|---|---|---|
| クラウン（リューズ） | Crown | ウォッチ側面の回転リューズ。本取説の「リューズ」＝アプリの「クラウン」 / The rotating side button |
| 標準モード（開始ボタン「標準モード開始」） | Standard | サウナ→水風呂→外気浴を繰り返す / The full sauna → cold → cool-down cycle |
| シンプルモード | Simple | サウナのみを繰り返す簡易計測 / Sauna-only simple timing |
| 準備時間（設定「準備時間から開始」）→ 準備フェーズ（表示「準備」） | Pre-sauna / Preparation | ON にすると最初に入る、着替え等の時間 / Optional first phase before the sauna |
| 外気浴 | Cool down | 休憩・外気浴のフェーズ / The rest / cool-down phase |
| その他フェーズ（休憩 / お風呂 / 給水 / シャワー / ストレッチ） | Extra phase | 外気浴の後に入る任意の第4フェーズ。名称を選択可 / Optional 4th phase after cool-down; name is selectable |
| クラウン回転量（少なめ / 標準 / 多め / 最多） | Crown rotation (Light / Standard / More / Most) | フェーズ移行に必要な回転量 / How far to turn the crown to act |

**「休憩」など第4フェーズを使いたいときは / To add a "rest" 4th phase:** 設定 →
ウォッチ設定で **「その他フェーズを使う」** を ON にすると、外気浴の後に第4フェーズが
入り、名称を **休憩・お風呂・給水・シャワー・ストレッチ** から選べます。
Turn on **"Use extra phase"** in Settings → Watch settings to insert a 4th phase after
cool-down, with a selectable name (rest / hot bath / hydration / shower / stretch).

---

## 関連 / See also

- [FAQ / よくある質問](faq.html)
- [Privacy Policy / プライバシーポリシー](privacy-policy.html)
- [Terms of Use / 利用規約](terms-of-use.html)

**Support / お問い合わせ:** maxsaunatimer@gmail.com
