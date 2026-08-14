# Personal Terminal — AGENTS.md
Version: 1.1
Baseline: Personal Terminal v1.1

## 1. Purpose
Personal Terminalは、予定・タスク・活動/学習・AI支援を統合するPWA型Personal Terminalである。

## 2. Baseline Rule
- Personal Terminal v1.1を基準版とする。
- 基準版の既存動作を、明示的なTaskなしに削除・破壊しない。
- 大規模変更より段階的変更を優先する。
- 原則1 Taskずつ作業する。

## 3. Project Owner
プロジェクトオーナーは非エンジニア。
報告は日本語で、専門用語だけに依存せず、
「何を変えたか」「なぜ」「何を確認すべきか」を明示する。

## 4. Development Principles
- HTML / CSS / JavaScriptを基本技術とする。
- 不要なフレームワーク・依存関係を追加しない。
- iPhone / iPad / Androidスマートフォン / Androidタブレットを正式対象とする。
- 1つのクロスプラットフォームPWAコードベースを基本とする。
- iOS専用版とAndroid専用版を安易に分岐しない。
- responsive/mobile-firstを基本とする。
- 標準Web APIとprogressive enhancementを優先する。
- UI、データ、アプリロジック、AI、外部連携を可能な限り分離する。

## 5. User Modes
将来以下を共通Core上でサポートする。
- standard
- kids
- junior
- student
- senior

Taskで指定されない限り、全モードを一度に実装しない。

## 6. Before Editing
必ず以下を確認する。
1. AGENTS.md
2. docs/00_PROJECT_OVERVIEW.md
3. docs/01_REQUIREMENTS.md
4. docs/02_ARCHITECTURE.md
5. docs/07_TASKS.md
6. docs/10_PLATFORM_COMPATIBILITY.md
7. Task対象の既存コード

## 7. Safety Rules
- 動いている機能を勝手に削除しない。
- 小さなTaskのために全体を書き換えない。
- 無関係なファイルを変更しない。
- APIキー・秘密情報・個人情報をコードに埋め込まない。
- iOS/Android差がある機能を、片方で動いたことだけで完了扱いしない。

## 8. Cross-Platform Rules
UI/PWA関連Taskでは最低限以下を考慮する。
- iPhone portrait
- iPad portrait / landscape
- Android phone portrait
- Android tablet portrait / landscape
- Safari/WebKit on iOS/iPadOS
- Chrome/Chromium on Android

ブラウザ・端末で能力差がある場合:
- 可能ならfeature detectionを使う。
- fallbackを用意する。
- 非対応/制限を明記する。
- silent failureを避ける。
- User-Agent判定を主戦略にしない。

## 9. Task Execution
1. Taskを読み、理解内容を明示。
2. 関連コードを調査。
3. 最小限の変更。
4. 利用可能なチェック/テストを実行。
5. 既存機能への影響を確認。
6. 完了時はdocs/08_CHANGELOG.mdを更新。
7. 結果を日本語で報告。

## 10. Completion Report
### 実施したこと
### 変更したファイル
### 動作確認
### クロスプラットフォーム確認
### 既存機能への影響
### 未解決事項
### 次の推奨作業

## 11. Definition of Done
- 要求された動作が実装されている。
- 明らかなconsole/runtime errorがない。
- 関連する既存機能が維持されている。
- 対象プラットフォーム差を確認・報告している。
- 未解決事項を隠していない。
