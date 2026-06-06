---
title: FAQ (Pixel Watch & Android)
---

# FAQ / よくある質問 — MaxSauna Timer for Pixel Watch & Android

**Last updated / 最終更新:** 2026-06-05
**Contact / 連絡先:** maxsaunatimer@gmail.com

> 🐛 **不具合・改善要望はこちら → [フィードバックフォーム](feedback.html)** / Report bugs & suggestions: **[Feedback form](feedback.html)**

---

## English

### 1. Subscription & Billing

**Q. How much is Premium?**
Check the current price for your region in Google Play (Subscriptions). A yearly
plan is also available at roughly **20% off** vs paying monthly. New
subscribers get a 30-day free trial.

**Q. What does Premium unlock?**
The recovery-slope score **β**, per-set **recovery curves**, the **advanced
Trends** (HRR trend, recovery-slope trend, by-set-count / by-session-length
averages, set-position HRR, the recovery-curve overlay, and the recovery
summary), the **PDF report**, **CSV import/export**, and **no banner ads**.
(The personal z-score / vs-previous comparison, the movement-quality score, the
end-location map, and the basic per-session and Trends analysis are **free** —
see below.)

**Q. What is free?**
The heart-rate chart with phase bands, the absolute Afterglow score, the
per-set breakdown, the history list, the **personal z-score (個人比) and
vs-previous (前回比)** comparisons, the movement-quality (Flow) score, the
**end-location map with the nearby-venue picker**, the **basic Trends**
(Afterglow-over-time, by-mode average, and the period summary), watch-settings
editing, and the Force-English toggle. The **in-app History analytics**
(current / longest streak and total count, the **Best Sessions TOP 10**, the
visit-frequency calendar heatmap, and the Sauna Map of your visited venues) are
also free, as are the **Sleep score** and the **resting-HR reference line** when
you connect Health Connect.

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
**Subscriptions** → MaxSauna Premium → Cancel subscription. After canceling,
you keep Premium features until the current billing period ends.

**Q. Does canceling delete my data?**
No. Your sessions, history, and settings all stay (they are stored locally on
each device). Only the Premium features (the β score, recovery curves, the
advanced Trends, the PDF report, CSV import/export, ad-free) revert to the free
tier.

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
vs-previous (前回比) comparisons are all **free**; the recovery-slope score β
is Premium. Reference value only — not a medical metric.

**Q. Can I use the app without a Pixel Watch?**
The timer works on the Android phone alone, but heart-rate measurement and the
Afterglow Score require a Pixel Watch (or other Wear OS smartwatch).

**Q. How do I control the timer with wet hands during a session?**
Use the **rotary crown**: rotate **up** to advance to the next phase, rotate
**down** to pause/resume. The on-screen buttons also work, and there is an
optional "tap screen to advance" setting (OFF by default). Phase times are
**haptic alerts only** — the app does not auto-advance, so you choose when to
move on.

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

**Q. What analytics are in the History tab?**
**Free.** At the top of the **History** tab the app shows your **current and
longest streak** plus your **total session count**, a **Best Sessions TOP 10**
ranking (by Afterglow score), a **visit-frequency calendar heatmap**, and a
**Sauna Map** that plots all of your visited venues on one map. These are all
free and live in the app (no Premium and no PDF required).

**Q. How do I generate a PDF report?**
Premium feature. From the **Trends** tab, generate the report and share it via
the Android share sheet. An A4-portrait, 3-page report is produced:
- **Page 1**: sessions summary, Afterglow trend, heart-rate trend, and recovery
  data (HRR1 / HRR3 / HRR5, plus recovery details)
- **Page 2**: recovery-curve small multiples (latest 11 sessions) plus a
  session-average overlay
- **Page 3**: **Best Sessions TOP 5**, a recent-sessions table, and a
  visit-frequency heatmap

The Best Sessions ranking and the visit/calendar heatmap are **also available
free in the History tab** (TOP 10 there); the PDF still includes its own
versions as part of the exported report.

**Q. What is in the Trends tab?**
The Trends tab is **partly free**. **Free:** Afterglow-over-time, average
Afterglow by mode, and the period summary. **Premium:** the HRR trend (1/3/5),
the recovery-slope trend, average Afterglow by set count / by session length,
set-position HRR, a recovery-curve overlay, the recovery summary (avg HRR1/3/5,
best set position, best HRR1, recovery completeness, time-to-bottom,
front-loading), and the PDF report button. A period filter (All / 30 days /
7 days) is available to everyone.

**Q. How does the venue / map work?**
**Free.** If Location permission is granted, the app captures the session **end**
location once when the session ends, shows it on a Google Map in the session
detail, and lists nearby sauna / bath facility candidates. The candidates come
from a Google Places search **plus your own past-visited venues within about
500 m**. Tap a candidate to set the venue. There is no continuous GPS tracking.
Each session can also have a 1–5 star rating.

### 4. Troubleshooting

**Q. Watch session data isn't reaching my Android phone.**
Open the MaxSauna app on both devices, keep them nearby with Bluetooth (or
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

## 日本語

### 1. サブスクリプション・課金

**Q. Premium はいくらですか？**
お住まいの地域の最新価格は Google Play（定期購入）でご確認ください。年額プラン
も用意されており、月額換算で **約 2 割お得** です。新規ユーザーは 30 日間の
無料トライアル付き。

**Q. Premium で何が変わりますか？**
回復勾配スコア **β**、セット別の**回復カーブ**、**高度なトレンド**（HRR 推移 /
回復勾配の推移 / セット数別・セッション長別の平均 / セット位置別 HRR / 回復カーブ
重ね描き / 回復サマリー）、**PDF レポート**、**CSV 入出力**、そして**広告なし**。
（個人比 / 前回比、動線品質スコア、終了位置の地図、基本のセッション解析と基本
トレンドは**無料**です。下記参照。）

**Q. 無料でできることは？**
フェーズ帯つき心拍チャート、ととのい度（絶対値）、セット別内訳、履歴一覧、
**個人比・前回比**、**動線品質（Flow）スコア**、**終了位置の地図と
近隣施設ピッカー**、**基本トレンド**（ととのい度の推移・モード別平均・期間サマリー）、
ウォッチ設定の編集、英語表示（強制）トグル。**履歴タブのアプリ内分析**（現在 /
最長の連続日数と合計回数、**ベストセッション TOP 10**、訪問頻度カレンダー
ヒートマップ、訪れた施設を表示するサウナマップ）も無料です。Health Connect を
連携した場合の**睡眠スコア**と**安静時心拍の参照ライン**も無料です。

**Q. ウォッチ ↔ スマホ同期は Premium 限定ですか？**
いいえ。完了したセッションは Pixel Watch から Android スマホへ Wearable Data
Layer 経由で自動転送され、全員が利用できます。任意の Google Drive クラウド同期
（下記「クラウド同期 / バックアップはどう動きますか？」参照）も**無料**で、
ここに Premium ゲーティングはありません。

**Q. 無料トライアルが終わるとどうなりますか？**
自動的に通常価格で課金されます。トライアル中はいつでもキャンセル可能で、終了
24 時間前までにキャンセルすれば課金されません。

**Q. キャンセル方法は？**
Google Play ストアを開く → プロフィール → 「**お支払いと定期購入**」 →
「**定期購入**」 → 「MaxSauna Premium」 → 「定期購入を解約」。キャンセル後も、
現在の請求期間の終わりまで Premium 機能を利用できます。

**Q. キャンセルするとデータは消えますか？**
消えません。セッション履歴・設定はすべて残ります（各デバイスのローカルに保存
されています）。失われるのは Premium 機能（β スコア・回復カーブ・高度なトレンド・
PDF レポート・CSV 入出力・広告非表示）だけで、無料版機能に戻ります。

**Q. 課金したのに新しい端末で Premium が有効になりません。**
設定を開いて「**購入を復元**」をタップし、Google Play の購入状態を再確認して
ください。

**Q. 返金は可能ですか？**
Google Play での購入の返金処理は Google が行います。
[play.google.com](https://play.google.com) の注文履歴から申請してください。

### 2. データとプライバシー

**Q. アプリは何のデータを集めますか？**
**開発者は一切収集していません。**サーバーもアカウントもありません。すべての
セッションデータ・心拍データ・位置情報はお使いのデバイス内にとどまり、開発者
には**送信されません**。

**Q. データはどこに保存されますか？**
既定では、Android スマホと Pixel Watch のローカル（JSON ファイル）に保存されます。
両者をペアリングすると、完了したセッションはウォッチ → スマホへ Wearable Data
Layer 経由（Bluetooth / Wi-Fi）で直接転送されます。ウォッチ設定は双方向同期する
ため、スマホからウォッチ設定を編集できます。**開発者のサーバーはなく、開発者への
ログインもありません。** **任意で**、**クラウド同期（Google Drive）**をオンにすると、
セッションのスナップショットを**あなた自身の** Google Drive にバックアップできます
（下記「クラウド同期 / バックアップはどう動きますか？」参照）。クラウド同期は、
サインインして同期をタップするまで **オフ** です。

**Q. クラウド同期 / バックアップはどう動きますか？**
クラウド同期は**任意で無料**です。**設定 → クラウド同期（Google Drive）**で
**「Google Drive と同期」**をタップすると、Google でサインインし、`drive.appdata`
権限を使ってセッションのスナップショットを**あなた自身の** Google Drive ——
お使いの Google アカウント配下の、アプリ専用で非表示の「App Data」フォルダ ——
に保存・取得します。目的はセッションのバックアップと端末間の移行で、同期は
**双方向（セッション単位でマージ）**です。重要な点として、**開発者は引き続き
サーバーを一切運用しておらず、何も保存しません**：データはあなた自身の Google
Drive に入り、開発者には渡らず、開発者はアクセスできません。サインイン / 同期を
タップするまでは **オフ** のままで、使わなければデータは従来どおりお使いの
デバイス内（ウォッチ ↔ スマホ、Wearable Data Layer 経由）にとどまります。同期した
データは、いつでもあなた自身の Google Drive から**削除**でき、アプリのアクセス権は
Google アカウントの権限（または設定）からいつでも**取り消せます**。

**Q. アプリを削除するとデータはどうなりますか？**
データは既定で端末内に保存されるため、アプリを削除するとローカルデータは消えます。
無料のバックアップ手段は **クラウド同期（Google Drive）** です。オンにしておくと
セッションがあなた自身の Google Drive に保存され、再インストール後に再同期できます。
Premium 会員は手動バックアップとして **CSV エクスポート**（設定 → データ入出力）も
利用でき、再インストール後に取り込めます。

**Q. 心拍数はどこから取得していますか？**
セッション中（セッション画面が表示されている間）に、Pixel Watch の光学式センサー
から Wear OS Health Services 経由でリアルタイムに読み取ります。実機センサーの
ないエミュレータでは、モックの心拍データにフォールバックします。
**任意で**、**Health Connect** を連携すると（設定 → Health Connect、ユーザーの
許可が必要）、**安静時心拍**を読み取ってセッションの心拍チャートに参照ラインと
して表示したり、**完了したセッションを** Health Connect に運動 + 心拍の記録と
して**書き戻して**他のアプリで使えるようにできます。Health Connect の連携は
完全に任意で、連携しなければ従来どおり、ヘルスデータ連携なしで動作します。

**Q. 睡眠スコア / 翌日ステータスとは何ですか？**
**Health Connect** を連携し、そこに**睡眠データ**が記録されている場合、セッション
詳細にセッションの**翌日（翌晩）**の **翌日ステータス**セクションを表示できます：
参考値の**睡眠スコア**（無料）と、その晩の平均呼吸数を Health Connect から
読み取って表示します。いずれも参考値のみで、Health Connect の連携と睡眠データ
の両方が必要です。どちらかが無い場合、このセクションは表示されません。

**Q. 無料版の広告は私のデータを共有しますか？**
無料版は AdMob のバナー広告を表示します。広告ネットワーク側のデータ処理は
Google のポリシーと端末のプライバシー設定（Android の広告 ID 制御：システム
設定 → プライバシー → 広告、および該当する場合は Google UMP / GDPR 同意ダイア
ログ）に従います。Premium では広告が表示されません。詳細はプライバシーポリシー
参照。

### 3. 使い方・機能

**Q. ととのい度とは何ですか？**
サウナ後に副交感神経（リラックス系）がどれだけ速やかに働き始めたかを心拍降下
量（HRR1 / HRR3 / HRR5）から推定する、0〜100 点のスコアです。サウナ文化の
「ととのう」を数値化する独自指標です。絶対値・個人比・前回比の比較はいずれも
**無料**で、回復勾配スコア β は Premium。参考値のみであり医療指標ではありません。

**Q. Pixel Watch なしで使えますか？**
Android スマホ単体でタイマー機能は使えますが、**心拍計測とととのい度の算出には
Pixel Watch（または他の Wear OS スマートウォッチ）が必要です。**

**Q. セッション中、濡れた手でどう操作しますか？**
**ロータリークラウン**を使います：**上**に回すと次のフェーズへ進み、**下**に回す
と一時停止/再開します。画面のボタンでも操作でき、任意設定の「画面タップで進む」
（デフォルト OFF）もあります。フェーズ時間は**ハプティック（振動）通知のみ**で、
アプリは自動では進みません。進むタイミングはご自身で選べます。

**Q. セッション中、記録はバックグラウンドでも続きますか？**
セッション画面が表示されている間、ウォッチは画面を点灯維持し、**常駐通知つきの
フォアグラウンドサービス**を実行します。これにより、セッションの間タイマーと
心拍計測が動き続けます。（画面オフ完全バックグラウンド記録は、実機での最終調整
・検証中です。）

**Q. 心拍チャートを操作できますか？**
はい。心拍チャートはインタラクティブです。**点をタップ**すると、その時点の
bpm・経過時間・フェーズを表示する値カードが出ます。**ピンチで最大 20 倍まで
拡大**、**ドラッグで時間軸をスクロール**、**ダブルタップで表示をリセット**でき
ます。

**Q. チャートに移動平均線を追加したり、準備フェーズを隠せますか？**
できます。**設定 → 表示**で、心拍チャートに 2 本の移動平均（後方移動平均）の
重ね描き — **60 秒**平均と **10 分**平均 — をそれぞれ個別にオンにできます。
さらに **「準備フェーズをチャートから隠す」**トグルがあり、サウナ入室を 0:00 と
して X 軸を取り直します。いずれも初期値は **OFF** です。

**Q. 標準モードとシンプルモードの違いは？**
標準モードはサウナ / 水風呂 / 外気浴のフェーズをセット単位で計測し、セット別の
時間・心拍しきい値を設定でき、任意の準備フェーズや「その他/追加」フェーズも
使えます。シンプルモードはフェーズ区切りなしの連続計測で、セットを自動推定し
ます（手動フェーズなし）。

**Q. HRR（HRR1 / HRR3 / HRR5）とは？**
HRR = Heart Rate Recovery（心拍回復）。HRR1 はピーク後 1 分時点の心拍降下、
HRR3 は 3 分後、HRR5 は 5 分後の降下量。値が大きいほど回復が速い、というのが
ととのい度算出のベースです。

**Q. 回復勾配とは？**
Premium の分析に含まれる指標（bpm/分）。回復カーブの中央部に直線をあてたとき
の傾き（β）で、急なほど回復が速いことを表します。

**Q. 動線品質スコアとは？**
スコア指標（0-100 点、優・良・平均・要改善）。サウナピーク後の心拍数スパイク
回数で算出。サウナ→水風呂→外気浴の移動が長い施設では心拍が再上昇しがちです
が、スパイクが少ないほど動線が良い施設と判定。セッション解析では**無料**で確認
でき、詳細内訳と期間平均（Premium の PDF レポート）は Premium です。

**Q. 履歴タブにはどんな分析がありますか？**
**無料です。**　**履歴**タブの上部に、**現在 / 最長の連続日数**と**合計セッション
回数**、**ベストセッション TOP 10**（ととのい度順）ランキング、**訪問頻度
カレンダーヒートマップ**、訪れたすべての施設を 1 枚の地図に表示する**サウナ
マップ**が表示されます。いずれも無料で、アプリ内で確認できます（Premium も PDF
も不要です）。

**Q. PDF レポートはどう生成しますか？**
Premium 機能です。**トレンド**タブからレポートを生成し、Android の共有シートで
共有します。A4 縦 3 ページの PDF が生成されます:
- **1 ページ目**: サマリー・ととのい度トレンド・心拍推移・回復データ
  （HRR1/3/5・回復関連の詳細）
- **2 ページ目**: 回復カーブのスモールマルチプル（直近 11 セッション）＋
  セッション平均の重ね描き
- **3 ページ目**: **ベストセッション TOP 5**・最近のセッション表・訪問頻度
  ヒートマップ

ベストセッションのランキングと訪問/カレンダーのヒートマップは、**履歴タブでも
無料で確認できます**（こちらは TOP 10）。PDF にもエクスポートレポートの一部
として独自に収録されています。

**Q. トレンドタブには何がありますか？**
トレンドタブは**一部無料**です。**無料：**ととのい度の推移、モード別の平均
ととのい度、期間サマリー。**Premium：**HRR トレンド（1/3/5）、回復勾配トレンド、
セット数別・セッション長別の平均ととのい度、セット位置別 HRR、回復カーブの
重ね描き、回復サマリー（平均 HRR1/3/5・ベストセット位置・ベスト HRR1・回復の
完了度・底打ちまでの時間・フロントローディング）、PDF レポートボタン。期間
フィルター（全期間 / 30 日 / 7 日）は誰でも利用できます。

**Q. 施設・地図はどう動きますか？**
**無料です。**位置情報の許可がある場合、セッション**終了**時に終了位置を一度だけ
取得し、セッション詳細で Google マップ上に表示、近隣のサウナ・温浴施設候補を
一覧表示します。候補は **Google Places の検索結果に加えて、約 500 m 圏内の
あなたの過去訪問施設**も含みます。候補をタップすると施設名が設定されます。連続
GPS トラッキングはありません。各セッションには 1〜5 の星評価も付けられます。

### 4. トラブルシューティング

**Q. Watch のセッションデータが Android スマホに届きません。**
両デバイスで MaxSauna を開いて近くに置き、Bluetooth（または Wi-Fi）を確認、
両方のアプリを再起動してください。再接続すると、ウォッチ側に保留中のセッション
があれば Wearable Data Layer 経由で自動再送されます。

**Q. Watch に心拍が表示されません。**
Watch を手首にしっかり装着し、アプリ初回起動時に **Body Sensors（心拍）** の
権限を許可したか確認してください。この権限を拒否すると、実際の心拍ではなく
デモ / モックデータにフォールバックします。

**Q. セッション中に Watch のバッテリーが減ります。**
セッション画面が表示されている間はタイマーと心拍を継続させるため、画面を点灯
維持し、フォアグラウンドサービスを実行します。そのため待機時よりバッテリーを
消費します。バッテリー保護のため、60 分間操作がないと自動終了します（先に警告
→ その後自動終了）。水風呂 / 外気浴中の低心拍警告（任意）もあります。

**Q. セッション後にととのい度が表示されません。**
ピーク後の心拍データが必要です。サウナピーク直後（1 分以内）に終了した場合や、
Watch との通信が大きく欠落した場合は計算不可になります。サンプルが少なすぎる
セッションは未スコア表示になります。

**Q. 安静時心拍ライン・睡眠スコア・翌日ステータスが表示されません。**
これらは **Health Connect** から取得します。**設定 → Health Connect** で連携し、
該当する読み取り権限を許可しているか、そしてデータが存在するか（安静時心拍の
記録、およびセッション翌晩の睡眠データ）を確認してください。Health Connect を
連携していない場合やデータが無い場合は、これらの項目が表示されないだけで、その他
のアプリ機能には影響しません。

### 5. その他

**Q. アプリを英語表示にできますか？**
できます。本アプリは日本語と英語に対応しています。設定を開いて「**英語表示
（強制）**」トグルをオンにすると、システム言語に関係なく英語 UI に固定されます。

**Q. 医療目的で使えますか？**
**いいえ。**ととのい度・心拍値・HRR・睡眠スコアその他すべての表示は参考値の
みで、医療指標ではありません。診断や治療判断には使用しないでください。健康に
不安がある場合は医師にご相談ください。

**Q. 推奨される使い方は？**
個人のウェルネス記録として。サウナ利用は自己責任で、施設のルールに従ってくだ
さい。サウナ前・サウナ中の飲酒は避けてください。

**Q. お問い合わせは？**
**maxsaunatimer@gmail.com** までメールしてください。Android / Wear OS のバー
ジョンと、症状の簡単な説明を添えていただけると助かります。

**Q. プライバシーポリシー・利用規約はどこ？**
[プライバシーポリシー](privacy-policy.html) /
[利用規約](terms-of-use.html)。

---

## 関連 / See also

- [Guide / 取扱説明書](guide.html)
- [FAQ / よくある質問](faq.html)
- [Privacy Policy / プライバシーポリシー](privacy-policy.html)
- [Terms of Use / 利用規約](terms-of-use.html)
