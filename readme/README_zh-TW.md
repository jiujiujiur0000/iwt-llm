<p align="center">
  <a href="../README.md">English</a> |
  <a href="README_zh-CN.md">简体中文</a> |
  <a href="README_zh-TW.md">繁體中文</a> |
  <a href="README_ja.md">日本語</a> |
  <a href="README_ko.md">한국어</a> |
  <a href="README_fr.md">Français</a> |
  <a href="README_de.md">Deutsch</a> |
  <a href="README_es.md">Español</a> |
  <a href="README_ru.md">Русский</a>
</p>

<h1 align="center"><img src="../assets/icon48.png" width="36" align="center" style="margin-bottom: -6px;" /> 基於多模態大模型的沉浸式網頁翻譯軟體 (Immersive Web Translator)</h1>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version" />
  <img src="https://img.shields.io/badge/Manifest-V3-green.svg" alt="Manifest" />
  <img src="https://img.shields.io/badge/license-MIT-orange.svg" alt="License" />
</p>

> [!IMPORTANT]
> **代碼公布說明**：本項目完整的源代碼、安裝腳本與程序包目前正在進行知識產權審查與登記。所有文件將在我們學術論文錄用/正式發表後，於本倉庫全量開源公布。目前您可以查看[演示影片](#🎥-演示影片)或閱讀下方技術文檔。

<p align="center">
  一款專為開發者和深度閱讀者打造的 <b>大型語言模型 (LLM)</b> 驅動的網頁翻譯擴充功能。它不僅提供精準的 AI 翻譯，更透過底層渲染優化，實現了接近原生網頁的反應速度。
</p>

---

## 📸 界面预览

| 插件弹窗 | API 配置 |
| :---: | :---: |
| ![插件弹窗](media/zh/extension_popup.png) | ![API 配置](media/zh/API_Configuration.png) |

| 阅读与翻译 | 存储与记录 | 备份与迁移 |
| :---: | :---: | :---: |
| ![阅读与翻译](media/zh/Translate&Read.png) | ![存储与记录](media/zh/Storage&Records.png) | ![备份与迁移](media/zh/Backup&Migrate.png) |

### 🎥 演示影片

<p align="center">
  <video src="media/video/Video Project 1.mp4" width="80%" controls>
    您的瀏覽器不支援 HTML5 影片播放。
  </video>
</p>

---

## ✨ 核心功能


- **🚀 極速順滑翻譯**
  - **無感秒翻體驗**：消除“原文閃爍”現象，翻譯結果如原生網頁般自然。
  - **智能請求優化**：基於段落聚合技術，大幅提升翻譯速度並節省 API Token。
  - **實時流式打字機**：支持流式輸出，翻譯結果逐句實時呈現，告別等待。

- **🎨 沉浸式交互體驗**
  - **🌍 多語言支持**：面板已適配 9 大語言，根據瀏覽器設置自動切換。
  - **智能懸浮球**：極簡設計，不打擾閱讀，實時反饋翻譯進度與狀態。
  - **網站記憶功能**：智能記憶“顯示原文”選項，同站跳轉不再反覆翻譯。
  - **三種展示模式**：提供行間雙語、左右分屏、僅顯譯文，滿足快覽與精讀需求。
  - **譯文人工糾錯**：右鍵點擊翻譯段落即可手動修改，打造完美閱讀體驗。

- **🛠️ 強悍的網頁兼容性**
  - **支持動態網站**：深度適配現代單頁應用，滑動或動態加載時翻譯不消失、排版不亂。
  - **深度穿透翻譯**：支持深入翻譯網頁內部複雜的隱藏組件（Shadow DOM）。

- **⚙️ 高階定制與數據資產**
  - **自由接入 LLM**：原生支持 OpenAI 兼容接口，可自由接入各類大模型或部署本地私有模型。
  - **自定義 Prompt**：支持注入自定義翻譯規則（如“保留術語”），讓 AI 聽從個性化指令。
  - **本地緩存省錢**：基於 IndexedDB 的海量緩存，歷史頁面秒級呈現，零 API Token 消耗。
  - **配置數據遷移**：支持 API 密鑰、配置及翻譯記錄的一鍵打包備份與無縫還原。

---

## 🛠️ 快速開始

- **1. 安裝擴充功能**

  - **Chrome / Edge 等 Chromium 瀏覽器**：
    1. 雙擊專案根目錄下的 [use-chrome-manifest.bat](use-chrome-manifest.bat) 切換為 Chromium 版本的設定。 *(Mac / Linux 用户请手动将 `manifest.chrome.json` 覆盖为 `manifest.json`)*
    2. 在瀏覽器網址列打開 `chrome://extensions/` 並開啟「開發者模式」。
    3. 點擊「載入未封裝的擴充功能」，選擇本專案根目錄。
  - **Firefox 瀏覽器**：
    1. 雙擊專案根目錄下的 [use-firefox-manifest.bat](use-firefox-manifest.bat) 切換為 Firefox 版本的設定。 *(Mac / Linux 用户请手动将 `manifest.firefox.json` 覆盖为 `manifest.json`)*
    2. 在瀏覽器網址列輸入並前往 `about:debugging#/runtime/this-firefox`。
    3. 點擊右側的 **「Load Temporary Add-on...」**。
    4. 選擇本專案根目錄下的 `manifest.json`。

- **2. 設定 API**

  - 點擊外掛圖示進入設定。
  - 填入您的 LLM API 設定。
  - 選擇目標語言。

- **3. 開始閱讀**

  - **自動翻譯**：系統會根據您的語種偏好自動觸發。
  - **手動控制**：透過右鍵選單或點擊懸浮球隨時切換。

---

## 🏗️ 技術架構

關於本擴充功能詳細的底層架構設計與渲染優化演算法，請參閱我們的學術論文：📄 **[點擊閱讀論文](https://#)**


---

## 📜 開源協議

本項目採用 [MIT License](../LICENSE) 協議。
