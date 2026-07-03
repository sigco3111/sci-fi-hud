# 🛸 sci-fi-hud

> 아이언맨의 자비스/SF 영화 스타일 사이버네틱 헤드업 디스플레이(HUD) — Pure CSS + SVG 애니메이션 기반

복잡한 원형 그래프 회전, 빠르게 흘러가는 데이터 스트림, 'ACCESS GRANTED'/'SYSTEM BREACH' 같은 경고 팝업이 무작위로 등장하는 긴박감 넘치는 해킹 인터페이스를 단일 HTML로 구현합니다.

[🇰🇷 한국어 (기본)](#) · [🇺🇸 English](./README.en.md)

---

## 🎬 라이브 데모 (Live Demo)

> **👉 곧 공개됩니다 (Work in progress)** — OpenCode에서 `MiniMax-M3` 모델이 작업 중

| | |
|---|---|
| ![Status](https://img.shields.io/badge/Status-In_Development-F59E0B?style=flat-square) | ![Stack](https://img.shields.io/badge/Stack-Pure_CSS_+_SVG-FF6B6B?style=flat-square) |
| ![License](https://img.shields.io/badge/License-MIT-F1C40F?style=flat-square) | ![Deps](https://img.shields.io/badge/Dependencies-0-9CA3AF?style=flat-square) |

---

## 🎮 빠른 사용법 (예정)
1. 페이지 열기 — 화면이 자동으로 SF HUD 모드로 활성화
2. 잠시 관전 — 원형 그래프 회전, 데이터 스트림 흘러감, 경고 팝업 등장
3. **마우스 인터랙션** — 추가 효과 트리거 (미정)
4. 풀스크린 모드(F11)로 정통 HUD 분위기 극대화

---

## 🤖 생성 정보 (Attribution)

이 프로젝트의 코드는 아래 모델과 프롬프트를 이용해 **자동으로 생성**됩니다.

| 항목 | 값 |
|---|---|
| **모델** | MiniMax-M3 |
| **실행 환경** | OpenCode CLI |
| **저장소** | [`sigco3111/sci-fi-hud`](https://github.com/sigco3111/sci-fi-hud) |
| **라이선스** | MIT |
| **의존성** | 없음 (Pure CSS + SVG, 단일 HTML) |

### 📝 사용된 프롬프트 (원문)

```
아이언맨의 자비스나 SF 영화에 나오는 해킹 화면처럼, 복잡한 원형 그래프가 회전하고 알 수 없는 데이터 스트림이 빠르게 흘러가며, 'ACCESS GRANTED', 'SYSTEM BREACH' 같은 경고창이 무작위로 팝업되는 매우 복잡하고 긴박감 넘치는 사이버네틱 헤드업 디스플레이(HUD) 화면을 HTML/CSS 애니메이션만으로 구현해줘.
Implementation Advice: Use Pure CSS Animations (Keyframes) and SVG for the cleanest circles and lines. Use transform: rotate(...) and opacity for the HUD elements. Javascript can be minimal, just to trigger classes or randomize text content. 모든 의존관계의 코드를 하나의 HTML에 담는 형태로 코드 작성.
```

---

## 🛠️ 기술 스택 (예정)

- **애니메이션** — Pure CSS `@keyframes` + `transform: rotate(...)` + `opacity`
- **그래픽** — SVG (`<circle>`, `<path>`, `<line>`) — 깔끔한 원/선/그래프
- **언어** — Vanilla JavaScript (randomize text만, minimal)
- **번들** — 모든 의존성을 단일 `index.html`에 임베드

---

## 📂 프로젝트 구조

```
sci-fi-hud/
├── index.html          # 단일 HTML 파일 (CSS + SVG + minimal JS)
├── README.md           # 본 문서 (한국어)
├── README.en.md        # English version
├── LICENSE             # MIT License
└── .gitignore          # Node/IDE 임시 파일 제외
```

---

## 🚀 로컬 실행

```bash
git clone https://github.com/sigco3111/sci-fi-hud.git
cd sci-fi-hud
open index.html   # macOS
# 또는 브라우저에서 index.html 직접 열기
```

**인터넷 연결 불필요** — 모든 자원이 단일 HTML에 내장되어 있습니다.

---

## 📜 라이선스

MIT License — 자유롭게 사용, 수정, 배포하세요.

---

> 🤖 *이 리드미의 README 구조는 검증된 [neon-fluid](https://github.com/sigco3111/neon-fluid), [gravity-typography](https://github.com/sigco3111/gravity-typography) 미션 형식을 차용했습니다.*
