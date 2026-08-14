# 09 — Codexへの指示の渡し方
Version: 1.1

## 結論
Codexには毎回長文説明せず、
AGENTS.md + docs/07_TASKS.mdを基準に1 Taskずつ作業させる。

## 最初の指示
```text
Personal Terminal v1.1の開発を開始します。

AGENTS.mdとdocs内のMarkdownを確認してください。
今回はdocs/07_TASKS.mdのPT-001だけを実施してください。

まだ大きなコード変更はしないでください。
iPhone、iPad、Androidスマートフォン、Androidタブレットで利用する前提で現行構造を監査してください。

結果はAGENTS.mdのCompletion Report形式に従い日本語で報告してください。
```

## 実装時
```text
AGENTS.mdとdocs/07_TASKS.mdを確認してください。
今回のTaskだけを実装してください。
範囲外の改善は行わないでください。
既存v1.1の動作を維持してください。
iOS/iPadOS/Android差がある場合は明示してください。
```

## 不具合修正
現象、期待動作、今回触ってよい範囲を書く。

## 停止
```text
ここで実装を止めてください。
これ以上変更せず、変更ファイルと変更内容、
元に戻す場合の手順を説明してください。
```

## 完了確認
```text
docs/07_TASKS.mdのDone Criteriaと照合してください。
未達項目があれば未達だけ報告してください。
満たしている場合はテスト結果と残存リスクを報告してください。
```

## Cross-Platform Audit専用
```text
AGENTS.md、01_REQUIREMENTS.md、03_UI_SPEC.md、
10_PLATFORM_COMPATIBILITY.md、11_TEST_MATRIX.mdを確認してください。

今回はコード変更せず、
iPhone/iPad/Android phone/Android tabletで
現行v1.1が問題になりそうな箇所を一覧化してください。
```
