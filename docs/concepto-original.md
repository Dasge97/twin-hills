# El camino hacia la torre
Documento de diseño v0.1 · 21 de noviembre de 2026 · Título de trabajo

## La partida que queremos que alguien cuente
«En el primer intento compré tanta velocidad que llegué al bosque antes de poder defenderme. Repetí la semilla y guardé fragmentos para la pisada. Esta vez, correr más rápido era precisamente lo que me mantenía vivo».

## Base acordada
- Fantasía y descubrimiento. Un personaje diminuto avanza entre dos colinas. La cámara deja espacio para mirar el camino. Al abrirse el valle se descubre una torre distante. Los faroles pueden dejar un rastro visible del viaje.
- El avance es continuo. Al principio se pulsa directamente sobre objetos y criaturas al entrar en alcance. Más adelante, combate y recogida funcionan solos. La intervención del jugador pasa a ser elegir mejoras. La precisión y los reflejos tienen poco peso.
- Hay muchas vías de inversión, con niveles sucesivos. Importan el orden de compra, el ahorro y el momento de acelerar. Llegar a una zona con una configuración insuficiente puede terminar la partida.
- Hay un destino y un tiempo que batir. Las zonas tienen identidad, pero la cantidad y disposición de encuentros varían. Una semilla compartida permite repetir el recorrido.
- La pantalla pasa de tranquila a desbordante. Las interacciones obedecen reglas observables. Una combinación extraordinariamente potente es un resultado deseable cuando el jugador ha descubierto cómo sostenerla.

## Reglas propuestas para la primera versión
El tiempo empieza con el primer paso y termina al cruzar la puerta con vida. Para la prueba corta, un farol hace de meta. Los enemigos que alcanzan al personaje le quitan vida. A cero, termina el intento. Se muestra distancia, tiempo y última fuente de daño, con opción de repetir la semilla.

Usar fragmentos como moneda común. Las compras se ofrecen durante la marcha y el saldo se puede guardar. Ataque manual y automático comparten intervalo. El primer nivel de recogida o ataque automático delega la tarea. Los siguientes amplían su capacidad. Una vez delegada, el jugador puede concentrarse en comprar.

Generar los encuentros por posición en el camino. En una misma semilla y versión, comprar velocidad cambia cuándo se llega y cuánto se aprovecha, mientras los encuentros mantienen su posición. Cada zona define familias de enemigos, recursos y densidades posibles. Probar la diversidad con varias semillas.

| Inversión | Cambio observable | Interacción importante |
|---|---|---|
| Marcha | Más metros por segundo | Acorta las ventanas de recogida y aumenta las pisadas por segundo. |
| Daño | Menos impactos para eliminar ciertos enemigos | Un nivel que cruza ese umbral puede liberar tiempo para otro objetivo. |
| Ataque automático | Primer golpe delegado y después menor intervalo | Permite sobrevivir a grupos incluso con poco daño por impacto. |
| Recogida | Primer recurso recogido solo y después mayor alcance | Recupera recursos que quedarían atrás al acelerar. |
| Pisada sísmica | Onda tras recorrer cierta distancia | Intervalo en segundos = distancia entre ondas / velocidad. Mostrar el cambio antes de comprar. |

## Ideas para ampliar tras el prototipo
Una luciérnaga puede tener radio de búsqueda, capacidad de vuelo y compañeras adicionales. Otra familia de mejoras podría enlazar recogidas, chispas y vetas. Cada fragmento recuperado por una luciérnaga contaría como recogida y podría activar la siguiente chispa. Una órbita de brasas ofrecería daño por tiempo de contacto. Preparar el final con una subida bajo asedio que permita llegar arrasando o escapar por poco. La semilla diaria es una opción posterior.

## Primera versión jugable
Objetivo provisional de unos tres minutos. Una cuesta entre colinas, entrada al bosque y farol final. Un enemigo, una veta, una moneda, cinco líneas de mejora y arte provisional. Priorizar que desde la cámara definitiva se distingan un recurso recogible, un enemigo peligroso y una pisada.

1. Recorrer el tramo, medir el tiempo, sufrir daño, morir, alcanzar la meta y reintentar.
2. Añadir encuentros por semilla, recogida y combate manual, compras y automatización. Comprobar que una partida automatizada solo exige tomar decisiones de inversión.
3. Incorporar la pisada. Repetir una semilla comprando velocidad primero, daño primero y ahorrando para pisada. Anotar compras con tiempo y distancia, causa de muerte o tiempo final y recursos abandonados.
4. Repetir en semillas distintas. Buscar al menos dos órdenes de inversión defendibles y una derrota comprensible. Observar si alguien reintenta por iniciativa propia para cambiar una compra. Si siempre domina la misma apertura, revisar ventanas de interacción, costes e ingresos antes de añadir contenido.

## Decisiones pendientes, por orden
| Momento | Decisión | Punto de partida |
|---|---|---|
| Antes de programar | Plataforma, control y motor | Probar en PC con ratón. Elegir un motor que permita iterar la cámara y usar los modelos GLB del proyecto. |
| Primera prueba | Vida, alcance, cadencia, precios y curva por nivel | Guardar los valores como datos ajustables. Medir cuántas compras caben antes del bosque. |
| Primera prueba | Compras y cronómetro | Probar compra con un clic durante la marcha. Observar si leer opciones penaliza demasiado al jugador. |
| Tras probar el recorrido | Pérdida al morir y progreso entre intentos | Empezar cada intento comparable con las mismas estadísticas. Valorar después descubrimientos o modos persistentes. |
| Tras varias semillas | Variabilidad, combinaciones dominantes y reglas de récord | Comparar por semilla y versión. Distinguir un hallazgo potente de una compra obligatoria en cada partida. |
| Cuando funcione el tramo | Duración total, zonas, catálogo, narrativa y presentación final | Ampliar a partir de decisiones que el jugador realmente disfrute repitiendo. |

## Cómo mantener este documento
Después de cada prueba, añadir una entrada breve con semilla, versión, orden de compra, resultado y cambio que se probará. Incorporar una regla al diseño consolidado cuando se decida conservarla. Llevar precios y fórmulas al archivo de datos del juego cuando exista el prototipo, para poder ajustar el equilibrio sin mantener dos copias.
