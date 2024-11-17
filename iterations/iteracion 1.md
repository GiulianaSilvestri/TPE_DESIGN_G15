# Iteración 1

| Aspecto| Descripción |
|------|-------------|
| Drivers Seleccionados | - Permitir el acceso a los datos de los clientes. <br>   - Uso de protocolos HTTP/REST. <br> - Seguridad, disponibilidad, usabilidad. |
| Objetivo de la Iteración |   Desacoplar el módulo de Clientes creando un microservicio. |
| Elemento a refinar |  Módulo de Clientes. |
| Elección de Conceptos de Diseño |  <ul><li> **Microservice** para desacoplar  clientes </li><li>**Aunthenticate y Authorize**: para verificar la identidad de un usuario y determinar si tiene permisos para la acciones requeridas.</li><li>**Encrypt Data**: para proteger los datos y asegurar que solo las usuarios autorizados puedan acceder a ellos.</li><li>**Redundant Spare**: para que asuma el control en caso de fallo y garantizar la disponibilidad.</li><li> **API REST**: para facilitar la comunicación con protocolos HTTP/REST. </li><li> **API gateway**: punto de entrada centralizado para redirigir solicitudes, manejar politicas de seguridad, auntenticacion y balanceo de carga.   </li><li> **Database per Service** para Clientes.  </li></ul>|
| Instanciar Elementos Arquitectónicos | Microservicio de Clientes: Responsabilidades incluyen CRUD de datos de clientes y pagos. <br> Interfaces: API gateway como unico punto de entrada, API REST para acceso a datos de clientes. |
| Diagramas y  Decisiones | Decisiones documentadas en **ADR 1**, **ADR 2**, **ADR 3**, **ADR4** y los diagramas correspondientes a la iteracion 1 son: **it1_view_component**, **it1_diagrama_de_secuencia**. |
