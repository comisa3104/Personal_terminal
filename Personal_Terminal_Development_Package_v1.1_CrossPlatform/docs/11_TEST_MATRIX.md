# 11 — TEST MATRIX
Version: 1.0

## Purpose
「自分のiPadで動いた」だけを完了条件にしないための最低試験表。

## A. Layout
- [ ] narrow phone portrait
- [ ] phone landscape
- [ ] tablet portrait
- [ ] tablet landscape
- [ ] desktop

## B. Browser / OS
可能な範囲で:
- [ ] Safari / iPhone
- [ ] Safari / iPad
- [ ] Chrome / Android phone
- [ ] Chrome / Android tablet
- [ ] Chrome or Edge / Windows

## C. Smoke Test
- [ ] 起動
- [ ] 今日の予定表示
- [ ] 予定追加/編集/削除
- [ ] タスク追加/完了
- [ ] Activity/学習
- [ ] AI支援UI
- [ ] 設定
- [ ] User Mode保存（導入後）
- [ ] JSON export/import（存在する場合）
- [ ] 再読み込み後のデータ
- [ ] portrait/landscape切替

## D. PWA
導入後:
- [ ] manifest認識
- [ ] icon
- [ ] Home Screen/Install
- [ ] standalone表示
- [ ] Service Worker登録
- [ ] offline時の最低動作
- [ ] update後のキャッシュ挙動

## E. Accessibility / Touch
- [ ] 小さすぎるタップ対象がない
- [ ] hoverなしで操作可能
- [ ] 文字拡大で致命的崩れなし
- [ ] software keyboardで入力不能にならない
- [ ] safe-areaで主要操作が隠れない

## F. Voice / Notification
実装後:
- [ ] 音声が使えない時のfallback
- [ ] 通知拒否時のfallback
- [ ] 権限エラーを利用者へ明示
