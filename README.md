# 🚀 Space Invaders - Vanilla JS & HTML5 Canvas

Un juego clásico de **Space Invaders** desarrollado en un único archivo HTML autocontenido (`spacerinvaders.html`) usando **Vanilla JavaScript** y **HTML5 `<canvas>`**, creado con fines educativos y de arquitectura de software para la carrera de **Ingeniería en Sistemas Informáticos**.

---

## 🎯 Características Principales

- **🎮 Renderizado 2D y Game Loop**: Ciclo de juego continuo a ~60 FPS sintonizado con `requestAnimationFrame` separando la actualización lógica (`actualizar()`) del renderizado gráfico (`renderizar()`).
- **🕹️ Control de Nave y Físicas**: Movimiento suave con delimitación de bordes cartesianos en Canvas.
- **💥 Sistema de Disparos y Gestión de Memoria**: Manejo dinámico de proyectiles con arreglos en JavaScript y liberación de memoria (`splice`) al salir de la pantalla.
- **👾 Horda de Enemigos en Matriz**: Generación de alienígenas mediante ciclos anidados (`for` 2D) con patrón de movimiento en zigzag descendente y aceleración progresiva.
- **🎯 Detección de Colisiones AABB**: Algoritmo *Axis-Aligned Bounding Box* para colisiones de precisión entre proyectiles, nave, enemigos y búnkeres.
- **🔴 Disparos Enemigos Aleatorios**: Sistema de fuego cruzado aleatorio basado en probabilidades por fotograma.
- **🛡️ Escudos / Búnkeres Defensivos**: 4 torres defensivas destruibles con degradación visual de color según la salud restante (Verde ➔ Naranja ➔ Rojo).
- **❤️ Sistema de Vidas y Puntuación**: HUD con 3 vidas, reaparición en el centro e indicador de puntuación en tiempo real.
- **💾 Persistencia con `localStorage`**: Almacenamiento local del récord histórico (*MÁXIMO puntaje*) guardado permanentemente en el navegador.
- **🔊 Sintetizador de Voz Nativo (Web Speech API)**: Anuncios por voz hablada (`speechSynthesis`) en español al ganar o perder.

---

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica y elemento `<canvas>` para gráficos 2D.
- **CSS3**: Diseño moderno, temas espaciales oscuros y estética cyberpunk/neón.
- **Vanilla JavaScript (ES6+)**: Lógica pura sin librerías externas ni frameworks.
- **Web APIs**:
  - HTML5 Canvas 2D Context API
  - Web Storage API (`localStorage`)
  - Web Speech API (`SpeechSynthesis`)

---

## 🚀 Cómo Ejecutar

No requiere servidores, `npm` ni instalaciones externas.

1. Clona o descarga este repositorio.
2. Haz doble clic en el archivo [spacerinvaders.html](file:///c:/Users/joell/Ingieneria%20en%20sistemas/mis%20proyectos/spacerinvaders.html) para abrirlo directamente en tu navegador web preferido (Chrome, Edge, Firefox, Brave, Safari).
3. ¡Sube el volumen y a jugar!

---

## 🕹️ Controles del Juego

| Tecla | Acción |
| :--- | :--- |
| **`Flecha Izquierda`** / **`A`** | Mover la nave hacia la izquierda |
| **`Flecha Derecha`** / **`D`** | Mover la nave hacia la derecha |
| **`Barra Espaciadora` (`Space`)** | Disparar láseres |
| **`F5`** | Reiniciar la partida |

---

## 📐 Arquitectura de Código

El código está completamente estructurado y comentado paso a paso:

```
spacerinvaders.html
├── HTML Base y Estilos CSS (Tema Neón/Espacial)
└── JavaScript Script
    ├── FASE 1: Configuración de Canvas & Contexto 2D
    ├── FASE 2: Objeto Jugador (Encapsulación de Estado)
    ├── FASE 4: Sistema de Disparo del Jugador
    ├── FASE 5: Matriz de Enemigos (Ciclos Anidados)
    ├── FASE 6: Detección de Colisiones AABB
    ├── FASE 7: Movimiento Zigzag de la Horda
    ├── FASE 8: Estado del Juego (Victoria, Game Over & UI)
    ├── FASE 9: Disparos Enemigos Aleatorios
    ├── FASE 10: Sistema de Vidas & Reposicionamiento
    ├── FASE 11: Torres Defensivas Destruibles (4 Búnkeres)
    ├── FASE 12: Persistencia (localStorage) & Web Speech API (Voz)
    └── Motor de Juego: Game Loop (actualizar -> renderizar -> requestAnimationFrame)
```

---

## 🎓 Propósito Educativo

Desarrollado como proyecto de aprendizaje socrático y práctico de programación y física de juegos 2D para la carrera de **Ingeniería en Sistemas Informáticos**.
