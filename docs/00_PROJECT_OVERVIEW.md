# 00 — PROJECT OVERVIEW
Version: 1.0

## Project Name
Personal Terminal

## Current Baseline
Personal Terminal v1.1

## Purpose
予定、タスク、活動・学習、AI支援を1つの画面に統合し、利用者が「今日何をするか」を簡単に整理できるPersonal Terminalを構築する。

## Product Direction
将来的には、共通Coreを維持しながら利用者に応じてUI・AI挙動を切り替える。

### Planned Modes
- Standard：一般利用者
- Kids：小学生
- Junior：中学生
- Student：高校生
- Senior：高齢者

## Core Concept
Personal Terminalは単なるカレンダーやToDoアプリではない。

利用者の
- 予定
- やること
- 集中・学習活動
- 現在時刻
- 利用者モード
を組み合わせ、AIが「次に何をするか」を整理・提案できることを目指す。

## Development Strategy
- v1.1を基準版として保存
- v1.xでCoreとUIの分離を進める
- 1機能ずつ実装
- 人間による実機確認を必須とする
- 年齢別モードを別アプリとして複製しない
