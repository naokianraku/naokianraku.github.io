---
title: 対応状況 / Fixed issues — MaxSauna Timer
---

# 対応状況 — MaxSauna Timer

**最終更新:** 2026-06-10（v0.1.5 / Phone v0.1.11 を準備中）

テスターの皆さまからいただいた不具合のご報告・ご要望と、その対応内容です。ご協力ありがとうございます！

> 🐛 新しいご報告はこちら → **[フィードバックフォーム](feedback.html)**

## Pixel Watch / Android

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
- 状態：✅ 追加・配信済み（v0.1.4）
- 内容：誤って進めてしまったとき、画面長押し（確認あり）または「戻る」ボタンで1つ前のフェーズに戻せるようにしました。

**F-011 本体ダブルタップで次へ（実験・要望）**
- 状態：✅ 実験的に追加・配信済み（v0.1.4／既定OFF）
- 内容：手がふさがる場面向けに、本体を2回トントンと叩くと次のフェーズへ進む実験機能を追加しました（加速度センサーで判定）。設定 → ウォッチ設定でON。誤検知することがあるため既定OFFで、合わない場合はOFFにしてください。

**F-009 「休憩」フェーズの追加（要望）**
- 状態：✅ 配信済み（v0.1.4／名称選択も追加）
- 内容：設定 → ウォッチ設定 →「その他フェーズを使う」をONにすると、外気浴のあとに第4フェーズが入り、名称を「休憩／お風呂／給水／シャワー／ストレッチ」から選べます（名称選択を今回追加）。取説に案内を追記しました。

### 🔧 次回アップデートで配信（Watch v0.1.5 / Phone v0.1.11）

**F-020 / F-021 画面を覆う・放置でセッションが消える／データが残らない（重大）**
- 状態：🔧 対策実装・次回配信（v0.1.5）
- 対策：計測中のセッションを自動保存し、画面を覆って消灯・アプリが終了しても、起動し直すと**セッションを復元してデータを失わない**ようにしました（画面オフでの完全な継続記録は引き続き改良中）。

**F-016 操作方法の見直し：濡れ・水しぶきによる誤操作の防止（重要）**
- 状態：🔧 実装・次回配信（v0.1.5）
- 内容：**計測中は画面タッチに反応しません（クラウンのみ）**。上＝次へ／下＝一時停止。**一時停止中だけ**画面に「再開／戻る／終了」のメニューが出ます。「操作ボタンを表示」をONにすると実行中も 次へ／停止 をタッチできます。（F-010「1つ前に戻る」は長押し→一時停止メニューに変更）

**F-015 フェーズを戻したとき経過時間を引き継ぐ**
- 状態：🔧 実装・次回配信（v0.1.5）
- 内容：1つ前のフェーズに戻ると、タイマーが0でなく**戻り先の経過時間から続く**ようにしました。

**F-011 本体ダブルタップの感度を改善**
- 状態：🔧 改善・次回配信（v0.1.5）
- 内容：「効かない」とのご報告を受け、検知感度を上げました（実験機能・既定OFF）。

**F-019 履歴の削除をスワイプ→ゴミ箱方式に（Phone）**
- 状態：🔧 実装・次回配信（Phone v0.1.11）
- 内容：履歴を左スワイプするとゴミ箱ボタンが現れ、タップで削除（全画面の確認ダイアログは廃止）。

**F-014 詳細データに「欠測（データ欠損）」を表示（Phone）**
- 状態：🔧 追加・次回配信（Phone v0.1.11）
- 内容：心拍の欠測の回数・合計時間・割合を「詳細データ」に表示します。

**F-017 ウォッチで設定できる項目をPhoneでも全て設定可能に（Phone）**
- 状態：🔧 追加・次回配信（Phone v0.1.11）
- 内容：セット毎の各フェーズ時間・閾値1/2もPhoneの「ウォッチ設定」で編集できるようにしました。

---

# Fixed issues — MaxSauna Timer (English)

**Last updated:** 2026-06-10 (v0.1.5 / Phone v0.1.11 in preparation)

This page summarizes the bug reports & requests from testers and how each was addressed. Thank you for your help!

> 🐛 Report new issues → **[Feedback form](feedback.html)**

## Pixel Watch / Android

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
- Status: ✅ Added & released (v0.1.4)
- What: If you advance by mistake, long-press the screen (with a confirmation) or use the Back button to return to the previous phase.

**F-011 Double-tap the watch body to advance (beta, request)**
- Status: ✅ Added (experimental) & released (v0.1.4 / off by default)
- What: For when your hands are occupied, a quick double-tap on the watch body advances to the next phase (detected via the accelerometer). Turn it on in Settings → Watch settings. It can misfire, so it is off by default — turn it off if it doesn't suit you.

**F-009 Add a "rest" phase (request)**
- Status: ✅ Released (v0.1.4 / name selection added)
- What: Turn on Settings → Watch settings → "Use extra phase" to insert a 4th phase after cool-down, with a selectable name (rest / hot bath / hydration / shower / stretch — name selection added in this update). We added a note to the guide.

### 🔧 Shipping in the next update (Watch v0.1.5 / Phone v0.1.11)

**F-020 / F-021 Session lost / data not saved when the screen is covered or left running (serious)**
- Status: 🔧 Fix implemented, shipping next (v0.1.5)
- Fix: The running session is now auto-saved, so even if the screen is covered/off or the app is killed, relaunching restores the session and your data is not lost. (Full screen-off continuous recording is still being improved.)

**F-016 Controls revised to prevent wet/splash mis-taps (important)**
- Status: 🔧 Implemented, shipping next (v0.1.5)
- What: During a running session the screen no longer responds to touch (crown only): up = next, down = pause. Only while paused does an on-screen menu (Resume / Go back / End) appear. Turn on "Show control buttons" to also use Next/Pause by touch while running. (Go back, F-010, moved from long-press to the pause menu.)

**F-015 Carry over elapsed time when going back a phase**
- Status: 🔧 Implemented, shipping next (v0.1.5)
- What: Going back one phase now resumes from that phase's previous elapsed time instead of resetting to 0.

**F-011 Improved double-tap sensitivity**
- Status: 🔧 Improved, shipping next (v0.1.5)
- What: Based on "it doesn't work" reports, we increased detection sensitivity (experimental, off by default).

**F-019 History delete is now swipe-to-reveal-trash (Phone)**
- Status: 🔧 Implemented, shipping next (Phone v0.1.11)
- What: Left-swipe a history row to reveal a trash button, then tap it to delete (the full-screen confirmation dialog was removed).

**F-014 Show "Missing data (dropouts)" in Detailed data (Phone)**
- Status: 🔧 Added, shipping next (Phone v0.1.11)
- What: The Detailed data card now shows the count / total time / percentage of heart-rate dropouts.

**F-017 Everything configurable on the watch is now also configurable on the phone (Phone)**
- Status: 🔧 Added, shipping next (Phone v0.1.11)
- What: Per-set phase durations and thresholds (1/2) can now be edited from the phone's Watch settings too.

---

ご不便をおかけした皆さま、ありがとうございました。引き続きご報告をお待ちしています。
Thanks for your patience and reports — please keep them coming!
