# Personal Terminal 開発管理パッケージ v1.0

このパッケージは、Personal Terminal v1.1 を基準に、ChatGPTで要件を整理し、Codexで実装を進めるための開発管理用Markdown一式です。

## 基本運用
1. `AGENTS.md` をプロジェクトのルートに置く
2. `docs/07_TASKS.md` に「今回Codexに実装してほしい1タスク」を書く
3. Codexに対象フォルダを開かせる
4. Codexへ「AGENTS.mdと07_TASKS.mdを確認して実装」と指示する
5. 実装後、ブラウザまたは実機で人間が確認する
6. 問題があれば同じTaskに修正条件を追記する
7. 完了したら `08_CHANGELOG.md` に記録する

## ファイル構成
- `AGENTS.md` : Codexが常に守る開発ルール
- `docs/00_PROJECT_OVERVIEW.md` : プロジェクト全体像
- `docs/01_REQUIREMENTS.md` : 現在の基本要件
- `docs/02_ARCHITECTURE.md` : 構造方針
- `docs/03_UI_SPEC.md` : UI/HCI設計方針
- `docs/04_USER_MODES.md` : 年齢・用途別モード
- `docs/05_AI_SPEC.md` : AI機能の設計方針
- `docs/06_ROADMAP.md` : 開発ロードマップ
- `docs/07_TASKS.md` : 現在のCodex作業指示
- `docs/08_CHANGELOG.md` : 変更履歴
- `docs/09_CODEX_GUIDE.md` : Codexへの指示の渡し方

## 最重要ルール
「全部まとめて改良して」ではなく、1タスクずつ進めます。
