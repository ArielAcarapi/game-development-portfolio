# EcoSort: Desafío de Reciclaje

[![Estado](https://img.shields.io/badge/Estado-Jugable-brightgreen?style=flat-square)](#)
[![Plataforma](https://img.shields.io/badge/Plataforma-Navegador_Web-blue?style=flat-square)](#)
[![Género](https://img.shields.io/badge/G%C3%A9nero-Arcade_%2F_Educativo-orange?style=flat-square)](#)
[![Tecnología](https://img.shields.io/badge/Tech-HTML5_%2F_CSS3_%2F_JS-yellow?style=flat-square)](#)

[Haga clic aquí para jugar en línea](https://ArielAcarapi.github.io/game-development-portfolio/EcoSort/)

---

## Descripción del Juego

EcoSort: Desafío de Reciclaje es un videojuego web educativo diseñado como solución al problema planteado por la organización ambiental EcoAcción. La propuesta aborda la falta de conocimiento sobre la separación correcta de residuos en la comunidad, especialmente en jóvenes y niños, mediante una experiencia dinámica e interactiva.

El jugador controla la posición horizontal de diferentes tipos de residuos que caen desde la parte superior de la pantalla. Su misión es guiarlos hacia el contenedor correspondiente antes de que toquen la base.

### Objetivo del Jugador
Clasificar la mayor cantidad posible de residuos orgánicos, papel/cartón y plásticos en sus respectivos contenedores para acumular puntos, conservar las vidas disponibles y establecer la puntuación máxima.

### Mecánica Principal
* Desplazamiento horizontal: Control de movimiento a la izquierda y derecha mediante teclado para dirigir el residuo activo mientras cae de forma continua.
* Clasificación por contenedores: Tres contenedores fijos en la base (Orgánicos, Papel/Cartón y Plásticos) con detección de colisión en tiempo real.
* Eventos especiales de salud: Aparición periódica de elementos de recuperación (corazones) que requieren ser dirigidos a un contenedor objetivo específico para restaurar una vida.
* Dificultad dinámica: Incremento progresivo de la velocidad de caída con cada acierto y penalización por errores.

---

## Ficha Técnica

| Parámetro | Detalle |
| :--- | :--- |
| Nombre Definitivo | EcoSort: Desafío de Reciclaje |
| Desarrollador | Ariel Vidal Acarapi Limachi |
| Género | Arcade / Educativo / Habilidad |
| Público Objetivo | Jóvenes y estudiantes de nivel secundario (11 a 16 años) |
| Plataforma | Web (Ejecución directa en navegador) |
| Lenguajes y Herramientas | HTML5, CSS3, JavaScript Vanilla, LocalStorage API |
| Estilo Visual | Interfaz adaptativa con degradados, animaciones CSS y elementos dinámicos |

---

## Controles e Instrucciones

### Controles de Teclado
* Flecha Izquierda / Tecla A: Mover el residuo hacia la izquierda.
* Flecha Derecha / Tecla D: Mover el residuo hacia la derecha.
* Botón de Inicio / Reinicio: Clic con el ratón o toque táctil para iniciar o reiniciar la partida.

### Reglas del Juego
1. Vidas Iniciales: La partida inicia con 3 vidas (con un límite máximo acumulable de 5).
2. Clasificación de Residuos:
   * Orgánicos: Residuos biodegradables como hojas, cáscaras o restos de comida.
   * Papel y Cartón: Hojas de papel, periódicos y cajas de cartón.
   * Plásticos: Botellas, envases y bolsas plásticas.
3. Puntuación y Dificultad:
   * Cada acierto otorga +10 puntos e incrementa ligeramente la velocidad de caída.
   * Los errores restan 1 vida e incrementan la velocidad como penalización adicional.
4. Evento de Corazón:
   * Cada 7 elementos aparece un corazón que indica un contenedor destino específico. Si se logra encajar correctamente, se restaura 1 vida y se otorgan +15 puntos.
5. Condición de Derrota: Perder todas las vidas disponibles. El juego almacena la puntuación máxima obtenida mediante la API de LocalStorage.

---

## Capturas de Pantalla

| Pantalla Principal | Pantalla de Juego |
| :---: | :---: |
| ![Pantalla de Inicio](./screenshots/EcoSortInicio.JPG) | ![Gameplay](./screenshots/EcoSortJuego.JPG) |

| Evento Especial | Pantalla de Game Over |
| :---: | :---: |
| ![Evento Corazón](./screenshots/EcoSortEvento.JPG) | ![Fin de Juego](./screenshots/EcoSortGameover.JPG) |
