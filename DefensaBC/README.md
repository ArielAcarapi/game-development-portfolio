# Defensa del Bolsillo Central

[![Estado](https://img.shields.io/badge/Estado-Jugable-brightgreen?style=flat-square)](#)
[![Plataforma](https://img.shields.io/badge/Plataforma-Navegador_Web-blue?style=flat-square)](#)
[![Género](https://img.shields.io/badge/G%C3%A9nero-Tower_Defense_%2F_Educativo-orange?style=flat-square)](#)
[![Tecnología](https://img.shields.io/badge/Tech-HTML5_%2F_CSS3_%2F_JS-yellow?style=flat-square)](#)

[Haga clic aquí para jugar en línea](https://ArielAcarapi.github.io/game-development-portfolio/03-defensa-bolsillo-central/)

---

## Descripción del Juego

Defensa del Bolsillo Central es un videojuego web educativo de estrategia en tiempo real diseñado para concientizar sobre la gestión responsable del presupuesto y la educación financiera. A través de una mecánica interactiva de Tower Defense en perspectiva isométrica, el jugador aprende la importancia de mantener fondos de reserva y atender el desgaste constante de las obligaciones financieras.

El jugador debe gestionar un capital limitado mientras construye e invierte en estructuras defensivas para detener hordas de gastos imprevistos, pasivos y deudas que intentan desequilibrar sus finanzas.

### Objetivo del Jugador
Superar las 10 oleadas de amenazas económicas protegiendo el centro financiero personal, administrando el flujo de caja sin superar el tope estricto de capital y evitando la bancarrota total.

### Mecánica Principal
* **Renderizado Isométrico:** Visualización en cuadrícula isométrica 2D proyectada dinámicamente sobre HTML5 Canvas sin motores gráficos externos.
* **Sistema de Durabilidad y Mantenimiento:** Las estructuras sufren una degradación continua por segundo (`hpDegradationRate`). El jugador debe reinvertir fondos para subirlas de nivel y restaurar su vida al 100%.
* **Tope de Reserva e Inversión:** Límite estricto de acumulación de capital en 1000 monedas. Es obligatorio construir Torres de Inversión para generar dividendos y financiar los costos de mantenimiento.
* **Síntesis de Audio Procedural:** Generación de efectos de sonido en tiempo real utilizando la Web Audio API mediante osciladores y nodos de ganancia.

---

## Ficha Técnica

| Parámetro | Detalle |
| :--- | :--- |
| Nombre Definitivo | Defensa del Bolsillo Central |
| Desarrollador | Ariel Vidal Acarapi Limachi |
| Género | Tower Defense / Educativo / Estrategia |
| Público Objetivo | Jóvenes, estudiantes y adultos interesados en finanzas personales |
| Plataforma | Web (Ejecución directa en navegador) |
| Lenguajes y Herramientas | HTML5 Canvas, CSS3, JavaScript Vanilla, Web Audio API |
| Estilo Visual | Proyección isométrica 2D con animaciones e interfaz adaptativa |

---

## Controles e Instrucciones

### Controles de Interacción
* **Clic Izquierdo / Toque Táctil:** Seleccionar casillas de la cuadrícula isométrica para construir torres o seleccionar una torre existente para ver sus estadísticas.
* **Menú de Compra / Mejora:** Hacer clic en los botones de interfaz para elegir el tipo de torre a desplegar o ejecutar la mejora/reparación de la torre seleccionada.

### Reglas del Juego
1. **Límite de Capital:** El jugador inicia con un presupuesto y un tope máximo acumulable de **1000 monedas**.
2. **Mantenimiento Obligatorio:** Las torres pierden salud paulatinamente. Si la barra de durabilidad llega a cero, la estructura colapsa y desaparece del mapa.
3. **Estructuras Disponibles:**
   * **Ahorro Primario:** Ataque continuo de costo accesible para frenar gastos menores.
   * **Fondo de Emergencia:** Alto daño de área diseñado para contener picos de gasto pesados.
   * **Torre de Inversión:** Estructura no ofensiva que genera flujo de caja periódico.
4. **Oleadas y Dificultad:**
   * A partir de la oleada 5, los enemigos incrementan sustancialmente sus puntos de vida y protección.
   * En la oleada 10 aparece el jefe final "Deuda de Tarjeta", requiriendo máxima capacidad defensiva.
5. **Condición de Derrota:** Permitir que las deudas y gastos destruyan la base financiera (agotar la vida del bolsillo principal).

---

## Capturas de Pantalla

| Pantalla Principal | Pantalla de Juego |
| :---: | :---: |
| ![Pantalla de Inicio](./screenshots/BolsilloInicio.JPG) | ![Gameplay Isométrico](./screenshots/BolsilloJuego.JPG) |

| Menú de Mantenimiento | Pantalla de Game Over |
| :---: | :---: |
| ![Reparación de Torres](./screenshots/BolsilloMejora.JPG) | ![Bancarrota](./screenshots/BolsilloGameover.JPG) |

---

### Tabla de Pre-producción

| Aspecto | Descripción |
| :--- | :--- |
| Nombre del juego | Defensa del Bolsillo Central |
| Género | Tower Defense / Educativo / Estrategia |
| Objetivo del jugador | Proteger la base económica de 10 oleadas de gastos manteniendo el presupuesto bajo control. |
| Mecánica principal | Construcción, gestión de dividendos y mantenimiento/reparación constante de torres isométricas. |
| Reglas del juego | Límite de 1000 monedas, degradación de salud por segundo y necesidad de mejorar torres para sanarlas. |
| Condición de victoria | Derrotar al jefe final "Deuda de Tarjeta" en la oleada 10. |
| Condición de derrota | Perder la salud total del bolsillo central ante las invasiones de deudas. |
| Enseñanza sobre finanzas | Comprensión del fondo de reserva, prevención de deudas e importancia del mantenimiento de activos. |
| Jugador objetivo | Jóvenes y adultos interesados en la toma de decisiones financieras estratégicas. |

### Registro de Iteraciones de Producción

| Versión | Problema Detectado | Acción Realizada | Resultado |
| :---: | :--- | :--- | :--- |
| V1 | La acumulación ilimitada de dinero provocaba que el jugador llenara el mapa sin esfuerzo táctico. | Se estableció un límite estricto de reserva de 1000 monedas e inclusión de dividendos periódicos. | Toma de decisiones más estratégica en el gasto e inversión del capital. |
| V2 | Las torres permanecían indefinidamente activas restando dinamismo a la partida. | Se añadió la tasa de degradación por segundo (`hpDegradationRate`) y reparación al subir de nivel. | Exigencia de mantenimiento activo e intervención constante del jugador. |
| V3 | Dependencia de archivos externos de audio generaba retrasos en la carga del navegador. | Se implementó la síntesis de sonido procedural mediante la Web Audio API. | Rendimiento óptimo, carga inmediata y cero dependencias de assets externos. |

---

## Aprendizajes y Mejoras Futuras

### Aprendizajes Clave
* Transformación de coordenadas de pantalla a matriz isométrica (`gridToScreen` / `screenToGrid`) en HTML5 Canvas.
* Programación de síntesis de audio procedural en tiempo real con Web Audio API.
* Gestión de sistemas económicos cerrados con límites de liquidez dentro de un game loop.

### Mejoras Futuras
* Persistencia del récord final de reserva mediante la integración de `LocalStorage API`.
* Implementación de habilidades especiales activas como "Ajuste Monetario" o "Congelación de Gastos".
* Refactorización modular dividiendo la lógica en componentes independientes (ES Modules).
