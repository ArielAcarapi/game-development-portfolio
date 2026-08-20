# Agualto: El Reto del Agua

<div align="center">

![Estado](https://img.shields.io/badge/Estado-Jugable-brightgreen?style=for-the-badge)
![Plataforma](https://img.shields.io/badge/Plataforma-Navegador_Web-blue?style=for-the-badge)
![Género](https://img.shields.io/badge/G%C3%A9nero-Arcade_%2F_Roguelike_%2F_Top--Down-orange?style=for-the-badge)
![Tecnología](https://img.shields.io/badge/Tech-HTML5_Canvas_%2F_JS-yellow?style=for-the-badge)

[HAGA CLIC AQUÍ PARA JUGAR EN LÍNEA](https://ArielAcarapi.github.io/game-development-portfolio/Agualto/)

</div>

---

## Descripción del Juego

**Agualto: El Reto del Agua** es un videojuego web de acción y gestión en perspectiva superior (Top-Down 2D)[cite: 9]. Está diseñado para jóvenes de 18 a 25 años con el objetivo de motivar el consumo responsable de agua e hidratación a través de una experiencia dinámica e interactiva.

El jugador controla a un estudiante urbano que recorre un mapa extenso de la ciudad durante una jornada de 145 segundos dividida en cuatro etapas[cite: 9]. Para sobrevivir al desgaste físico y esquivar obstáculos en movimiento, debe gestionar su nivel de energía recolectando agua en estaciones distribuidas por el mapa.

### Objetivo del Jugador
Recolectar un total de **2.000 ml** de agua en las estaciones de hidratación antes de que finalice el tiempo límite (145 segundos) o de sufrir colapso por deshidratación y agotamiento físico.

### Mecánica Principal
* **Navegación y Exploración:** Desplazamiento omnidireccional sobre un mapa urbano de gran tamaño con cámara de seguimiento suave.
* **Hidratación y Dash:** Presionar la tecla **E** al acercarse a las estaciones para beber agua (+250 ml de agua y +50% de energía) y utilizar la **Barra Espaciadora** para realizar un impulso veloz (*dash*) de esquive.

---

## Ficha Técnica

| Parámetro | Detalle |
| :--- | :--- |
| **Nombre Definitivo** | Agualto: El Reto del Agua |
| **Desarrollador** | Ariel Vidal Acarapi Limachi |
| **Género** | Arcade / Roguelike / Top-Down 2D |
| **Público Objetivo** | Jóvenes de 18 a 25 años |
| **Plataforma** | Web (Ejecución directa en navegador) |
| **Lenguajes y Herramientas** | HTML5, CSS3, JavaScript Vanilla (Sin librerías externas), HTML5 Canvas API |
| **Estilo Visual** | Vista superior (*Top-Down*) con iluminación dinámica por ciclo diario y efectos de viñeta por fatiga |

---

## Controles e Instrucciones

El juego está diseñado para ejecutarse en computadoras y laptops mediante teclado:

* **W / A / S / D o Flechas de Dirección:** Mover al personaje por el mapa urbano.
* **Tecla E:** Interactuar con las estaciones de hidratación para beber agua.
* **Barra Espaciadora:** Realizar un *dash* de aceleración instantánea.

### Reglas de Juego
1. **Duración de la Jornada:** El recorrido dura **145 segundos** distribuidos en 4 fases del día (Mañana, Mediodía, Tarde y Noche).
2. **Consumo de Energía:** Correr desgasta constantemente la barra de vitalidad del jugador.
3. **Obstáculos y Daño:** Colisionar contra los elementos rojos en movimiento descuenta un **28% de energía** inmediatamente.
4. **Efecto de Cansancio:** Si la energía cae por debajo del **25%**, la velocidad del personaje se reduce y la pantalla genera un filtro visual de viñeta simulando fatiga.
5. **Condición de Victoria:** Alcanzar los **2.000 ml** de agua recolectada en las estaciones antes de agotarse el tiempo.
6. **Condición de Derrota:** Quedarse sin energía (0%) o finalizar los 145 segundos sin completar los 2.000 ml de agua.

---

## Capturas de Pantalla

| Pantalla Principal | Exploración del Mapa |
| :---: | :---: |
| ![Pantalla de Inicio](./screenshots/AgualtoInicio.JPG) | ![Mapa en Vivo](./screenshots/AgualtoJuego.JPG) |

| Estación de Hidratación | Pantalla de Victoria |
| :---: | :---: |
| ![Estación de Agua](./screenshots/AgualtoEstacion.JPG) | ![Pantalla Final](./screenshots/AgualtoVictoria.JPG) |

---

### Registro de Mejoras e Iteraciones

| Versión | Problema Detectado | Acción Realizada | Resultado |
| :---: | :--- | :--- | :--- |
| **V1** | El mapa era reducido y la recolección de agua no representaba un reto de exploración. | Se expandió el escenario a 2400x1500 píxeles con cámara de seguimiento fluido. | Obliga al jugador a navegar y planificar su ruta urbana. |
| **V2** | No se percibía el impacto físico real de la deshidratación en el gameplay. | Se implementó la penalización de velocidad y el filtro radial por fatiga al bajar del 25% de energía. | Transmite visualmente la sensación de cansancio extremo. |
| **V3** | Las estaciones no recuperaban suficiente vitalidad para justificar el uso del *dash*. | Se ajustó la recarga a +250 ml de agua y +50% de energía inmediata. | Experiencia de juego más equilibrada y competitiva. |

---

## Aprendizajes y Mejoras Futuras

### Aprendizajes Clave
* Implementación de sistemas de cámara 2D con desplazamiento y límites de mundo en HTML5 Canvas.
* Diseños de mecánicas de juego donde los estados de vitalidad alteran directamente los parámetros de movilidad y renderizado visual.
* Estructuración de bucles de juego estilo *Roguelike* adaptados a sesiones cortas para navegador web.

### Mejoras para Versiones Futuras
* **Minimapa:** Inclusión de un radar en la esquina de la pantalla para ubicar las estaciones disponibles.
* **Efectos de Audio:** Integración de sonido sintetizado para el paso de fases, colisiones y recarga de agua.
* **Tabla de Marcadores:** Registro local y en línea de los mejores tiempos de finalización.
