---
title: Delete your data (Pixel Watch & Android)
---

# Delete your data / データの削除 — MaxRecovery Timer for Pixel Watch & Android

**App / アプリ:** MaxRecovery Timer (Pixel Watch & Android; formerly MaxSauna Timer / 旧名 MaxSauna Timer)
**Developer / 開発者:** Anraku Tech (Naoki Anraku / 安樂直樹)
**Contact / 連絡先:** anraku.tech@gmail.com
**Last updated / 最終更新:** (set on release / 公開時に設定)

---

## English

The developer has no server and no user accounts, and **does not receive or keep
any of your data**. Your data lives on your own devices and, only if you turn on
cloud sync, in your own Google Drive. You can delete all of it yourself, at any
time, with the steps below. You do not need to contact us, but you can email
anraku.tech@gmail.com if you need help.

### 1. Data on your phone (sessions, heart rate, venue names, settings)
- **One session:** History tab → swipe the session to the left → tap the trash
  icon.
- **All sessions:** Settings → Data → "Delete all received data".
- If you use cloud sync, sessions deleted in these two ways are also removed from
  your Google Drive and your other synced devices the next time each of them
  syncs (devices must run the latest version of the app).
- After you delete sessions, the app keeps only their session IDs and deletion
  times (no heart rate, location or venue names) so that deleted sessions don't
  come back from the watch or from cloud sync.
- **Everything:** Android Settings → Apps → the app → Storage → Clear storage,
  or uninstall the app. Uninstalling removes all of the app's data on the phone,
  including the deletion records above and any set-aside (unreadable) history
  files.
- **Android backup:** if Android's automatic backup ("Backup by Google One") is
  on, the app's data may also be in your device backup and can come back when
  you reinstall the app. To remove it, delete the sessions in the app after
  reinstalling, or delete the device backup in Google Drive → Storage →
  Backups (or Google One → Storage). The developer cannot see or access this
  backup.

### 2. Data on your Pixel Watch (up to the latest 20 sessions, sessions not yet received by the phone, settings, an in-progress draft)
- Watch Settings → Apps → the app → Clear storage, or uninstall the app from
  the watch.

### 3. Cloud backup in your Google Drive (only if you used "Sync with Google Drive")
- The backup (your sessions and the list of deleted sessions) is stored in the
  app's hidden folder in **your** Google Drive.
  Open Google Drive on the web → Settings (gear icon) → Manage apps → the app →
  Options → **Delete hidden app data**.
- To also remove the app's access to your Drive: Google Account → Security →
  Your connections to third-party apps & services
  (https://myaccount.google.com/connections) → the app → delete the connection.

### 4. Data you exported to Health Connect (only if you used the export)
- Open Health Connect (Android 14 and later: system Settings → Security & privacy
  → Privacy → Health Connect; earlier versions: the Health Connect app) →
  App permissions → the app → Delete app data.

### 5. Files you exported yourself
- CSV files, PDF reports, saved graph images and exported set-aside history files
  are ordinary files on your device (e.g. Downloads, Pictures/MaxRecoveryTimer, and
  Pictures/MaxSaunaTimer for images saved with earlier versions). Delete them with
  your file manager or Photos app.

### What is deleted and what is kept
- The steps above delete the data **immediately and permanently** on the device
  or in your Drive. Nothing is kept by the developer, because the developer never
  receives it.
- Data processed by Google services the app uses (Google Mobile Ads without
  Premium, Google's ad-consent service (UMP), Google Maps / Places for maps and
  nearby-venue search)
  is handled by Google under the Google Privacy Policy
  (https://policies.google.com/privacy). You can reset or delete your advertising
  ID in Android Settings → Privacy → Ads, and, where shown, change your ad consent
  in the app's Settings → Help & legal → "Ad privacy settings".

---

## 日本語

開発者はサーバーもユーザーアカウントも持っておらず、**皆さまのデータを受け取ったり
保管したりしていません**。データはお使いの端末と、クラウド同期を有効にした場合に限り
ご自身の Google ドライブにだけ保存されます。以下の手順で、いつでもご自身ですべて
削除できます。開発者への連絡は不要ですが、お困りの場合は anraku.tech@gmail.com
までご連絡ください。

### 1. スマホのデータ（セッション・心拍・施設名・設定）
- **1 件ずつ:** 履歴タブ → セッションを左にスワイプ → ゴミ箱アイコンをタップ。
- **すべてのセッション:** 設定 → データ →「全受信データを削除」。
- クラウド同期を使っている場合、この 2 つの方法で削除したセッションは、それぞれの
  端末が次に同期したときに、ご自身の Google ドライブと同期しているほかの端末からも
  削除されます（各端末のアプリを最新版にしてください）。
- セッションを削除すると、削除したセッションがウォッチやクラウド同期から戻らない
  よう、そのセッションの ID と削除した時刻だけを記録します（心拍・位置・施設名は
  含みません）。
- **すべて:** Android の設定 → アプリ → 本アプリ → ストレージ → ストレージを消去、
  またはアプリをアンインストール。アンインストールすると、上記の削除の記録や、
  退避した（読めなかった）履歴ファイルを含め、スマホ上の本アプリのデータはすべて
  削除されます。
- **Android のバックアップ:** Android の自動バックアップ（「Google One バックアップ」）
  が有効な場合、本アプリのデータが端末のバックアップにも含まれ、再インストール時に
  戻ることがあります。不要な場合は、再インストール後にアプリ内で削除するか、
  Google ドライブ → 保存容量 → バックアップ（または Google One → 保存容量）から
  端末のバックアップを削除してください。開発者はこのバックアップを見ることも、
  取り出すこともできません。

### 2. Pixel Watch のデータ（直近 20 件までのセッション・スマホに未転送のセッション・設定・計測中の下書き）
- ウォッチの設定 → アプリ → 本アプリ → ストレージを消去、またはウォッチから
  アプリをアンインストール。

### 3. Google ドライブのクラウドバックアップ（「Google Drive と同期」を使った場合のみ）
- バックアップ（セッションと、削除したセッションの一覧）は**ご自身の** Google
  ドライブ内の、本アプリ専用の非表示フォルダにあります。ウェブ版 Google ドライブ → 設定（歯車）→ アプリの管理 → 本アプリ →
  オプション →「**アプリの隠しデータを削除**」。
- ドライブへのアクセス権も取り消す場合: Google アカウント → セキュリティ →
  サードパーティ製のアプリとサービスとの接続
  （https://myaccount.google.com/connections）→ 本アプリ → 接続を削除。

### 4. Health Connect に書き出したデータ（書き出しを使った場合のみ）
- Health Connect を開く（Android 14 以降: 設定 → セキュリティとプライバシー →
  プライバシー → Health Connect、それ以前: Health Connect アプリ）→ アプリの権限 →
  本アプリ → アプリのデータを削除。

### 5. ご自身で書き出したファイル
- 書き出した CSV・PDF レポート・保存したグラフ画像・書き出した退避ファイルは、
  端末上の通常のファイル（ダウンロード、Pictures/MaxRecoveryTimer、旧版で保存した
  画像は Pictures/MaxSaunaTimer など）です。ファイル管理アプリやフォトアプリで
  削除してください。

### 削除されるデータと保持されるデータ
- 上記の手順で、端末上またはドライブ上のデータは**直ちに完全に**削除されます。
  開発者はデータを受け取っていないため、開発者側に保持されるデータはありません。
- 本アプリが利用する Google のサービス（Premium 未加入時の Google モバイル広告、
  広告の同意の確認（UMP）、地図と近くの施設の検索に使う Google Maps / Places）で処理される
  データは、Google のプライバシーポリシー（https://policies.google.com/privacy）に
  従って Google が取り扱います。広告 ID は Android の設定 → プライバシー → 広告
  からリセット・削除でき、表示されている場合は本アプリの 設定 → ヘルプ・規約 →
  「広告のプライバシー設定」から広告の同意を変更できます。
