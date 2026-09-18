# Personal Terminal 開発管理パッケージ v1.1
## iOS / iPadOS / Android クロスプラットフォーム対応版

## 現在の基準版（2026-09-18確認）

公開中の [Personal AI Terminal 1.1](https://personal-terminal-wireframe.skomy3810155.chatgpt.site/) を動作基準とする。`app/` は公開配信ファイルから取得した保全用スナップショットで、元の開発リポジトリではない。配信時に追加されたホスティング用スクリプトは除去した。サイトへの更新はこのリポジトリの変更だけでは行われない。

現状調査と次の作業順は [docs/12_BASELINE_AUDIT.md](docs/12_BASELINE_AUDIT.md) を参照する。まず PT-001 の実機確認を終え、次の機能を一件ずつ決める。

Personal Terminal v1.1を基準に、ChatGPTで要件・Taskを整理し、Codexで実装するためのMarkdown一式。

## 基本運用
1. このパッケージの`AGENTS.md`と`docs`をPersonal Terminalプロジェクト直下へ置く。
2. `docs/07_TASKS.md`に今回の1 Taskを記載する。
3. Codexにプロジェクトフォルダを開かせる。
4. CodexへAGENTS.mdと07_TASKS.mdを読ませる。
5. Codexが調査/実装/テスト。
6. 人間がブラウザ・実機で確認。
7. 問題があれば同じTaskで修正。
8. 完了後、次Taskへ進む。

## ファイル
- AGENTS.md : Codex共通ルール
- docs/00_PROJECT_OVERVIEW.md : 全体像
- docs/01_REQUIREMENTS.md : 基本要件
- docs/02_ARCHITECTURE.md : 構造方針
- docs/03_UI_SPEC.md : UI/HCI
- docs/04_USER_MODES.md : 年齢別モード
- docs/05_AI_SPEC.md : AI設計
- docs/06_ROADMAP.md : ロードマップ
- docs/07_TASKS.md : 現在の作業指示
- docs/08_CHANGELOG.md : 変更履歴
- docs/09_CODEX_GUIDE.md : Codex運用手順
- docs/10_PLATFORM_COMPATIBILITY.md : iPhone/iPad/Android共通設計
- docs/11_TEST_MATRIX.md : 端末・ブラウザ試験表

## v1.1での重要変更
- Androidスマートフォン/タブレットを正式ターゲット化
- 1つのPWAコードベースを基本方針化
- responsive/touch/orientation/safe-areaを要件化
- Web App Manifest / Service Worker等を監査対象化
- 音声/通知等のOS差にfallbackを必須化
- クロスプラットフォーム試験をDefinition of Doneへ追加
