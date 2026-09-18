# 07 — CURRENT TASKS
Version: 1.1

# PT-001 — Baseline Protection & Cross-Platform Audit

## 2026-09-18 現状

公開版 v1.1 の配信ファイルを `app/` に保全し、コードの一次調査を `docs/12_BASELINE_AUDIT.md` に記録した。公開版の元開発リポジトリと GitHub のこのリポジトリは別である。残る PT-001 は、iPhone/iPad/Android 実機での表示、操作、保存、バックアップ、オフライン動作の確認と、その結果の記録。これが終わるまで PT-002 の実装には進まない。

## Purpose
Personal Terminal v1.1を基準版として保全し、
iPhone/iPad/Android対応の観点から現行構造を把握する。

## Required Actions
1. 現在のプロジェクト構成を確認。
2. v1.1の主要機能を一覧化。
3. 各主要ファイルの役割を整理。
4. 既存コードを大きく変更しない。
5. User Mode導入候補箇所を特定。
6. iPhone/iPad/Android phone/Android tabletの観点でコードを監査。
7. viewport、固定幅、media query、touch、orientation依存を確認。
8. manifest、service worker、icons、PWA設定の有無を確認。
9. iOS/iPadOSとAndroidで差が出そうなAPI/機能を一覧化。
10. PT-002の実装手順を提案。

## Deliverables
- 主要ファイル一覧
- 各ファイルの役割
- 主要機能一覧
- User Mode導入候補
- クロスプラットフォーム対応状況表
- Android対応で必要な修正候補
- PWA基盤不足項目
- リスク
- PT-002推奨手順

## Do Not
- UI全面変更
- Senior/Kids/Junior/Student実装
- 新規framework導入
- AI API接続
- データ形式破壊
- Android専用コードの安易な追加
- iOS専用コードの安易な追加

## Done Criteria
- v1.1構造を説明できる。
- iOS/iPadOS/Androidの主要互換性リスクを把握できる。
- 次実装箇所を非エンジニア向けに説明できる。
- 既存コードを不用意に破壊していない。

---

# NEXT DRAFT — PT-002 User Mode Foundation
PT-001確認後に確定する。

候補:
- userProfile.mode
- default: standard
- standard/kids/junior/student/senior
- Standardの既存UI維持
- 保存方式は既存仕様を調査後に決定
