# ADR005: Uso de Event-Driven Architecture (EDA)

## Contexto y Planteamiento del Problema
El sistema requiere un procesamiento eficiente y desacoplado de eventos como la creación y actualización de pedidos. La arquitectura actual basada en interacciones síncronas puede ser un cuello de botella para la escalabilidad y rendimiento del sistema.

## Impulsores de la Decisión
- Escalabilidad: El sistema debe soportar pedidos simultaneos sin afectar el rendimiento.
- Desacoplamiento: Minimizar dependencias directas entre servicios.
- Rendimiento: Permitir un procesamiento eficiente de eventos de pedidos de forma paralela.

## Opciones Consideradas
* Arquitectura basada en eventos (EDA)
* Sin EDA: Mantener las interacciones síncronas.

## Resultado de la Decisión
Opción elegida: Arquitectura basada en eventos (EDA) porque permite procesar cada fase del pedido como un evento independiente, mejorando la escalibilidad y el rendimiento.


## Consecuencias
- Bueno, porque permite procesamiento distribuido y eficiente de pedidos.

- Malo, porque introduce complejidad en la configuración y monitoreo del sistema de mensajería.



## Pros y Contras de las Opciones
### Sin EDA
- Malo: Dificultad para escalar y desacoplar servicios.

### Arquitectura basada en eventos (EDA)
- Bueno: Procesamiento eficiente, escalabilidad y desacoplamiento.
- Malo: Complejidad adicional en la implementación y monitoreo.
