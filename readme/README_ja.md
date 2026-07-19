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

<h1 align="center"><img src="../assets/icon48.png" width="36" align="center" style="margin-bottom: -6px;" /> マルチモーダルLLMに基づく没入型Web翻訳ソフトウェア (Immersive Web Translator)</h1>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version" />
  <img src="https://img.shields.io/badge/Manifest-V3-green.svg" alt="Manifest" />
  <img src="https://img.shields.io/badge/license-MIT-orange.svg" alt="License" />
</p>

<p align="center">
  開発者およびディープリーダー向けに設計された、<b>大規模言語モデル（LLM）</b>駆動のWeb翻訳拡張機能です。正確なAI翻訳を提供するだけでなく、基盤となるレンダリングの最適化を通じて、ネイティブのWebページに近い応答速度を実現します。
</p>

---

## 📸 Interface Preview

| Extension Popup | API Configuration |
| :---: | :---: |
| ![Extension Popup](media/en/extension_popup.png) | ![API Configuration](media/en/API_Configuration.png) |

| Translate & Read | Storage & Records | Backup & Migrate |
| :---: | :---: | :---: |
| ![Translate & Read](media/en/Translate&Read.png) | ![Storage & Records](media/en/Storage&Records.png) | ![Backup & Migrate](media/en/Backup&Migrate.png) |

---

## ✨ コア機能


- **🚀 高速でスムーズな翻訳**
  - **ちらつきのない読書**: 原文のちらつきを排除し、翻訳されたページをネイティブのように見せます。
  - **スマートAPI最適化**: 段落の集約により、速度が大幅に向上し、APIトークンを節約します。
  - **リアルタイム表示**: ストリーミング出力をサポートし、翻訳を文ごとに瞬時にレンダリングします。

- **🎨 没入型のユーザー体験**
  - **🌍 多言語サポート**: パネルは9言語に適応し、ブラウザの設定に基づいて自動的に切り替わります。
  - **スマートホバーアシスタント**: ミニマリストのホバーボールが、読書を妨げることなくリアルタイムの進行状況を提供します。
  - **スマートメモリ**: 「原文を表示」の選択を記憶し、同じサイト内での再翻訳を防ぎます。
  - **3つの表示モード**: ざっと読むか、深く読むかに合わせて、行間バイリンガル、左右分割画面、翻訳のみを提供します。
  - **手動補正**: 翻訳されたセグメントを右クリックして手動で編集し、完璧な体験を実現します。

- **🛠️ 完璧なWeb互換性**
  - **動的サイトのサポート**: 現代のSPAに深く適応。スクロールや動的ロード中も翻訳はそのまま維持されます。
  - **深い翻訳**: 複雑な隠しWebコンポーネント（Shadow DOM）にシームレスに浸透します。

- **⚙️ 高いカスタマイズ性とデータ管理**
  - **独自のLLMを持ち込む**: OpenAI互換APIをネイティブにサポートし、大規模またはローカルのプライベートモデルを統合します。
  - **カスタムプロンプト**: 個人的な翻訳ルール（例：「専門用語を保持する」）を注入して、AI出力を調整します。
  - **コスト削減キャッシュ**: IndexedDBローカルストレージにより、訪問済みページの即時ロードを保証し、APIトークンコストをゼロにします。
  - **ワンクリックバックアップ**: すべてのAPIキー、設定、および翻訳履歴をデバイス間で安全にエクスポートおよびインポートします。

---

## 🛠️ クイックスタート

- **1. 拡張機能のインストール**

  - **Chrome / Edge およびその他のChromiumブラウザ**:
    1. ルートディレクトリの [use-chrome-manifest.bat](use-chrome-manifest.bat) をダブルクリックして、Chromium構成に切り替えます。 *(Mac/Linuxユーザー：`manifest.chrome.json`を`manifest.json`に手動でリネームしてください)*
    2. ブラウザで `chrome://extensions/` を開き、「デベロッパーモード」を有効にします。
    3. 「パッケージ化されていない拡張機能を読み込む」をクリックし、このプロジェクトのルートディレクトリを選択します。
  - **Firefox**:
    1. ルートディレクトリの [use-firefox-manifest.bat](use-firefox-manifest.bat) をダブルクリックして、Firefox構成に切り替えます。 *(Mac/Linuxユーザー：`manifest.firefox.json`を`manifest.json`に手動でリネームしてください)*
    2. ブラウザで `about:debugging#/runtime/this-firefox` に移動します。
    3. **「一時的なアドオンを読み込む...」** をクリックします。
    4. このプロジェクトのルートディレクトリにある `manifest.json` を選択します。

- **2. APIの構成**

  - 拡張機能アイコンをクリックして設定に入ります。
  - LLM API構成（例：OpenAI互換インターフェースなど）を入力します。
  - ターゲット言語を選択します。

- **3. 読み始めます**

  - **自動翻訳**: 言語設定に基づいて自動的にトリガーされます。
  - **手動コントロール**: 右クリックメニューまたはホバーボールをクリックして、いつでも切り替えることができます。


---

## 📜 ライセンス

このプロジェクトは [MIT License](../LICENSE) の下でライセンスされています。
