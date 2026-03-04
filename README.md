# Videojuego de la paz


## 1. Introducción
**La paz** es un videojuego de temática pacifista desarrollado en Java utilizando el framework **libGDX**. 

* **Temática:** Captura las bombas con cursores o ratón en un limite de tiempo.
* **Personaje:** El jugador controla un guerrillero que recoge las bombas para que no caigan en la gente.
* **Condición de Victoria:** Rescatar al menos **10 elementos** en un tiempo límite de **2 minutos**.
* **Condición de Derrota:** Si el temporizador llega a cero y no se ha alcanzado el cupo mínimo de rescate.

## 2. Desarrollo Técnico

### Lógica y Mecánicas
* **Colisiones (AABB):** Se utiliza la clase `Rectangle` y el método `overlaps()` para detectar la colisión entre el avatar y los elementos de caída. Es una detección basada en cajas delimitadoras alineadas a los ejes.
* **Movimiento Independiente:** El desplazamiento del avatar y la caída de los objetos se multiplican por `Gdx.graphics.getDeltaTime()`. Esto garantiza que el juego corra a la misma velocidad en un PC potente o en un móvil antiguo.
* **Sistema de Estados:** Se implementó un `enum GameState` con los estados `PLAYING`, `WIN` y `LOSS` para gestionar el flujo de la partida.

### Estructura del Proyecto
* **Módulo Core:** Contiene la clase `Main.java` donde reside toda la lógica compartida.

* **Viewport:** Uso de `FitViewport(8, 5)` para mantener la relación de aspecto sin deformaciones en diferentes pantallas.

## 3. Conclusiones
El desarrollo de este proyecto permitió familirizarme con la plataforma y aprender un poco más de lógica, mecánica etc. También a manejar mejor los assets.
---
**Desarrollado por:** [Hector RG]
**Versión:** 1.0 - 2026
