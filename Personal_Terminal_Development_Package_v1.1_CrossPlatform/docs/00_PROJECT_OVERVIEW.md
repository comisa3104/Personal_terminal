# 00 — PROJECT OVERVIEW
Version: 1.1

## Project
Personal Terminal

## Baseline
Personal Terminal v1.1

## Purpose
予定、タスク、活動・学習、AI支援を1画面に統合し、
利用者が「今日何をするか」を簡単に整理できるPersonal Terminalを構築する。

## Target Platforms
Primary:
- iPhone
- iPad
- Android smartphone
- Android tablet

Secondary:
- PC browser

## Product Direction
共通Coreを維持しながら、利用者に応じてUI・AI挙動を切り替える。

### Planned Modes
- Standard
- Kids
- Junior
- Student
- Senior

## Core Concept
単なるカレンダーやToDoではなく、
予定・タスク・活動・現在時刻・User Mode等を組み合わせ、
AIが次の行動を整理・提案できることを目指す。

## Development Strategy
- v1.1を基準版として保存。
- 1つのPWAコードベースを維持。
- OS別アプリの複製を避ける。
- v1.xでCore/UI/Capabilityを分離。
- 1機能ずつ実装。
- 重要Phaseでは実機確認。
