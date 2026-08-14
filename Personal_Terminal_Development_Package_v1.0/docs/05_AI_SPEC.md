# 05 — AI SPEC
Version: 1.0

## Purpose
Personal TerminalのAIは、単なる自由会話ではなく「利用者の今日の行動を整理する支援機能」として設計する。

## Core AI Functions
- 今日を整理
- 空き時間を使う
- 一日を振り返る
- 利用者からの質問

## AI Input Context
将来AIへ渡す候補:
- current time
- today's schedule
- incomplete tasks
- activity/learning progress
- user mode
- relevant user preferences

## Mode-Specific Behavior

### standard
簡潔な行動整理と選択肢提示。

### kids
すぐ答えを与えすぎず、一緒に考える。

### junior
自己管理を促し、課題の優先順位を整理する。

### student
学習計画・進捗・目標から具体的な行動提案を行う。

### senior
短文・確認・復唱を重視し、複雑な選択肢を一度に出しすぎない。

## AI Safety
- AIの提案と確定操作を分ける
- 削除・送信など重大操作は確認する
- APIキーをHTML/JSへ直接埋め込まない
- 子ども向けでは依存を促進する表現を避ける
- 医療・法律・金融など高リスク判断の自動確定を行わない
