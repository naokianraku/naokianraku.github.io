---
title: 対応状況 / Fixed issues — MaxSauna Timer
---

# 対応状況 — MaxSauna Timer

**最終更新:** 2026-06-09

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

### 🔧 修正済み（次回アップデートで配信）

**F-005 サウナの設定時間あたりでフェーズが勝手に進むことがある**
- 状態：🔧 修正済み・次回配信（v0.1.4）
- 対策：クラウンの誤反応が原因でした。フェーズ移行に必要な回転量を大きくし（約2倍）、ごく小さな回転が時間とともに溜まって誤作動するのをリセットするようにして、意図的に回したときだけ進むよう調整しました。

---

# Fixed issues — MaxSauna Timer (English)

**Last updated:** 2026-06-09

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

### 🔧 Fixed (shipping in the next update)

**F-005 The phase sometimes advanced on its own near the set sauna time**
- Status: 🔧 Fixed, shipping next (v0.1.4)
- Fix: It was caused by accidental crown input. We increased the rotation needed to change phase (about 2×) and reset tiny rotations that built up over time, so the phase only advances when you turn the crown deliberately.

---

ご不便をおかけした皆さま、ありがとうございました。引き続きご報告をお待ちしています。
Thanks for your patience and reports — please keep them coming!
