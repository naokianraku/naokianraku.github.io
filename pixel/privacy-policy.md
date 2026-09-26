---
title: Privacy Policy (Pixel Watch & Android)
---

# Privacy Policy / プライバシーポリシー — MaxRecovery Timer for Pixel Watch & Android

**Last updated / 最終更新:** (set on release / 公開時に設定)
**Effective date / 施行日:** (set on Google Play release / Google Play 公開日に設定)
**Developer / 開発者:** Anraku Tech (Naoki Anraku / 安樂直樹, an individual developer / 個人開発者)
**Contact / 連絡先:** maxsaunatimer@gmail.com

---

## English

### 1. Overview

MaxRecovery Timer ("the App", formerly MaxSauna Timer) is a Pixel Watch (Wear OS)
and Android phone app that times hot-bath and sauna sessions and records
heart-rate-based data. This Privacy Policy
explains what data the App handles and how.

**The developer does not operate any server and does not collect, receive, or
store your personal data.** Your session data, heart-rate data, and location
data stay on your devices (your watch and your phone) as local files. The App
has no developer-side cloud account and no login to the developer. When your
watch and phone are paired, finished sessions are transferred directly from the
watch to the phone over the Wearable Data Layer (Bluetooth/Wi-Fi); they are not
routed through the developer or any cloud of the App. The developer has no
access to your data. (If Android's backup is turned on for your devices, Android
may also back up a copy of the App's data to your Google Account — see Section 3.)

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
| Heart-rate data | Heart-rate samples read live from the watch's optical sensor during a session (none for a session recorded without heart rate — see Section 4) | Show session history, heart-rate charts, recovery analytics, and the "Afterglow Score" |
| Location data | Precise location (latitude/longitude) captured at the end of each session, only if you grant Location (approximate if you choose "Approximate" in the system dialog) | Saved with each session as the venue location, and used to show that session's map, the Venue Map of all your sessions' locations, and your past-visited venues within about 500 m; sent to Google to load the maps, and for a nearby-venue search only when you tap "Find nearby venues" |
| Session data | Session times, phases, computed scores, the venue name you enter, a 1–5 star rating, the reason heart rate was unavailable (if it was), and — only when something went wrong during recording — a short technical note (for example, that the heart-rate sensor stopped or the app restarted) | Core app functionality and troubleshooting recording problems |
| Health Connect data (optional) | Resting heart rate, Sleep, and Respiratory rate **read** from Health Connect; exercise + heart-rate records **written** to Health Connect — only if you connect it | Show a resting-HR reference line, a next-day Sleep score / respiratory-rate reference, and let other apps use your sessions |
| Cloud sync data (optional) | A snapshot of your sessions, plus a list of deleted sessions (session IDs and deletion times only), stored in **your own** Google Drive's app-private folder, only if you turn on Cloud sync | Back up your sessions, move them between your devices, and keep deleted sessions from coming back |
| Deletion records | Session IDs and deletion times of the sessions you deleted, kept on your phone (no heart-rate, location or venue data) | Keep deleted sessions from coming back from the watch or from Cloud sync |
| Advertising data | Device information, the advertising ID, ad-interaction information, the IP address (from which Google may estimate an approximate location), and your ad-consent choices, handled by Google AdMob and Google's User Messaging Platform (only without Premium, except the consent check described in Section 8) | Show banner ads and manage ad consent |

The App has no account or login. It does not ask for your name or email. A short
export-name label you may optionally enter is stored only on your device.

The App reads heart rate **live from the watch's optical sensor** via Wear OS
Health Services during a session. **Health Connect is optional** and, only when
you connect it, the App reads and writes specific data through it (see Section
5). The App does not access any other apps' health data except through Health
Connect with your permission.

When you open the session map / venue feature, the App shows a Google Map of
that session's end location, which sends those coordinates to Google so it can
load the map. The App looks up nearby sauna/bath facility suggestions through
Google Maps / Google Places **only when you tap "Find nearby venues"** (up to 5
searches a day per device); it never searches automatically. Each search sends
that session's end-location coordinates (the device location recorded when the
session ended) to Google so it can fetch the nearby places. Google's handling of
that data is governed by Google's own privacy policy
(https://policies.google.com/privacy); the developer receives nothing.

The suggestions are shown for reference only. They are kept only in the phone's
memory for up to 30 minutes and are **never saved** — not in your session files,
backups, Cloud sync, CSV, PDF, or Health Connect. **The only venue names the App
saves are the ones you type in yourself** (or bring in with CSV import). Your
past-visited venues within about 500 m, shown before any search, are those
names read from the local session files on your device; showing them does not
search Google, and they are not sent to the developer.

### 3. Where your data is stored

- **On your devices:** Session and heart-rate data are stored locally on your
  Pixel Watch and your Android phone as JSON files.
- **Watch → phone transfer:** When the devices are paired, finished sessions are
  sent from the watch to the phone over the Wearable Data Layer, and watch
  settings sync bidirectionally between the two. The watch keeps each finished
  session until the phone confirms it was received, then removes it from its send
  queue (the watch's own history keeps the latest 20 sessions). This is a direct
  device-to-device transfer; there is **no developer-side cloud account and no
  login to the developer**. Only you have access to the data on your devices. The
  developer cannot.
- **Unreadable files:** If a history file on the phone can't be read, the App sets
  it aside on the phone instead of overwriting it, so you can export it (for example
  to attach it when contacting support). It stays on the device until you clear the
  App's storage or uninstall it.
- **Android backup (by Google):** The phone app allows Android's automatic backup.
  If backup to your Google Account is turned on in your phone's settings, Android may
  back up a copy of the App's data (such as your session history, deletion records
  and settings) to your Google Account, and restore it when you reinstall the App or
  set up a new phone with the same account. This means your sessions may come back
  after you uninstall and reinstall the App. The watch app's data may likewise be
  included in the watch's backup (except a session in progress). This backup is
  handled by Google under your Google Account and is separate from the App's
  optional Cloud sync; the developer cannot access it. You can turn backup on or off
  in your device's settings (the exact path varies by device / Android version).
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
- If you connect Health Connect and export your sessions, the App **writes**
  each session's heart-rate record to Health Connect on your device (see
  Section 5). This is a local, on-device exchange governed by Health Connect; it
  is not sent to the developer.
- The watch reads heart rate through Wear OS Health Services' workout feature,
  requesting heart rate only (no GPS).

**Sessions without heart rate.** If heart rate can't be read — for example, the Heart
rate permission is not granted, the watch has no heart-rate sensor, or no readings
arrive — the App keeps timing without heart rate and shows "Heart rate
unavailable" on the watch. It never substitutes demo or estimated values. The
session is saved with its times and phases, marked as recorded without heart rate,
and, if known, the reason (for example, "heart rate permission off"). Such
sessions are stored, transferred and synced like other sessions, are not used to
calculate scores, and are exported to Health Connect as exercise only.

### 5. Health Connect (optional)

Health Connect is **optional** and off until you connect it in **Settings →
Health Connect**. If you do not connect it, the App works exactly as before,
with no health-data integration. When you connect it, you grant each permission
explicitly through the system Health Connect screen, and you can change or revoke
those permissions at any time in Health Connect (your device's system settings
on Android 14 and later, or the Health Connect app on earlier versions).

With your permission, the App:

- **Reads your Resting heart rate** and shows it as a reference line on the
  session heart-rate chart.
- **Reads your Sleep and average Respiratory rate** for the night *after* a
  session and shows them in a "Next-day status" section (Sleep is shown as a
  reference "Sleep score").
- **Writes your sessions to Health Connect** as an exercise record plus a
  heart-rate record, so other apps you choose can use your sessions. This
  happens only when you tap **Settings → Health Connect → "Export sessions to
  Health Connect"**; sessions are not written automatically. Each record carries
  an identifier for its session, so exporting again replaces the earlier records
  instead of duplicating them. The exercise record is named after the venue name
  you entered, or "MaxRecovery" if there is none (records exported by earlier
  versions may be named "Sauna"). "Clean up duplicates from earlier exports"
  deletes records this App exported earlier for the sessions on your phone and
  exports them again; it never deletes other apps' data.

**This data flows only between the App and Health Connect on your device.** It is
governed entirely by your Health Connect permissions and stays on your device.
**It is never sent to the developer**, never used for advertising, never shared
with Google AdMob or any other advertising network, and never sold or shared with
any third party. Health Connect data is not transmitted to any server operated by
the developer or to any cloud of the App. The privacy screen that Health Connect
opens for this App shows this policy.

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
and move them between devices**. Syncing runs only when you tap the sync button.

The folder also holds a list of the sessions you deleted (session IDs and deletion
times only), so that a deletion reaches your other synced devices and deleted
sessions don't come back. If the cloud data can't be fetched or read, or if saving
would reduce the number of sessions in the cloud, the App stops without changing
the cloud data.

**Crucially, this snapshot goes to *your own* Google Drive, under your own Google
account — not to the developer.** The developer still operates **no server** and
**stores nothing**. The `drive.appdata` scope only lets the App see this app's
own App Data folder; it does not give the App (or the developer) access to the
rest of your Drive, and **the developer cannot access your synced data**.

You stay in control:

- **Delete the synced data** at any time from your own Google Drive (the App Data
  / hidden app data of your Drive).
- **Revoke the app's access** at any time in your **Google Account → Security →
  Your connections to third-party apps & services**
  (https://myaccount.google.com/connections): select the app and delete its
  connection. (It may be listed under its former name, "MaxSauna Timer".) The
  App itself has no disconnect setting.

The App's use of information received from Google APIs adheres to the Google API
Services User Data Policy (https://developers.google.com/terms/api-services-user-data-policy),
including the Limited Use requirements. Data from Google Drive is used only to
provide Cloud sync to you; it is never transferred to the developer or others,
never used for advertising, and never read by humans.

### 7. Permissions

The App requests only the permissions it needs. On the watch, the permissions
below are explained on a "Before you start" screen and requested when you first
start a session, not at app launch.

- **Heart rate (watch):** required to read your real heart rate from the watch's
  optical sensor during a session. The watch shows this permission as "Heart rate",
  or as "Sensors" on earlier watch software (Android's `BODY_SENSORS` permission). If
  you deny it, the App keeps timing without heart rate and shows "Heart rate
  unavailable"; it does not use substitute data (see Section 4). The App does not
  request background access for it; heart rate is read only while a session is
  running in the foreground service.
- **Notifications (watch):** used to show the ongoing notification and the
  ongoing-activity icon on the watch face for the foreground service that keeps a
  session recording. The notification simply indicates that a session is in
  progress and shows its current phase.
- **Location (watch, optional):** asked only once. Used only to capture your
  location once at the end of each session (precise location, unless you choose "Approximate" in
  the system dialog). The location is saved with that session, so you can tag
  the session venue, see it on the session map and the Venue Map, get
  suggestions from your past-visited venues, and search for nearby venues when
  you tap "Find nearby venues". Because each session keeps its
  location, your session history shows where each session took place until you
  delete that session. There is no continuous GPS tracking; the location is
  read only when a session ends. If you deny it, the App works normally without
  a venue location.
- **Health Connect (optional):** used only if you connect Health Connect, to
  read Resting heart rate, Sleep, and Respiratory rate, and to write exercise
  and heart-rate records (see Section 5). Each permission is granted explicitly
  and can be revoked at any time.
- **Google sign-in + Google Drive `drive.appdata` (optional):** used only if you
  turn on Cloud sync, to store and retrieve a snapshot of your sessions in your
  own Google Drive's app-private folder (see Section 6). It is limited to this
  app's own App Data folder and can be revoked at any time.
- **Internet (phone):** used by the phone app for maps, nearby-venue search (only
  when you tap it), ads and ad consent, optional Cloud sync, and Google Play
  Billing.

### 8. Advertising (without Premium)

Without a Premium subscription, the App shows banner ads through **Google AdMob**.
AdMob is a third-party service operated by Google and may collect device
information, an advertising identifier, and ad-interaction data to deliver and
measure ads, in accordance with Google's policies.

- AdMob also receives your IP address, which Google may use to estimate the
  approximate location of your device for ad delivery. The App itself never
  shares the venue location it records with AdMob.
- **Heart-rate data, Health Connect data, and the locations and venue names the
  App records are never used for advertising** and are never shared with AdMob or
  any other advertising network.
- **Ad consent (Google User Messaging Platform):** each time the App starts, it
  uses Google's User Messaging Platform (UMP) to check whether ad consent or an
  opt-out choice is required where you are (Google determines this, for example
  from your IP address). Ads are requested only when UMP allows it.
  - In the **EEA, the UK and Switzerland**, a consent form is shown before ads are
    loaded, as required by the GDPR and similar laws. If you do not consent, Google
    may still show limited, non-personalized ads where permitted.
  - In **US states with applicable privacy laws**, you can opt out of the sale or
    sharing of your personal information for targeted advertising.
  - You can review or change your choices at any time in **Settings → Help &
    legal → "Ad privacy settings"**. This item is shown only where such a choice is
    required (it normally does not appear in Japan, where no consent form is shown).
- On Android, the advertising identifier is governed by the system's
  **advertising-ID controls**. You can reset or delete the advertising ID in
  **Settings → Privacy → Ads** (the exact path varies by device/Android
  version); if you do, you still see ads, but they are non-personalized.
- Google's handling of advertising data is governed by Google's own privacy
  policy: https://policies.google.com/privacy
- **With Premium, no ads are shown**: the App does not show the consent form or
  start the Mobile Ads SDK. It still checks with UMP (as above) so that "Ad privacy
  settings" can be offered where required.

### 9. Other Google services (diagnostics)

The App is built on Google Play Services and may include Firebase components.
These may collect standard diagnostic and crash logs as part of their normal,
transparent operation, governed by Google's privacy policy
(https://policies.google.com/privacy). This is not used to identify you to the
developer, and your sauna/heart-rate data is not included.

### 10. Purchases

Premium is an auto-renewing subscription (monthly or yearly plans, with a free
period for first-time subscribers where offered) sold through **Google Play
Billing**. Payments are processed by Google; the App never sees your payment
details. The App receives only the status of your subscription from Google Play
(for example, whether it is active or on hold) to turn Premium features on or off,
and keeps that status on your phone. You can see the price, manage, or cancel the
subscription in Google Play under Subscriptions.

### 11. Your rights (GDPR, EU DSA, US state privacy laws, and similar laws)

Because the developer holds none of your personal data, there is no developer-
side database to access, correct, or delete. You remain in full control:

- **Delete your data:** Delete sessions in the App, or uninstall the App from
  your watch and phone. Uninstalling removes the local data files on that device
  (if Android's backup is on, a backed-up copy may be restored when you reinstall
  the App — see Section 3; you can delete restored sessions in the App).
  If you use Cloud sync, sessions you delete in the App are also removed from your
  Drive and your other synced devices at the next sync. Records the App wrote to
  Health Connect can be deleted in Health Connect. See also the
  [data deletion page](data-deletion.html).
- **Delete your cloud backup (if you used Cloud sync):** Remove the synced
  snapshot from your own Google Drive's app-private ("App Data") folder, and/or
  revoke the App's access in your Google Account → Security → Your connections
  to third-party apps & services (see Section 6). Because the developer holds
  nothing, there is no developer-side copy to delete.
- **Export your data:** You can export your session data as CSV files from
  Settings → Data import/export (CSV) (a Premium feature).
- **Limit ad personalization:** Reset or delete the advertising ID in Android
  Settings → Privacy → Ads.
- **Change your ad consent or opt out:** Use Settings → Help & legal → "Ad privacy
  settings" (shown where required; see Section 8).
- **Manage Health Connect:** Revoke the App's Health Connect permissions at any
  time in Health Connect (your device's system settings on Android 14 and
  later, or the Health Connect app on earlier versions).

For requests or questions, contact the developer at the address above.

### 12. Children

The App is a wellness timer intended for general audiences and is not directed
at children. It does not knowingly collect data from children.

### 13. Data retention

Data is retained in local files on your devices until you delete it (by deleting
sessions or uninstalling). The watch keeps its latest 20 sessions, plus any
finished sessions the phone has not yet confirmed receiving. Deletion records
(session IDs and deletion times) stay on your phone until you clear the App's
storage or uninstall it. If you used Cloud sync, the synced snapshot and deletion
list stay in your own Google Drive's app-private folder until you delete them there
or revoke the App's access. Any records written to Health Connect remain there until
you delete them in Health Connect. If Android's backup is on, a copy of the App's data
may also be kept in your Google Account's backup, as managed by Google (see Section 3).
The developer retains nothing.

### 14. Changes

This Privacy Policy may be updated. Material changes will be reflected on this
page with a new effective date.

### 15. Contact

Questions about this Privacy Policy: maxsaunatimer@gmail.com

---

## 日本語

### 1. 概要

MaxRecovery Timer（以下「本アプリ」。旧名 MaxSauna Timer）は、温浴・サウナの
セッションを計測し心拍ベースのデータを記録する Pixel Watch（Wear OS）/ Android
スマートフォン用アプリです。
本ポリシーは、本アプリが扱うデータとその取扱いを説明します。

**開発者はサーバーを一切運用しておらず、利用者の個人データを収集・受領・保管
しません。** セッションデータ・心拍データ・位置情報は利用者の端末（ウォッチと
スマートフォン）内にローカルファイルとして留まります。開発者側のクラウド
アカウントや開発者へのログインはありません。ウォッチとスマートフォンを
ペアリングしている場合、終了したセッションは Wearable Data Layer（Bluetooth /
Wi-Fi）を通じてウォッチからスマートフォンへ直接転送され、開発者やアプリの
クラウドを経由することはありません。開発者はこれらにアクセスできません。
（端末で Android のバックアップがオンになっている場合は、Android が本アプリの
データのコピーを利用者の Google アカウントにバックアップすることもあります。
第 3 条参照）

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
| 心拍データ | セッション中にウォッチの光学センサーからリアルタイムで読み取る心拍サンプル（心拍なしで記録したセッションには含まれません。第 4 条参照） | セッション履歴・心拍チャート・回復分析・「ととのい度」の表示 |
| 位置情報 | 各セッションの終了時に取得する正確な位置（緯度・経度。位置情報を許可した場合のみ。システムの許可画面で「おおよその位置」を選んだ場合はおおよその位置） | 各セッションの場所として保存し、そのセッションの地図、全セッションの場所を示す施設マップ、約 500 m 以内の過去に訪れた施設の表示に使用。地図の読み込みのため Google に送信するほか、近隣施設の検索のためには「近くの施設を探す」をタップしたときだけ Google に送信 |
| セッションデータ | セッション時刻・フェーズ・算出スコア・入力した施設名・1〜5 の星評価・心拍を取得できなかった理由（該当する場合）、および記録中に問題があったときだけ付く短い技術的なメモ（心拍センサーが止まった、アプリが再起動した など） | アプリの中核機能と、記録の不具合の調査 |
| Health Connect データ（任意） | Health Connect から**読み取る**安静時心拍数・睡眠・呼吸数、Health Connect へ**書き込む**運動＋心拍レコード（接続した場合のみ） | 安静時心拍の基準線、翌日の睡眠スコア／呼吸数の参考表示、他アプリでのセッション利用 |
| クラウド同期データ（任意） | クラウド同期をオンにした場合のみ、**利用者自身の** Google Drive のアプリ専用フォルダに保存されるセッションのスナップショットと、削除したセッションの一覧（セッション ID と削除した時刻のみ） | セッションのバックアップと端末間の移行、削除したセッションが戻らないようにするため |
| 削除の記録 | 利用者が削除したセッションの ID と削除した時刻（心拍・位置・施設名は含みません）。スマートフォン内に保持 | 削除したセッションがウォッチやクラウド同期から戻らないようにするため |
| 広告データ | Google AdMob と Google のユーザー向けメッセージ プラットフォーム（UMP）が扱う端末情報・広告 ID・広告操作情報・IP アドレス（Google がおおよその位置を推定する場合があります）・広告の同意の選択（Premium 未加入時のみ。第 8 条の同意の確認を除く） | バナー広告の表示と広告の同意の管理 |

本アプリにアカウント登録・ログインはありません。氏名やメールアドレスを求める
こともありません。任意で入力できる短いエクスポート名ラベルは端末内にのみ
保存されます。

本アプリは、セッション中にウォッチの光学センサーから **心拍をリアルタイムで**
（Wear OS Health Services 経由で）読み取ります。**Health Connect は任意**で、
接続した場合に限り、本アプリは Health Connect を通じて特定のデータを読み書き
します（第 5 条参照）。本アプリは、Health Connect を通じて利用者が許可した
場合を除き、他アプリの健康データにアクセスすることはありません。

セッションの地図／施設機能を開くと、本アプリは該当セッションの終了位置の
Google マップを表示します。地図の読み込みのため、その座標が Google に送信され
ます。近隣のサウナ・入浴施設の候補は、**「近くの施設を探す」をタップしたとき
だけ**（1 台につき 1 日 5 回まで）、Google マップ／Google プレイス を通じて検索
します。自動で検索することはありません。検索のたびに、該当セッションの終了位置
（セッション終了時に端末が取得した位置）の座標が Google に送信され、近隣施設の
取得に使われます。この座標の Google による取扱いは Google のプライバシー
ポリシー（https://policies.google.com/privacy）に従います。開発者は何も受け
取りません。

検索で表示される候補は参考表示です。スマートフォンのメモリ上に最長 30 分保持
するだけで、**保存はしません**（セッションファイル・バックアップ・クラウド同期・
CSV・PDF・Health Connect のいずれにも残りません）。**本アプリが保存する施設名は、
利用者が自分で入力したもの**（と CSV で取り込んだもの）**だけ**です。検索の前に
表示する約 500 m 以内の過去に訪れた施設は、端末内のローカルセッションファイル
から読み出したこれらの施設名です。表示のために Google を検索することはなく、
開発者に送信されることもありません。

### 3. データの保存場所

- **端末内:** セッションデータ・心拍データは Pixel Watch と Android スマート
  フォン内に JSON ファイルとしてローカル保存されます。
- **ウォッチ→スマートフォンへの転送:** ペアリングしている場合、終了した
  セッションは Wearable Data Layer を通じてウォッチからスマートフォンへ送信
  され、ウォッチ設定は双方向に同期されます。ウォッチは、スマートフォンが受け
  取ったことを確認するまで終了したセッションを保持し、確認後に送信待ちから
  外します（ウォッチ自身の履歴には直近 20 件を保持します）。これは端末間の
  直接転送であり、**開発者側のクラウドアカウントや開発者へのログインはありま
  せん**。端末内のデータにアクセスできるのは利用者本人のみで、開発者はアクセス
  できません。
- **読めなかったファイル:** スマートフォンの履歴ファイルを読めなかった場合、
  本アプリは上書きせずに端末内に退避し、利用者が書き出せるようにします（お問い
  合わせの際の添付など）。退避したファイルは、アプリのストレージを消去するか
  アンインストールするまで端末内に残ります。
- **Android のバックアップ（Google による）:** スマートフォン側アプリは、Android の
  自動バックアップを許可しています。スマートフォンの設定で Google アカウントへの
  バックアップがオンになっている場合、Android が本アプリのデータ（セッションの履歴、
  削除の記録、設定など）のコピーを利用者の Google アカウントにバックアップし、
  同じアカウントで本アプリを再インストールしたときや、新しいスマートフォンを
  設定したときに復元することがあります。そのため、アンインストールしたあとに
  再インストールすると、記録が戻ることがあります。ウォッチ側アプリのデータも、
  ウォッチのバックアップの対象になることがあります（計測中の下書きを除きます）。
  このバックアップは、利用者の Google アカウントのもとで Google が扱うもので、
  本アプリのクラウド同期とは別であり、開発者はアクセスできません。バックアップの
  オン・オフは、端末の設定で変更できます（正確な経路は端末や Android の
  バージョンにより異なります）。
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
- Health Connect を接続してセッションを書き出した場合、本アプリは各セッションの
  心拍レコードを端末上の Health Connect に**書き込みます**（第 5 条参照）。
  これは Health Connect が管理する端末内・ローカルのやり取りであり、開発者に
  送信されることはありません。
- ウォッチは Wear OS Health Services のワークアウト機能で心拍を読み取ります。
  要求するのは心拍だけで、GPS は使いません。

**心拍なしのセッション：** 心拍を読み取れない場合（心拍数の権限がない、
ウォッチに心拍センサーがない、心拍が届かない など）、本アプリは心拍なしで計時を
続け、ウォッチに「心拍を取得できません」と表示します。デモや推定の値で置き換える
ことはありません。そのセッションは時刻とフェーズとともに、心拍なしで記録した旨と、
分かる場合はその理由（例：「心拍数の権限なし」）を付けて保存されます。
こうしたセッションは他のセッションと同じように保存・転送・同期されますが、スコアの
計算には使わず、Health Connect には運動の記録だけを書き出します。

### 5. Health Connect（任意）

Health Connect は**任意**で、**設定 → Health Connect** で接続するまでは無効
です。接続しない場合、本アプリは従来どおり動作し、健康データの連携は一切あり
ません。接続する際は、システムの Health Connect 画面で各権限を明示的に許可
します。権限はいつでも Health Connect（Android 14 以降は端末のシステム設定、
それより前は Health Connect アプリ）から変更・取り消しできます。

利用者の許可のもとで、本アプリは以下を行います。

- **安静時心拍数を読み取り**、セッションの心拍チャートに基準線として表示します。
- セッション*後*の夜について、**睡眠と平均呼吸数を読み取り**、
  「翌日のコンディション」セクションに表示します（睡眠は参考の「睡眠スコア」として
  表示）。
- セッションを運動レコードと心拍レコードとして **Health Connect に書き込み**、
  利用者が選んだ他アプリでセッションを利用できるようにします。書き込みは
  **設定 → Health Connect →「セッションを Health Connect に書き出し」** を
  タップしたときだけ行い、自動では書き込みません。各レコードにはセッションごとの
  識別子を付けるため、書き出し直すと以前のレコードが置き換わり、重複しません。
  運動レコードの名前は、利用者が入力した施設名（無い場合は「MaxRecovery」）です
  （以前のバージョンで書き出したレコードは「Sauna」の場合があります）。
  「以前の書き出しの重複を整理」は、スマートフォンにあるセッションについて、本
  アプリが以前書き出したレコードを削除してから書き出し直すもので、他アプリの
  データを削除することはありません。

**これらのデータは、端末上の本アプリと Health Connect の間でのみやり取りされ
ます。** すべて利用者の Health Connect 権限によって管理され、端末内に留まり
ます。**開発者に送信されることはなく**、広告に使用されることも、Google AdMob を
はじめとする広告ネットワークに渡すことも、第三者に販売・共有されることもあり
ません。Health Connect データが開発者の運用するサーバーやアプリのクラウドに送信
されることはありません。Health Connect が本アプリ向けに開くプライバシーの画面
には、本ポリシーが表示されます。

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
できます。同期は、利用者が同期のボタンをタップしたときだけ行います。

このフォルダには、削除したセッションの一覧（セッション ID と削除した時刻のみ）も
保存します。削除を同期しているほかの端末に伝え、削除したセッションが戻らない
ようにするためです。クラウドのデータを取得・読み取りできない場合や、保存すると
クラウドの記録が減る場合は、クラウドのデータを変更せずに同期を中止します。

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
  サードパーティ製のアプリとサービスとの接続**
  （https://myaccount.google.com/connections）で本アプリを選び、接続を削除
  すれば、いつでも取り消せます（一覧には旧名の「MaxSauna Timer」と表示される
  場合があります）。アプリ内に接続を解除する設定はありません。

本アプリによる Google API から受け取った情報の利用は、Limited Use（利用制限）の
要件を含む Google API サービスのユーザーデータに関するポリシー
（https://developers.google.com/terms/api-services-user-data-policy）に準拠します。
Google Drive のデータは、利用者にクラウド同期を提供するためだけに使い、開発者や
第三者に移転することも、広告に使うことも、人が読むこともありません。

### 7. 権限について

本アプリは必要な権限のみを要求します。ウォッチでは、以下の権限をアプリの起動時
ではなく、最初にセッションを始めるときに「計測の前に」画面で説明してから求めます。

- **心拍数（ウォッチ）:** セッション中にウォッチの光学センサーから実際の心拍を
  読み取るために必要です。ウォッチには、この権限が「心拍数」として表示されます
  （以前の版のウォッチでは、センサーの権限として表示されます。Android の権限名は
  `BODY_SENSORS`）。拒否した場合は、心拍なしで計時を続け、「心拍を取得できません」と
  表示します。代わりのデータは使いません（第 4 条参照）。この権限をバックグラウンドで
  使うことは求めず、心拍はフォアグラウンドサービスでセッションを実行している間だけ
  読み取ります。
- **通知（ウォッチ）:** セッションを記録し続けるフォアグラウンドサービスの常駐
  通知と、文字盤の進行中のアイコンを表示するために使用します。この通知は
  セッションが進行中であることと、今のフェーズを示すだけのものです。
- **位置情報（ウォッチ・任意）:** 尋ねるのは一度だけです。各セッションの終了時に
  一度だけ位置を取得するためだけに利用します（システムの許可画面で「おおよその位置」を選ばない限り
  正確な位置）。取得した位置はそのセッションに保存され、施設の記録、セッションの
  地図と施設マップの表示、過去に訪れた施設の候補表示、「近くの施設を探す」を
  タップしたときの近隣施設の検索に使います。各セッションが
  位置を保持するため、セッションを削除するまでは、履歴から各セッションを行った
  場所が分かります。連続的な GPS トラッキングは行わず、位置を読み取るのは
  セッション終了時だけです。拒否しても、施設の位置なしで通常どおり動作します。
- **Health Connect（任意）:** Health Connect を接続した場合のみ、安静時心拍数・
  睡眠・呼吸数の読み取りと、運動・心拍レコードの書き込みに使用します（第 5 条
  参照）。各権限は明示的に許可するもので、いつでも取り消せます。
- **Google サインイン＋Google Drive `drive.appdata`（任意）:** クラウド同期を
  オンにした場合のみ、利用者自身の Google Drive のアプリ専用フォルダに
  セッションのスナップショットを保存・取得するために使用します（第 6 条参照）。
  本アプリ自身のアプリデータフォルダに限定され、いつでも取り消せます。
- **インターネット（スマートフォン）:** スマートフォン側アプリが地図・近隣施設の
  検索（タップしたときのみ）・広告と広告の同意・任意のクラウド同期・Google Play
  Billing のために利用します。

### 8. 広告（Premium 未加入時）

Premium 未加入時は、**Google AdMob** を通じてバナー広告を表示します。AdMob は
Google が運営する第三者サービスで、Google のポリシーに従い、広告の配信・計測の
ため端末情報・広告識別子・広告操作データを収集する場合があります。

- AdMob には IP アドレスも送信され、Google が広告配信のために端末のおおよその
  位置を推定することがあります。本アプリが記録する施設の位置情報を AdMob に
  渡すことはありません。
- **心拍データ・Health Connect のデータ・本アプリが記録する位置や施設名を広告に
  使うことはなく**、AdMob をはじめとする広告ネットワークに渡すこともありません。
- **広告の同意（Google のユーザー向けメッセージ プラットフォーム）:** 本アプリは
  起動のたびに、Google のユーザー向けメッセージ プラットフォーム（UMP）を使って、
  利用者のいる地域で広告の同意やオプトアウトの選択が必要かを確認します（判定は
  Google が IP アドレスなどから行います）。広告は、UMP が許可した場合にだけ
  リクエストします。
  - **EEA・英国・スイス** では、GDPR などの要請に従い、広告を読み込む前に同意
    フォームを表示します。同意しない場合も、法令で認められる範囲で、制限された
    非パーソナライズ広告が表示されることがあります。
  - プライバシー法が適用される **米国の州** では、ターゲティング広告のための個人
    情報の販売・共有をオプトアウトできます。
  - 選択は **設定 → ヘルプ・規約 →「広告のプライバシー設定」** からいつでも確認・
    変更できます。この項目は、選択が必要な地域でだけ表示されます（同意フォームを
    表示しない日本では、通常表示されません）。
- Android では広告識別子はシステムの **広告 ID 設定** により管理されます。
  **設定 → プライバシー → 広告** で広告 ID をリセット／削除できます（正確な
  経路は端末や Android バージョンにより異なります）。リセットしても広告は
  表示されますが、その場合は非パーソナライズ広告になります。
- 広告データの Google による取扱いは Google のプライバシーポリシーに従います:
  https://policies.google.com/privacy
- **Premium では広告は表示されません**。同意フォームの表示や Mobile Ads SDK の
  起動も行いません。ただし、必要な地域で「広告のプライバシー設定」を表示できる
  よう、上記の UMP による確認は行います。

### 9. その他の Google サービス（診断）

本アプリは Google Play Services 上で動作し、Firebase コンポーネントを含む場合
があります。これらは通常かつ透明な動作の一環として、標準的な診断ログや
クラッシュログを収集する場合があり、Google のプライバシーポリシー
（https://policies.google.com/privacy）に従います。これは利用者を開発者に
対して特定するためのものではなく、サウナ／心拍データは含まれません。

### 10. 課金

Premium は **Google Play Billing** で販売される自動更新サブスクリプション
（月額プラン・年額プラン。提供している場合は、初めて登録する方向けの無料期間
あり）です。決済は Google が処理し、本アプリが決済情報を見ることはありません。
本アプリが Google Play から受け取るのは定期購入の状態（有効か、一時停止中か など）
だけで、Premium 機能の有効・無効の切り替えに使い、その状態をスマートフォン内に
保持します。価格の確認・管理・解約は、Google Play の「定期購入」から行えます。

### 11. 利用者の権利（GDPR・EU DSA・米国の州のプライバシー法 等）

開発者は利用者の個人データを一切保持していないため、開発者側に閲覧・訂正・
削除すべきデータベースは存在しません。利用者が完全に管理権を持ちます。

- **データの削除:** アプリ内でセッションを削除する、またはウォッチと
  スマートフォンからアプリをアンインストールします。アンインストールすると、
  その端末上のローカルデータファイルが削除されます（Android のバックアップが
  オンの場合は、再インストールしたときに、バックアップのコピーが復元されることが
  あります。第 3 条参照。復元されたセッションは、アプリ内で削除できます）。
  クラウド同期を利用している場合、アプリ内で削除したセッションは、次の同期で Drive と同期しているほかの
  端末からも削除されます。本アプリが Health Connect に書き込んだレコードは
  Health Connect 内で削除できます。[データの削除](data-deletion.html)の
  ページもご覧ください。
- **クラウドバックアップの削除（クラウド同期を利用した場合）:** 利用者自身の
  Google Drive のアプリ専用（「アプリデータ」）フォルダから同期スナップショットを
  削除する、かつ／または Google アカウント → セキュリティ → サードパーティ製の
  アプリとサービスとの接続 から本アプリのアクセス権を取り消します（第 6 条参照）。
  開発者は何も保持していないため、開発者側に削除すべきコピーは存在しません。
- **データのエクスポート:** 設定 → データ入出力（CSV） から、セッションデータを
  CSV で書き出せます（Premium 機能）。
- **広告のパーソナライズの制限:** Android の設定 → プライバシー → 広告 で
  広告 ID をリセット／削除できます。
- **広告の同意の変更・オプトアウト:** 設定 → ヘルプ・規約 →
  「広告のプライバシー設定」（必要な地域でのみ表示。第 8 条参照）から行えます。
- **Health Connect の管理:** 本アプリの Health Connect 権限は、Health Connect
  （Android 14 以降は端末のシステム設定、それより前は Health Connect アプリ）
  からいつでも取り消せます。

ご要望・ご質問は上記の連絡先までお問い合わせください。

### 12. 子どもについて

本アプリは一般利用者向けのウェルネス用タイマーであり、子どもを対象としていません。
子どものデータを意図的に収集することはありません。

### 13. データの保持期間

データは、利用者が削除する（セッションの削除またはアンインストール）まで、
端末内のローカルファイルに保持されます。ウォッチは直近 20 件のセッションと、
スマートフォンの受信確認がまだの終了したセッションを保持します。削除の記録
（セッション ID と削除した時刻）は、アプリのストレージを消去するかアンインス
トールするまでスマートフォン内に保持されます。クラウド同期を利用した場合、同期
スナップショットと削除の一覧は、利用者が利用者自身の Google Drive のアプリ専用
フォルダで削除するか本アプリのアクセス権を取り消すまで、そこに保持されます。
Health Connect に書き込まれたレコードは、利用者が Health Connect 内で削除する
までそこに保持されます。Android のバックアップがオンの場合は、本アプリのデータの
コピーが、Google の管理のもとで、利用者の Google アカウントのバックアップにも
保持されることがあります（第 3 条参照）。開発者は何も保持しません。

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
