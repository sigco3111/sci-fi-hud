# 🛸 sci-fi-hud

> J.A.R.V.I.S.-style cybernetics Head-Up Display — Pure CSS + SVG animations

A 24-module complex HUD inspired by Iron Man's JARVIS and sci-fi hacking screens — rotating ring graphs, fast-flowing matrix rain, randomly popping warning alerts (`ACCESS GRANTED`, `SYSTEM BREACH`), 3D wireframe icosahedron, mouse parallax effects. Single HTML file, zero dependencies, fully offline.

[🇰🇷 한국어 (기본)](./README.md) · [🇺🇸 English](#)

---

## 🎬 Live Demo

> **👉 [https://sci-fi-hud.vercel.app/](https://sci-fi-hud.vercel.app/)** — Strongly recommend fullscreen (F11)

| | |
|---|---|
| ![Demo](https://img.shields.io/badge/Live-Demo-7C3AED?style=for-the-badge&logo=vercel&logoColor=white) | [![Repo](https://img.shields.io/badge/GitHub-sigco3111%2Fsci--fi--hud-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sigco3111/sci-fi-hud) |
| ![Status](https://img.shields.io/badge/Status-Live-22C55E?style=flat-square) | ![Stack](https://img.shields.io/badge/Stack-Pure_CSS_+_SVG-FF6B6B?style=flat-square) |
| ![License](https://img.shields.io/badge/License-MIT-F1C40F?style=flat-square) | ![Deps](https://img.shields.io/badge/Dependencies-0-9CA3AF?style=flat-square) |
| ![Size](https://img.shields.io/badge/Size-99_KB_single_file-FFA500?style=flat-square) | ![Offline](https://img.shields.io/badge/Offline-OK-22C55E?style=flat-square) |

### 🎮 Quick Controls
1. Click the demo link above → page opens in your browser
2. **Boot sequence** auto-plays (1.8s) — `J.A.R.V.I.S.` title appears
3. Watch 24 modules run in real-time:
   - ⏱️ Live clock (HH:MM:SS) + uptime counter
   - 📊 CPU/MEM/DSK/NET process bars + sparklines
   - 🌐 Data stream (hex) flowing infinitely
   - 🛰️ GPS micro-jitter + threat level fluctuating
   - 🚨 Random WARNING popups (`ACCESS GRANTED`, `SYSTEM BREACH` etc)
4. **Mouse interaction**
   - **Move** — center HUD parallax + icosahedron rotation
   - **Click** — screen shake + ripple effect
   - **Spacebar** — force-trigger WARNING
   - **Esc** — fullscreen overlay
5. **Fullscreen (F11)** — maximize the HUD vibe

---

## 🤖 Attribution

This project's code is **auto-generated** using the model and prompt below.

| Field | Value |
|---|---|
| **Model** | MiniMax-M3 |
| **Environment** | OpenCode CLI |
| **Repository** | [`sigco3111/sci-fi-hud`](https://github.com/sigco3111/sci-fi-hud) |
| **License** | MIT |
| **Dependencies** | None (Pure CSS + SVG, 99KB single HTML) |

### 📝 Prompt Used

```
아이언맨의 자비스나 SF 영화에 나오는 해킹 화면처럼, 복잡한 원형 그래프가 회전하고 알 수 없는 데이터 스트림이 빠르게 흘러가며, 'ACCESS GRANTED', 'SYSTEM BREACH' 같은 경고창이 무작위로 팝업되는 매우 복잡하고 긴박감 넘치는 사이버네틱 헤드업 디스플레이(HUD) 화면을 HTML/CSS 애니메이션만으로 구현해줘.
Implementation Advice: Use Pure CSS Animations (Keyframes) and SVG for the cleanest circles and lines. Use transform: rotate(...) and opacity for the HUD elements. Javascript can be minimal, just to trigger classes or randomize text content. 모든 의존관계의 코드를 하나의 HTML에 담는 형태로 코드 작성.
```

---

## ✨ Features

- 🛸 **24 HUD modules** — Clock, Diagnostics, System Metrics, Uptime, Process Bars, Data Stream, Access Log, File Index, GPS Jitter, Threat Level, Warnings, Alerts, 3D Wireframe, and more
- 🎨 **33 `@keyframes` animations** — rotation, pulse, glitch, matrix rain, sparkle, boot sequence
- 📐 **SVG graphics** — 50 `<circle>` + 65 `<line>` + 15 `<path>` + 17 `<svg>` containers
- ⚡ **Real-time data updates** — 17 `setInterval` (0.7~22s cadence) constantly refreshing hex streams / metrics / threat level
- 🌧️ **Matrix Rain** — Korean + Latin characters flowing from screen top
- 🎲 **Random WARNING popups** — 9 messages (`ACCESS GRANTED`, `SYSTEM BREACH`, `THREAT DETECTED` etc)
- 💥 **Full-screen ALERT OVERLAY** — 45% chance every 9 seconds
- 🎭 **Mouse parallax** — 3D icosahedron follows mouse
- 🌊 **Click ripple + screen shake** — click visual feedback
- 🔤 **JetBrains Mono + Orbitron fonts** — cyberpunk vibe
- 📦 **Single HTML (99KB)** — zero external dependencies
- 🔒 **Fully offline-capable** — all assets self-embedded
- ⚙️ **Customizable** — one CSS variable for accent color

---

## 🚀 Run It

### Option 1: Live Demo (Vercel) — easiest
👉 [https://sci-fi-hud.vercel.app/](https://sci-fi-hud.vercel.app/) — works out of the box.

### Option 2: Open Locally
```bash
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```
**No internet required** — all assets are embedded.

### Option 3: Local Server (recommended)
```bash
python3 -m http.server 8000
# → http://localhost:8000
```

---

## 🎮 Controls

| Input | Effect |
|---|---|
| **Watch (default)** | 24 modules auto-run, random WARNING/ALERT popups |
| **Mouse move** | Center HUD parallax + 3D icosahedron rotation |
| **Mouse click** | Screen shake + ripple effect |
| **Spacebar** | Force-trigger WARNING |
| **Esc** | Fullscreen overlay |
| **Fullscreen (F11)** | Maximize HUD vibe |

---

## 🛠️ Tech Stack

| Domain | Technology |
|---|---|
| **Animation** | Pure CSS `@keyframes` (33) + `transform: rotate/translate/scale` + `opacity` |
| **Graphics** | SVG (`<circle>`, `<line>`, `<path>`, `<text>`) — clean circles, lines, graphs |
| **Layout** | CSS Grid + Flexbox |
| **Fonts** | JetBrains Mono + Orbitron (with system fallback) |
| **Live data** | 17 `setInterval` (hex/metrics/threat level refreshing) |
| **JS role** | Minimal — `setInterval` triggers + class toggling + random text |
| **Dependencies** | **Zero** (everything in single HTML) |
| **Bundle size** | 99KB (gzip ~24KB) |
| **Browsers** | Chrome/Firefox/Safari/Edge — modern (CSS Grid + clamp()) |

### CSS Design Tokens (top of `<style>`)

```css
:root {
  --bg:          #02070d;   /* background */
  --primary:     #00f0ff;   /* electric cyan (accent) */
  --accent:      #ff2d75;   /* pink (warning) */
  --ok:          #4dff9c;   /* green (success) */
  --warn:        #ffd23f;   /* yellow (caution) */
  --danger:      #ff3c4d;   /* red (danger) */
  --text:        #d8e9f5;   /* body text */
  --text-dim:    #5a7385;   /* secondary text */
}
```

Change just `--primary` and the entire HUD tone shifts (cyan → lime / magenta / gold etc).

---

## 📂 Project Structure

```
sci-fi-hud/
├── index.html          # Single HTML file (CSS + SVG + minimal JS)
├── README.md           # Korean (default)
├── README.en.md        # English version
├── LICENSE             # MIT
└── .gitignore          # Node/IDE/OpenCode temp file exclusion
```

---

## 🎨 Design Choices

Decisions made during brainstorming:

| Decision | Choice | Rationale |
|---|---|---|
| **Rendering strategy** | SVG over Canvas | 50 `<circle>` + 65 `<line>` via CSS, no per-frame redraw |
| **Animation** | CSS `@keyframes` + GPU-accelerated `transform` | 60fps stable without requestAnimationFrame loop |
| **JS role** | Minimal (`setInterval` + class toggling) | Let CSS handle what it can, JS only for live data |
| **Color palette** | Electric cyan (`#00f0ff`) + pink accent | cyberpunk classic + signature film HUD |
| **Fonts** | JetBrains Mono + Orbitron | monospace (data) + display (title) split |
| **Module count** | 24 (intentionally excessive) | meet "very complex and tense" requirement |
| **Live refresh** | 17 setInterval | never feels static, constant change |
| **WARNING frequency** | avg 4-22s random | short messages, frequent pulse → tension maintained |
| **Bundle** | single 99KB HTML | zero CDN deps, offline-capable |

### Customize It Yourself

Tune the CSS variables at the top of `index.html` to change the vibe:

```css
/* Matrix green */
:root { --primary: #4dff9c; --accent: #00f0ff; }

/* Tron orange */
:root { --primary: #ff7800; --accent: #00d2ff; }

/* Blade Runner magenta */
:root { --primary: #ff2d75; --accent: #00f0ff; }
```

For deeper tuning, see §15 (CSS LAYOUT) and §18 (3D WIREFRAME) in `index.html`:
- Icosahedron vertex array → swap for other polyhedra
- WARNING message list → add Korean/English variants
- `setInterval` cadence → faster/slower real-time updates

---

## 📜 License

MIT © 2026 sigco3111

---

## 🙏 Acknowledgments

This project was auto-generated by the [MiniMax-M3](https://example.com) model in the OpenCode CLI environment. Prompt engineering and design decisions were made by the repository owner.

---

> 🤖 *This README structure is adapted from the verified [neon-fluid](https://github.com/sigco3111/neon-fluid) mission template.*
