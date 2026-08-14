# 03 — UI SPEC
Version: 1.1

## General HCI
- 見て何ができるか分かる。
- 重要操作を上部/中央に置く。
- 情報を詰め込みすぎない。
- 操作結果を明確に表示。
- 誤操作から戻れる。
- タッチ操作を優先。

## Phone
対象:
- iPhone
- Android smartphone

方針:
- portraitは1列中心。
- 重要カード・Actionを上位へ。
- 横スクロールを主要操作にしない。
- ソフトウェアキーボードで入力欄が隠れない。

## Tablet
対象:
- iPad
- Android tablet

方針:
- 2列/カード配置を許容。
- portrait/landscape双方に対応。
- 広すぎる場合はmax-width等で可読性維持。

## Desktop
開発・管理・補助利用として主要機能利用可能にする。

## Cross-Platform UI Rules
- OS固有フォントへ過度に依存しない。
- hover必須禁止。
- タップ対象を十分確保。
- CSS media queryだけでなく柔軟なlayoutを使う。
- safe-area/notchで主要ボタンが隠れない。
- OSテーマ差で文字が読めなくならない。

## Mode Notes
### Standard
v1.1 UIを基準。

### Kids
大きめのボタン、分かりやすい語彙。

### Junior
宿題・提出物・部活・テスト中心。

### Student
学習計画・模試・進路を扱える情報密度。

### Senior
大きな文字・操作対象、機能削減、音声+画面、確認重視。
