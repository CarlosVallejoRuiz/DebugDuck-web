🌍 English | [Español](README.md)

# DebugDuck — Official Website 🦆

Landing page for [DebugDuck](https://github.com/CarlosVallejoRuiz/DebugDuck), the desktop widget for rubber duck debugging with local AI.

**Live site:** [carlosvallejoruiz.github.io/DebugDuck-web](https://carlosvallejoruiz.github.io/DebugDuck-web/)

---

## What is this?

This repository contains the DebugDuck presentation website.  
Plain HTML, CSS and JavaScript — no frameworks, no dependencies, ready for GitHub Pages.

The app it showcases:  
**DebugDuck** is a desktop widget (Tauri v2 + React + Rust) that lets you talk to a rubber duck powered by local AI via voice. No subscriptions, no data sent anywhere.

---

## Local development

```bash
git clone https://github.com/CarlosVallejoRuiz/DebugDuck-web.git
cd DebugDuck-web
python3 -m http.server 8080
```

Open [http://localhost:8080](http://localhost:8080) in your browser.

> No npm, Node.js or any other tooling required.

---

## Structure

```
DebugDuck-web/
├── index.html              # Main file (CSS and JS inline)
├── public/
│   └── games.html          # Arcade — 12 mini-games
└── image/
    ├── DebugDuck_Idle/     # 36 frames — idle animation
    ├── DebugDuck_RascaCabeza/
    ├── DebugDuck_Asiente/
    ├── lmstudio-logo.png
    └── ollama-logo.png
```

---

## Page sections

| Section | Description |
|---|---|
| Hero | Animated duck + download buttons |
| Story | Why this project exists |
| How to use | 5 visual steps |
| Features | Asymmetric bento grid with key features |
| History | New — last 50 conversations saved |
| Arcade | 12 retro mini-games with infinite carousel |
| Settings | Interactive cards (personality, sarcasm, Tamagotchi, memory, mini-games) |
| Requirements | Step-by-step LM Studio setup guide |
| Download | Final CTA |

---

## Deployment

GitHub Pages from the `main` branch.  
Every `git push` updates the site in ~30 seconds.

```bash
git add .
git commit -m "description"
git push
```

---

## The app

| | |
|---|---|
| **Repository** | [github.com/CarlosVallejoRuiz/DebugDuck](https://github.com/CarlosVallejoRuiz/DebugDuck) |
| **Download** | [Releases](https://github.com/CarlosVallejoRuiz/DebugDuck/releases) |
| **Mac (Apple Silicon)** | `DebugDuck_0.3.0_aarch64.dmg` |
| **Windows (x64)** | `DebugDuck_0.3.0_x64-setup.exe` |

---

## Tech stack

- **Local AI:** LM Studio · Ollama · any OpenAI-compatible server
- **Voice recognition:** Web Speech API
- **Desktop:** Tauri v2 + React + Rust
- **Website:** Plain HTML · CSS · JavaScript

---

## License

MIT — [view license](https://github.com/CarlosVallejoRuiz/DebugDuck/blob/main/LICENSE)
