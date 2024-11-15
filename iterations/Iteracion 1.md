
# Iteración 1

| **Aspectos**                      | **Descripción**                                                                                                                                                 |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Objetivo**           |  Migrar a una nueva arquitectura menos rígida y mas fácil de evolucionar.                                                                               |
| **Drivers seleccionados**           |  Escalabilidad, modificabilidad y disponibilidad.                                                                               |
| **Alternativas consideradas**   | - Mantener arquitectura monolítica                   - Migrar a una arquitectura de microservicios.    |
| **Decisión**             | Se optó por la arquitectura de microservicios documentado en **ADR 1**, que permite desacoplamiento, escalabilidad y despliegue independiente.                             |
| **Instanciar elementos**| Clientes, Pedidos, Pagos, Repartos y Rutas, Incidencias, y Estadisticas cada uno implementado como microservicio independiente.                            |
