# Iteración 1

| Aspecto| Descripción |
|------|-------------|
| Drivers Seleccionados |  Interoperabilidad, Modificabilidad, Escalabilidad, Disponibilidad.|
| Objetivo de la Iteración |  Desacoplar los módulos funcionales existentes en microservicios independientes.   |
| Elección de Conceptos de Diseño |  <ul><li> **Microservice** para cada módulo funcional. </li><li> **API REST**: para facilitar la comunicación con protocolos HTTP/REST.  </li><li>  **Database per Service**: Bases de datos separadas por microservicio.  </li></ul>|
| Instanciar Elementos Arquitectónicos | Clientes, Pedidos, Pagos, Repartos y Rutas, Incidencias, y Estadisticas cada uno implementado como microservicio independiente, y base de datos particulares para cada microservicio.  <br> Interface: API REST para la comunicación. |
| Diagramas y  Decisiones | Decisiones: <br>- [Arquitectura basada en Microservicios](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/ADRs/ADR001-microservice-style.md) <br>- [Comunicación a través de HTTP/REST](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/ADRs/ADR002-API-REST.md) <br>- [Bases de datos separadas para cada microservicio](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/ADRs/ADR004-database-per-microservice.md)<br><br>Diagramas:<br> [Vista de componentes](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it1_view_components.png) <br> [Vista de despliegue](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it1_view_deployment.png) 
