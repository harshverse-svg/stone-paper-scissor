# Stone Paper Scissor 3.0 ⚡

<p align="center">
  <a href="https://harshverse-svg.github.io/stone-paper-scissor/"><img src="https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-4F5BD5?style=for-the-badge&logo=github" alt="Live Demo" /></a>
  <img src="https://img.shields.io/badge/Audio-Procedural%20Web%20Audio%20API-00e5ff?style=for-the-badge" alt="Web Audio API" />
  <img src="https://img.shields.io/badge/AI-Markov%20Predictive%20Engine-ff5722?style=for-the-badge" alt="Predictive AI" />
  <img src="https://img.shields.io/badge/Engine-Vanilla%20JS%20%26%20CSS3-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="Vanilla JS" />
  <img src="https://img.shields.io/badge/Storage-Local%20Persistence-7c3aed?style=for-the-badge" alt="Local Storage" />
  <a href="https://github.com/harshverse-svg/stone-paper-scissor"><img src="https://img.shields.io/badge/License-MIT-gray?style=for-the-badge" alt="License" /></a>
</p>

<p align="center">
  <strong>A high-octane cyberpunk arcade edition of Stone Paper Scissors featuring procedural audio synthesis, adaptive AI opponents, and competitive Elo progression.</strong><br>
  <em>Built with pure vanilla web technologies: zero external sound libraries, zero frameworks, and zero build dependencies.</em>
</p>

---

## 🌐 Live Game

Play instantly in your browser:  
👉 **[https://harshverse-svg.github.io/stone-paper-scissor/](https://harshverse-svg.github.io/stone-paper-scissor/)**

---

## 🎮 Game Architecture & Key Features

### 1. 🔊 Procedural Web Audio Engine
The audio experience is synthesized entirely in real time using the browser's native **Web Audio API** (`AudioContext` oscillators, gain envelopes, and frequency ramps)—requiring zero audio file downloads:
- **Countdown Tones**: Ascending frequency pitch cues during decision countdowns.
- **Dynamic Outcome Audio**: Bright harmonic major chords on victory, descending detuned saw waves on defeat.
- **Combo Sweeps**: Resonant frequency sweeps scaling upward with consecutive win streaks.
- **Match Point Heartbeat**: Sub-bass tension pulse triggered automatically whenever either side reaches 4 points in a first-to-5 match.

### 2. 🧠 Adaptive AI Difficulty Engine
The CPU opponent doesn't just pick random choices:
- **EASY**: Uniform random move selection. Ideal for warm-ups.
- **MEDIUM**: Evaluates the player's recent move distribution and biases towards winning counters.
- **HARD**: Employs a **Markov transition matrix** analyzing your last 8 decisions to recognize subconscious repetition, counter-switching habits, and win-stay/lose-shift patterns.

### 3. 🔥 Momentum & Combo Streaks
Consecutive round wins trigger visual screen shakes, glowing neon callouts, and bonus XP multipliers:
- **2 Wins**: `DOUBLE STRIKE`
- **3 Wins**: `HAT TRICK 🔥`
- **4 Wins**: `DOMINATING!`
- **5+ Wins**: `UNSTOPPABLE!!` (Screen shake + neon violet overdrive)
- **Deficit Flip**: `COMEBACK!` (Triggered when winning after opponent held a match lead)

### 4. 🏆 Competitive Elo & Profile Persistence
All match telemetry is preserved across sessions using `localStorage`:
- Dynamic **Elo Rating** calculating skill adjustments based on opponent difficulty.
- Tracked metrics: Total matches, win/loss/tie ratios, best streaks, and move-by-move affinity.
- Unlockable achievements and competitive XP rank tiers.

### 5. 🎨 Cyberpunk Visual Themes
Switch seamlessly between 4 responsive neon color palettes with real-time CSS variable updates:
- **Cyber Blue**: Electric cyan and deep space navy.
- **Jungle**: Acid green and tactical dark moss.
- **Blood Arena**: Crimson and ember red.
- **Legendary**: Sovereign gold and midnight black.

---

## 🕹️ Controls & Rules

| Choice | Beats | Loses To |
| :---: | :---: | :---: |
| 🪨 **Stone** | ✂️ Scissor | 📄 Paper |
| 📄 **Paper** | 🪨 Stone | ✂️ Scissor |
| ✂️ **Scissor** | 📄 Paper | 🪨 Stone |

- **Match Objective**: First to score **5 points** wins the match.
- **Input**: Mouse click, touch tap, or keyboard keys (`1` for Stone, `2` for Paper, `3` for Scissor).

---

## 🛠️ Local Development

### 1. Clone
```bash
git clone https://github.com/harshverse-svg/stone-paper-scissor.git
cd stone-paper-scissor
```

### 2. Run
Simply double-click `index.html` or run:
```bash
python -m http.server 8000
```
Open `http://localhost:8000` in any web browser.

---

## 📄 License

Distributed under the [MIT License](LICENSE).
