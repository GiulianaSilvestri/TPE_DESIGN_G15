
# ADR 001: Uso del estilo de arquitectura de microservicios

## Contexto y planteamiento del problema

El sistema de la compañía de productos alimenticios se ha desarrollado con una arquitectura monolítica. Esto implica que todas las funcionalidades están integradas en un único sistema interdependiente, lo que dificulta su escalabilidad, mantenibilidad, y adaptabilidad a nuevos requerimientos. La compañía desea transformar su sistema actual en uno más flexible y adaptable.


## Impulsores de la decisión

* Escalabilidad: Escalar cada componente por separado es clave para gestionar picos de demanda.

* Disponibilidad: Mantener el sistema operativo incluso cuando un componente específico falla.

* Modificabilidad y Despliegue: Facilitar el despliegue y actualización independiente de cada funcionalidad.

* Flexibilidad y Adaptabilidad: Permitir que el sistema evolucione y se adapte más fácilmente a cambios en los requerimientos.

## Opciones consideradas

* Mantener la Arquitectura Monolítica
* Migrar a una Arquitectura de Microservicios


## Resultado de la decisión

Migrar el sistema de una [arquitectura monolítica](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/Architecture/Arquitectura_inicial.png) a una [arquitectura de microservicios](https://github.com/GiulianaSilvestri/TPE_DESIGN_G15/blob/main/diagrams/it1_view_components.png), porque permite el desacoplamiento entre los distintos módulos del sistema, adaptándose mejor a los drivers.


### Consecuencias

* Bueno porque permite mayor flexibilidad para modificar, escalar y desplegar módulos.
* Bueno porque reduce el impacto de fallos, mejorando la disponibilidad general del sistema.
* Malo porque aumenta la complejidad de la comunicación entre servicios y la administración de infraestructura.
