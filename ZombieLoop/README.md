```markdown
# Zombie Loop: Mazmorra Matemática

[![Estado](https://img.shields.io/badge/Estado-Jugable-brightgreen?style=flat-square)](#)
[![Plataforma](https://img.shields.io/badge/Plataforma-Navegador_Web-blue?style=flat-square)](#)
[![Género](https://img.shields.io/badge/G%C3%A9nero-Arcade_%2F_Puzzle_%2F_RPG-orange?style=flat-square)](#)

## Descripción del Juego

**Zombie Loop: Mazmorra Matemática** es un videojuego educativo con estética Pixel Art retro ambientado en una mazmorra[cite: 2, 3]. El jugador controla a un zombie que camina automáticamente a través de catacumbas y criptas[cite: 3]. A lo largo del camino se topa con diversos monstruos (slimes, espectros, bestias) y debe derrotarlos resolviendo problemas aritméticos para llegar al cofre final[cite: 3].

* **¿Cuál es el objetivo del jugador?** Superar los 10 combates contra enemigos en la mazmorra respondiendo correctamente las preguntas para conservar sus vidas y obtener la puntuación máxima (10/10)[cite: 2, 3].
* **Mecánica Principal:** Desplazamiento automático por mapa 2D (Top-down) interconectado con un sistema de combate por turnos tipo quiz/RPG[cite: 3].

---

## Ficha Técnica

* **Nombre del Juego:** Zombie Loop: Mazmorra Matemática[cite: 3]
* **Género:** Arcade / Puzzle / Dungeon Crawler[cite: 3]
* **Público Objetivo:** Estudiantes de 1ro de secundaria (repaso aritmético)[cite: 2]
* **Tecnologías:** HTML, JavaScript, CSS (Google Fonts 'Press Start 2P')[cite: 3]
* **Enlace para Jugar:** [ Jugar Zombie Loop en GitHub Pages](https://ArielAcarapi.github.io/game-development-portfolio/01-zombie-loop/)

---

## Controles e Instrucciones

El juego se opera completamente mediante la interfaz gráfica del navegador (Mouse o Pantalla Táctil)[cite: 2, 3]:

* **Selección de Respuesta:** Haz clic sobre uno de los 4 botones de respuesta presentados en cada combate[cite: 2, 3].
* **Avanzar / Iniciar:** Clic en el botón `INICIAR` o `JUGAR OTRA VEZ`[cite: 3].

### Reglas del Juego
1. Inicias con **3 vidas** (corazones) y un puntaje de **0**[cite: 2, 3].
2. Se presentan **10 preguntas** elegidas aleatoriamente de operaciones de suma (+), resta (-), multiplicación (×) y división (÷)[cite: 2, 3].
3. Responder correctamente Inflige daño al enemigo, avanza el mapa y suma +1 punto[cite: 2, 3].
4. Responder erróneamente resta 1 vida[cite: 3]. Si pierdes las 3 vidas, es *Game Over*[cite: 3].

---

## Capturas de Pantalla


| Pantalla de Inicio | Mapa y Exploración | Sistema de Combate |
| :---: | :---: | :---: |
| ![Inicio](./screenshots/inicio.png) | ![Mapa](./screenshots/mapa.png) | ![Combate](./screenshots/combate.png) |

---

## Uso de Inteligencia Artificial

Este proyecto fue desarrollado utilizando herramientas de **IA Generativa** mediante prompts estructurados[cite: 2]:

* **Generación de Sprites y Arte:** Modelado de personajes Pixel Art en formato matriz directamente renderizados con JavaScript Canvas (sin requerir imágenes externas)[cite: 3].
* **Lógica del Juego:** Generación aleatoria de preguntas matemáticas equilibradas con distractores coherentes y algoritmos de interpolación suave para el movimiento[cite: 3].

### Registro de Iteraciones
| Versión | Problema Detectado | Acción Realizada | Resultado |
| :---: | :--- | :--- | :--- |
| **V1** | Movimiento del personaje en el mapa era brusco y sin transición. | Se implementó animación fluida por sub-tiles e interpolación (*eased lerp*). | Desplazamiento orgánico con efectos de polvo y balanceo[cite: 3]. |
| **V2** | Las preguntas podían generar resultados negativos en restas. | Se ajustaron los rangos del generador de operaciones aritméticas[cite: 3]. | Preguntas adecuadas para el nivel escolar[cite: 2, 3]. |

---

## Aprendizajes y Mejoras Futuras

### Aprendizajes
* Manipulación de canvas 2D para renderizar Pixel Art programático mediante matrices de color[cite: 3].
* Integración de mecánicas de juego RPG con feedback educativo inmediato[cite: 2, 3].
* Diseño de interfaces estilo *Retro Arcade* adaptables[cite: 3].

### Mejoras Futuras
* Agregar efectos de sonido de 8 bits y música de fondo para mayor inmersión.
* Incluir ítems equipables o pociones al responder preguntas complejas.
* Agregar distintos niveles de dificultad ajustables.
