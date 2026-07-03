# 🛸 sci-fi-hud

> J.A.R.V.I.S. 스타일 사이버네틱 헤드업 디스플레이 — Pure CSS + SVG 애니메이션 기반

자비스(Iron Man JARVIS)나 SF 영화의 해킹 화면처럼, 24개 모듈로 구성된 복잡한 HUD가 실시간으로 작동합니다 — 회전하는 원형 그래프, 흘러가는 매트릭스 데이터 비, 무작위로 팝업되는 `ACCESS GRANTED` / `SYSTEM BREACH` 경고창, 3D 와이어프레임 이코사헤드론, 마우스 패럴랙스 효과까지. 단일 HTML 파일 + zero dependencies, 오프라인에서도 완전 작동합니다.

[🇰🇷 한국어 (기본)](#) · [🇺🇸 English](./README.en.md)

---

## 🎬 라이브 데모 (Live Demo)

> **👉 [https://sci-fi-hud.vercel.app/](https://sci-fi-hud.vercel.app/)** — 풀스크린으로 보는 것을 강력 권장 (F11)

| | |
|---|---|
| ![Demo](https://img.shields.io/badge/Live-Demo-7C3AED?style=for-the-badge&logo=vercel&logoColor=white) | [![Repo](https://img.shields.io/badge/GitHub-sigco3111%2Fsci--fi--hud-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sigco3111/sci-fi-hud) |
| ![Status](https://img.shields.io/badge/Status-Live-22C55E?style=flat-square) | ![Stack](https://img.shields.io/badge/Stack-Pure_CSS_+_SVG-FF6B6B?style=flat-square) |
| ![License](https://img.shields.io/badge/License-MIT-F1C40F?style=flat-square) | ![Deps](https://img.shields.io/badge/Dependencies-0-9CA3AF?style=flat-square) |
| ![Size](https://img.shields.io/badge/Size-99_KB_single_file-FFA500?style=flat-square) | ![Offline](https://img.shields.io/badge/Offline-OK-22C55E?style=flat-square) |

### 🎮 빠른 사용법
1. 위 데모 링크 클릭 → 브라우저에서 페이지 열기
2. **부팅 시퀀스** 자동 재생 (1.8초) — `J.A.R.V.I.S.` 타이틀 등장
3. 잠시 관전 — 24개 모듈이 실시간으로 작동:
   - ⏱️ 실시간 클럭 (HH:MM:SS) + 업타임 카운터
   - 📊 CPU/MEM/DSK/NET 프로세스 바 + 스파크라인
   - 🌐 데이터 스트림 (16진수 hex) 무한 흘러감
   - 🛰️ GPS 마이크로 지터 + 위협 레벨 동적 변화
   - 🚨 무작위 WARNING 팝업 (`ACCESS GRANTED`, `SYSTEM BREACH` 등)
4. **마우스 인터랙션**
   - **이동** — 중앙 HUD 패럴랙스 + 클릭 시 ripple effect
   - **클릭** — 화면 흔들림 (screen shake) + icosahedron 회전
   - **Spacebar** — WARNING 강제 트리거
   - **Esc** — 풀스크린 오버레이
5. **풀스크린 (F11)** — 정통 HUD 정취 극대화

---

## 🤖 생성 정보 (Attribution)

이 프로젝트의 코드는 아래 모델과 프롬프트를 이용해 **자동으로 생성**되었습니다.

| 항목 | 값 |
|---|---|
| **모델** | MiniMax-M3 |
| **실행 환경** | OpenCode CLI |
| **저장소** | [`sigco3111/sci-fi-hud`](https://github.com/sigco3111/sci-fi-hud) |
| **라이선스** | MIT |
| **의존성** | 없음 (Pure CSS + SVG, 단일 HTML 99KB) |

### 📝 사용된 프롬프트 (원문)

```
아이언맨의 자비스나 SF 영화에 나오는 해킹 화면처럼, 복잡한 원형 그래프가 회전하고 알 수 없는 데이터 스트림이 빠르게 흘러가며, 'ACCESS GRANTED', 'SYSTEM BREACH' 같은 경고창이 무작위로 팝업되는 매우 복잡하고 긴박감 넘치는 사이버네틱 헤드업 디스플레이(HUD) 화면을 HTML/CSS 애니메이션만으로 구현해줘.
Implementation Advice: Use Pure CSS Animations (Keyframes) and SVG for the cleanest circles and lines. Use transform: rotate(...) and opacity for the HUD elements. Javascript can be minimal, just to trigger classes or randomize text content. 모든 의존관계의 코드를 하나의 HTML에 담는 형태로 코드 작성.
```

---

## ✨ 주요 특징 (Features)

- 🛸 **24개 HUD 모듈** — Clock, Diagnostics, System Metrics, Uptime, Process Bars, Data Stream, Access Log, File Index, GPS Jitter, Threat Level, Warnings, Alerts, 3D Wireframe 등
- 🎨 **33개 `@keyframes` 애니메이션** — 회전, 펄스, 글리치, 매트릭스 레인, 스파클, 부팅 시퀀스
- 📐 **SVG 그래픽** — 50개 `<circle>` + 65개 `<line>` + 15개 `<path>` + 17개 `<svg>` 컨테이너
- ⚡ **실시간 데이터 라이브 업데이트** — 17개 `setInterval` (0.7~22초 주기)이 hex 스트림/메트릭/위협 레벨 무작위 갱신
- 🌧️ **Matrix Rain** — 한국어 + 라틴 문자가 화면 상단에서 흘러내림
- 🎲 **무작위 WARNING 팝업** — 9종 메시지 (`ACCESS GRANTED`, `SYSTEM BREACH`, `THREAT DETECTED` 등)
- 💥 **풀스크린 ALERT OVERLAY** — 9초마다 45% 확률로 화면 가득 플래시
- 🎭 **마우스 패럴랙스** — 3D icosahedron이 마우스 따라 회전
- 🌊 **클릭 ripple + screen shake** — 클릭 시 시각 피드백
- 🔤 **JetBrains Mono + Orbitron font** — cyberpunk 분위기
- 📦 **단일 HTML (99KB)** — 외부 의존성 0개, 인덱스만 열면 실행
- 🔒 **오프라인 동작 가능** — 모든 자원이 자체 임베드
- ⚙️ **커스터마이즈** — CSS 변수 한 줄로 액센트 색 변경 가능

---

## 🚀 실행 방법 (Quick Start)

### 방법 1: 라이브 데모 (Vercel) — 가장 간단
👉 [https://sci-fi-hud.vercel.app/](https://sci-fi-hud.vercel.app/) — 별도 설치 없이 바로 실행됩니다.

### 방법 2: 그냥 브라우저로 열기
```bash
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```
**인터넷 연결 불필요** — 모든 자원이 단일 HTML에 내장되어 있습니다.

### 방법 3: 로컬 서버 (권장)
```bash
python3 -m http.server 8000
# → http://localhost:8000
```

---

## 🎮 조작법 (Controls)

| 입력 | 효과 |
|---|---|
| **관전 (기본)** | 24개 모듈 자동 작동, WARNING/ALERT 무작위 팝업 |
| **마우스 이동** | 중앙 HUD 패럴랙스 + 3D icosahedron 회전 |
| **마우스 클릭** | 화면 흔들림(screen shake) + ripple effect |
| **Spacebar** | WARNING 즉시 트리거 |
| **Esc** | 풀스크린 오버레이 |
| **풀스크린 (F11)** | HUD 분위기 극대화 |

---

## 🛠️ 기술 스택 (Tech Stack)

| 영역 | 사용 기술 |
|---|---|
| **애니메이션** | Pure CSS `@keyframes` (33개) + `transform: rotate/translate/scale` + `opacity` |
| **그래픽** | SVG (`<circle>`, `<line>`, `<path>`, `<text>`) — 깔끔한 원/선/그래프 |
| **레이아웃** | CSS Grid + Flexbox |
| **폰트** | JetBrains Mono + Orbitron (system fallback 포함) |
| **데이터 라이브** | `setInterval` 17개로 hex/메트릭/위협 레벨 갱신 |
| **JS 역할** | 최소 — `setInterval` 트리거 + 클래스 토글 + 무작위 텍스트 |
| **의존성** | **0개** (모든 게 단일 HTML에 임베드) |
| **번들 크기** | 99KB (gzip ~24KB) |
| **브라우저** | Chrome/Firefox/Safari/Edge — 모던 (CSS Grid + clamp() 지원) |

### CSS 디자인 토큰 (`<style>` 최상단)

```css
:root {
  --bg:          #02070d;   /* 배경 */
  --primary:     #00f0ff;   /* 일렉트릭 시안 (액센트) */
  --accent:      #ff2d75;   /* 핑크 (경고) */
  --ok:          #4dff9c;   /* 그린 (성공) */
  --warn:        #ffd23f;   /* 옐로우 (주의) */
  --danger:      #ff3c4d;   /* 레드 (위험) */
  --text:        #d8e9f5;   /* 본문 텍스트 */
  --text-dim:    #5a7385;   /* 보조 텍스트 */
}
```

원하는 분위기에 따라 `--primary` 값 하나만 바꾸면 전체 HUD 톤이 바뀝니다 (cyan → lime / magenta / gold 등).

---

## 📂 프로젝트 구조

```
sci-fi-hud/
├── index.html          # 단일 HTML 파일 (CSS + SVG + minimal JS)
├── README.md           # 한국어 (기본)
├── README.en.md        # English version
├── LICENSE             # MIT
└── .gitignore          # Node/IDE/OpenCode 임시 파일 제외
```

---

## 🎨 디자인 결정 (Design Choices)

브레인스토밍 단계에서 내린 결정:

| 결정 포인트 | 선택 | 이유 |
|---|---|---|
| **렌더링 전략** | SVG over Canvas | 50개 `<circle>` + 65 `<line>` CSS로 즉시 표시 가능, Canvas는 매 프레임 redraw |
| **애니메이션** | CSS `@keyframes` + GPU 가속 `transform` | requestAnimationFrame 루프 없이도 60fps 안정 |
| **JS 역할** | 최소 (`setInterval` + 클래스 토글) | CSS로 가능한 건 전부 CSS에서, JS는 데이터 라이브 갱신만 |
| **색 팔레트** | 일렉트릭 시안(`#00f0ff`) + 핑크 액센트 | 사이버펑크 정통 + 영화 HUD 시그니처 |
| **폰트** | JetBrains Mono + Orbitron | 모노스페이스(데이터) + 디스플레이(타이틀) 분리 |
| **모듈 수** | 24개 (의도적 과잉) | "아주 복잡하고 긴박감 넘치는" 요구사항 충족 |
| **라이브 갱신** | 17개 setInterval | 화면 정적 느낌 없이 끊임없이 변화 |
| **WARNING 빈도** | 평균 4-22초마다 무작위 | 강도는 짧게, 빈도는 자주 (긴장 유지) |
| **번들** | 단일 HTML 99KB | CDN 의존성 0, 오프라인 동작 가능 |

### 직접 커스터마이즈하고 싶다면

`index.html` 최상단 CSS 변수 한 줄로 분위기를 바꿀 수 있어요:

```css
/* 매트릭스 그린 */
:root { --primary: #4dff9c; --accent: #00f0ff; }

/* 트론 오렌지 */
:root { --primary: #ff7800; --accent: #00d2ff; }

/* 블레이드러너 마젠타 */
:root { --primary: #ff2d75; --accent: #00f0ff; }
```

더 깊이 튜닝하려면 `index.html`의 §15 (CSS LAYOUT) 또는 §18 (3D WIREFRAME)를 참고해서:
- icosahedron 정점 배열 → 다른 다면체로 교체 가능
- WARNING 메시지 리스트 → 한국어/영문 추가 가능
- `setInterval` 주기 → 더 빠르거나 느리게 조정 가능

---

## 📜 License

MIT © 2026 sigco3111

---

## 🙏 Acknowledgments

이 프로젝트는 [MiniMax-M3](https://example.com) 모델과 OpenCode CLI 환경에서 생성되었습니다. 프롬프트 엔지니어링과 디자인 결정은 저장소 소유자가 직접 수행했습니다.

---

> 🤖 *이 README 구조는 검증된 [neon-fluid](https://github.com/sigco3111/neon-fluid) 미션 형식을 차용했습니다.*
