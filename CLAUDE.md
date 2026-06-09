# Contexto del Proyecto: DebugDuck-web

Landing page oficial de DebugDuck — un widget de escritorio 
para Rubber Duck Debugging con IA local.

## 1. Qué es este repositorio
Web de presentación estática (HTML/CSS/JS puro) para la app 
DebugDuck. Sin frameworks. Lista para GitHub Pages.
URL publicada: https://carlosvallejoruiz.github.io/DebugDuck-web/

## 2. La app que presenta
DebugDuck es un widget de escritorio (Tauri v2 + React + Rust)
que permite hablar con un pato de goma con IA local via voz.
Repositorio de la app: https://github.com/CarlosVallejoRuiz/DebugDuck
Releases: https://github.com/CarlosVallejoRuiz/DebugDuck/releases

## 3. Historia del proyecto
- Nació al ver cómo se gastaban tokens premium en consultas
  que cualquier IA local resuelve igual de bien.
  "No era culpa suya — nadie te explica que existe una 
  alternativa gratuita, local y privada para el 80% de 
  las consultas."
- La chispa vino de explicar el rubber duck debugging a 
  compañeros de un curso de soldadura — lo adoptaron para
  su vida cotidiana, no solo para programar
- Conclusión: explicar problemas en voz alta funciona para
  todo el mundo, no solo para developers

## 4. Público objetivo
- Developers que quieren ahorrar tokens premium
- Cualquier persona — NO es solo para programadores
- Tono: casual, divertido, accesible, NO técnico ni frío
- Nunca culpar a nadie de "malgastar" — el mensaje es 
  que la alternativa local simplemente no era conocida

## 5. Personalidad y estilo visual
- Protagonista: el pato (image/DebugDuck_Idle/ para animaciones)
- Colores: amarillo pato (#FFD700), blanco, negro suave (#1a1a1a)
- Fuentes: Space Mono (títulos) + Inter (cuerpo)
- Animación idle: 36 frames a 12fps en loop
- Hover → RascaCabeza, Click → Asiente, CTA → EscribeLibreta
- Mobile-first, responsive (3 cols → 2 → 1)
- Cálido y humano, nunca frío ni corporativo
- Scroll reveal escalonado en todas las secciones

## 6. Estructura de archivos
DebugDuck-web/
├── index.html              # Archivo principal (todo en uno)
├── image/
│   ├── DebugDuck_Idle/     # 36 frames idle animation
│   ├── DebugDuck_RascaCabeza/  # hover animation
│   ├── DebugDuck_Asiente/      # click animation
│   └── DebugDuck_EscribeLibreta/ # CTA animation
└── CLAUDE.md               # Este archivo

## 7. Secciones de la web (en orden con IDs)
1. `#inicio` — Hero: pato animado flotante + botones descarga
2. `#historia` — Narrativa casual: tokens, soldadura, rubber duck
3. `#como-usar` — 5 pasos visuales con flechas
4. `#features` — Grid 6 cards con features principales
5. `#configuracion` — Cards interactivas con JS:
   - Personalidad (tabs Programador/General con características)
   - Nivel de sarcasmo (slider funcional con descripción dinámica)
   - Modo Tamagotchi (toggle ON/OFF con lógica condicional)
   - Memoria de conversación (toggle ON/OFF)
6. `#requisitos` — Mac + Windows, LM Studio
7. `#descargar` — CTA final con botón de descarga
8. Footer — créditos + links

## 8. Navbar
- Sticky siempre visible (NO se oculta en scroll)
- Fondo oscuro semi-transparente con blur
- Logo pato pequeño + "DebugDuck" izquierda
- Links: Inicio | Historia | Cómo usar | Configuración | Descargar
- Scroll suave al hacer clic

## 9. Interactividad implementada (JS puro)
- Sprite animation: 36 frames idle en loop a 12fps
- Hover → RascaCabeza, Click → Asiente
- Scroll reveal con IntersectionObserver
- Card Personalidad: tabs con contenido dinámico
- Slider sarcasmo: color dinámico + texto descriptivo
- Toggle Tamagotchi: muestra/oculta barra de vida y lógica
- Toggle Memoria: descripción ON/OFF

## 10. Links importantes
- Web publicada: https://carlosvallejoruiz.github.io/DebugDuck-web/
- Descarga (todos): https://github.com/CarlosVallejoRuiz/DebugDuck/releases
- DMG Mac: https://github.com/CarlosVallejoRuiz/DebugDuck/releases/download/v0.1.1/DebugDuck_0.1.1_aarch64.dmg
- EXE Windows: https://github.com/CarlosVallejoRuiz/DebugDuck/releases/download/v0.1.1/DebugDuck_0.1.1_x64-setup.exe
- GitHub repo app: https://github.com/CarlosVallejoRuiz/DebugDuck
- GitHub repo web: https://github.com/CarlosVallejoRuiz/DebugDuck-web

## 11. Publicación
- GitHub Pages desde rama main (activo)
- Auto-deploy en cada git push
- Dominio futuro: debugduck.dev o debugduck.app

## 12. Reglas de desarrollo
- UN SOLO archivo index.html (CSS y JS inline)
- Sin frameworks — HTML/CSS/JS puro
- Sin dependencias externas excepto Google Fonts
- Imágenes locales desde image/ — sin CDN para el pato
- Compatible con file:// para pruebas locales
- Probar con: python3 -m http.server 8080

## 13. Comandos útiles
```bash
# Servidor local para pruebas
cd ~/Desktop/DebugDuck-web
python3 -m http.server 8080

# Subir cambios
git add . && git commit -m "descripción" && git push

# La web se actualiza en ~30 segundos tras el push
```