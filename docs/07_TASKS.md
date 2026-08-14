# 07 — CURRENT TASKS
Version: 1.0

# Task PT-001 — Baseline Protection

## Purpose
Personal Terminal v1.1を基準版として保全し、今後の開発をv1.2-dev側で進められる状態にする。

## Required Actions
1. 現在のプロジェクト構成を確認する。
2. v1.1の主要機能を一覧化する。
3. 既存コードを大きく変更しない。
4. 開発用コピーまたは安全な開発ブランチ/作業領域を使う方法を提案する。
5. 次のTaskでUser Mode基盤を導入できる箇所を特定する。

## Deliverables
- 現在の主要ファイル一覧
- 各ファイルの役割
- v1.1で確認できる主要機能
- User Mode導入候補箇所
- リスク
- PT-002の推奨実装手順

## Do Not
- UIを全面変更しない
- Senior Modeを実装しない
- Kids/Junior/Student Modeを実装しない
- 新しいフレームワークを入れない
- AI APIを接続しない
- データ形式を破壊しない

## Done Criteria
- v1.1の現状構造が把握できる
- 次の実装箇所が説明できる
- 既存コードを不用意に破壊していない
- 非エンジニアにも理解できる日本語で結果報告される

---

# NEXT TASK DRAFT — PT-002 User Mode Foundation
※ PT-001確認後に実施。

## Goal
User Mode基盤を追加する。

## Proposed Requirements
- `userProfile.mode` を導入
- 初期値 `standard`
- modes:
  - standard
  - kids
  - junior
  - student
  - senior
- 現段階ではStandard以外の大幅なUI変更をしない
- 保存方式は既存仕様との整合を確認して決める
