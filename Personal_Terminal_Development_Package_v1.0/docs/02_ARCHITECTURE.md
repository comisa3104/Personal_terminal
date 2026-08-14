# 02 — ARCHITECTURE
Version: 1.0

## Goal
Personal Terminal v1.1を、将来の年齢別モードへ拡張できる構造に段階的に整理する。

## Logical Layers

### 1. Core Data
共通して利用するデータ。
- schedule
- tasks
- activities
- settings
- userProfile

### 2. Core Logic
共通処理。
- データの追加・更新・削除
- 保存・読み込み
- 今日の状態計算
- AIに渡すコンテキストの生成

### 3. UI Layer
表示・入力。
- Standard UI
- Kids UI
- Junior UI
- Student UI
- Senior UI

### 4. AI Layer
- AI入力データ作成
- モード別プロンプト
- AI回答表示
- 将来的な外部AI API連携

### 5. Integration Layer
将来追加する外部連携。
- calendar
- notifications
- family sharing
- cloud database

## userProfile Proposed Shape

```javascript
const userProfile = {
  mode: "standard",
  fontSize: "normal",
  voiceEnabled: false,
  simpleUI: false
};
```

これは確定実装仕様ではなく、現在の設計基準。

## Architectural Rules
- Modeごとにアプリ本体を複製しない
- 共通ロジックを可能な限り再利用する
- UIの違いを設定または描画処理で吸収する
- 既存localStorageデータを不用意に破壊しない
- APIキーをフロントエンドへ直接固定しない
