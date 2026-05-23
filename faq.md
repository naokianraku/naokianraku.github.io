---
title: FAQ
---

# FAQ / よくある質問 — MaxSauna Timer

**Last updated / 最終更新:** 2026-05-20
**Contact / 連絡先:** maxsaunatimer@gmail.com

---

## English

### 1. Subscription & Billing

**Q. How much is Premium?**
Monthly ¥100, yearly ¥1,000 (regional prices may differ). New subscribers get a
30-day free trial.

**Q. What does Premium unlock?**
Advanced analytics (recovery slope, recovery curves, HRR trends), sharing with
a heart-rate chart image, CSV export, a dedicated Premium app icon, and no
banner ads.

**Q. iCloud sync — is it Premium?**
No. iCloud sync is free for everyone. Data protection is infrastructure, not a
paid feature.

**Q. What happens when the free trial ends?**
Your subscription auto-renews at the regular price. You can cancel at any time
during the trial — if you cancel at least 24 hours before the trial ends, you
are not charged.

**Q. How do I cancel?**
On your iPhone: Settings → tap your Apple ID at the top → Subscriptions →
MaxSauna Premium → Cancel Subscription. After canceling, you keep Premium
features until the current billing period ends.

**Q. Does canceling delete my data?**
No. Your sessions, history, settings, and iCloud sync all stay. Only the
Premium features (advanced analytics, chart-image sharing, CSV export, Premium
app icon, ad-free) revert to the free tier.

**Q. Refunds?**
Apple handles all refund requests. Use
[reportaproblem.apple.com](https://reportaproblem.apple.com).

### 2. Data and Privacy

**Q. What data do you collect?**
The developer does not collect, receive, or store any of your data. There is no
server. All session data, health data, and locations stay on your device, and
if iCloud is enabled, in your own private iCloud account.

**Q. Where is my data stored?**
On your iPhone (SwiftData) and Apple Watch (a local JSON file). With iCloud
enabled, sessions sync through your private CloudKit database — accessible
only by you.

**Q. What if I delete the app?**
With iCloud sync enabled, your data is restored automatically when you
reinstall. Without iCloud, local data is lost — Premium users can use CSV
export as a manual backup.

**Q. Does the app use Apple Health?**
Yes. With your permission, the app reads heart rate during a session and
writes the session as a HealthKit workout, visible in the Apple Health app.

**Q. Does the free version share my data with advertisers?**
The free version shows AdMob banner ads in the History, Analytics, and Session
Detail screens. Ad network data handling follows Google's policies and your
device's privacy settings (ATT / Limit Ad Tracking). See the Privacy Policy
for details.

### 3. Usage & Features

**Q. What is the Afterglow Score?**
A 0–100 score estimating how quickly your parasympathetic nervous system
("rest mode") engages after a sauna session, derived from your heart-rate
recovery (HRR1 / HRR3 / HRR5). It puts a number on what Japanese sauna culture
calls "totonou". Reference value only — not a medical metric.

**Q. Can I use the app without an Apple Watch?**
The timer works on iPhone alone, but heart-rate measurement and the Afterglow
Score require an Apple Watch.

**Q. Do I need to touch the screen during a sauna session?**
No. Once you start a session, measurement continues hands-free — useful with
wet hands or a towel.

**Q. What's the difference between Standard and Simple mode?**
Standard mode tracks distinct phases (sauna → cold plunge → cool-down) per
set. Simple mode runs as one continuous session and detects sets afterwards
from heart-rate peaks.

**Q. What is HRR (HRR1 / HRR3 / HRR5)?**
HRR = Heart Rate Recovery. HRR1 is your heart-rate drop 1 minute after the
peak, HRR3 at 3 minutes, HRR5 at 5 minutes. Higher means faster recovery,
which is the basis for the Afterglow Score.

**Q. What is the recovery slope?**
A Premium analytics metric (bpm/min) — the slope of the linear-fitted central
portion of your recovery curve. Steeper means faster recovery.

### 4. Troubleshooting

**Q. Watch session data isn't reaching my iPhone.**
Open the MaxSauna app on both devices, keep them nearby with Bluetooth on, and
relaunch both apps. The Watch resends pending data automatically. You can also
trigger a manual resend in iPhone Settings → Apple Watch sync status.

**Q. Heart rate isn't showing on the Watch.**
Make sure the Watch is worn snugly and wrist detection is enabled. Confirm
that you granted Health permissions when first launching the app
(iPhone Settings → Health → Data Access & Devices).

**Q. "Save to Photos" fails after I tap save.**
Check iPhone Settings → MaxSauna → Photos → set to "Add Only" or higher. If
the issue persists, rebuild the app from the App Store update or restart your
iPhone.

**Q. Watch battery drains quickly.**
A 60-minute sauna session uses about 10–15% of an Apple Watch Series 7+
battery in our testing. Disable Always-On Display in the Watch system settings
if you need more headroom. The app also auto-ends after 60 minutes of
inactivity to protect the battery.

**Q. The Afterglow Score didn't appear after my session.**
The score needs valid heart-rate data after the peak. If you ended the session
within 1 minute of the sauna peak, or the watch lost contact (dropouts), the
score may be missing. Sessions with too few samples are marked as unscored.

**Q. The app switches away when water hits the Watch screen.**
This is an Apple Watch system behavior — water on the touchscreen registers as
multi-touch input, which can trigger OS-level gestures (Control Center, app
switching, returning to the watch face). The app's own "no screen tap" policy
only blocks taps within the app, not the OS-level gestures. The fix is to enable
**Apple Watch's Water Lock**:

- **In-app setting (recommended)**: iPhone MaxSauna → Settings → Session →
  toggle on "Auto Water Lock in Pre-sauna" and/or "Auto Water Lock in
  Cool-down". The Watch turns on Water Lock automatically when those phases
  start.
- **Manual**: On the Watch, swipe up to open Control Center → tap the 💧
  droplet icon.

To unlock, rotate the Digital Crown (this also ejects water from the speaker
via sound waves — Apple's standard behavior).

### 5. Other

**Q. Can I use this for medical purposes?**
No. The Afterglow Score, heart-rate values, HRR, and all other figures are
reference information only. They are not medical metrics and must not be used
for diagnosis or treatment decisions. Consult a physician if you have
concerns.

**Q. What is the Recommended use?**
Personal wellness tracking. Use saunas at your own risk and follow your local
sauna's rules. Avoid alcohol before and during sauna use.

**Q. How do I contact support?**
Email **maxsaunatimer@gmail.com**. Please include your iOS / watchOS versions
and a brief description of the issue.

**Q. Where can I find the Privacy Policy and Terms of Use?**
[Privacy Policy](privacy-policy.html) / [Terms of Use](terms-of-use.html).

---

## 日本語

### 1. サブスクリプション・課金

**Q. Premium はいくらですか？**
月額 ¥100、年額 ¥1,000（地域により価格が異なる場合あり）。新規ユーザーは 30 日
間の無料トライアル付き。

**Q. Premium で何が変わりますか？**
高度な分析（回復勾配・回復カーブ・HRR 推移）、心拍チャート画像つきの共有、
CSV エクスポート、専用アプリアイコン、広告なし。

**Q. iCloud 同期は Premium 限定ですか？**
いいえ。iCloud 同期は無料・有料を問わず全員が利用できます。データ保護は機能
ではなくインフラ、という方針です。

**Q. 無料トライアルが終わるとどうなりますか？**
自動的に通常価格で課金されます。トライアル中はいつでもキャンセル可能で、終了
24 時間前までにキャンセルすれば課金されません。

**Q. キャンセル方法は？**
iPhone の「設定」アプリ → 上部の Apple ID → 「サブスクリプション」 →
「MaxSauna Premium」 → 「サブスクリプションをキャンセル」。キャンセル後も、
現在の請求期間の終わりまで Premium 機能を利用できます。

**Q. キャンセルするとデータは消えますか？**
消えません。セッション履歴・設定・iCloud 同期はすべて残ります。失われるのは
Premium 機能（高度な分析、チャート画像共有、CSV エクスポート、専用アイコン、
広告非表示）だけで、無料版機能に戻ります。

**Q. 返金は可能ですか？**
返金処理は Apple が行います。[reportaproblem.apple.com](https://reportaproblem.apple.com)
から申請してください。

### 2. データとプライバシー

**Q. アプリは何のデータを集めますか？**
**開発者は一切収集していません。**サーバーも持っていません。すべてのセッショ
ンデータ・健康データ・位置情報はお使いのデバイス内に、iCloud 同期が有効な場合
はあなた自身の iCloud アカウントに保存されます。

**Q. データはどこに保存されますか？**
iPhone（SwiftData）と Apple Watch（ローカル JSON）に保存。iCloud 同期が有効な
場合は、あなた自身の Private CloudKit データベース経由で同期されます。

**Q. アプリを削除するとデータはどうなりますか？**
iCloud 同期が有効なら、再インストール時に自動復元されます。無効の場合はローカ
ルデータは消失するため、Premium ユーザーは CSV エクスポートを手動バックアップ
として推奨します。

**Q. ヘルスケアアプリとの連携は？**
はい。許可をいただければ、心拍数をセッション中に読み取り、セッション全体を
HealthKit のワークアウトとして書き込みます。Apple ヘルスケアアプリから振り返
れます。

**Q. 無料版の広告は私のデータを共有しますか？**
無料版は AdMob のバナー広告を履歴 / 分析 / セッション詳細の 3 画面に表示します。
広告ネットワーク側のデータ処理は Google のポリシーと端末のプライバシー設定
（ATT / 広告トラッキング制限）に従います。詳細はプライバシーポリシー参照。

### 3. 使い方・機能

**Q. ととのい度とは何ですか？**
サウナ後に副交感神経（リラックス系）がどれだけ速やかに働き始めたかを心拍降下
量（HRR1 / HRR3 / HRR5）から推定する、0〜100 点のスコアです。サウナ文化の
「ととのう」を数値化する独自指標で、参考値のみであり医療指標ではありません。

**Q. Apple Watch なしで使えますか？**
iPhone 単体でタイマー機能は使えますが、**心拍計測とととのい度の算出には Apple
Watch が必要です。**

**Q. サウナ中に画面操作が必要ですか？**
いいえ。一度セッションを開始すれば、画面に触れずに測定が続きます。濡れた手や
タオル越しでも操作不要です。

**Q. 標準モードとシンプルモードの違いは？**
標準モードはサウナ / 水風呂 / 外気浴のフェーズを切り替えながらセット単位で計
測。シンプルモードはフェーズ区切りなしの連続計測で、あとから心拍ピーク検出で
セットを推定します。

**Q. HRR（HRR1 / HRR3 / HRR5）とは？**
HRR = Heart Rate Recovery（心拍回復）。HRR1 はピーク後 1 分時点の心拍降下、
HRR3 は 3 分後、HRR5 は 5 分後の降下量。値が大きいほど回復が速い、というのが
ととのい度算出のベースです。

**Q. 回復勾配とは？**
Premium の高度な分析に含まれる指標（bpm/分）。回復カーブの中央 60% に直線をあ
てたときの傾きで、急なほど回復が速いことを表します。

### 4. トラブルシューティング

**Q. Watch のセッションデータが iPhone に届きません。**
両デバイスで MaxSauna を開いて近くに置き、Bluetooth を確認、両方のアプリを再
起動してください。Watch 側に保留中のデータがあれば自動再送されます。iPhone の
設定からも手動再送できます（設定 → Apple Watch → 同期ステータス）。

**Q. Watch に心拍が表示されません。**
Watch を手首にしっかり装着しているか、手首検知が有効か確認してください。アプリ
初回起動時にヘルスケアの権限を許可したかも確認（iPhone 設定 → ヘルスケア →
データアクセスとデバイス）。

**Q. 「写真への保存」が失敗します。**
iPhone の「設定」 → MaxSauna → 「写真」を「追加のみ」以上に設定してください。
それでも改善しない場合は App Store からのアップデート後にやり直すか、iPhone を
再起動してください。

**Q. Watch のバッテリーが早く減ります。**
当方検証では 60 分セッションで Apple Watch Series 7 以降のバッテリーを 10〜15%
消費します。さらに節約したい場合は Watch システム設定で「常時表示」をオフに
してください。アプリは 60 分操作なしで自動終了します（バッテリー保護のため）。

**Q. セッション後にととのい度が表示されません。**
ピーク後の心拍データが必要です。サウナピーク直後（1 分以内）に終了した場合や、
Watch との通信が大きく欠落した場合は計算不可になります。サンプルが少なすぎる
セッションは未スコア表示になります。

**Q. 準備中（シャワーなど）に画面が濡れて、アプリが別画面に切り替わってしまいます。**
これは Apple Watch の仕様で、濡れた画面のタッチセンサーが水を多点タッチとして誤検
知し、OS のシステムジェスチャ（コントロールセンター呼び出し・アプリ切替・文字盤
に戻る等）を誤発火させることがあります。MaxSauna 内の「画面タップ無反応」設定は
**アプリ内のタップしか抑制できず、OS のジェスチャは止められません**。対策は
**Apple Watch の Water Lock（水ロック）** を有効にすることです:

- **アプリ内設定（推奨）**: iPhone の MaxSauna → 設定 → セッション →
  「準備フェーズで Water Lock を自動有効化」/「休憩フェーズで Water Lock を
  自動有効化」をオン。該当フェーズに入ると Watch が自動で Water Lock を有効化します。
- **手動**: Apple Watch のコントロールセンター（画面下端から上スワイプ）→ 💧
  アイコンをタップ。

解除は **Digital Crown を回転**（音波で水を排出する副作用つき・Apple 標準）。

### 5. その他

**Q. 医療目的で使えますか？**
**いいえ。**ととのい度・心拍値・HRR その他すべての表示は参考値のみで、医療指
標ではありません。診断や治療判断には使用しないでください。健康に不安がある場
合は医師にご相談ください。

**Q. 推奨される使い方は？**
個人のウェルネス記録として。サウナ利用は自己責任で、施設のルールに従ってくだ
さい。サウナ前・サウナ中の飲酒は避けてください。

**Q. お問い合わせは？**
**maxsaunatimer@gmail.com** までメールしてください。iOS / watchOS のバージョン
と、症状の簡単な説明を添えていただけると助かります。

**Q. プライバシーポリシー・利用規約はどこ？**
[プライバシーポリシー](privacy-policy.html) /
[利用規約](terms-of-use.html)。

---
