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

<h1 align="center"><img src="../assets/icon48.png" width="36" align="center" style="margin-bottom: -6px;" /> 멀티모달 LLM 기반 몰입형 웹 번역기 (Immersive Web Translator)</h1>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version" />
  <img src="https://img.shields.io/badge/Manifest-V3-green.svg" alt="Manifest" />
  <img src="https://img.shields.io/badge/license-MIT-orange.svg" alt="License" />
</p>

<p align="center">
  개발자와 심층 독자를 위해 설계된 <b>대형 언어 모델(LLM)</b> 구동 웹 번역 확장 프로그램입니다. 정확한 AI 번역을 제공할 뿐만 아니라 기본 렌더링 최적화를 통해 기본 웹 페이지에 가까운 응답 속도를 달성합니다.
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

## ✨ 핵심 기능

- **🚀 극한의 성능 파이프라인**

  - **렌더 게이트 (Render Gate)**: 독창적인 렌더링 잠금 기술. 캐시 미스 시 "통과"하여 번역 프로세스 중 흰 화면 불안을 완전히 제거합니다.
  - **스냅샷-런타임 매칭**: 밀리초 수준의 메모리 스냅샷 기술로 페이지 이동 시 읽은 콘텐츠를 "순간 번역"합니다.
  - **적응형 일괄 처리**: 16~20개의 텍스트 세그먼트를 지능적으로 집계하여 동시 번역함으로써 API 요청 횟수를 40% 이상 줄입니다.

- **🎨 몰입형 UI 상호 작용**

  - **🌍 네이티브 국제화 (i18n)**: 인터페이스는 9개 주요 언어에 완벽하게 적응되어 브라우저 환경에 따라 원활하게 전환됩니다.
  - **스마트 호버 볼**: 번역 진행률, 언어 상태 및 파이프라인 상태에 대한 실시간 피드백을 제공하는 미니멀리스트 디자인.
  - **도메인 인식 고정성**: 수동으로 "원문 보기"를 선택한 후 현재 사이트 내의 하위 링크 이동 시 상태가 자동으로 유지되며, 사이트를 전환하면 자동으로 재설정됩니다.
  - **이중 언어 / 전체 대체**: 빠른 탐색에서 딥 러닝에 이르는 다양한 시나리오를 충족하기 위해 여러 표시 모드를 지원합니다.


---

## 📜 라이선스

이 프로젝트는 [MIT License](../LICENSE)에 따라 라이선스가 부여됩니다。
