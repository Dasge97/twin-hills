# Twin Hills

Un viajero diminuto cruza dos colinas hacia una torre apagada. Empieza recogiendo fragmentos a mano y acaba atravesando el valle entre ondas sísmicas, brasas y descargas automáticas. El récord depende de cuánto puede acelerar sin morir antes de llegar.

**Estado:** diseño para implementación. **Destino acordado:** Windows x86-64 descargable, ratón, Godot con GDScript. Partida individual local. La v1 comprende tres zonas y una meta. Los valores iniciales requieren pruebas de juego.

## Empezar en el PC

1. Clonar con `git clone https://github.com/Dasge97/twin-hills.git` y entrar en `twin-hills`.
2. Instalar Godot estándar 4.5.1 estable y sus plantillas de exportación de la misma versión. Versión fijada para reproducibilidad. [Descarga oficial](https://godotengine.org/download/archive/4.5.1-stable/)
3. Abrir el repositorio en el editor de código y entregar al modelo [las instrucciones de implementación](AGENTS.md). Su primer encargo es el hito H1. El proyecto Godot se creará en la raíz.
4. Una vez implementado H1, importar project.godot en Godot y ejecutar con F6 la escena de recorrido o con F5 el juego.

## Documentos vigentes

- [Experiencia, interfaz y alcance](docs/juego.md)
- [Simulación, economía y contenido](docs/reglas.md)
- [Generación reproducible y arquitectura Godot](docs/tecnica.md)
- [Hitos y pruebas de aceptación](docs/entrega.md)
- [Inventario visual completo de la v1](arte/inventario.csv) y [producción con assets gratuitos y MeshFactory](arte/produccion.md)

El [concepto original](docs/concepto-original.md) conserva la conversación inicial. Los documentos vigentes resuelven sus preguntas abiertas.
