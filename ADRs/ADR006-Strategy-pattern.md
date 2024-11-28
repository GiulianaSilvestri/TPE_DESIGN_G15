# ADR007: Uso del patrón Strategy 

## Contexto y Planteamiento del Problema
El módulo de Rutas y Repartos requiere optimizar las rutas para los camiones de reparto en función de la demora y eficiencia del transporte.

## Impulsores de la Decisión
- Rendimiento: Los algoritmos de optimización de rutas deben calcular rutas en menos de 5 segundos 
- Escalabilidad:El sistema debe soportar un incremento en la cantidad de camiones y puntos de entrega 
- interoperabilidad: necesidad de interactuar con sistemas externos sin imponer restricciones en los algoritmos internos de optimización. 
- modificabilidad: El sistema debe ser capaz de incorporar nuevos algoritmos de optimización de rutas en el futuro sin afectar el resto del microservicio.

## Opciones Consideradas
* Mantener los algoritmos fijos
* Usar Patrón Strategy para la selección dinámica de algoritmos


## Resultado de la Decisión
Opción elegida: Patrón Strategy, para seleccionar dinámicamente los algoritmos de optimización de rutas. Esto permitirá que el sistema elija el algoritmo adecuado para optimizar las rutas en función de los diferentes factores, cómo en tiempo real, congestión del tráfico, disponibilidad de camiones.

## Consecuencias
- Bueno, porque el sistema puede elegir el algoritmo según las condiciones del momento.
- Bueno, porque permite desacoplar la lógica de selección de algoritmos, facilitando la incorporación de nuevos algoritmos sin modificar el microservicio.
- Malo, porque implementar el patrón Strategy puede agregar complejidad inicial.
- Malo, porque si se integran muchos algoritmos, la gestión y el mantenimiento puede ser más complejo.


## Pros y Contras de las Opciones
### Mantener los algoritmos fijos
- Bueno, implementación sencilla, sin la necesidad de adaptarse dinámicamente a cambios en el entorno. 
- Malo, falta de flexibilidad para adaptarse a diferentes condiciones.
### Patrón Strategy 
- Bueno, flexibilidad para elegir algoritmos adecuados en función de las condiciones del momento.
- Bueno, puede adaptarse a nuevas funciones sin necesidad de modificar otras partes del sistema.
- Bueno, mejora la escalabilidad y la eficiencia del sistema. 
- Malo, introduce complejidad adicional en la arquitectura.