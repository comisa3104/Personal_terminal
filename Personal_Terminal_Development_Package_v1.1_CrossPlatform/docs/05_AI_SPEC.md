# 05 — AI SPEC
Version: 1.1

## Purpose
AIは自由会話だけでなく「今日の行動整理」を支援する。

## Core AI Functions
- 今日を整理
- 空き時間を使う
- 一日を振り返る
- 質問対応

## Candidate Context
- current time
- today's schedule
- incomplete tasks
- activity progress
- user mode
- relevant preferences

## Mode Behavior
- standard: 簡潔な行動整理
- kids: すぐ答えを与えすぎない
- junior: 優先順位と自己管理支援
- student: 学習進捗・目標に基づく提案
- senior: 短文・確認・復唱

## Cross-Platform AI UI
AI機能は特定OS固有UIに依存させない。
音声はoptional capabilityとし、文字/タッチfallbackを持つ。

## Safety
- AI提案と確定操作を分ける。
- 削除/送信等の重要操作は確認。
- APIキーをHTML/JSへ直書きしない。
- 子ども向けで依存を促進しない。
- 高リスク判断をAIだけで自動確定しない。
