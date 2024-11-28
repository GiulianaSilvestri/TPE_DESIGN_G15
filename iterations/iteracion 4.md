# Iteración 4

| Aspecto| Descripción |
|------|-------------|
| Drivers Seleccionados |   - Asignar rutas a los camiones de reparto y optimizarlas en función de la demora.<br> - Permitir el uso de dos algoritmos de optimización para calcular las rutas más eficientes. <br> - Rendimiento en la optimización de rutas.|
| Objetivo de la Iteración | Optimizar y asignar rutas de reparto de manera eficiente. |
| Elemento a refinar | Microservicio de Reparto y Rutas. |
| Elección de Conceptos de Diseño |   <ul><li> **Increase Efficiency**: para almacenar resultados recientes de optimización, especialmente para rutas repetidas. </li><li> **Strategy**: para implementar cada algoritmo de optimización como una estrategia intercambiable, y permitir la seleccion del algoritmo en tiempo de ejecución basándose en las demoras de los camiones.</li></ul>|
| Instanciar Elementos Arquitectónicos | - Microservicio Reparto y Rutas:Responsabilidades: Asignación de rutas, optimización en tiempo real y comunicación con sistemas externos.  |
| Diagramas y  Decisiones | Decisiones: <br> [Strategy](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/ADRs/ADR006-Strategy-pattern.md) <br><br> Diagramas:<br> [Vista de modulo Strategy](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it4_view_module.png) 
