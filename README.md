<p align="center">
  <a href="README.md">English</a> |
  <a href="readme/README_zh-CN.md">简体中文</a> |
  <a href="readme/README_zh-TW.md">繁體中文</a> |
  <a href="readme/README_ja.md">日本語</a> |
  <a href="readme/README_ko.md">한국어</a> |
  <a href="readme/README_fr.md">Français</a> |
  <a href="readme/README_de.md">Deutsch</a> |
  <a href="readme/README_es.md">Español</a> |
  <a href="readme/README_ru.md">Русский</a>
</p>

<h1 align="center"><img src="assets/icon48.png" width="36" align="center" style="margin-bottom: -6px;" /> Immersive Web Translator based on Large Language Models</h1>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version" />
  <img src="https://img.shields.io/badge/Manifest-V3-green.svg" alt="Manifest" />
  <img src="https://img.shields.io/badge/license-MIT-orange.svg" alt="License" />
</p>

<p align="center">
  A web translation extension powered by <b>Large Language Models (LLMs)</b>, designed specifically for developers and deep readers. It not only provides accurate AI translation but also achieves near-native web page response speeds through underlying rendering optimizations.
</p>

---

## 📸 Interface Preview

| Extension Popup | API Configuration |
| :---: | :---: |
| ![Extension Popup](readme/media/en/extension_popup.png) | ![API Configuration](readme/media/en/API_Configuration.png) |

| Translate & Read | Storage & Records | Backup & Migrate |
| :---: | :---: | :---: |
| ![Translate & Read](readme/media/en/Translate&Read.png) | ![Storage & Records](readme/media/en/Storage&Records.png) | ![Backup & Migrate](readme/media/en/Backup&Migrate.png) |

### 🎥 Demo Video

<p align="center">
  <video src="readme/media/video/Video Project 1.mp4" width="80%" controls>
    Your browser does not support the video tag.
  </video>
</p>

---

## ✨ Core Features


- **🚀 Fast & Smooth Translation**
  - **Zero-Flicker Reading**: Eliminates original text flashing, making translated pages look native.
  - **Smart API Optimization**: Paragraph aggregation significantly boosts speed and saves API Tokens.
  - **Real-Time Display**: Supports streaming output, rendering translations sentence-by-sentence instantly.

- **🎨 Immersive User Experience**
  - **🌍 Multi-Language Support**: Panel adapted to 9 languages, auto-switching based on browser settings.
  - **Smart Hover Assistant**: Minimalist hover ball provides real-time progress without disrupting reading.
  - **Smart Memory**: Remembers your "Show Original" choice, preventing re-translation across the same site.
  - **Three Display Modes**: Interlinear Bilingual, Split Screen, and Translation Only to suit skimming or deep reading.
  - **Manual Correction**: Right-click any translated segment to edit it manually for a perfect experience.

- **🛠️ Perfect Web Compatibility**
  - **Dynamic Site Support**: Deeply adapted for modern SPAs. Translations stay intact during scrolling or dynamic loading.
  - **Deep Translation**: Penetrates complex hidden web components (Shadow DOM) seamlessly.

- **⚙️ High Customizability & Data Management**
  - **Bring Your Own LLM**: Natively supports OpenAI-compatible APIs to integrate any large or local private models.
  - **Custom Prompts**: Inject personal translation rules (e.g., "keep technical terms") for tailored AI outputs.
  - **Cost-Saving Cache**: IndexedDB local storage ensures instant loads for visited pages with zero API token cost.
  - **One-Click Backup**: Safely export and import all API keys, settings, and translation history across devices.

---

## 🛠️ Quick Start

- **1. Install Extension**

  - **Chrome / Edge and other Chromium browsers**:
    1. Double-click [use-chrome-manifest.bat](use-chrome-manifest.bat) in the root directory to switch to Chromium configuration. *(Mac/Linux users: please manually rename `manifest.chrome.json` to `manifest.json`)*
    2. Open `chrome://extensions/` in your browser and enable "Developer mode".
    3. Click "Load unpacked" and select the root directory of this project.
  - **Firefox**:
    1. Double-click [use-firefox-manifest.bat](use-firefox-manifest.bat) in the root directory to switch to Firefox configuration. *(Mac/Linux users: please manually rename `manifest.firefox.json` to `manifest.json`)*
    2. Go to `about:debugging#/runtime/this-firefox` in your browser.
    3. Click **"Load Temporary Add-on..."**.
    4. Select `manifest.json` in the root directory of this project.
  - **Safari**: You can run `xcrun safari-web-extension-converter /path/to/project` via macOS terminal to convert it into an Xcode project and load it in Safari, or check "Allow Unsigned Extensions" in the Safari Developer menu.

- **2. Configure API**

  - Click the extension icon to enter settings.
  - Fill in your LLM API configuration (e.g., OpenAI compatible interfaces).
  - Select target language.

- **3. Start Reading**

  - **Auto Translation**: Triggers automatically based on your language preferences.
  - **Manual Control**: Switch at any time via right-click menu or clicking the hover ball.

---

## 🏗️ Technical Architecture

For detailed architectural design and rendering optimization algorithms, please refer to our academic paper: 📄 **[Read the Paper](https://#)**


---

## 📜 License

This project is licensed under the [MIT License](LICENSE) .
