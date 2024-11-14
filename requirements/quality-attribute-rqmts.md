# Requisitos de atributos de calidad
---

## Clientes
---

### Seguridad
Los datos personales deben estar protegidos mediante autenticación, encriptación y control de acceso para evitar accesos no autorizados.

---

### Disponibilidad

En caso de caída del servidor de datos de clientes, el sistema debe usar réplicas de respaldo para mantener el acceso a los datos, recuperándose en menos de 2 segundos sin interrupciones visibles para el usuario.

---

### Usabilidad

 El sistema debe permitir que el usuario visualice y edite los datos de clientes de manera rápida y sencilla.

---
## Pedidos
---

### Disponibilidad

Si falla alguna fase del proceso de pedidos, el sistema debe reintentar la operación hasta tres veces y, si persiste el fallo, redirigir el pedido a un servidor de respaldo sin perder el estado actual del proceso. El tiempo total para la recuperación no debe superar los 2 segundos.

---

### Escalabilidad

El sistema debe ser capaz de soportar hasta 1000 pedidos por hora y distribuir carga en picos de demanda, escalando horizontalmente.

---

### Rendimiento

La fase de pedido debe completarse en menos de 3 segundos, y cada fase (preprocesado, autorización, aceptación) debe procesarse secuencialmente sin demoras perceptibles.

---

# Reparto y rutas

---
### Rendimiento
Los algoritmos de optimización de rutas deben realizarse en menos de 5 segundos para ajustar las rutas en tiempo real sin afectar la entrega.

---
## Interoperabilidad
 El sistema debe permitir la integracion con sistemas logísticos externos, usando API REST para una comunicación estandarizada y segura.

---

# Estadisticas
---

### Interoperabilidad
 El sistema debe permitir que el módulo de estadísticas se integre con sistemas externos para recibir o exportar datos de manera eficiente.

---
# Incidencias
---
### Rendimiento
Las notificaciones de incidencias deben procesarse en menos de 1 segundo desde su registro para ser visibles de inmediato por los gestores de rutas.


---

# Pagos
---
### Interoperabilidad

El sistema debe permitir la integracion con la pasarela de MercadoLibre de forma segura y rapida mediante API REST.

---
### Rendimiento
Cada transacción de pago debe completarse en menos de 2 segundos para asegurar fluidez en la experiencia del usuario.

---
### Seguridad
 Las transacciones deben protegerse mediante encriptación y autenticación para garantizar la privacidad y evitar fraudes.

---
### Disponibilidad
Si el servicio de pagos de MercadoLibre está fuera de línea, el sistema debe encolar las solicitudes de pago y procesarlas cuando la pasarela esté disponible, garantizando que ningún pago quede sin registrar.

---