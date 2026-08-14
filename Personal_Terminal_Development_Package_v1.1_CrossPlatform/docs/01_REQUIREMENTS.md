# 01 — REQUIREMENTS
Version: 1.1

## A. Core Functions

### Schedule
- 今日の予定を表示・追加・編集・削除できる。
- 時刻と内容を保持できる。

### Tasks
- 今日のタスクを表示・追加できる。
- 完了/未完了を管理できる。

### Activity / Learning
- 今日取り組む活動を表示できる。
- 目標時間・実施時間を記録できる。
- 将来「学習」以外にも利用できる汎用構造を目指す。

### AI Support
- 今日を整理。
- 空き時間活用。
- 一日の振り返り。
- User Modeに応じた説明・介入レベル変更。

### Settings
- 配色。
- User Mode。
- 将来: 文字サイズ、音声、簡易UI。

### Data
試作段階はローカル保存を基本とする。
将来、複数端末同期・家族共有を別Phaseで設計。

## B. UX / Non-Functional
- 非エンジニアでも扱いやすい。
- iPhone/Android phoneの狭い画面で主要機能が使える。
- iPad/Android tabletのportrait/landscapeに対応。
- 文字・ボタンが小さすぎない。
- 主要操作を深い階層にしない。
- PWA化を妨げない。
- 既存機能を壊さず段階改良できる。

## C. Cross-Platform / PWA

### Responsive
- viewportを適切に設定。
- 固定幅前提を避ける。
- portrait/landscapeで主要操作が隠れない。
- safe-area/notchを考慮。
- ソフトウェアキーボード表示時に入力不能にならない。

### Touch
- hoverだけに依存しない。
- マウス前提にしない。
- 主要タッチ対象を十分大きくする。
- 特殊ジェスチャーを唯一の操作方法にしない。

### PWA Foundation
段階的に確認/実装:
- Web App Manifest
- icons
- start_url
- display
- theme/background settings
- Service Worker
- cache/offline policy
- HTTPS
- installability

### Browser Compatibility
主要確認:
- Safari on iPhone/iPad
- Chrome on Android
- Chromium desktop

Web APIは対応可否を確認し、可能ならfeature detectionを使う。

### Voice
音声入力/読み上げはブラウザ差を前提とする。
音声不可でもタッチ/文字入力で基本機能を使えること。

### Notifications
OS・ブラウザ・権限・インストール状態で差があるため、
通知をCoreの必須前提にしない。
通知不可でもアプリ内で予定/リマインド情報を確認可能にする。

### Data Portability
ローカル保存は端末単位であることを前提とする。
JSON等のexport/importを維持・改善候補とする。

## D. Current Out of Scope
- 本番クラウドDB
- 本番ユーザー認証
- 課金
- 本番家族/保護者アカウント
- フロントエンドへのAI APIキー埋め込み
