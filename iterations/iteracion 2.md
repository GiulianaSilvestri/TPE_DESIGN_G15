# Iteración 2

| Aspecto| Descripción |
|------|-------------|
| Drivers Seleccionados | - Acceso a los datos de los clientes. <br> - Seguridad, rendimiento, usabilidad. |
| Objetivo de la Iteración |  Evitar accesos no autorizados. |
| Elección de Conceptos de Diseño |  <ul><li>**Aunthenticate y Authorize**: para verificar la identidad de un usuario y determinar si tiene permisos para la acciones requeridas.</li><li>**Encrypt Data**: para proteger los datos y asegurar que solo las usuarios autorizados puedan acceder a ellos.</li><li> **API gateway**: punto de entrada centralizado para redirigir solicitudes, manejar politicas de seguridad, auntenticacion y balanceo de carga.    </li></ul>|
| Instanciar Elementos Arquitectónicos |  Interface: API gateway como único punto de entrada al sistema. |
| Diagramas y  Decisiones |  Decisiones: <br>- [API Gateway](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/ADRs/ADR003-API-gateway.md) <br><br>Diagramas:<br> [Vista de modulo API gateway](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it2_view_module.png) <br> [Vista de componentes](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it2_view_components.png) <br>- [Diagrama de secuencia](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it2_diagrama_de_secuencia.png) |