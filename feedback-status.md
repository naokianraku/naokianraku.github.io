---
title: 対応状況 / Fixed issues — MaxRecovery Timer
---

# 対応状況 — MaxRecovery Timer

**最終更新:** 2026-09-27（9/26 に v0.1.7／Phone v0.2.0 を配信）

テスターの皆さまからいただいた不具合のご報告・ご要望と、その対応内容です。ご協力ありがとうございます！

> 🐛 新しいご報告はこちら → **[フィードバックフォーム](feedback.html)**

## Pixel Watch / Android

### ⚠️ ご注意

**手首を返すと「セッション終了？」が出ることがある（2026年9月の Pixel Watch アップデート）**
- 状態：⚠️ v0.1.7 までの注意点（今後の版で対応予定）
- 内容：2026年9月の Pixel Watch のアップデートで、手首をひねる（返す）動作がシステムの「戻る」になりました。v0.1.7 までは、計測中にこの動作をすると「セッション終了？」の確認が出ることがあります。**5秒で自動的に取り消され、記録は続きます。** 今後の版で、計測中はこの動作に反応しないようにする予定です。（F-022「手首をひねると意図せず次フェーズへ進む」とは別の現象です）

### 🔎 調査中

**F-026 2セット目以降の記録が途切れ、同じ頃に「計測中」の通知が消えた（重大）**
- 状態：🔎 調査中（v0.1.7 で対策の第1段を配信）
- 内容：2セット目以降の心拍・フェーズの記録が途切れ、同じ頃に「計測中」の通知も消えていた、とのご報告です（画面のタイマーは動いていました）。原因はまだ特定できていません。
- 対策（v0.1.7）：
  - 計測中の前面サービス（「計測中」の通知を出して計測を続けるための仕組み）を、画面の作り直し（文字サイズの変更など）で止めないようにしました。
  - 心拍が届かないときは、画面に「心拍を取得できません」と出るようにしました（止まった数字を出し続けません）。
  - 異常があったときの診断メモを、記録に残すようにしました。
- 次の版：計測を画面から完全に切り離す対策を準備中です。
- お願い：同じ症状が出たら、[フィードバックフォーム](feedback.html)で次の点を教えてください。
  - ウォッチの機種とアプリの版
  - 何セット目で、どんな操作をしたか（画面を手で覆った・文字盤に戻った など）
  - 「計測中」の通知が消えた時刻

### ✅ 修正・配信済み

**F-001 セッション中にクラウン（リューズ）が反応しない**
- 状態：✅ 修正・配信済み（v0.1.1）
- 対策：クラウンの回転操作が画面に正しく届くよう修正し、ウォッチ用の表示ライブラリを更新しました。回転による「次へ／一時停止」が確実に効くようになりました。

**F-002 / F-006 セッションが多重起動する／離脱・通知から戻ると操作できなくなる**
- 状態：✅ 修正・配信済み（v0.1.1〜0.1.3）
- 対策：アプリの起動を常に1つに限定し、通知やホームから戻ったときは実行中のセッション画面に復帰するようにしました。二重起動や「操作できなくなる」状態が起きません。

**F-003 セッション中の右スワイプでセッションが終了してしまう**
- 状態：✅ 修正・配信済み（v0.1.3）
- 対策：計測中はセッション画面を独立した全画面表示にし、右スワイプ（戻る）で終了しないようにしました。戻る操作をした場合は「終了しますか？」の確認を表示します。

**F-004 一時停止からの再開操作の分離（改善要望）**
- 状態：✅ 対応・配信済み（v0.1.3）
- 対策：「クラウンを上に回す＝再開（一時停止中）／次へ（通常時）」「下に回す＝一時停止のみ」に分離し、回しすぎによる誤再開を防ぎました。

**F-005 サウナの設定時間あたりでフェーズが勝手に進むことがある**
- 状態：✅ 修正・配信済み（v0.1.4）
- 対策：クラウンの誤反応が原因でした。フェーズ移行に必要な回転量を大きくし（約2倍）、ごく小さな回転が時間とともに溜まって誤作動するのをリセットするようにして、意図的に回したときだけ進むよう調整しました。

**F-007 準備フェーズ中にクラウンを回しても反応しない（サウナに進めない）**
- 状態：✅ 修正・配信済み（v0.1.4）
- 対策：セッション開始直後に画面が操作対象を受け取り切れず、クラウン入力を取りこぼすことがありました。受け取りを確実化し、各フェーズの切り替え時にも取り直すようにしました。

**F-008 クラウンの回転量を設定で調整できるように（要望）**
- 状態：✅ 追加・配信済み（v0.1.4）
- 内容：フェーズ移行に必要なクラウンの回転量を「少なめ／標準／多め／最多」から選べるようにしました（不意の接触による誤操作を防げます）。設定 → ウォッチ設定。

**F-010 1つ前のフェーズに戻れるように（要望）**
- 状態：✅ 追加・配信済み（v0.1.4）→ v0.1.7 で修正（下の「F-010 / F-015 訂正とお詫び」）
- 内容：誤って進めてしまったとき、1つ前のフェーズに戻せる機能です。v0.1.7 からは、一時停止中に画面の「戻る」→確認で戻ります（画面長押しでの操作は v0.1.5 で廃止）。

**F-011 本体ダブルタップで次へ（実験・要望）**
- 状態：✅ 実験的に追加・配信済み（v0.1.4／既定OFF）
- 内容：手がふさがる場面向けに、本体を2回トントンと叩くと次のフェーズへ進む実験機能を追加しました（加速度センサーで判定）。設定 → ウォッチ設定でON。誤検知することがあるため既定OFFで、合わない場合はOFFにしてください。

**F-009 「休憩」フェーズの追加（要望）**
- 状態：✅ 配信済み（v0.1.4／名称選択も追加）
- 内容：設定 → ウォッチ設定 →「その他フェーズを使う」をONにすると、外気浴のあとに第4フェーズが入り、名称を「休憩／お風呂／給水／シャワー／ストレッチ」から選べます（名称選択を今回追加）。取説に案内を追記しました。

**F-020 / F-021 画面を覆う・放置でセッションが消える／データが残らない（重大）**
- 状態：✅ 対策実装・配信済み（v0.1.5）
- 対策：計測中のセッションを自動保存し、画面を覆って消灯・アプリが終了しても、起動し直すと**セッションを復元してデータを失わない**ようにしました（画面オフでの完全な継続記録は引き続き改良中）。

**F-016 操作方法の見直し：濡れ・水しぶきによる誤操作の防止（重要）**
- 状態：✅ 実装・配信済み（v0.1.5）
- 内容：**計測中は画面タッチに反応しません（クラウンのみ）**。上＝次へ／下＝一時停止。**一時停止中だけ**画面に「再開／戻る／終了」のメニューが出ます。「操作ボタンを表示」をONにすると実行中も 次へ／停止 をタッチできます。（F-010「1つ前に戻る」は長押し→一時停止メニューに変更。実際に戻れるのは v0.1.7 から＝下の「F-010 / F-015 訂正とお詫び」）

**F-015 フェーズを戻したとき経過時間を引き継ぐ**
- 状態：✅ 実装・配信済み（v0.1.5）→ 実際に使えるのは v0.1.7 から（下の「F-010 / F-015 訂正とお詫び」）
- 内容：1つ前のフェーズに戻ると、タイマーが0でなく**戻り先の経過時間から続く**ようにしました。

**F-011 本体ダブルタップの感度を改善**
- 状態：✅ 改善・配信済み（v0.1.5）
- 内容：「効かない」とのご報告を受け、検知感度を上げました（実験機能・既定OFF）。

**F-019 履歴の削除をスワイプ→ゴミ箱方式に（Phone）**
- 状態：✅ 実装・配信済み（Phone v0.1.11）
- 内容：履歴を左スワイプするとゴミ箱ボタンが現れ、タップで削除（全画面の確認ダイアログは廃止）。

**F-014 詳細データに「欠測（データ欠損）」を表示（Phone）**
- 状態：✅ 追加・配信済み（Phone v0.1.11）
- 内容：心拍の欠測の回数・合計時間・割合を「詳細データ」に表示します。

**F-017 ウォッチで設定できる項目をPhoneでも全て設定可能に（Phone）**
- 状態：✅ 追加・配信済み（Phone v0.1.11）
- 内容：セット毎の各フェーズ時間・閾値1/2もPhoneの「ウォッチ設定」で編集できるようにしました。

**F-022 手首をひねると意図せず次フェーズへ進む**
- 状態：✅ 修正・配信済み（v0.1.6）
- 対策：実験機能「本体ダブルタップで次へ」が、手首をひねる動きを誤ってダブルタップと判定していました。ジャイロ（回転）センサーを併用し、**手首をひねっている間はタップ判定を無視**するようにし、検知のしきい値も上げました。

**F-023 防水ロック中にクラウンも効かない**
- 状態：✅ 取説/FAQで案内
- 内容：Wear OS の「水ロック」は**クラウンを回して解除する**仕様のため、ロック中はクラウン操作もできません。セッション中はアプリが既に画面タッチを無視するので、**水ロックは使わずクラウンで操作**してください（取説・FAQに追記）。

**F-024 セッション中画面に現在時刻を表示**
- 状態：✅ 追加・配信済み（v0.1.6）
- 内容：セッション中の画面上部に現在時刻を常時表示します。

**F-025 セッション中画面に最大・最小心拍を表示**
- 状態：✅ 追加・配信済み（v0.1.6）
- 内容：セッション開始からの最大・最小心拍を表示します（「全」がセッション全体、「↓↑」が直近5分）。

**F-010 / F-015 訂正とお詫び：1つ前のフェーズに戻れなかった**
- 状態：✅ 修正・配信済み（v0.1.7）
- 内容：v0.1.6 までは、一時停止メニューに「戻る」が表示されず、1つ前のフェーズに実際には戻れない不具合がありました（そのため F-015 の経過時間の引き継ぎも使えませんでした）。「戻れる」とご案内していたのに使えない状態が続き、申し訳ありませんでした。
- 対策：v0.1.7 で修正しました。クラウンを下に回して一時停止 → 画面の「戻る」→ 確認で、1つ前のフェーズに戻ります。戻ったフェーズは経過時間を引き継ぎ、戻ったあとも**一時停止のまま**です。クラウンを上に回すと再開します。（「戻る」は、戻れるフェーズがあるときだけ表示されます）

**F-027 経過時間の小数点以下（1/10秒）を表示しない**
- 状態：✅ 対応・配信済み（v0.1.7）
- 内容：セッション画面の経過時間を「分:秒」（例 01:23）で表示し、1/10秒の桁をなくしました。

**v0.1.7 のその他の改善**
- 状態：✅ 配信済み（v0.1.7）
- 内容：
  - 心拍を取得できないときは、仮の心拍を記録せず、画面に「心拍を取得できません」と表示します。
  - 心拍（身体センサー）の権限を許可しなかったときに、アプリが落ちる問題を直しました。
  - 前回の計測が途中で止まっていたときは、「続ける／保存して終了／破棄」を選べるようにしました。
  - クラウンを1回回すと、1フェーズだけ進むようにしました（続けて進めるときは、いったん手を止めてから回してください）。
  - 丸い画面の端で文字が欠けないよう、配置を見直しました。
  - 記録と設定の保存を壊れにくくしました。

**Phone v0.2.0 の変更点**
- 状態：✅ 配信済み（Phone v0.2.0）
- 内容：
  - 最新の Android に対応しました。
  - プレミアムを購入済みでも、無料版として扱われることがある問題を直しました。
  - 施設名は、手入力した名前だけを保存するようにしました。近くの施設は「近くの施設を探す」を押したときだけ検索します（1日5回まで）。以前に保存した施設名は消去されます（アプリ内でお知らせします）。
  - 位置情報の権限を使わなくなりました。
  - Health Connect の設定から、データの使い方とプライバシーポリシーを確認できるようにしました。

---

# Fixed issues — MaxRecovery Timer (English)

**Last updated:** 2026-09-27 (v0.1.7 / Phone v0.2.0 released on 2026-09-26)

This page summarizes the bug reports & requests from testers and how each was addressed. Thank you for your help!

> 🐛 Report new issues → **[Feedback form](feedback.html)**

## Pixel Watch / Android

### ⚠️ Please note

**Turning your wrist can bring up "End session?" (September 2026 Pixel Watch update)**
- Status: ⚠️ Applies up to v0.1.7 (to be addressed in a future version)
- What: With the September 2026 Pixel Watch update, twisting (turning) your wrist became the system "Back" gesture. Up to v0.1.7, doing this during a session may bring up the "End session?" confirmation. **It cancels itself after 5 seconds and recording continues.** In a future version, the app will ignore this gesture during a session. (This is different from F-022, "Twisting the wrist unintentionally advances to the next phase".)

### 🔎 Investigating

**F-026 Recording stopped from the 2nd set onward, and the "recording" notification disappeared around the same time (serious)**
- Status: 🔎 Investigating (first round of countermeasures released in v0.1.7)
- What: A tester reported that heart-rate and phase recording stopped from the 2nd set onward, and that the "recording" notification had disappeared around the same time (the timer on screen kept running). We have not identified the cause yet.
- Countermeasures (v0.1.7):
  - The foreground service that keeps the session recording (and shows the "recording" notification) is no longer stopped when the screen is rebuilt (for example, when the font size changes).
  - When no heart rate is coming in, the screen now shows "Heart rate unavailable" (instead of keeping a frozen number).
  - When something goes wrong, a short diagnostic note is saved with the session.
- Next version: We are preparing a fix that fully separates recording from the screen.
- Request: If you see the same problem, please tell us the following via the [Feedback form](feedback.html):
  - Your watch model and the app version
  - Which set it happened in, and what you did (covered the screen with your hand, went back to the watch face, etc.)
  - The time the "recording" notification disappeared

### ✅ Fixed & released

**F-001 Crown didn't respond during a session**
- Status: ✅ Fixed & released (v0.1.1)
- Fix: Made crown rotation reach the screen reliably and updated the watch UI library, so rotating to go "Next / Pause" works consistently.

**F-002 / F-006 Duplicate sessions, or controls stopped working after leaving / returning via notification**
- Status: ✅ Fixed & released (v0.1.1–0.1.3)
- Fix: The app now always runs a single instance, and returning from a notification or the home screen brings you back to the running session — no duplicate sessions or stuck controls.

**F-003 Swiping right ended the session**
- Status: ✅ Fixed & released (v0.1.3)
- Fix: During a session the screen is shown as its own full-screen view, so swiping right (back) no longer ends it. If you do go back, an "End session?" confirmation appears.

**F-004 Separated the resume gesture (request)**
- Status: ✅ Done & released (v0.1.3)
- Fix: "Rotate crown up = resume (while paused) / next (normally)", "rotate down = pause only" — this prevents accidental resume from over-rotating.

**F-005 The phase sometimes advanced on its own near the set sauna time**
- Status: ✅ Fixed & released (v0.1.4)
- Fix: It was caused by accidental crown input. We increased the rotation needed to change phase (about 2×) and reset tiny rotations that built up over time, so the phase only advances when you turn the crown deliberately.

**F-007 The crown didn't respond during the preparation phase (couldn't move to sauna)**
- Status: ✅ Fixed & released (v0.1.4)
- Fix: Right after a session starts, the screen could miss crown input before it was ready. We made input acquisition reliable and re-acquire it on every phase change.

**F-008 Adjustable crown rotation amount (request)**
- Status: ✅ Added & released (v0.1.4)
- What: You can now choose how far to turn the crown to act — Light / Standard / More / Most — to avoid accidental triggers. Settings → Watch settings.

**F-010 Go back one phase (request)**
- Status: ✅ Added & released (v0.1.4) → fixed in v0.1.7 (see "F-010 / F-015 Correction and apology" below)
- What: If you advance by mistake, you can return to the previous phase. From v0.1.7, while paused, tap "Go back" on the screen and confirm (the long-press was removed in v0.1.5).

**F-011 Double-tap the watch body to advance (beta, request)**
- Status: ✅ Added (experimental) & released (v0.1.4 / off by default)
- What: For when your hands are occupied, a quick double-tap on the watch body advances to the next phase (detected via the accelerometer). Turn it on in Settings → Watch settings. It can misfire, so it is off by default — turn it off if it doesn't suit you.

**F-009 Add a "rest" phase (request)**
- Status: ✅ Released (v0.1.4 / name selection added)
- What: Turn on Settings → Watch settings → "Use extra phase" to insert a 4th phase after cool-down, with a selectable name (rest / hot bath / hydration / shower / stretch — name selection added in this update). We added a note to the guide.

**F-020 / F-021 Session lost / data not saved when the screen is covered or left running (serious)**
- Status: ✅ Fix implemented & released (v0.1.5)
- Fix: The running session is now auto-saved, so even if the screen is covered/off or the app is killed, relaunching restores the session and your data is not lost. (Full screen-off continuous recording is still being improved.)

**F-016 Controls revised to prevent wet/splash mis-taps (important)**
- Status: ✅ Implemented & released (v0.1.5)
- What: During a running session the screen no longer responds to touch (crown only): up = next, down = pause. Only while paused does an on-screen menu (Resume / Go back / End) appear. Turn on "Show control buttons" to also use Next/Pause by touch while running. (Go back, F-010, moved from long-press to the pause menu. It actually works from v0.1.7 — see "F-010 / F-015 Correction and apology" below.)

**F-015 Carry over elapsed time when going back a phase**
- Status: ✅ Implemented & released (v0.1.5) → actually usable from v0.1.7 (see "F-010 / F-015 Correction and apology" below)
- What: Going back one phase now resumes from that phase's previous elapsed time instead of resetting to 0.

**F-011 Improved double-tap sensitivity**
- Status: ✅ Improved & released (v0.1.5)
- What: Based on "it doesn't work" reports, we increased detection sensitivity (experimental, off by default).

**F-019 History delete is now swipe-to-reveal-trash (Phone)**
- Status: ✅ Implemented & released (Phone v0.1.11)
- What: Left-swipe a history row to reveal a trash button, then tap it to delete (the full-screen confirmation dialog was removed).

**F-014 Show "Missing data (dropouts)" in Detailed data (Phone)**
- Status: ✅ Added & released (Phone v0.1.11)
- What: The Detailed data card now shows the count / total time / percentage of heart-rate dropouts.

**F-017 Everything configurable on the watch is now also configurable on the phone (Phone)**
- Status: ✅ Added & released (Phone v0.1.11)
- What: Per-set phase durations and thresholds (1/2) can now be edited from the phone's Watch settings too.

**F-022 Twisting the wrist unintentionally advances to the next phase**
- Status: ✅ Fixed & released (v0.1.6)
- Fix: The experimental "Double-tap body to advance" was mis-reading a wrist twist as a double-tap. We now use the gyroscope to ignore taps while the wrist is rotating, and raised the detection threshold.

**F-023 Crown also locked during the system Water Lock**
- Status: ✅ Documented in the guide / FAQ
- What: Wear OS Water Lock is exited by turning the crown, so the crown is unavailable while it's on. During a session the app already ignores screen touch, so just leave Water Lock off and use the crown (added to the guide / FAQ).

**F-024 Show the current time on the session screen**
- Status: ✅ Added & released (v0.1.6)
- What: The current time is shown at the top of the session screen.

**F-025 Show session max / min heart rate on the session screen**
- Status: ✅ Added & released (v0.1.6)
- What: The session's max / min heart rate is shown ("全" = whole session, "↓↑" = last 5 minutes).

**F-010 / F-015 Correction and apology: going back one phase did not work**
- Status: ✅ Fixed & released (v0.1.7)
- What: Up to v0.1.6, "Go back" did not appear in the pause menu, so you could not actually return to the previous phase (which also meant F-015's elapsed-time carry-over could not be used). We said it was available when it wasn't — we're sorry.
- Fix: Fixed in v0.1.7. Rotate the crown down to pause → tap "Go back" on the screen → confirm, and you return to the previous phase. The phase keeps its elapsed time, and the session **stays paused** after going back. Rotate the crown up to resume. ("Go back" only appears when there is a previous phase to return to.)

**F-027 Remove the tenths of a second from the elapsed time**
- Status: ✅ Done & released (v0.1.7)
- What: The elapsed time on the session screen is now shown as minutes:seconds (e.g. 01:23), without the 1/10-second digit.

**Other improvements in v0.1.7**
- Status: ✅ Released (v0.1.7)
- What:
  - When heart rate can't be read, the app no longer records a placeholder heart rate; it shows "Heart rate unavailable" on the screen instead.
  - Fixed a crash when the heart-rate (body sensors) permission was not granted.
  - If your previous session stopped partway, you can now choose "Continue", "Save" (save and end) or "Discard".
  - One turn of the crown now advances exactly one phase (to advance again, pause your hand briefly before turning).
  - Adjusted the layout so text isn't cut off at the edge of round screens.
  - Made saving of sessions and settings more robust.

**Changes in Phone v0.2.0**
- Status: ✅ Released (Phone v0.2.0)
- What:
  - Supports the latest Android.
  - Fixed an issue where Premium could be treated as the free version even after purchase.
  - Venue names are now saved only when you type them yourself. Nearby venues are searched only when you tap "Find nearby venues" (up to 5 times a day). Venue names saved previously are deleted (the app lets you know).
  - The app no longer uses the location permission.
  - You can now check how data is used and the privacy policy from Health Connect's settings.

---

ご不便をおかけした皆さま、ありがとうございました。引き続きご報告をお待ちしています。
Thanks for your patience and reports — please keep them coming!
