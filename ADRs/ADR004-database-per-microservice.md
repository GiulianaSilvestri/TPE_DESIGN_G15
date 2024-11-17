
# ADR 004: Base de datos para cada microservicio

## Contexto y planteamiento del problema
Cada microservicio debe gestionar su propia base de datos para que pueda escalar y evolucionar de manera independiente, maximizando la modularidad y reduciendo el acoplamiento entre servicios.

## Impulsores de la decisión
* Desacoplamiento: Reducir dependencias entre microservicios.
* Escalabilidad: Escalar cada base de datos según las necesidades del microservicio.
* Mantenibilidad: Permitir la evolución independiente de cada base de datos.



## Opciones consideradas
* Base de Datos Compartida
* Bases de Datos Independientes



## Resultado de la decisión

Opción elegida: Bases de Datos Independientes, porque permite independencia en el manejo de datos y escalabilidad según las necesidades de cada servicio.

### Consecuencias

* Bueno: Desacoplamiento total entre servicios, mejorando la escalabilidad y modificabilidad.
* Malo: Requiere sincronización de datos 


## Pros y contras de las opciones

### Base de Datos Compartida
* Bueno, porque reduce la complejidad de gestión de datos.
* Malo, porque introduce dependencias directas entre los microservicios y limita la escalabilidad.

### Bases de Datos Independientes
* Bueno, porque permite escalabilidad y evolución independiente de cada base de datos.
* Malo, porque requiere sincronización y dificulta la gestión de datos. .


