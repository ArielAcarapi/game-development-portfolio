# Zombie Loop: Mazmorra Matemática

<div align="center">

![Estado](https://img.shields.io/badge/Estado-Jugable-brightgreen?style=for-the-badge)
![Plataforma](https://img.shields.io/badge/Plataforma-Navegador_Web-blue?style=for-the-badge)
![Género](https://img.shields.io/badge/G%C3%A9nero-Arcade_%2F_Puzzle_%2F_RPG-orange?style=for-the-badge)
![Tecnología](https://img.shields.io/badge/Tech-HTML5_Canvas_%2F_JS-yellow?style=for-the-badge)

[HAGA CLIC AQUÍ PARA JUGAR EN LÍNEA](https://ArielAcarapi.github.io/game-development-portfolio/01-zombie-loop/)

</div>

---

## Descripción del Juego

**Zombie Loop: Mazmorra Matemática** es un videojuego educativo con estética retro *Pixel Art* de 8 bits. Está diseñado para estudiantes de nivel secundario (1ro de secundaria) con el objetivo de ejercitar operaciones aritméticas básicas de forma entretenida e interactiva.

El jugador toma el control de un zombie que recorre automáticamente una mazmorra llena de trampas y monstruos (slimes, espectros y bestias). Para avanzar y sobrevivir a cada encuentro en las catacumbas, el jugador debe resolver correctamente preguntas matemáticas de opción múltiple antes de quedarse sin vidas.

### Objetivo del Jugador
Superar los 10 combates en la mazmorra respondiendo correctamente a las operaciones aritméticas para llegar al final con la mayor cantidad de vidas posibles y obtener una puntuación perfecta (**10/10**).

### Mecánica Principal
* **Exploración:** Desplazamiento automático sobre un mapa 2D en cuadrícula (*Top-down*) con animaciones fluidas y efectos visuales retro.
* **Sistema de Combate Turn-Based (Quiz RPG):** Al colisionar con un enemigo, se activa una arena de combate por turnos donde atacar o recibir daño depende de seleccionar la respuesta correcta entre 4 alternativas.

---

## Ficha Técnica

| Parámetro | Detalle |
| :--- | :--- |
| **Nombre Definitivo** | Zombie Loop: Mazmorra Matemática |
| **Desarrollador** | Ariel Vidal Acarapi Limachi |
| **Género** | Arcade / Puzzle / Dungeon Crawler / RPG |
| **Público Objetivo** | Estudiantes de 1ro de secundaria (11-13 años) |
| **Plataforma** | Web (Ejecución directa en navegador) |
| **Lenguajes y Herramientas** | HTML5, CSS3, JavaScript Vanilla (Sin librerías externas), HTML5 Canvas |
| **Estilo Visual** | Pixel Art renderizado por matrices CSS/Canvas con tipografía *Press Start 2P* |

---

## Controles e Instrucciones

El juego está diseñado para jugarse cómodamente desde cualquier dispositivo (PC, Tablet o Móvil) utilizando interfaz táctil o puntero de ratón:

* **Mouse / Clic / Pantalla Táctil:** Seleccionar las opciones de respuesta durante los combates y navegar entre los menús de la interfaz.

### Reglas de Juego
1. **Vidas Iniciales:** Comienzas la aventura con **3 vidas** (representadas por corazones).
2. **Progreso y Enemigos:** La mazmorra contiene **10 enemigos** generados a lo largo del camino.
3. **Preguntas Aritméticas:** Cada combate presenta una operación aleatoria de suma (`+`), resta (`-`), multiplicación (`×`) o división (`÷`).
4. **Retroalimentación (Feedback):**
   * **Respuesta Correcta:** Realizas un ataque, eliminas al enemigo, sumas **+1 punto** y el personaje continúa su camino hacia la siguiente zona.
   * **Respuesta Incorrecta:** El enemigo te ataca, pierdes **1 vida** y se muestra la respuesta correcta para aprender del error.
5. **Condición de Victoria:** Derrotar a los 10 enemigos manteniendo al menos 1 vida.
6. **Condición de Derrota:** Perder las 3 vidas durante la exploración (Game Over). Al finalizar se muestra una tabla de revisión con todas tus respuestas.

---

## Capturas de Pantalla

| Pantalla Principal | Exploración de la Mazmorra |
| :---: | :---: |
| ![Pantalla de Inicio](./screenshots/ZombieLoopInicio.jpg) | ![Mapa en Vivo](./screenshots/ZombieLoopExploracion.jpg) |

| Arena de Combate | Pantalla de Resultados |
| :---: | :---: |
| ![Sistema de Preguntas](./screenshots/ZombieLoopCombate.jpg) | ![Tabla Final](./screenshots/ZombieLoopPantallaFinal.jpg) |

---

## Desarrollo con IA Generativa e Iteraciones

Este videojuego fue desarrollado integrando herramientas de **Inteligencia Artificial Generativa** para el diseño de lógica, generación de código web y estructuración de código Pixel Art dinámico mediante código JavaScript (renderizado matricial sin imágenes externas pesadas).

### Registro de Mejoras e Iteraciones

| Versión | Problema Detectado | Acción Realizada | Resultado |
| :---: | :--- | :--- | :--- |
| **V1** | El movimiento del jugador en el mapa era rígido y saltaba de casilla en casilla bruscamente. | Se implementó un algoritmo de interpolación suave por sub-tiles (*eased lerp*) con efecto de rebote (*bobding*) y partículas de polvo. | Movimiento fluido y visualmente atractivo. |
| **V2** | Las restas generaban ocasionalmente números negativos inadecuados para el nivel escolar. | Se ajustó la lógica de generación del banco de preguntas asegurando minuendos mayores que los sustraendos. | Operaciones adaptadas al público objetivo. |
| **V3** | En pantallas pequeñas la arena de combate se recortaba y no se leían bien las opciones. | Se aplicaron consultas de medios CSS (*Media Queries*) y tamaños fluidos con `clamp()`. | Interfaz 100% responsiva para computadoras y móviles. |

---

## Tabla de Validación y Pruebas (Peer Review)

Evaluación realizada durante la prueba cruzada de prototipo:

| Elemento Evaluado | Cumplimiento | Observaciones / Resultado |
| :--- | :---: | :--- |
| **Inicio correcto** | Sí | Carga de manera rápida sin errores en consola. |
| **Comprensión del juego** | Sí | Las instrucciones en la portada son claras. |
| **4 alternativas por pregunta** | Sí | Cada pregunta presenta 1 respuesta correcta y 3 distractores lógicos. |
| **Feedback de respuesta** | Sí | Muestra animación de ataque e indicadores visuales en verde o rojo. |
| **Actualización de puntaje** | Sí | El marcador HUD y la barra de progreso responden inmediatamente. |
| **Pantalla y resumen final** | Sí | Presenta el puntaje sobre 10 y un desglose detallado de las respuestas. |

---

## Aprendizajes y Mejoras Futuras

### Aprendizajes Clave
* Implementación de gráficos *Pixel Art* generados totalmente por código Canvas sin depender de assets externos.
* Manejo de estados de juego complejos (Navegación del mapa, Pausa de combate, Animaciones de feedback y Pantallas de fin de juego).
* Diseño UX/UI adaptado al estilo retro de los juegos de 8 bits.

### Mejoras para Versiones Futuras
* **Audio 8-Bit:** Integración de efectos de sonido sintetizados en Web Audio API para golpes, selección y victoria.
* **Power-ups / Ítems:** Añadir cofres secretos en el mapa con pociones para recuperar vidas al responder preguntas difíciles.
* **Modo de Dificultad:** Selección de nivel (Fácil, Medio, Difícil) incrementando el número de dígitos en las operaciones.
