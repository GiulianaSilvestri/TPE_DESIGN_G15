# Iteración 3

| Aspecto| Descripción |
|------|-------------|
| Drivers Seleccionados |  Escalabilidad|
| Objetivo de la Iteración | Garantizar un procesamiento eficiente y escalable de pedidos. |
| Elemento a refinar | Microservicio de Pedidos.|
| Elección de Conceptos de Diseño | **Event-Driven**: para desacoplar y procesar los pedidos como eventos asincronicamente y poder comunicarse con otros microservicios(Reparto y rutas, Estadisticas, etc).|
| Instanciar Elementos Arquitectónicos |   Event Bus: Canal de comunicación entre el microservicio de Pedidos y otros microservicios. |
| Diagramas y  Decisiones | Decisiones: <br> [Event Driven](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/ADRs/ADR005-EDA-pattern.md) <br><br> Diagramas:<br> [Vista de componentes](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it3_view_components.png) <br> [Diagrama de secuencia](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it3_diagrama_de_secuencia.png) 