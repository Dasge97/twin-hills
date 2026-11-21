# Reglamento v1.0 de partida

Valores de diseño iniciales para implementar y medir. Metros, segundos y puntos enteros de vida. Inicio: 12 PV, 0 fragmentos, velocidad 2 m/s, alcance manual 8 m, daño 2, intervalo de ataque 1 s. Sin curación pasiva. Sin límite de nivel programado. Las fuentes comparten moneda y todos los niveles se reinician al morir.

## Compras
Coste del siguiente nivel con n niveles adquiridos = base + paso × n × (n+1)/2. Compra atómica si alcanza el saldo. Todas las habilidades avanzadas se habilitan al entrar al bosque. El prototipo incluye las primeras cinco desde el comienzo.

| ID | Base/paso | Efecto total al nivel n |
|---|---|---|
| marcha | 3/1 | 2 + 0,45n m/s |
| fuerza | 3/2 | 2 + 2n daño por golpe manual o automático |
| ataque | 4/2 | A partir de 1, golpe automático al enemigo en alcance con menor distancia absoluta longitudinal. Intervalo compartido con clic: 1/(1+0,2n) s, mínimo un tick. Sin enemigo, mina la veta más próxima en alcance. |
| recogida | 3/1 | Desde 1, luciérnaga recoge un fragmento cada 0,5 s dentro de 3+2n m. Vuelo de ida y vuelta visual. Manual siempre disponible. |
| pisada | 6/3 | Desde 1, onda cada 12/(1+0,25(n−1)) metros, daño 3+n en radio 5. Mantener distancia residual entre ondas, empezar a contar al comprar. |
| chispa | 7/2 | Cada quinta unidad física recogida dispara un rayo de 3+2n de daño a veta más cercana en 12 m, o enemigo si falta veta. Sin objetivo, se consume el disparo. |
| brasas | 6/2 | Cada 0,8 s inflige 2n a cada enemigo en radio 3+n m. Anillo visible alrededor del héroe. |
| eco | 8/3 | Cada muerte por daño del jugador suma n cargas. Por cada 4 cargas lanzar una pisada adicional de potencia igual a la actual (4 si falta pisada). Sus bajas vuelven a cargar eco. |

Una recogida cuenta una vez por entidad aunque valga varios fragmentos. Una veta rota genera unidades independientes a recoger; los enemigos muertos también. Los efectos pueden activar otros efectos. Cada muerte y cada rotura se resuelven una sola vez. Un grupo denso puede sostener una reacción completa; conservar estas interacciones. Las compras de recogida y ataque juntas automatizan el ciclo de extracción, combate y cobro.

## Encuentros
Todos usan distancia euclídea sobre el plano del camino. Recursos inmóviles. Clic en veta en alcance aplica fuerza con el enfriamiento compartido; clic en botín lo cobra inmediatamente. Daño de pisada y brasas afecta a enemigos, chispa también a vetas. Botín nace en el punto de muerte o rotura; valor de cada unidad = 1 salvo indicación. Retirar entidades a más de 18 m detrás. Distancias y activación enemiga se evalúan también durante persecuciones.

| Entidad | PV | Conducta | Recompensa |
|---|---:|---|---|
| Escarabajo | 4 | Desde 9 m se aproxima al viajero a 1,6 m/s. En contacto (1 m) causa 2 y desaparece. | 2 unidades |
| Lobo | 8 | Desde 12 m persigue a 3,6 m/s; contacto 3 y desaparece. | 3 unidades |
| Guardián | 16 | Desde 10 m avanza a 1 m/s; ataca en radio 2,5 m por 5 y desaparece. | 4 unidades |
| Cuarzo | 2 | Veta de pradera | 3 unidades |
| Ámbar | 5 | Veta de bosque | 4 unidades |
| Basalto rúnico | 8 | Veta de calzada | 5 unidades |
| Fragmento suelto | 1 recogida | Brillo fijo en el suelo | 1 unidad |

Distribuir el botín en círculo de radio 0,6 m; ángulos equidistantes según índice. Desaparición por contacto o descarte no da botín. Salud a cero prevalece sobre meta si coinciden en un tick. Faroles, farolera y torre son hitos escénicos. La torre no exige DPS mínimo ni matar jefe.
