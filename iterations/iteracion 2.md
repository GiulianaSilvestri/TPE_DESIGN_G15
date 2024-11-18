# Iteración 2

| Aspecto| Descripción |
|------|-------------|
| Drivers Seleccionados | - Permitir a los clientes realizar pedidos. <br>   - Uso de protocolos HTTP/REST. <br> - Escalabilidad, disponibilidad, rendimiento. |
| Objetivo de la Iteración |  Desacoplar el módulo de Pedidos creando un microservicio. |
| Elemento a refinar |  Módulo de Pedidos. |
| Elección de Conceptos de Diseño |  <ul><li> **Microservice** para desacoplar  Pedidos. </li><li> **API REST**: para facilitar la comunicación con protocolos HTTP/REST. </li><li>  **API gateway**: punto de entrada centralizado para redirigir solicitudes, manejar politicas de seguridad, auntenticacion y balanceo de carga.   </li><li>  **Database per Service** para Pedidos.</li><li> **Circuit Breaker**: para manejar fallos en las fases del proceso de pedidos.</li><li>**Event-Driven**: para desacoplar y procesar los pedidos como eventos asinconicamente, mejorando la escalabilidad y rendimiento.</li></ul>|
| Instanciar Elementos Arquitectónicos | Microservicio de Pedidos: Responsabilidades incluyen preprocesado, autorización y aceptación de pedidos. <br> Interfaces: API gateway como unico punto de entrada, API REST para gestión de pedidos. |
| Diagramas y  Decisiones | Decisiones documentadas en **ADR 1**, **ADR 2**, **ADR 3**, **ADR4**, **ADR5**, **ADR6** y los diagramas correspondientes a la iteracion 2 son: **it2_view_component**, **it2_diagrama_de_secuencia**. |