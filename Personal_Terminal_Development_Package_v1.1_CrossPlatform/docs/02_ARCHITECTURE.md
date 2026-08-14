# 02 — ARCHITECTURE
Version: 1.1

## Goal
Personal Terminal v1.1を、年齢別モードと複数OSへ拡張できる構造へ段階整理する。

## Layers

### Core Data
- schedule
- tasks
- activities
- settings
- userProfile

### Core Logic
- CRUD
- save/load
- 今日の状態計算
- AI context生成

### UI / Responsive Layer
- phone layout
- tablet layout
- orientation adaptation
- mode-specific presentation

### AI Layer
- AI context
- mode prompts
- output presentation
- future API integration

### PWA Layer
- manifest
- service worker
- install/offline behavior

### Capability / Integration Layer
OS/ブラウザ差が出やすい機能を隔離:
- voice
- notifications
- share
- calendar integration
- future cloud sync

## userProfile Candidate
```javascript
const userProfile = {
  mode: "standard",
  fontSize: "normal",
  voiceEnabled: false,
  simpleUI: false
};
```

## Rules
- Modeごとにアプリ本体を複製しない。
- iOS版/Android版を安易に分岐しない。
- 共通ロジックを再利用。
- 既存localStorageを不用意に破壊しない。
- APIキーをフロントエンドへ固定しない。
- Web APIはfeature detectionを優先。

## Data Portability
クラウド同期前でも、
JSON backup/export/import等で端末移行の余地を残す。
