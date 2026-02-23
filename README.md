<img width="1911" height="887" alt="image" src="https://github.com/user-attachments/assets/fdb86e7b-6034-4f71-b882-798d760598b7" />


<h1 align="center">🪐 Cosmic Explorer</h1>

<p align="center">
  <strong>An interactive 3D solar system experience built entirely with vanilla JavaScript and Three.js</strong>
</p>

<p align="center">
  <a href="https://rtm20.github.io/cosmic-explorer/">🚀 Live Demo</a> &nbsp;·&nbsp;
  <a href="#features">Features</a> &nbsp;·&nbsp;
  <a href="#controls">Controls</a> &nbsp;·&nbsp;
  <a href="#tech-stack">Tech Stack</a> &nbsp;·&nbsp;
  <a href="#license">License</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Three.js-r128-blue?logo=three.js" alt="Three.js" />
  <img src="https://img.shields.io/badge/JavaScript-ES6+-yellow?logo=javascript" alt="JavaScript" />
  <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey" alt="License" />
  <img src="https://img.shields.io/badge/Build-Zero%20Config-green" alt="No Build Tools" />
</p>

---

## About

**Cosmic Explorer** is a fully interactive 3D solar system that runs in the browser. Explore all 9 celestial bodies with real NASA textures, fly a spaceship in free-flight mode, travel through wormholes at light speed, and survive the Asteroid Escape mini-game — all powered by procedural generation and Web Audio.

No build tools. No frameworks. A single HTML file.

---

## Features

### 🌍 Solar System Exploration
- **10 celestial bodies** — Sun, Mercury, Venus, Earth (with Moon), Mars, Jupiter, Saturn (with rings), Uranus, Neptune
- Real NASA satellite textures with procedural FBM noise fallbacks
- Detailed info panels with orbital stats, atmosphere composition, temperature data, exploration missions, and fun facts
- Click any planet or use the bottom navigation bar to explore

### 🚀 Spaceship Free-Flight Mode
- First-person spaceship with full 6-DOF movement
- HUD with crosshair, throttle bar, speed readout, compass, and proximity scanner
- Engine audio that responds to speed
- Mobile-friendly with dual virtual joysticks

### 🌀 Wormhole Travel
- Animated wormhole tunnel with real-time speed HUD
- Light-speed and superluminal status indicators
- Warp between any two planets instantly
- Dramatic entry/exit flash + audio effects

### ☄️ Asteroid Escape Game
- **5 progressive zones**: Inner Belt → Kessler Field → Shattered Core → Debris Storm → The Gauntlet
- **4 difficulty levels**: Cadet, Pilot, Ace, Insane
- 6 asteroid types (rocky, metallic, dark, volcanic, crystal, icy) + 3 collectible star types (gold, crystal, rainbow)
- Cockpit view toggle, health/boost system, combo scoring, level-up transitions
- Full touch controls for mobile

### 🎵 Procedural Soundtrack
Interstellar-inspired ambient score generated entirely with the Web Audio API — **no audio files loaded**:
- Pipe organ drone with 10 simulated organ ranks
- Ticking clock motif (48 BPM)
- Evolving Am → Dm → F → Em chord progression
- Ethereal bell melody in Am pentatonic
- Sub-bass rumbles, cosmic wind, high shimmer
- 6-second cathedral reverb impulse response

### 📷 Photo Mode
- Press `P` to capture cinematic screenshots
- Auto-adds letterbox bars, watermark, date stamp, and planet label
- Downloads as PNG with auto-generated filename
- Camera shutter sound effect

### 🏆 Achievement System
22 unlockable achievements rewarding exploration:

| Icon | Achievement | Trigger |
|------|-------------|---------|
| 🔭 | First Contact | Explore your first celestial body |
| 🪨 | Inner System | Visit all rocky planets |
| ⛽ | Gas Giant Hunter | Visit all gas/ice giants |
| 🌟 | Cosmic Completionist | Visit all 9 bodies |
| 💍 | Lord of the Rings | Visit Saturn |
| 🏠 | Home Sweet Home | Visit Earth |
| 👁 | Face the Storm | Visit Jupiter |
| ☀ | Too Close to the Sun | Visit the Sun |
| 🌀 | Wormhole Navigator | First wormhole travel |
| 🎙 | Cosmic Guide | Start the guided tour |
| 🪐 | Grand Tour Complete | Finish the full guided tour |
| 📷 | Space Photographer | Take your first screenshot |
| 🕹 | Retro Gamer | Enter the Konami Code |
| ⏳ | Don't Let Me Leave, Murph! | Type "MURPH" |
| 🤖 | Humor 75% | Type "TARS" |
| 🎬 | Sit Back & Relax | Activate screensaver mode |
| 🪨 | Asteroid Dodger | Play Asteroid Escape |
| 🏅 | Commander | Beat all 5 zones |
| 👑 | Legendary Pilot | Win on Insane difficulty |
| 🌌 | Deep Space | Travel 50 KM in-game |
| 😎 | Near Miss Master | Hit a 5x near-miss combo |
| 🏆 | Ten Thousand | Score 10,000+ points |

### 🗺️ Additional Features
- **Minimap** — real-time radar showing planet positions and camera FOV
- **Guided Tour** — narrated walk-through of every planet
- **Screensaver Mode** — auto-pilot that tours the solar system with wormhole jumps
- **Welcome Screen** — animated intro with feature overview and keyboard guide
- **Loading Screen** — step-by-step progress tracker with percentage counter
- **Cinematic Intro** — sweeping flythrough on launch
- **Easter Eggs** — Konami Code (rainbow mode), type "MURPH" or "TARS" for movie references

---

## Controls

### Desktop

| Key | Action |
|-----|--------|
| `Scroll` | Zoom in / out |
| `Click + Drag` | Orbit camera |
| `Click Planet` | Open info panel |
| `← →` | Cycle through planets |
| `1` – `9` | Jump to planet (Sun = 1, Neptune = 9) |
| `F` | Toggle spaceship mode |
| `T` | Start guided tour |
| `N` | Next tour step |
| `M` | Toggle music |
| `P` | Photo mode screenshot |
| `G` | Launch Asteroid Escape |
| `Esc` | Close panel / exit mode |

### Spaceship Mode

| Key | Action |
|-----|--------|
| `W / A / S / D` | Thrust forward / left / back / right |
| `Space` | Ascend |
| `Shift` | Descend |
| `Q` | Speed boost |
| `Mouse` | Look direction |

### Asteroid Escape

| Key | Action |
|-----|--------|
| `← → ↑ ↓` or `W A S D` | Steer ship |
| `Shift` | Boost |
| `V` | Toggle cockpit view |
| `Esc` | Exit game |

### Mobile
- Dual virtual joysticks (move + look) for spaceship mode
- Virtual joystick + action buttons for Asteroid Escape
- Touch-optimized UI across all screens

---

## Tech Stack

| Technology | Details |
|------------|---------|
| **Three.js** | v0.128.0 — OrbitControls, UnrealBloomPass, EffectComposer, Lensflare, custom GLSL shaders |
| **Web Audio API** | Full procedural soundtrack & SFX — zero audio files |
| **WebGL** | Hardware-accelerated 3D rendering with bloom post-processing |
| **NASA Textures** | Real satellite imagery for planets (Blue Marble Earth, etc.) |
| **Google Fonts** | Orbitron (display) + Exo 2 (body) |
| **Vanilla JS/CSS** | No frameworks, no build tools, no dependencies beyond Three.js |
| **SEO** | JSON-LD structured data, Open Graph, Twitter Cards, sitemap.xml, robots.txt |

---

## Project Structure

```
cosmic-explorer/
├── index.html              # Entire application (HTML + CSS + JS)
├── LICENSE                  # CC BY-NC 4.0
├── README.md                # This file
├── robots.txt               # Search engine crawl rules
├── sitemap.xml              # Sitemap for SEO
└── google6f3b8ce4bcccc567.html  # Google Search Console verification
```

---

## Getting Started

No install needed. Choose one:

**Option 1 — Visit the live site:**
> [https://rtm20.github.io/cosmic-explorer/](https://rtm20.github.io/cosmic-explorer/)

**Option 2 — Run locally:**
```bash
git clone https://github.com/rtm20/cosmic-explorer.git
cd cosmic-explorer
# Open index.html in any modern browser, or use a local server:
npx serve .
```

> **Requirements:** Any modern browser with WebGL support (Chrome, Firefox, Edge, Safari).

---

## Browser Support

| Browser | Status |
|---------|--------|
| Chrome 90+ | ✅ Full support |
| Firefox 90+ | ✅ Full support |
| Edge 90+ | ✅ Full support |
| Safari 15+ | ✅ Full support |
| Mobile Chrome | ✅ Touch controls |
| Mobile Safari | ✅ Touch controls |

---

## Performance Tips

- For the best experience, use a device with a dedicated GPU
- Close other GPU-intensive tabs to free up WebGL resources
- If frame rate drops, reduce browser zoom level
- The Asteroid Escape game is more demanding — lower difficulty helps on older hardware

---

## Author

**Ritesh Meena**
- GitHub: [@rtm20](https://github.com/rtm20)

---

## License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License** (CC BY-NC 4.0).

You are free to share and adapt this work for non-commercial purposes with appropriate credit.

See [LICENSE](LICENSE) for details | [Full license text](https://creativecommons.org/licenses/by-nc/4.0/legalcode)

---

<p align="center">
  Built with ❤️ and Three.js &nbsp;|&nbsp; If you enjoyed this, give it a ⭐
</p>
