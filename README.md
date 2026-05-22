<div align="center">
  <h3 align="center">Azurlane Build (TW Only Fork)</h3>

  <p align="center">
    本 fork 僅維護 <b>台服 (TW)</b> 的 XAPK 自動構建
    <br />
    Fork 自 <a href="https://github.com/Chtholly344/Azurlane-Build">Chtholly344/Azurlane-Build</a>
  </p>
</div>

---

## ⚠️ 重要提示

本項目僅用於學習和研究，請在遵守相關法律法規的前提下使用，若違規使用導致的一切後果由使用者本人承擔。

- **風險警告**：使用 mod 可能涉及未知風險，包括但不限於遊戲帳號被封禁
- **登入問題**：重新打包的 APK 簽名與官方版本不同，第三方授權登入會失敗。請使用 Yostar 帳號 / 信箱驗證碼登入

---

## 🚀 如何構建最新 TW 版本

### 方法 A：一鍵構建（推薦）
1. 進入 [Actions](../../actions) 分頁
2. 左側選 **Build TW (One-Click)**
3. 點右上 **Run workflow** → **Run workflow**
4. 等待 5–10 分鐘，到 [Releases](../../releases) 下載 7z 分卷

### 方法 B：使用原 workflow
1. 進入 Actions → **XAPK AzurLane JMBQ Build Work**
2. Run workflow → 選 `TW`（其他區服已註解）→ Run

### 方法 C：gh CLI
```bash
gh workflow run tw.yml -R <your-account>/Azurlane-Build
```

---

## 📦 安裝說明

1. 下載 Release 中所有 `TW-V.x.x.x.7z.00*` 分卷
2. 用 7-Zip 解壓 `.7z.001` 即可（會自動合併分卷）
3. 取得 `.xapk` 後安裝（需 XAPK 安裝器，例如 APKPure App 或 SAI）

---

## 🔧 版本對照

- **MOD 補丁版本**：Release tag 為 `{版本}-XAPK`，對照 [JMBQ/azurlane releases](https://github.com/JMBQ/azurlane/releases/latest)
- **遊戲本體版本**：檔名 `TW-V.{版本}.7z.001` 即 Google Play 當下最新版

---

## 📚 致謝

- [Chtholly344/Azurlane-Build](https://github.com/Chtholly344/Azurlane-Build) — 原始構建腳本
- [JMBQ/azurlane](https://github.com/JMBQ/azurlane) — MOD 補丁
- [n0k0m3/PerseusCI](https://github.com/n0k0m3/PerseusCI)
