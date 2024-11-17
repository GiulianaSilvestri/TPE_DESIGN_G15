
# ADR 003: Uso de API gateway para control de acceso

## Contexto y planteamiento del problema
El sistema requiere un único punto de entrada para manejar la autenticación, autorización, y balanceo de carga, facilitando la administración de seguridad y simplificando el acceso del cliente a los servicios.

## Impulsores de la decisión
* Seguridad: Control centralizado de autenticación y autorización.
* Simplicidad para el cliente: Un único punto de entrada para acceder a los servicios.
* Balanceo de carga: Redistribuir tráfico de manera eficiente.


## Opciones consideradas
* API Gateway
* Acceso Directo


## Resultado de la decisión

Opción elegida: API Gateway, ya que centraliza el acceso, simplifica el control de autenticación y autorización, y permite balanceo de carga

### Consecuencias

* Bueno, porque permite controlar y proteger el acceso a los microservicios de manera centralizada.
* Malo, porque introduce un punto único de fallo y agrega latencia al flujo de datos.

## Pros y contras de las opciones

### API Gateway
* Bueno, porque centraliza la gestión de acceso y facilita la autenticación y autorización.
* Bueno, porque permite balanceo de carga y análisis de tráfico.
* Malo, porque introduce un punto único de fallo y puede añadir latencia.

### Acceso Directo
* Bueno, porque simplifica la configuración de los microservicios.
* Malo, porque cada cliente debe gestionar su acceso a cada microservicio.