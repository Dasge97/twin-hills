# Orden de desarrollo

| Hito | Entrega comprobable | Prueba de salida |
|---|---|---|
| H1 · Escala y recorrido | Proyecto Godot, colinas, viajero, torre, giro visual, farol y cámara. Avance de 360 m, reloj y reinicio. | Ver captura a 720p y 1080p; distinguir héroe, punto interactivo y horizonte. A 2 m/s la llegada tarda 180 s con tolerancia de un tick. |
| H2 · Decisión | Fragmentos, cuarzo, escarabajo, clic, vida, daño, tienda, muerte y semilla. | Repetir semilla 42: lista inicial idéntica; nueva compra cambia saldo exactamente una vez. Una compra sin fondos mantiene el estado. |
| H3 · Prototipo jugable | Ataque, luciérnaga, pisada, historial, tiempo final, pausa de lectura. | Completar un intento tras automatizar sin más clics en el mundo. Comparar órdenes de compra en 1, 42 y 9001. Ver por qué murió una apertura imprudente. |
| H4 · Carrera completa | Bosque, calzada, especies y minerales restantes, farolera, encuentros en cadena, torre y registros. | Reproducir mismos comandos por tick a 30 y 144 FPS: mismo resultado. Romper una veta con chispa y comprobar que cada fragmento cuenta. Una baja por eco puede sostener otra onda. |
| H5 · Arte y entrega | Sustitución de modelos priorizados, opciones, audio, rendimiento y ZIP Windows. | Repetir la misma carrera antes/después de sustituir un GLB. Verificar controles, récords y arranque del ZIP extraído en Windows. |

## Prueba de equilibrio en H3 y H4
Registrar versión, semilla, orden y tick de compra, distancia final, vida, tiempo y causa. Comparar marcha primero, fuerza primero y ahorro para pisada. Buscar al menos dos aperturas defendibles en las tres semillas y que una inversión excesiva en marcha pueda acabar en derrota. Si una compra domina en todas, ajustar un parámetro y repetir. Comprobar también una partida de H4 con todas las habilidades activas y que el jugador entienda de dónde sale la reacción. La duración final es resultado del equilibrio; referencia inicial 5–10 minutos. Para H3, prueba humana: dejar jugar sin explicar la mejor compra y observar si la persona propone espontáneamente un cambio para el segundo intento.

## Audio
Prototipo con tonos sintetizados propios; señales diferenciadas para recogida, compra, daño, muerte, farol y victoria. H5 añade ambiente de viento, bosque y ascenso, con mezcla que atenúe repeticiones rápidas de recogida. Persistir volumen maestro. No requiere archivos visuales adicionales.
