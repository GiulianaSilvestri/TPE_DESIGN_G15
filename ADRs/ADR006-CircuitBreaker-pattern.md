# ADR006: Uso del patrón Circuit Breaker

## Contexto y Planteamiento del Problema
El sistema requiere un procesamiento eficiente y desacoplado de eventos como la creación y actualización de pedidos. La arquitectura actual basada en interacciones síncronas puede ser un cuello de botella para la escalabilidad y rendimiento del sistema.

## Impulsores de la Decisión
- Alta disponibilidad: Evitar interrupciones completas del sistema frente a fallas de servicios dependientes.
- Rendimiento: Reducir el tiempo de espera durante fallos.
- Resiliencia: Proveer mecanismos para manejar fallos y recuperarse de forma controlada.

## Opciones Consideradas
* Circuit Breaker.
* Sin Circuit Breaker.

## Resultado de la Decisión
Opción elegida: Circuit Breaker porque permite proteger el sistema de sobrecarga y fallos propagados.


## Consecuencias
- Bueno, porque mejora la experiencia del usuario al evitar tiempos de espera excesivos y simplifica el manejo de fallos.
- Malo, porque introduce complejidad adicional.



## Pros y Contras de las Opciones
### Sin Circuit Breaker
- Bueno: Diseño más simple.
- Malo: Riesgo de sobrecarga y fallos en cascada.

### Circuit Breaker
- Bueno: Manejo de fallos más robusto, protege contra efectos en cascada.
- Malo: Incrementa la complejidad del diseño.
