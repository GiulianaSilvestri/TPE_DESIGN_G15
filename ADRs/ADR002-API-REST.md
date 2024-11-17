
# ADR 002: API REST para la comunicación

## Contexto y planteamiento del problema

El sistema debe asegurar una comunicación rápida, segura y estandarizada entre los microservicios, también con sistemas externos como pasarelas de pago y logística. Esto es esencial para cumplir con los requisitos de interoperabilidad y seguridad.


## Impulsores de la decisión

* Interoperabilidad: Comunicación estándar y compatible con sistemas externos.
* Seguridad: Debe ser segura para proteger la integridad de los datos.
* Eficiencia: Bajo tiempo de respuesta en comunicación.

## Opciones consideradas

* API REST

## Resultado de la decisión
API REST, ya que permite interoperabilidad usando HTTP simplificando la integración con sistemas externos y asegurando la transmisión de datos.


### Consecuencias

* Bueno, porque facilita la integración con sistemas externos, utilizando estándares conocidos como HTTP.
* Malo, porque puede introducir una ligera sobrecarga en el rendimiento frente a opciones.
