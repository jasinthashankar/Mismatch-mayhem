# 🧠 Mismatch Mayhem — The Ultimate Memory Challenge ⚡

Mismatch Mayhem is a premium, fully-responsive, single-file browser memory-matching game crafted using HTML5, CSS3, and Vanilla JavaScript. The game features an immersive visual design, live-synthesized audio effects, multiple difficulty settings, power-ups, customizable timers, a progression system, achievements, and persistent local statistics.

---

## 🚀 Live Demo

Check out the live deployment of Mismatch Mayhem:
[![Vercel Deployment](https://img.shields.io/badge/Vercel-Deployed-black?style=for-the-badge&logo=vercel)](https://mismatch-mayhem.vercel.app)

*(Note: The link above points to the deployment URL. We will update it once the Vercel deploy finishes successfully).*

---

## 🛡️ Project Badges

<div align="center">

[![GitHub License](https://img.shields.io/github/license/jasinthashankar/Mismatch-mayhem?style=for-the-badge&color=blue)](https://github.com/jasinthashankar/Mismatch-mayhem/blob/main/LICENSE)
[![GitHub Repo Size](https://img.shields.io/github/repo-size/jasinthashankar/Mismatch-mayhem?style=for-the-badge&color=success)](https://github.com/jasinthashankar/Mismatch-mayhem)
[![GitHub Languages Count](https://img.shields.io/github/languages/count/jasinthashankar/Mismatch-mayhem?style=for-the-badge&color=orange)](https://github.com/jasinthashankar/Mismatch-mayhem)
[![GitHub Contributors](https://img.shields.io/github/contributors/jasinthashankar/Mismatch-mayhem?style=for-the-badge&color=red)](https://github.com/jasinthashankar/Mismatch-mayhem/graphs/contributors)

</div>

---

## ✨ Key Features

- 🎮 **Adaptive Game Modes**: Choose from 5 difficulty levels:
  - **Easy**: 4 cards, 5 lives, 60s
  - **Medium**: 8 cards, 5 lives, 90s
  - **Hard**: 16 cards, 6 lives, 130s
  - **Expert**: 24 cards, 7 lives, 170s
  - **Nightmare**: 36 cards, 8 lives, 220s
- ⏱️ **Customizable Countdown**: Override standard timers with your own custom limit (from 15 seconds up to 10 minutes).
- ❄️ **Strategic Power-ups**: Rescue tight games using:
  - 💡 **Hint**: Briefly highlight a matching pair.
  - ❄️ **Freeze**: Pause the countdown timer for 5 seconds.
  - ❤️‍🩹 **Extra Life**: Grant yourself 1 additional life.
  - 👁 **Reveal**: Temporarily flip all cards face-up.
  - ✨ **2x Score**: Double all match points for 15 seconds.
  - 🔀 **Shuffle**: Reshuffle all remaining unmatched cards on the board.
- 🎵 **Synthesized Sound Engine**: Audio synthesized directly in-browser using the Web Audio API—no external assets or heavy files required!
- 🎨 **Visual Themes**: Immerse yourself in 9 different visual worlds:
  - **Free Themes**: Galaxy, Ocean, Forest, Sunset, Halloween, Christmas.
  - **Premium Themes** (Unlockable with coins): Cyberpunk (150🪙), Space (200🪙), Neon (250🪙).
- 🏆 **Progression & Stats**:
  - Earn **XP** to level up your player profile.
  - Collect **Coins** by winning matches to unlock premium themes.
  - Track **31 achievements** and view your detailed statistics (accuracy, best times, win/loss ratio, high scores).
- 💾 **Local Persistence**: All progress, XP, coins, settings, and achievements are saved locally in the browser using the Web Storage API (`localStorage`).

---

## 📁 Folder & File Structure

This project is designed as a modular, lightweight **single-page application (SPA)** contained within a single file for maximum portability and zero setup.

```bash
Mismatch-mayhem/
│
├── .vscode/               # Editor configurations (VS Code Workspace settings)
│   └── settings.json
│
├── LICENSE                # MIT License
│
├── index.html             # The entire game codebase (HTML, CSS, JS)
│
└── README.md              # Project documentation (this file)
```

### 🔍 Inside `index.html`

The code is strictly organized into clean logical blocks mirroring a multi-file architecture:
1. **HTML5 Shell**: Contains the responsive viewport, SVG icon definitions (hand-crafted shapes), and basic layout screens.
2. **CSS3 Stylesheets**:
   - **Theme Variables**: Custom color tokens (`--bg`, `--accent`, etc.) supporting 9 themes.
   - **Background Effects**: Interactive canvas particles and dynamic radial gradient mouse-tracking lighting.
   - **Layout Shell**: Flexbox and CSS Grid designs adapting dynamically to mobile, tablet, and desktop screens.
   - **Transitions & Animations**: Custom keyframe animations for card flips, wrong guesses, power-up effects, and screen transitions.
3. **Vanilla JS Modules**:
   - **Storage Module**: Manages JSON serialization/deserialization with `localStorage`.
   - **Sound Synthesizer**: Utilizes the browser's `AudioContext` to generate oscillators, gains, and LFOs dynamically.
   - **Background Particle Loop**: Controls the HTML5 Canvas particles animation loop.
   - **UI Engine**: Updates screen states, triggers Toast notifications, and generates particle-based confetti.
   - **Game Loop**: Orchestrates deck building, card flip matching, lives, timers, score logic, and power-up usage.
   - **Progression & Achievements**: Validates triggers for 31 achievements, registers level-ups, and manages coins.

---

## 🛠️ How to Play Locally

Since the game uses purely client-side technologies, you can run it without any local build server.

### Option 1: Direct Run (Double-Click)
Simply double-click the `index.html` file in your file explorer to open and play the game in your default web browser.

### Option 2: Live Server (Recommended)
If you use VS Code, open the project directory and use the **Live Server** extension to launch a local dev server with auto-reload capabilities.

---

## 🔧 Technologies Used

- **Markup**: HTML5 Semantic Elements, Inline SVGs
- **Styling**: CSS3 Custom Properties (Variables), Canvas Particles, Flexbox, Grid Layouts, Glassmorphism
- **Logic**: ES6+ JavaScript, Web Audio API, Web Storage API, Canvas 2D Context API
- **Tooling**: Git, Vercel

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](file:///d:/Game/LICENSE) file for more details.
