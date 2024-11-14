Este documento describe los requerimientos funcionales y los actores involucrados en el sistema de la compañía de productos alimenticios.

---

 ## Actores

- **Cliente**
- **Administrador del sistema**
- **Gestor de rutas**
- **Pasarela de pago**
- **Sistema de monitoreo externo**

---

## Requerimientos Funcionales

---
###  Clientes
- **Descripción**: Permite el acceso a los datos personales de los clientes.
- **Criticidad**: Crítico
- **Requisitos**:
  - El sistema debe permitir la consulta y actualización de los datos personales de cada cliente.
  - Los datos deben estar protegidos y solo accesibles por usuarios autorizados.

---

###  Pedidos
- **Descripción**: Permite a los clientes realizar pedidos de productos a la empresa.
- **Criticidad**: Semi-crítico
- **Requisitos**:
  - Cada cliente puede realizar un máximo de 3 intentos para hacer un pedido.
  - El sistema debe manejar eficientemente un gran número de pedidos simultáneos.
  - El proceso de pedido debe pasar por tres fases: preprocesado, autorización y aceptación. No es posible pasar a la siguiente fase sin completar la anterior.
  
---

###  Reparto y Rutas
- **Descripción**: Gestiona el reparto de flotas de transporte y las rutas de los camiones.
- **Criticidad**: Crítico
- **Requisitos**:
    - Asignar rutas a los camiones de reparto y optimizarlas en función de la demora.
    - Permitir el uso de dos algoritmos de optimización para calcular las rutas más eficientes.

---

###  Estadísticas
- **Descripción**: Proporciona información sobre el estado de los pedidos y la situación en tiempo real de los camiones.
- **Criticidad**: No crítico
- **Requisitos**:
  - El sistema debe mostrar estadísticas en tiempo real sobre los pedidos y la ubicación de los camiones.
  - Debe incluir información de clientes.

---

###  Incidencias
- **Descripción**: Reporta incidencias en la gestión de rutas, como camiones averiados o repartos no realizados.
- **Criticidad**: Semi-crítico
- **Requisitos**:
  - Los gestores de rutas deben recibir notificaciones de incidencias en tiempo real.

---

###  Pagos
- **Descripción**: Procesa los pagos de los clientes de forma segura utilizando una pasarela de pago externa.
- **Criticidad**: Crítico
- **Requisitos**:
    - Realizar pagos a través de la pasarela de MercadoLibre.
    - Confirmar transacciones y gestionar su verificación.

---