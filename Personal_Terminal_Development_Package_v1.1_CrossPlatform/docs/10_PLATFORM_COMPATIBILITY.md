# 10 — PLATFORM COMPATIBILITY
Version: 1.0

## 1. Policy
Personal TerminalはApple専用ではなく、
標準Web技術を使ったクロスプラットフォームPWAとして設計する。

Primary:
- iPhone
- iPad
- Android smartphone
- Android tablet

Secondary:
- PC browser

## 2. Compatibility Matrix

| Area | iPhone/iPad | Android | Policy |
|---|---|---|---|
| HTML/CSS/JS Core | 必須 | 必須 | 共通コード |
| Responsive UI | 必須 | 必須 | 画面幅中心 |
| Touch | 必須 | 必須 | hover依存禁止 |
| Manifest | 確認 | 確認 | 標準manifest |
| Service Worker | 確認 | 確認 | 共通方針 |
| Home Screen/Install | 実機確認 | 実機確認 | OS差を文書化 |
| Offline | 実機確認 | 実機確認 | 共通SW |
| Voice | API差確認 | API差確認 | fallback必須 |
| Notifications | 条件差確認 | 条件差確認 | Core依存禁止 |
| Export/Import | 必須 | 必須 | 移行余地 |
| Orientation | 必須 | 必須 | portrait/landscape |

## 3. Browser Targets
Primary:
- Safari on iOS/iPadOS
- Chrome on Android
Secondary:
- Chrome/Edge desktop

特定ブラウザ限定APIをCoreの必須要件にしない。

## 4. Responsive Policy
製品名別の固定幅を大量にハードコードせず、
コンテンツが崩れるポイントでbreakpointを決める。

## 5. Touch
主要ボタンは指で押しやすい領域を確保。
Senior/Kidsはさらに大きくする。

## 6. PWA Files to Inspect
Codexは以下を確認する。
- manifest.webmanifest / manifest.json
- service worker
- service worker registration
- icons
- favicon
- theme-color
- viewport
- start_url
- display
- offline handling

PT-001では不足があっても勝手に実装せず報告する。

## 7. Feature Detection
端末名より機能存在確認を優先。

例:
```javascript
if ("serviceWorker" in navigator) {
  // supported
}
```

## 8. Fallback
- voice input -> text/touch
- voice output -> on-screen text
- notification -> in-app reminder
- install prompt -> manual guidance
- offline unavailable -> clear status

## 9. Device-Specific Risks
- Home Screen/Install導線
- Web Push条件
- 音声API
- permission UI
- software keyboard resize
- safe-area/notch
- background behavior
- storage persistence/cleanup
- file import/export UX

実装時は最新仕様を確認する。
