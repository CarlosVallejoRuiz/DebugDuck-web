# Contexto del Proyecto: DebugDuck-web

Landing page oficial de DebugDuck — un widget de escritorio 
para Rubber Duck Debugging con IA local.

## 1. Qué es este repositorio
Web de presentación estática (HTML/CSS/JS puro) para la app 
DebugDuck. Sin frameworks. Lista para GitHub Pages o Vercel.

## 2. La app que presenta
DebugDuck es un widget de escritorio (Tauri v2 + React + Rust)
que permite hablar con un pato de goma con IA local via voz.
Repositorio de la app: https://github.com/CarlosVallejoRuiz/DebugDuck

## 3. Historia del proyecto
- Nació al ver cómo se gastaban tokens premium en consultas
  que cualquier IA local resuelve igual de bien
- La chispa vino de explicar el rubber duck debugging a 
  compañeros de un curso de soldadura — lo adoptaron para
  su vida cotidiana, no solo para programar
- Conclusión: explicar problemas en voz alta funciona para
  todo el mundo, no solo para developers

## 4. Público objetivo
- Developers que quieren ahorrar tokens
- Cualquier persona — NO es solo para programadores
- Tono: casual, divertido, accesible, NO técnico ni frío

## 5. Personalidad y estilo visual
- Protagonista: el pato (DebugDuck.png en assets/)
- Colores: amarillo pato (#FFD700), blanco, negro suave
- Fuente: Inter o similar
- Animaciones suaves — el pato flota
- Mobile-first, responsive
- Cálido y humano, nunca frío ni corporativo

## 6. Estructura de archivos
DebugDuck-web/
├── index.html          # Archivo principal (todo en uno)
├── assets/
│   └── duck.png        # Imagen del pato
├── images/             # Frames de animaciones si se usan
└── CLAUDE.md           # Este archivo

## 7. Secciones de la web (en orden)
1. Hero — pato flotante + botones descarga
2. La Historia — narrativa casual y humana
3. Cómo funciona — 3 pasos visuales
4. Features — grid 6 cards
5. Requisitos — simple y visual
6. Descarga — CTA final
7. Footer

## 8. Links importantes
- Descarga DMG: https://github.com/CarlosVallejoruiz/DebugDuck/releases/download/v0.1.1/DebugDuck_0.1.1_aarch64.dmg
- GitHub repo: https://github.com/CarlosVallejoRuiz/DebugDuck
- Releases: https://github.com/CarlosVallejoRuiz/DebugDuck/releases

## 9. Publicación
- GitHub Pages desde rama main
- O Vercel con deploy automático
- Dominio futuro: debugduck.dev o debugduck.app

## 10. Reglas de desarrollo
- UN SOLO archivo index.html (CSS y JS inline)
- Sin frameworks — HTML/CSS/JS puro
- Sin dependencias externas excepto Google Fonts
- Debe funcionar sin servidor (file://)
- Imágenes locales, sin CDN para assets del pato