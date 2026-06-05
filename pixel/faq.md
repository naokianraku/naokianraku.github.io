---
title: FAQ (Pixel Watch & Android)
---

# FAQ / よくある質問 — MaxSauna Timer for Pixel Watch & Android

**Last updated / 最終更新:** 2026-06-05
**Contact / 連絡先:** maxsaunatimer@gmail.com

---

## English

### 1. Subscription & Billing

**Q. How much is Premium?**
Check the current price for your region in Google Play (Subscriptions). A yearly
plan is also available at roughly **20% off** vs paying monthly. New
subscribers get a 30-day free trial.

**Q. What does Premium unlock?**
Detailed metrics (personal z-score / vs-previous comparison / recovery slope β
/ movement-quality detail), recovery curves, the entire Trends tab, the
end-location map with nearby-venue picker, the PDF report, and no banner ads.
(CSV import/export and the basic per-session analysis are **free** — see below.)

**Q. What is free?**
The heart-rate chart with phase bands, the absolute Afterglow score, the
per-set breakdown, the history list, the movement-quality score, **CSV
import/export** (Settings → Data import/export), watch-settings editing, and
the Force-English toggle.

**Q. Is watch ↔ phone sync Premium?**
No. Finished sessions transfer from the Pixel Watch to your Android phone
automatically over the Wearable Data Layer, for everyone. There is no cloud
account, so there is nothing to gate behind Premium here.

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
each device). Only the Premium features (detailed metrics, recovery curves,
the Trends tab, the venue map, the PDF report, ad-free) revert to the free
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
Locally on your Android phone and your Pixel Watch (local JSON files). When the
two are paired, finished sessions transfer Watch → Phone directly over the
Wearable Data Layer (Bluetooth / Wi-Fi). Watch settings sync bidirectionally,
so you can edit watch settings from the phone. There is **no** cloud, no
Google-account sync, and no login.

**Q. What if I delete the app?**
Data is stored only on-device, so deleting the app removes its local data.
Use **CSV export** (Settings → Data import/export, free) as a manual backup,
then re-import after reinstalling.

**Q. Where does the heart rate come from?**
The app reads heart rate live from the Pixel Watch's optical sensor via Wear OS
Health Services during a session (while the session screen is on). It does
**not** read from or write to Health Connect or Google Fit. On an emulator
without a real sensor, it falls back to mock heart-rate data.

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
calls "totonou". The absolute score is free; the personal z-score (個人比) and
vs-previous (前回比) comparisons are Premium. Reference value only — not a
medical metric.

**Q. Can I use the app without a Pixel Watch?**
The timer works on the Android phone alone, but heart-rate measurement and the
Afterglow Score require a Pixel Watch (or other Wear OS smartwatch).

**Q. How do I control the timer with wet hands during a session?**
Use the **rotary crown**: rotate **up** to advance to the next phase, rotate
**down** to pause/resume. The on-screen buttons also work, and there is an
optional "tap screen to advance" setting (OFF by default). Phase times are
**haptic alerts only** — the app does not auto-advance, so you choose when to
move on.

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

**Q. How do I generate a PDF report?**
Premium feature. From the **Trends** tab, generate the report and share it via
the Android share sheet. An A4-portrait, 3-page report is produced:
- **Page 1**: sessions summary, Afterglow trend, heart-rate trend, and recovery
  data (HRR1 / HRR3 / HRR5, plus recovery details)
- **Page 2**: recovery-curve small multiples (latest 11 sessions) plus a
  session-average overlay
- **Page 3**: **Best Sessions TOP 5**, a recent-sessions table, and a
  visit-frequency heatmap

The **Best Sessions ranking and the visit/calendar heatmap exist only inside
this PDF** — there is no separate Best-Sessions or heatmap screen in the app.

**Q. What is in the Trends tab?**
Premium. The Trends tab shows Afterglow-over-time, the HRR trend (1/3/5), the
recovery-slope trend, average Afterglow by set count / by session length / by
mode, a recovery-curve overlay, and a recovery summary (avg HRR1/3/5, best set
position, best HRR1, recovery completeness, time-to-bottom, front-loading). A
period filter lets you view All / 30 days / 7 days.

**Q. How does the venue / map work?**
Premium. If Location permission is granted, the app captures the session **end**
location once when the session ends, shows it on a Google Map in the session
detail, and lists nearby sauna / bath facility candidates from Google Places.
Tap a candidate to set the venue. There is no continuous GPS tracking and no
past-visit radius history. Each session can also have a 1–5 star rating.

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
While a session screen is on, the display is kept awake so the timer and
heart-rate keep running, which uses more battery than an idle watch. The app
auto-ends after 60 minutes with no input (it warns first, then auto-ends) to
protect the battery. There is also an optional low-HR warning during cold water
/ cool-down.

**Q. The Afterglow Score didn't appear after my session.**
The score needs valid heart-rate data after the peak. If you ended the session
within 1 minute of the sauna peak, or the watch lost contact (dropouts), the
score may be missing. Sessions with too few samples are marked as unscored.

### 5. Other

**Q. Can I switch the app to English?**
Yes. The app is available in Japanese and English. Open Settings and turn on
the **Force English** toggle to force the English UI regardless of your system
language.

**Q. Can I use this for medical purposes?**
No. The Afterglow Score, heart-rate values, HRR, and all other figures are
reference information only. They are not medical metrics and must not be used
for diagnosis or treatment decisions. Consult a physician if you have
concerns.

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
詳細指標（個人比 / 前回比 / 回復勾配 β / 動線品質の詳細）、回復カーブ、トレンド
タブ全体、終了位置の地図と近隣施設ピッカー、PDF レポート、そして広告なし。
（CSV の入出力と基本のセッション解析は**無料**です。下記参照。）

**Q. 無料でできることは？**
フェーズ帯つき心拍チャート、ととのい度（絶対値）、セット別内訳、履歴一覧、
動線品質スコア、**CSV 入出力**（設定 → データ入出力）、ウォッチ設定の編集、
英語表示（強制）トグル。

**Q. ウォッチ ↔ スマホ同期は Premium 限定ですか？**
いいえ。完了したセッションは Pixel Watch から Android スマホへ Wearable Data
Layer 経由で自動転送され、全員が利用できます。クラウドアカウントは存在しない
ため、ここに Premium ゲーティングはありません。

**Q. 無料トライアルが終わるとどうなりますか？**
自動的に通常価格で課金されます。トライアル中はいつでもキャンセル可能で、終了
24 時間前までにキャンセルすれば課金されません。

**Q. キャンセル方法は？**
Google Play ストアを開く → プロフィール → 「**お支払いと定期購入**」 →
「**定期購入**」 → 「MaxSauna Premium」 → 「定期購入を解約」。キャンセル後も、
現在の請求期間の終わりまで Premium 機能を利用できます。

**Q. キャンセルするとデータは消えますか？**
消えません。セッション履歴・設定はすべて残ります（各デバイスのローカルに保存
されています）。失われるのは Premium 機能（詳細指標・回復カーブ・トレンドタブ・
施設地図・PDF レポート・広告非表示）だけで、無料版機能に戻ります。

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
Android スマホと Pixel Watch のローカル（JSON ファイル）に保存されます。両者を
ペアリングすると、完了したセッションはウォッチ → スマホへ Wearable Data Layer
経由（Bluetooth / Wi-Fi）で直接転送されます。ウォッチ設定は双方向同期するため、
スマホからウォッチ設定を編集できます。**クラウドも、Google アカウント同期も、
ログインもありません。**

**Q. アプリを削除するとデータはどうなりますか？**
データは端末内のみに保存されるため、アプリを削除するとローカルデータも消えます。
手動バックアップとして **CSV エクスポート**（設定 → データ入出力、無料）を行い、
再インストール後に取り込んでください。

**Q. 心拍数はどこから取得していますか？**
セッション中（セッション画面が表示されている間）に、Pixel Watch の光学式センサー
から Wear OS Health Services 経由でリアルタイムに読み取ります。Health Connect
や Google Fit からの読み書きは**行いません**。実機センサーのないエミュレータ
では、モックの心拍データにフォールバックします。

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
「ととのう」を数値化する独自指標です。絶対値は無料、個人比・前回比の比較は
Premium。参考値のみであり医療指標ではありません。

**Q. Pixel Watch なしで使えますか？**
Android スマホ単体でタイマー機能は使えますが、**心拍計測とととのい度の算出には
Pixel Watch（または他の Wear OS スマートウォッチ）が必要です。**

**Q. セッション中、濡れた手でどう操作しますか？**
**ロータリークラウン**を使います：**上**に回すと次のフェーズへ進み、**下**に回す
と一時停止/再開します。画面のボタンでも操作でき、任意設定の「画面タップで進む」
（デフォルト OFF）もあります。フェーズ時間は**ハプティック（振動）通知のみ**で、
アプリは自動では進みません。進むタイミングはご自身で選べます。

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

**Q. PDF レポートはどう生成しますか？**
Premium 機能です。**トレンド**タブからレポートを生成し、Android の共有シートで
共有します。A4 縦 3 ページの PDF が生成されます:
- **1 ページ目**: サマリー・ととのい度トレンド・心拍推移・回復データ
  （HRR1/3/5・回復関連の詳細）
- **2 ページ目**: 回復カーブのスモールマルチプル（直近 11 セッション）＋
  セッション平均の重ね描き
- **3 ページ目**: **ベストセッション TOP 5**・最近のセッション表・訪問頻度
  ヒートマップ

**ベストセッションのランキングと訪問/カレンダーのヒートマップは、この PDF の
中だけに存在します** — アプリ内に別画面はありません。

**Q. トレンドタブには何がありますか？**
Premium。トレンドタブには、ととのい度の推移、HRR トレンド（1/3/5）、回復勾配
トレンド、セット数別・セッション長別・モード別の平均ととのい度、回復カーブの
重ね描き、回復サマリー（平均 HRR1/3/5・ベストセット位置・ベスト HRR1・回復の
完了度・底打ちまでの時間・フロントローディング）が表示されます。期間フィルター
で 全期間 / 30 日 / 7 日 を切り替えられます。

**Q. 施設・地図はどう動きますか？**
Premium。位置情報の許可がある場合、セッション**終了**時に終了位置を一度だけ
取得し、セッション詳細で Google マップ上に表示、Google Places から近隣のサウナ
・温浴施設候補を一覧表示します。候補をタップすると施設名が設定されます。連続
GPS トラッキングや過去訪問の半径履歴はありません。各セッションには 1〜5 の
星評価も付けられます。

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
セッション画面が表示されている間はタイマーと心拍を継続させるため画面を点灯
維持します。そのため待機時よりバッテリーを消費します。バッテリー保護のため、
60 分間操作がないと自動終了します（先に警告 → その後自動終了）。水風呂 / 外気浴
中の低心拍警告（任意）もあります。

**Q. セッション後にととのい度が表示されません。**
ピーク後の心拍データが必要です。サウナピーク直後（1 分以内）に終了した場合や、
Watch との通信が大きく欠落した場合は計算不可になります。サンプルが少なすぎる
セッションは未スコア表示になります。

### 5. その他

**Q. アプリを英語表示にできますか？**
できます。本アプリは日本語と英語に対応しています。設定を開いて「**英語表示
（強制）**」トグルをオンにすると、システム言語に関係なく英語 UI に固定されます。

**Q. 医療目的で使えますか？**
**いいえ。**ととのい度・心拍値・HRR その他すべての表示は参考値のみで、医療指
標ではありません。診断や治療判断には使用しないでください。健康に不安がある場
合は医師にご相談ください。

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
