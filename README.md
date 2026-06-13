🌍 [English](README.en.md) | Español

# DebugDuck — Web oficial 🦆

Landing page de [DebugDuck](https://github.com/CarlosVallejoRuiz/DebugDuck), el widget de escritorio para rubber duck debugging con IA local.

**Web publicada:** [carlosvallejoruiz.github.io/DebugDuck-web](https://carlosvallejoruiz.github.io/DebugDuck-web/)

---

## ¿Qué es esto?

Este repositorio contiene la web de presentación de DebugDuck.  
HTML, CSS y JavaScript puros — sin frameworks, sin dependencias, lista para GitHub Pages.

La app que presenta:  
**DebugDuck** es un widget de escritorio (Tauri v2 + React + Rust) que permite hablar con un pato de goma con IA local via voz. Sin suscripciones, sin enviar datos a ningún lado.

---

## Desarrollo local

```bash
git clone https://github.com/CarlosVallejoRuiz/DebugDuck-web.git
cd DebugDuck-web
python3 -m http.server 8080
```

Abre [http://localhost:8080](http://localhost:8080) en tu navegador.

> No se necesita npm, Node.js ni ninguna otra herramienta.

---

## Estructura

```
DebugDuck-web/
├── index.html              # Archivo principal (CSS y JS inline)
├── public/
│   └── games.html          # Arcade — 12 minijuegos
└── image/
    ├── DebugDuck_Idle/     # 36 frames — animación idle
    ├── DebugDuck_RascaCabeza/
    ├── DebugDuck_Asiente/
    ├── lmstudio-logo.png
    └── ollama-logo.png
```

---

## Secciones de la web

| Sección | Descripción |
|---|---|
| Hero | Pato animado + botones de descarga |
| Historia | Por qué existe el proyecto |
| Cómo usar | 5 pasos visuales |
| Features | Bento grid asimétrico con las características |
| Historial | Nueva sección — las últimas 50 conversaciones |
| Arcade | 12 minijuegos retro con carrusel infinito |
| Configuración | Cards interactivas (personalidad, sarcasmo, Tamagotchi, memoria, minijuegos) |
| Requisitos | Guía LM Studio paso a paso |
| Descarga | CTA final |

---

## Despliegue

GitHub Pages desde la rama `main`.  
Cada `git push` actualiza la web en ~30 segundos.

```bash
git add .
git commit -m "descripción"
git push
```

---

## La app

| | |
|---|---|
| **Repositorio** | [github.com/CarlosVallejoRuiz/DebugDuck](https://github.com/CarlosVallejoRuiz/DebugDuck) |
| **Descarga** | [Releases](https://github.com/CarlosVallejoRuiz/DebugDuck/releases) |
| **Mac (Apple Silicon)** | `DebugDuck_0.3.0_aarch64.dmg` |
| **Windows (x64)** | `DebugDuck_0.3.0_x64-setup.exe` |

---

## Tecnologías

- **IA local:** LM Studio · Ollama · cualquier servidor compatible con la API de OpenAI
- **Reconocimiento de voz:** Web Speech API
- **Desktop:** Tauri v2 + React + Rust
- **Web:** HTML · CSS · JavaScript puros

---

## Licencia

MIT — [ver licencia](https://github.com/CarlosVallejoRuiz/DebugDuck/blob/main/LICENSE)
