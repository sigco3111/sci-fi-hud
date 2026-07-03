# 🛸 sci-fi-hud

> Sci-fi cybernetics HUD in the style of Iron Man's JARVIS / hacking screens from sci-fi movies — Pure CSS + SVG animations

Complex rotating circular graphs, fast-flowing data streams, and randomly popping warning alerts ('ACCESS GRANTED', 'SYSTEM BREACH') — a tense cybernetics head-up display in a single HTML file.

[🇰🇷 한국어 (기본)](./README.md) · [🇺🇸 English](#)

---

## 🎬 Live Demo

> **👉 Coming soon (Work in progress)** — `MiniMax-M3` is working on it via OpenCode

| | |
|---|---|
| ![Status](https://img.shields.io/badge/Status-In_Development-F59E0B?style=flat-square) | ![Stack](https://img.shields.io/badge/Stack-Pure_CSS_+_SVG-FF6B6B?style=flat-square) |
| ![License](https://img.shields.io/badge/License-MIT-F1C40F?style=flat-square) | ![Deps](https://img.shields.io/badge/Dependencies-0-9CA3AF?style=flat-square) |

---

## 🎮 Quick Controls (planned)
1. Open the page — HUD activates automatically
2. Watch — rotating rings, data streams, warning popups
3. **Mouse interaction** — additional effects (TBD)
4. Fullscreen mode (F11) for the immersive HUD vibe

---

## 🤖 Attribution

This project's code is **auto-generated** using the following model and prompt.

| Field | Value |
|---|---|
| **Model** | MiniMax-M3 |
| **Environment** | OpenCode CLI |
| **Repository** | [`sigco3111/sci-fi-hud`](https://github.com/sigco3111/sci-fi-hud) |
| **License** | MIT |
| **Dependencies** | None (Pure CSS + SVG, single HTML) |

### 📝 Prompt Used

```
아이언맨의 자비스나 SF 영화에 나오는 해킹 화면처럼, 복잡한 원형 그래프가 회전하고 알 수 없는 데이터 스트림이 빠르게 흘러가며, 'ACCESS GRANTED', 'SYSTEM BREACH' 같은 경고창이 무작위로 팝업되는 매우 복잡하고 긴박감 넘치는 사이버네틱 헤드업 디스플레이(HUD) 화면을 HTML/CSS 애니메이션만으로 구현해줘.
Implementation Advice: Use Pure CSS Animations (Keyframes) and SVG for the cleanest circles and lines. Use transform: rotate(...) and opacity for the HUD elements. Javascript can be minimal, just to trigger classes or randomize text content. 모든 의존관계의 코드를 하나의 HTML에 담는 형태로 코드 작성.
```

---

## 🛠️ Tech Stack (planned)

- **Animations** — Pure CSS `@keyframes` + `transform: rotate(...)` + `opacity`
- **Graphics** — SVG (`<circle>`, `<path>`, `<line>`) — clean circles, lines, graphs
- **Language** — Vanilla JavaScript (text randomization only, minimal)
- **Bundle** — all dependencies embedded in single `index.html`

---

## 📂 Project Structure

```
sci-fi-hud/
├── index.html          # Single HTML (CSS + SVG + minimal JS)
├── README.md           # Korean (default)
├── README.en.md        # English version
├── LICENSE             # MIT License
└── .gitignore          # Node/IDE temp files exclusion
```

---

## 🚀 Run Locally

```bash
git clone https://github.com/sigco3111/sci-fi-hud.git
cd sci-fi-hud
open index.html        # macOS
# or open index.html in any browser directly
```

**No internet required** — all assets are embedded in the single HTML.

---

## 📜 License

MIT License — use, modify, and distribute freely.

---

> 🤖 *This README structure is adapted from the verified [neon-fluid](https://github.com/sigco3111/neon-fluid) and [gravity-typography](https://github.com/sigco3111/gravity-typography) mission templates.*
