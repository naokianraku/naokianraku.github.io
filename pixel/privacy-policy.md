---
title: Privacy Policy (Pixel Watch & Android)
---

# Privacy Policy / プライバシーポリシー — MaxRecover Timer for Pixel Watch & Android

**Last updated / 最終更新:** 2026-06-05
**Effective date / 施行日:** (set on Google Play release / Google Play 公開日に設定)
**Developer / 開発者:** Naoki Anraku (安樂直樹), an individual developer
**Contact / 連絡先:** maxsaunatimer@gmail.com

---

## English

### 1. Overview

MaxRecover Timer ("the App") is a Pixel Watch (Wear OS) and Android phone app that
times sauna sessions and records heart-rate-based data. This Privacy Policy
explains what data the App handles and how.

**The developer does not operate any server and does not collect, receive, or
store your personal data.** Your session data, heart-rate data, and location
data stay on your devices (your watch and your phone) as local files. The App
has no developer-side cloud account and no login to the developer. When your
watch and phone are paired, finished sessions are transferred directly from the
watch to the phone over the Wearable Data Layer (Bluetooth/Wi-Fi); they are not
routed through the developer or any cloud of the App. The developer has no
access to your data.

**Cloud sync is optional and goes only to your own Google Drive.** If you choose
to turn it on (**Settings → Cloud sync (Google Drive) → "Sync with Google
Drive"**), the App stores a snapshot of your sessions in **your own** Google
Drive's app-private ("App Data") folder, under your Google account. This is
free. The developer still operates no server and holds nothing — your data goes
to your Drive, not to the developer, and the developer cannot access it. Cloud
sync is **off until you sign in / tap Sync**; if you never use it, your data
stays on your devices exactly as before. See Section 6 for details.

If you choose to connect **Health Connect**, the App can read and write certain
health data on your device through Health Connect, with your explicit
permission. This stays on your device and is **never sent to the developer** —
see Section 5 for details.

### 2. Data the App handles

| Category | Examples | Purpose |
|---|---|---|
| Heart-rate data | Heart-rate samples read live from the watch's optical sensor during a session | Show session history, heart-rate charts, recovery analytics, and the "Afterglow Score" |
| Location data | Approximate location captured once at the end of a session (latitude/longitude), only if you grant Location | Saved with the session as the venue location, for your reference, and to show the map / nearby-venue picker (including your past-visited venues within about 500 m) |
| Session data | Session times, phases, computed scores, the venue you pick and a 1–5 star rating | Core app functionality |
| Health Connect data (optional) | Resting heart rate, Sleep, and Respiratory rate **read** from Health Connect; exercise + heart-rate records **written** to Health Connect — only if you connect it | Show a resting-HR reference line, a next-day Sleep score / respiratory-rate reference, and let other apps use your sessions |
| Cloud sync data (optional) | A snapshot of your sessions stored in **your own** Google Drive's app-private folder, only if you turn on Cloud sync | Back up your sessions and move them between your devices |
| Advertising data | Device and ad-interaction information collected by Google AdMob (free version only) | Show banner ads |

The App has no account or login. It does not ask for your name or email. A short
export-name label you may optionally enter is stored only on your device.

The App reads heart rate **live from the watch's optical sensor** via Wear OS
Health Services during a session. **Health Connect is optional** and, only when
you connect it, the App reads and writes specific data through it (see Section
5). The App does not access any other apps' health data except through Health
Connect with your permission.

When you open the session map / venue feature, the App shows
a Google Map and looks up nearby sauna/bath facility candidates through Google
Maps / Google Places. This sends that session's end-location coordinates to
Google so it can load the map and fetch the nearby places. Google's handling of
that data is governed by Google's own privacy policy
(https://policies.google.com/privacy); the developer receives nothing. Your
past-visited venues used in venue suggestions are read from the local session
files on your device and are not sent to the developer.

### 3. Where your data is stored

- **On your devices:** Session and heart-rate data are stored locally on your
  Pixel Watch and your Android phone as JSON files.
- **Watch → phone transfer:** When the devices are paired, finished sessions are
  sent from the watch to the phone over the Wearable Data Layer, and watch
  settings sync bidirectionally between the two. This is a direct device-to-device
  transfer; there is **no developer-side cloud account and no login to the
  developer**. Only you have access to the data on your devices. The developer
  cannot.
- **Cloud sync (optional):** If you turn on Cloud sync, a snapshot of your
  sessions is stored in **your own** Google Drive's app-private ("App Data")
  folder, under your Google account. The developer operates no server and stores
  nothing; the data lives in your Drive, not with the developer, and the
  developer has no access to it (see Section 6).
- **Health Connect (optional):** If you connect Health Connect, the data read
  from and written to Health Connect stays on your device under Health Connect's
  own controls. It is not copied to the developer or any cloud of the App.

### 4. Heart-rate data

The App reads heart-rate samples from the watch's optical sensor (via Wear OS
Health Services) only while a session is running, to power its features:
session history, heart-rate charts, and recovery analytics such as the Afterglow
Score and HRR (heart-rate recovery at 1/3/5 minutes after the sauna peak).

- Heart-rate data is **never used for advertising**.
- Heart-rate data is **never sold or shared** with the developer or any third
  party.
- Heart-rate data is processed on your devices and kept in local files. It is
  never sent to Google AdMob.
- If you connect Health Connect, the App **writes** each session's heart-rate
  record to Health Connect on your device (see Section 5). This is a local,
  on-device exchange governed by Health Connect; it is not sent to the developer.

### 5. Health Connect (optional)

Health Connect is **optional** and off until you connect it in **Settings →
Health Connect**. If you do not connect it, the App works exactly as before,
with no health-data integration. When you connect it, you grant each permission
explicitly through the system Health Connect screen, and you can change or revoke
those permissions at any time in Health Connect or in **Settings → Health
Connect**.

With your permission, the App:

- **Reads your Resting heart rate** and shows it as a reference line on the
  session heart-rate chart.
- **Reads your Sleep and average Respiratory rate** for the night *after* a
  session and shows them in a "Next-day status" section (Sleep is shown as a
  reference "Sleep score").
- **Writes each session to Health Connect** as an exercise record plus a
  heart-rate record, so other apps you choose can use your sessions.

**This data flows only between the App and Health Connect on your device.** It is
governed entirely by your Health Connect permissions and stays on your device.
**It is never sent to the developer**, never used for advertising, and never sold
or shared with any third party. Health Connect data is not transmitted to any
server operated by the developer or to any cloud of the App.

### 6. Cloud sync (optional)

Cloud sync is **optional** and **off until you sign in / tap Sync**. You turn it
on in **Settings → Cloud sync (Google Drive)** by tapping **"Sync with Google
Drive"**. It is **free**. If you never use it, your data stays on your devices
(Watch ↔ Phone over the Wearable Data Layer) exactly as before, with no cloud
involved.

When you turn it on, you sign in with Google and grant the **`drive.appdata`**
permission. With that permission, the App stores and retrieves a snapshot of
your sessions in your Google Drive's **app-private ("App Data") folder** — a
hidden area of your Drive reserved for this app. Sync is **two-way**: it merges
sessions between your device and your Drive, so you can **back up your sessions
and move them between devices**.

**Crucially, this snapshot goes to *your own* Google Drive, under your own Google
account — not to the developer.** The developer still operates **no server** and
**stores nothing**. The `drive.appdata` scope only lets the App see this app's
own App Data folder; it does not give the App (or the developer) access to the
rest of your Drive, and **the developer cannot access your synced data**.

You stay in control:

- **Delete the synced data** at any time from your own Google Drive (the App Data
  / hidden app data of your Drive).
- **Revoke the app's access** at any time in your **Google Account → Security →
  Third-party access** permissions, or from **Settings** in the App.

### 7. Permissions

The App requests only the permissions it needs:

- **Body Sensors (watch):** required to read your real heart rate from the
  watch's optical sensor during a session. If you deny it, the App falls back to
  demo/mock heart-rate data.
- **Body Sensors – background (watch):** allows the heart-rate sensor to keep
  reading during a session while the foreground service runs, so the timer and
  heart rate keep going during the session.
- **Notifications (watch):** used to show the ongoing notification for the
  foreground service that keeps a session recording while the session screen is
  on. The notification simply indicates that a session is in progress.
- **Location (watch, optional):** used only to capture your approximate location
  once at the end of a session, so you can tag the session venue and see it on
  the map. There is no continuous GPS tracking and no
  past-visit history. If you deny it, the App works normally without a venue
  location.
- **Health Connect (optional):** used only if you connect Health Connect, to
  read Resting heart rate, Sleep, and Respiratory rate, and to write exercise
  and heart-rate records (see Section 5). Each permission is granted explicitly
  and can be revoked at any time.
- **Google sign-in + Google Drive `drive.appdata` (optional):** used only if you
  turn on Cloud sync, to store and retrieve a snapshot of your sessions in your
  own Google Drive's app-private folder (see Section 6). It is limited to this
  app's own App Data folder and can be revoked at any time.
- **Internet (phone):** used by the phone app for maps, ads, optional Cloud sync,
  and Google Play Billing.

### 8. Advertising (free version)

The free version of the App shows banner ads through **Google AdMob**. AdMob is
a third-party service operated by Google and may collect device information, an
advertising identifier, and ad-interaction data to deliver and measure ads, in
accordance with Google's policies.

- On Android, the advertising identifier is governed by the system's
  **advertising-ID controls**. You can reset or delete the advertising ID in
  **Settings → Privacy → Ads** (the exact path varies by device/Android
  version); if you do, you still see ads, but they are non-personalized.
- In the EEA, UK, and Switzerland, the App shows a **consent form (Google UMP)**
  before serving ads, as required by GDPR.
- Google's handling of advertising data is governed by Google's own privacy
  policy: https://policies.google.com/privacy
- The **Premium version shows no ads**, and the App does not request tracking or
  ad consent from Premium users.

### 9. Other Google services (diagnostics)

The App is built on Google Play Services and may include Firebase components.
These may collect standard diagnostic and crash logs as part of their normal,
transparent operation, governed by Google's privacy policy
(https://policies.google.com/privacy). This is not used to identify you to the
developer, and your sauna/heart-rate data is not included.

### 10. Purchases

Premium is an auto-renewing subscription sold through **Google Play Billing**.
Payments are processed by Google; the App never sees your payment details. You
can see the price, manage, or cancel the subscription in Google Play under
Subscriptions.

### 11. Your rights (GDPR, EU DSA, and similar laws)

Because the developer holds none of your personal data, there is no developer-
side database to access, correct, or delete. You remain in full control:

- **Delete your data:** Delete sessions in the App, or uninstall the App from
  your watch and phone. Uninstalling removes the local data files on that device.
  Records the App wrote to Health Connect can be deleted in Health Connect.
- **Delete your cloud backup (if you used Cloud sync):** Remove the synced
  snapshot from your own Google Drive's app-private ("App Data") folder, and/or
  revoke the App's access in your Google Account → Security → Third-party access
  (or from Settings in the App). Because the developer holds nothing, there is no
  developer-side copy to delete.
- **Export your data:** You can export your session data as CSV files from
  Settings → Data import/export.
- **Withdraw ad consent:** Adjust the advertising-ID setting in Android Settings
  → Privacy → Ads, or use the in-app consent options where shown.
- **Manage Health Connect:** Revoke the App's Health Connect permissions at any
  time in Health Connect or in Settings → Health Connect.

For requests or questions, contact the developer at the address above.

### 12. Children

The App is a sauna tool intended for general audiences and is not directed at
children. It does not knowingly collect data from children.

### 13. Data retention

Data is retained in local files on your devices until you delete it (by deleting
sessions or uninstalling). If you used Cloud sync, the synced snapshot stays in
your own Google Drive's app-private folder until you delete it there or revoke
the App's access. Any records written to Health Connect remain there until you
delete them in Health Connect. The developer retains nothing.

### 14. Changes

This Privacy Policy may be updated. Material changes will be reflected on this
page with a new effective date.

### 15. Contact

Questions about this Privacy Policy: maxsaunatimer@gmail.com

---

## 日本語

### 1. 概要

MaxRecover Timer（以下「本アプリ」）は、サウナセッションを計測し心拍ベースの
データを記録する Pixel Watch（Wear OS）/ Android スマートフォン用アプリです。
本ポリシーは、本アプリが扱うデータとその取扱いを説明します。

**開発者はサーバーを一切運用しておらず、利用者の個人データを収集・受領・保管
しません。** セッションデータ・心拍データ・位置情報は利用者の端末（ウォッチと
スマートフォン）内にローカルファイルとして留まります。開発者側のクラウド
アカウントや開発者へのログインはありません。ウォッチとスマートフォンを
ペアリングしている場合、終了したセッションは Wearable Data Layer（Bluetooth /
Wi-Fi）を通じてウォッチからスマートフォンへ直接転送され、開発者やアプリの
クラウドを経由することはありません。開発者はこれらにアクセスできません。

**クラウド同期は任意で、保存先は利用者自身の Google Drive のみです。** オンに
する場合は、**設定 → クラウド同期（Google Drive） → 「Google Drive と同期」**
から行います。これにより本アプリは、利用者の Google アカウント配下にある
**利用者自身の** Google Drive のアプリ専用（「アプリデータ」）フォルダに
セッションのスナップショットを保存します。**無料**です。開発者は引き続き
サーバーを運用せず、何も保持しません——データは開発者ではなく利用者自身の
Drive に保存され、開発者はアクセスできません。クラウド同期は、**サインインまたは
同期をタップするまでオフ**です。利用しない場合、データは従来どおり利用者の
端末内に留まります。詳細は第 6 条をご覧ください。

**Health Connect** を接続した場合は、利用者の明示的な許可のもとで、本アプリが
Health Connect を通じて端末上の一部の健康データを読み書きできます。これらは
端末内に留まり、**開発者に送信されることはありません**。詳細は第 5 条をご覧
ください。

### 2. 本アプリが扱うデータ

| 種別 | 例 | 目的 |
|---|---|---|
| 心拍データ | セッション中にウォッチの光学センサーからリアルタイムで読み取る心拍サンプル | セッション履歴・心拍チャート・回復分析・「ととのい度」の表示 |
| 位置情報 | セッション終了時に一度だけ取得するおおよその位置（緯度・経度。位置情報を許可した場合のみ） | セッションの場所として参考用に保存し、地図／近隣施設の選択（約 500 m 以内の過去に訪れた施設を含む）に使用 |
| セッションデータ | セッション時刻・フェーズ・算出スコア・選択した施設・1〜5 の星評価 | アプリの中核機能 |
| Health Connect データ（任意） | Health Connect から**読み取る**安静時心拍数・睡眠・呼吸数、Health Connect へ**書き込む**運動＋心拍レコード（接続した場合のみ） | 安静時心拍の基準線、翌日の睡眠スコア／呼吸数の参考表示、他アプリでのセッション利用 |
| クラウド同期データ（任意） | クラウド同期をオンにした場合のみ、**利用者自身の** Google Drive のアプリ専用フォルダに保存されるセッションのスナップショット | セッションのバックアップと端末間の移行 |
| 広告データ | Google AdMob が収集する端末情報・広告操作情報（無料版のみ） | バナー広告の表示 |

本アプリにアカウント登録・ログインはありません。氏名やメールアドレスを求める
こともありません。任意で入力できる短いエクスポート名ラベルは端末内にのみ
保存されます。

本アプリは、セッション中にウォッチの光学センサーから **心拍をリアルタイムで**
（Wear OS Health Services 経由で）読み取ります。**Health Connect は任意**で、
接続した場合に限り、本アプリは Health Connect を通じて特定のデータを読み書き
します（第 5 条参照）。本アプリは、Health Connect を通じて利用者が許可した
場合を除き、他アプリの健康データにアクセスすることはありません。

セッションの地図／施設機能を開くと、本アプリは Google マップを
表示し、Google マップ／Google プレイス を通じて近隣のサウナ・入浴施設の候補を
検索します。これにより該当セッションの終了位置の座標が Google に送信され、
地図の読み込みと近隣施設の取得に使われます。この座標の Google による取扱いは
Google のプライバシーポリシー（https://policies.google.com/privacy）に従います。
開発者は何も受け取りません。施設候補に使う過去に訪れた施設は、端末内の
ローカルセッションファイルから読み出すもので、開発者に送信されることはありません。

### 3. データの保存場所

- **端末内:** セッションデータ・心拍データは Pixel Watch と Android スマート
  フォン内に JSON ファイルとしてローカル保存されます。
- **ウォッチ→スマートフォンへの転送:** ペアリングしている場合、終了した
  セッションは Wearable Data Layer を通じてウォッチからスマートフォンへ送信
  され、ウォッチ設定は双方向に同期されます。これは端末間の直接転送であり、
  **開発者側のクラウドアカウントや開発者へのログインはありません**。
  端末内のデータにアクセスできるのは利用者本人のみで、開発者はアクセスでき
  ません。
- **クラウド同期（任意）:** クラウド同期をオンにした場合、セッションの
  スナップショットが、利用者の Google アカウント配下にある **利用者自身の**
  Google Drive のアプリ専用（「アプリデータ」）フォルダに保存されます。開発者は
  サーバーを運用せず何も保持しません。データは開発者ではなく利用者自身の
  Drive に保存され、開発者はアクセスできません（第 6 条参照）。
- **Health Connect（任意）:** Health Connect を接続した場合、Health Connect
  から読み取ったデータや書き込んだデータは、Health Connect 自身の管理のもとで
  端末内に留まります。開発者やアプリのクラウドにコピーされることはありません。

### 4. 心拍データ

本アプリは、セッション実行中のみ、ウォッチの光学センサーから（Wear OS Health
Services 経由で）心拍サンプルを読み取り、機能を提供します：セッション履歴、
心拍チャート、ととのい度や HRR（サウナのピーク後 1/3/5 分の心拍回復）などの
回復分析。

- 心拍データを**広告に使用することはありません**。
- 心拍データを開発者や第三者に**販売・共有することはありません**。
- 心拍データは端末内で処理され、ローカルファイルに保持されます。Google AdMob
  に送信されることはありません。
- Health Connect を接続した場合、本アプリは各セッションの心拍レコードを端末上の
  Health Connect に**書き込みます**（第 5 条参照）。これは Health Connect が
  管理する端末内・ローカルのやり取りであり、開発者に送信されることはありません。

### 5. Health Connect（任意）

Health Connect は**任意**で、**設定 → Health Connect** で接続するまでは無効
です。接続しない場合、本アプリは従来どおり動作し、健康データの連携は一切あり
ません。接続する際は、システムの Health Connect 画面で各権限を明示的に許可
します。権限はいつでも Health Connect または **設定 → Health Connect** から
変更・取り消しできます。

利用者の許可のもとで、本アプリは以下を行います。

- **安静時心拍数を読み取り**、セッションの心拍チャートに基準線として表示します。
- セッション*後*の夜について、**睡眠と平均呼吸数を読み取り**、「翌日のコンディ
  ション」セクションに表示します（睡眠は参考の「睡眠スコア」として表示）。
- 各セッションを運動レコードと心拍レコードとして **Health Connect に書き込み**、
  利用者が選んだ他アプリでセッションを利用できるようにします。

**これらのデータは、端末上の本アプリと Health Connect の間でのみやり取りされ
ます。** すべて利用者の Health Connect 権限によって管理され、端末内に留まり
ます。**開発者に送信されることはなく**、広告に使用されることも、第三者に販売・
共有されることもありません。Health Connect データが開発者の運用するサーバーや
アプリのクラウドに送信されることはありません。

### 6. クラウド同期（任意）

クラウド同期は**任意**で、**サインインまたは同期をタップするまでオフ**です。
**設定 → クラウド同期（Google Drive）** で **「Google Drive と同期」** を
タップしてオンにします。**無料**です。利用しない場合、データは従来どおり利用者の
端末内（ウォッチ ↔ スマートフォンの Wearable Data Layer）に留まり、クラウドは
一切関与しません。

オンにする際は、Google でサインインし、**`drive.appdata`** 権限を許可します。
この権限により、本アプリは利用者の Google Drive の**アプリ専用（「アプリデータ」）
フォルダ**——本アプリ用に確保された Drive 内の隠しフォルダ——にセッションの
スナップショットを保存・取得します。同期は**双方向**で、端末と Drive の間で
セッションを統合（マージ）するため、**セッションのバックアップと端末間の移行**が
できます。

**重要な点として、このスナップショットは開発者ではなく、利用者自身の Google
アカウント配下にある利用者自身の Google Drive に保存されます。** 開発者は
引き続き**サーバーを運用せず**、**何も保持しません**。`drive.appdata` の権限は
本アプリ自身のアプリデータフォルダのみを対象とし、Drive の他の部分へのアクセス
権を本アプリ（や開発者）に与えるものではありません。**開発者は同期データに
アクセスできません**。

利用者が管理権を持ちます。

- **同期データの削除:** 利用者自身の Google Drive（Drive のアプリデータ／隠し
  アプリデータ）から、いつでも削除できます。
- **アプリのアクセス権の取り消し:** **Google アカウント → セキュリティ →
  サードパーティによるアクセス** の権限、またはアプリの**設定**から、いつでも
  取り消せます。

### 7. 権限について

本アプリは必要な権限のみを要求します。

- **ボディーセンサー（ウォッチ）:** セッション中にウォッチの光学センサーから
  実際の心拍を読み取るために必要です。拒否した場合はデモ／モックの心拍データに
  フォールバックします。
- **ボディーセンサー（バックグラウンド・ウォッチ）:** フォアグラウンド
  サービスの実行中もセッション中の心拍センサーの読み取りを継続し、セッション中
  にタイマーと心拍を動かし続けるために使用します。
- **通知（ウォッチ）:** セッション画面が表示されている間、セッションを記録し
  続けるフォアグラウンドサービスの常駐通知を表示するために使用します。この通知
  はセッションが進行中であることを示すだけのものです。
- **位置情報（ウォッチ・任意）:** セッション終了時に一度だけおおよその位置を
  取得し、施設の記録や地図表示に使うためだけに利用します。
  連続的な GPS トラッキングや過去の来訪履歴はありません。拒否しても、施設の
  位置なしで通常どおり動作します。
- **Health Connect（任意）:** Health Connect を接続した場合のみ、安静時心拍数・
  睡眠・呼吸数の読み取りと、運動・心拍レコードの書き込みに使用します（第 5 条
  参照）。各権限は明示的に許可するもので、いつでも取り消せます。
- **Google サインイン＋Google Drive `drive.appdata`（任意）:** クラウド同期を
  オンにした場合のみ、利用者自身の Google Drive のアプリ専用フォルダに
  セッションのスナップショットを保存・取得するために使用します（第 6 条参照）。
  本アプリ自身のアプリデータフォルダに限定され、いつでも取り消せます。
- **インターネット（スマートフォン）:** スマートフォン側アプリが地図・広告・
  任意のクラウド同期・Google Play Billing のために利用します。

### 8. 広告（無料版）

無料版は **Google AdMob** を通じてバナー広告を表示します。AdMob は Google が
運営する第三者サービスで、Google のポリシーに従い、広告の配信・計測のため
端末情報・広告識別子・広告操作データを収集する場合があります。

- Android では広告識別子はシステムの **広告 ID 設定** により管理されます。
  **設定 → プライバシー → 広告** で広告 ID をリセット／削除できます（正確な
  経路は端末や Android バージョンにより異なります）。リセットしても広告は
  表示されますが、その場合は非パーソナライズ広告になります。
- EEA・英国・スイスでは、GDPR の要請に従い、広告配信前に **同意フォーム
  （Google UMP）** を表示します。
- 広告データの Google による取扱いは Google のプライバシーポリシーに従います:
  https://policies.google.com/privacy
- **Premium 版では広告は表示されず**、Premium 利用者にトラッキングや広告同意
  を求めることもありません。

### 9. その他の Google サービス（診断）

本アプリは Google Play Services 上で動作し、Firebase コンポーネントを含む場合
があります。これらは通常かつ透明な動作の一環として、標準的な診断ログや
クラッシュログを収集する場合があり、Google のプライバシーポリシー
（https://policies.google.com/privacy）に従います。これは利用者を開発者に
対して特定するためのものではなく、サウナ／心拍データは含まれません。

### 10. 課金

Premium は **Google Play Billing** で販売される自動更新サブスクリプションです。
決済は Google が処理し、本アプリが決済情報を見ることはありません。価格の確認・
管理・解約は、Google Play の「定期購入」から行えます。

### 11. 利用者の権利（GDPR・EU DSA 等）

開発者は利用者の個人データを一切保持していないため、開発者側に閲覧・訂正・
削除すべきデータベースは存在しません。利用者が完全に管理権を持ちます。

- **データの削除:** アプリ内でセッションを削除する、またはウォッチと
  スマートフォンからアプリをアンインストールします。アンインストールすると、
  その端末上のローカルデータファイルが削除されます。本アプリが Health Connect
  に書き込んだレコードは Health Connect 内で削除できます。
- **クラウドバックアップの削除（クラウド同期を利用した場合）:** 利用者自身の
  Google Drive のアプリ専用（「アプリデータ」）フォルダから同期スナップショットを
  削除する、かつ／または Google アカウント → セキュリティ → サードパーティに
  よるアクセス（もしくはアプリの設定）から本アプリのアクセス権を取り消します。
  開発者は何も保持していないため、開発者側に削除すべきコピーは存在しません。
- **データのエクスポート:** 設定 → データ入出力 から、セッションデータを
  CSV で書き出せます。
- **広告同意の撤回:** Android の設定 → プライバシー → 広告 で広告 ID 設定を
  変更するか、アプリ内の同意オプションを利用してください。
- **Health Connect の管理:** 本アプリの Health Connect 権限は、Health Connect
  または 設定 → Health Connect からいつでも取り消せます。

ご要望・ご質問は上記の連絡先までお問い合わせください。

### 12. 子どもについて

本アプリは一般利用者向けのサウナ用ツールであり、子どもを対象としていません。
子どものデータを意図的に収集することはありません。

### 13. データの保持期間

データは、利用者が削除する（セッションの削除またはアンインストール）まで、
端末内のローカルファイルに保持されます。クラウド同期を利用した場合、同期
スナップショットは、利用者が利用者自身の Google Drive のアプリ専用フォルダで
削除するか本アプリのアクセス権を取り消すまで、そこに保持されます。Health
Connect に書き込まれたレコードは、利用者が Health Connect 内で削除するまで
そこに保持されます。開発者は何も保持しません。

### 14. 変更

本ポリシーは更新されることがあります。重要な変更はこのページに新しい施行日
とともに反映されます。

### 15. お問い合わせ

本ポリシーに関するお問い合わせ: maxsaunatimer@gmail.com

---

## 関連 / See also

- [User Guide / 取扱説明書](guide.html)
- [FAQ / よくある質問](faq.html)
- [Privacy Policy / プライバシーポリシー](privacy-policy.html)
- [Terms of Use / 利用規約](terms-of-use.html)
