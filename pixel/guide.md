---
title: Quick Guide (Pixel Watch & Android)
---

# Quick Guide / 簡易取説 — MaxSauna Timer for Pixel Watch & Android

**Last updated / 最終更新:** 2026-06-05

> 🐛 **不具合・改善要望はこちら → [フィードバックフォーム](../feedback.html)** / Report bugs & suggestions: **[Feedback form](../feedback.html)**

---

## English

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
2. Choose **Standard** or **Simple** mode (set in phone Settings → Session).
3. Tap **Start**.

### 3. During the session — hands-free

Once started, you don't need to touch the screen. With wet hands you can advance
phases and pause using the **rotary crown**:

- **Rotate the crown UP** = advance to the next phase. This is the recommended
  hands-free action.
- **Rotate the crown DOWN** = pause / resume.
- **On-screen buttons** also work.
- **Screen tap** — only if you enable it under Settings → Session →
  "Tap screen to advance phase" (off by default).

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

- **Latest tab (最新)** — shows the latest session's full analysis directly:
  heart-rate chart with phase bands, Afterglow Score, set-level breakdown,
  personal z-score / vs-previous, movement quality, and (Premium) the β score &
  recovery curve.
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
- **History tab (履歴)** — at the **top** of this tab you get **in-app
  analytics, FREE**:
  - **Streaks & count** — your **current** and **longest** streak plus your
    **total session count**.
  - **Best Sessions TOP 10** — your highest sessions by **Afterglow score**.
  - **Visit-frequency calendar heatmap** — a calendar showing how often you go.
  - **Sauna Map** — all your visited venues shown on a single map.
  - Below the analytics is the **list of past sessions**. Tap one to open its
    detail, including the **end-location map (FREE)** with venue candidates you
    tap to set the venue. Suggestions include the nearby Places search **and
    your past-visited venues within about 500 m**.
- **Next-day status (with Health Connect)** — if connected, for the night
  **after** a session the app shows a reference **Sleep score (FREE)** and your
  **average respiratory rate**.
- **Trends tab (トレンド)** — **partly free**. FREE: afterglow over time,
  average by mode, and the period summary. Premium: HRR trend (1/3/5), the
  recovery-slope trend, averages by set count / session length, set-position
  HRR, a recovery-curve overlay, and a recovery summary. The period filter
  (All / 30 days / 7 days) is available to everyone.
- **PDF report (Premium)** — generated from the Trends tab and shared via the
  Android share sheet. A4 portrait, 3 pages, including **Best Sessions** and a
  **visit-frequency heatmap** (these are also available in-app for free, in the
  History tab).
- **Settings → Data import/export** — CSV import/export (Premium) for offline
  backup or analysis.
- **Settings → Cloud sync (Google Drive)** — back up to your own Drive, FREE,
  optional (see the Cloud sync section below).

**Free vs Premium:** the personal z-score / vs-previous, the movement-quality
(Flow) score, the end-location map / venue picker, the **basic Trends**
(afterglow-over-time, by-mode, summary), cloud sync (Google Drive), the in-app
History analytics (streaks / Best Sessions / heatmap / Sauna Map), the Sleep
score, and the resting-HR reference line are all **FREE**. The β score, the
recovery curve, the **advanced Trends**, the PDF report, and CSV import/export
are **Premium**.

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
- Add a **1–5 star rating** to each session.
- Check the **History tab** for your streaks, Best Sessions and visit heatmap —
  all free.
- The Afterglow Score and the Sleep score are **reference values**, not medical
  metrics.

### 8. Typical workflow — time-limited sauna venues

A recommended flow for time-limited sauna venues (e.g. 60–90 min facilities)
doing **3 sets of sauna → cold plunge → cool-down**.

**Setup before you arrive**:
- Use **Standard mode** (phone Settings → Session).
- Enable **"Use Pre-sauna phase"** in Settings → Session.

**At the venue**:
1. When the venue starts your timer (entry tag / locker), tap **Standard** on
   the watch to start the session. The session enters the **Preparation**
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

## 日本語

### 1. セットアップ

- Android スマホの **Google Play** から **MaxSauna Timer** をインストール。
- まず **Pixel Watch / Wear OS** アプリで Pixel Watch をペアリングし、続けて
  ウォッチアプリ（**MaxSauna Timer**）を腕時計側にインストールします（スマホの
  Play ストア / Wear OS アプリ経由）。
- 初回起動時に **ボディーセンサー**（心拍。ウォッチ側）・（任意）**位置情報** の
  権限を許可してください。位置情報はセッション終了時に施設をタグ付けする目的の
  みに使われます。
- ペアリング済みなら、終了したセッションは **ウォッチ → スマホへ自動転送** され
  ます（Wearable Data Layer、Bluetooth / Wi-Fi）。ウォッチ設定は双方向同期なの
  で、スマホから編集できます。既定では **クラウドアカウント / ログインはありませ
  ん**。データは各端末のローカルに保存されます。
- **クラウド同期（任意・無料）：** **設定 → クラウド同期（Google ドライブ）→
  「Google ドライブと同期」** で、セッションを **あなた自身の** Google ドライブに
  バックアップし、端末間で移行できます。**サインイン / 同期をタップするまでオフ**
  で、開発者は **サーバーを持たず、何も保存しません** — データはあなた自身のドラ
  イブのアプリ専用フォルダに保存され、開発者には渡りません。詳しくは後述のクラウ
  ド同期セクションを参照。

### 2. セッションを開始

1. Pixel Watch で **MaxSauna** を開く。
2. **標準モード** / **シンプルモード** を選ぶ（スマホ 設定 → セッション）。
3. **開始** をタップ。

### 3. セッション中 — ハンズフリー操作

一度開始すれば、画面に触れずに操作できます。濡れた手でも **リューズ（回転クラウ
ン）** で操作できます:

- **リューズを上方向に回す** = 次のフェーズへ進む。最も推奨のハンズフリー操作で
  す。
- **リューズを下方向に回す** = 一時停止 / 再開。
- **画面のボタン** でも操作できます。
- **画面タップ** — 任意設定（設定 → セッション → 「画面タップでフェーズ進行」、
  デフォルトはオフ）。

ウォッチには現在のフェーズ・経過時間・心拍数・直近 5 分の心拍ピーク / ボトムが
表示されます。設定した各フェーズの時間は **ハプティック通知のタイミング**で、
**自動進行はしません**（自分のタイミングで進めるため）。

**バックグラウンド記録：** セッション画面が表示されている間、ウォッチは
**画面を点灯させたまま** にし、**常駐通知付きのフォアグラウンドサービス** を
動かすので、セッション中もタイマーと心拍が動き続けます。（画面オフでの完全な
バックグラウンド記録は、実機での最終確認・検証を進めているところです。）

### 4. セッションを終える

- 最後のフェーズで先へ進めると終了します。
- **60 分操作がないと自動終了**します（先に警告が表示されます）。
- 終了したセッションは Wearable Data Layer 経由で自動でスマホに転送されます。

### 5. Android スマホで振り返り

- **最新タブ（Latest）** — 最新セッションの解析を直接表示: フェーズ帯付きの心拍
  チャート・ととのい度スコア・セット別の内訳・個人比 / 前回比・動線品質、
  （Premium）β スコアと回復カーブ。
- **インタラクティブな心拍チャート** — 心拍チャートは操作できます:
  - **点をタップ** すると値カード（bpm・経過時間・その時点のフェーズ）を表示。
  - **ピンチで最大 20 倍までズーム**。
  - **ドラッグで時間軸をスクロール**。
  - **ダブルタップで表示をリセット**。
- **チャートの表示オプション（設定 → 表示）** — 心拍チャート向けの任意オーバー
  レイ／表示。いずれも **初期値は OFF**:
  - **60 秒移動平均** — 直近 60 秒の移動平均線。
  - **10 分移動平均** — 直近 10 分の移動平均線。
  - **準備フェーズをチャートから隠す** — X 軸を **サウナ入室（0:00）** 起点に
    し直します。
  - Health Connect を連携すると、**安静時心拍数** をチャートの基準線として
    表示することもできます（後述の Health Connect 参照）。
- **履歴タブ（History）** — このタブの **最上部** に **アプリ内分析（無料）** が
  表示されます:
  - **連続記録と回数** — **現在** と **最長** の連続記録、**累計セッション数**。
  - **ベストセッション TOP 10** — **ととのい度スコア** が高い順。
  - **訪問頻度カレンダーヒートマップ** — 通った頻度をカレンダーで表示。
  - **サウナマップ** — 訪問したすべての施設を 1 枚の地図に表示。
  - その下に **過去のセッション一覧**。タップで詳細が開き、**終了地点の地図
    （無料）** と施設候補（タップで施設を設定）が見られます。候補には
    近くの Places 検索に加えて **過去に訪問した約 500 m 以内の施設** も含まれ
    ます。
- **翌日ステータス（Health Connect 連携時）** — 連携している場合、セッションの
  **翌晩** の参考 **睡眠スコア（無料）** と **平均呼吸数** を表示します。
- **トレンドタブ（Trends）** — **一部無料**。無料: ととのい度の推移、モード別の
  平均、期間サマリー。Premium: HRR トレンド（1/3/5）、回復スロープの推移、
  セット数 / セッション長別の平均、セット位置別 HRR、回復カーブの重ね表示、回復
  サマリー。期間フィルタ（全期間 / 30 日 / 7 日）は誰でも利用できます。
- **PDF レポート（Premium）** — トレンドタブから生成し、Android の共有メニューで
  共有。A4 縦・3 ページで、**ベストセッション** と **訪問頻度ヒートマップ** を
  含みます（これらは履歴タブのアプリ内でも無料で見られます）。
- **設定 → データ入出力** — CSV の入出力（Premium）。ローカルバックアップや自前解析
  に。
- **設定 → クラウド同期（Google ドライブ）** — あなた自身のドライブへバックアップ
  （無料・任意。後述のクラウド同期セクション参照）。

**無料と Premium：** 個人比 / 前回比、動線品質（Flow）スコア、終了地点の地図 /
施設ピッカー、**基本トレンド**（ととのい度の推移・モード別・サマリー）、クラウド
同期（Google ドライブ）、アプリ内の履歴分析（連続記録 / ベストセッション /
ヒートマップ / サウナマップ）、睡眠スコア、安静時心拍の基準線はすべて **無料**
です。β スコア、回復カーブ、**高度なトレンド**、PDF レポート、CSV の入出力は
**Premium** です。

### 5a. クラウド同期（任意・無料）

クラウド同期は **任意** で、**オンにするまでオフ** です。使わなければ、データは
これまでどおり各端末（ウォッチ ↔ スマホ、Wearable Data Layer 経由）に保存され
ます。

- **設定 → クラウド同期（Google ドライブ）→「Google ドライブと同期」** からオン
  にします。Google でサインインし、**アプリデータ（`drive.appdata`）** 権限を
  許可します。
- **あなた自身の Google ドライブのアプリ専用フォルダ**（あなたの Google アカウン
  ト配下の非表示「App Data」領域）に **セッションのスナップショット** を保存・取得
  するので、**セッションをバックアップし、端末間で移行** できます。
- 同期は **双方向** で、**セッション単位でマージ** します。
- **開発者はサーバーを持たず、何も保存しません。** データは **あなた自身の**
  Google ドライブに保存され、開発者には渡らず、開発者は **アクセスできません**。
- 同期データは **あなた自身の Google ドライブからいつでも削除** でき、アプリの
  アクセスは **Google アカウントの権限**（または設定）からいつでも **取り消せ**
  ます。

### 6. Health Connect（任意）

Health Connect は **任意** で、**あなたの許可がある場合のみ** 使用します。連携
しなければ、これまでどおり健康データ連携なしで動作します。

- **安静時心拍数を読み取り**、セッションの心拍チャートに基準線として表示します。
- セッションの **翌晩** の **睡眠を読み取り**（参考の **睡眠スコア**として無料
  表示）、**平均呼吸数** を **翌日ステータス** セクションに表示します。
- **各セッションを** Health Connect に **運動 + 心拍の記録** として **書き込み**、
  他のアプリでも使えるようにします。
- 連携・管理はいつでも **設定 → Health Connect** から行えます。

### 7. ちょっとしたコツ

- 心拍を安定して取るため、ウォッチは手首に **しっかり装着** してください。
- 心拍チャートの **点をタップ** すると、その時点の bpm / 時間 / フェーズが分かり
  ます。気になる箇所は **ピンチでズーム** しましょう。
- **設定 → 表示** で **移動平均オーバーレイ** や **準備フェーズを隠す** を ON に
  すると、カーブがより見やすくなります。
- 各セッションの詳細から **施設名**（近くの候補、または約 500 m 以内の過去訪問
  施設から選択、無料）を入れると、サウナマップ・訪問ヒートマップ・PDF レポート
  に反映されます。
- 各セッションに **1〜5 星の評価** をつけられます。
- 連続記録・ベストセッション・訪問ヒートマップは **履歴タブ** で確認できます
  （すべて無料）。
- ととのい度スコアと睡眠スコアは **参考値** であり、医療指標ではありません。

### 8. 典型的な使用例 — 時間制限のあるサウナ施設

時間制限のあるサウナ施設（60〜90 分など）で **3 セット（サウナ → 水風呂 →
外気浴 を 3 回繰り返す）** を行う場合の推奨ワークフロー。

**事前設定**:
- **スタンダードモード** を使用（スマホの設定 → セッション）。
- 設定 → セッションで **「準備フェーズを使う」を ON**。

**施設での操作**:
1. 施設の時間カウントが始まったタイミング（入店タグ・ロッカー）で ウォッチの
   **「スタンダード」をタップしてセッション開始**。準備フェーズに入る（着替
   え・体を洗う時間に活用）。
2. **1 回目のサウナに入る直前** に **リューズを上に回す** →
   「**サウナ**」フェーズに進む。
3. **水風呂（水風呂・湖・プールなど）に入る** タイミングでリューズを上に回す →
   「**水風呂**」フェーズに進む。
4. **椅子やビーチチェアで横になる** タイミングでリューズを上に回す →
   「**外気浴**」フェーズに進む。
5. **次のサウナに入る** タイミングで再度リューズを上に回す → 次のセットの
   「サウナ」フェーズへ。
6. 3 セット目の外気浴が終わるまで 2〜5 を繰り返し、最後に
   **最終フェーズの先へ進める（または画面の「終了」を使う）** とセッションを
   終了。途中でいつでも **リューズを下に回して一時停止** もできます。

3 セットでのリューズ上回し合計：**約 9 回**（サウナ 3 + 水風呂 3 + 外気浴 3）。
最初の「準備 → サウナ」の上回しもこの合計に含まれます。

---

## 関連 / See also

- [FAQ / よくある質問](faq.html)
- [Privacy Policy / プライバシーポリシー](privacy-policy.html)
- [Terms of Use / 利用規約](terms-of-use.html)

**Support / お問い合わせ:** maxsaunatimer@gmail.com
