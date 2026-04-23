# 🌱 Agroflow — Product Backlog

**Proyecto:** Agroflow  
**Versión:** 1.0  
**📋 [Ver Historias en Trello](https://trello.com/invite/b/69e693841df73bb526e68bdf/ATTI29cdcbf8fc0a7585a1c116a0b63e618cF91A12E6/historias-de-usuario)**

---

## 👥 Stakeholders

| Rol | Descripción |
|-----|-------------|
|  Productor | Agricultores que ofrecen productos |
|  Comerciante | Compran productos a los productores |
|  Transportista | Ofrecen servicios de transporte |
|  Administrador | Gestiona la plataforma |

---

## ✅ Requerimientos Funcionales

| ID | Requerimiento | Descripción |
|----|---------------|-------------|
| RF01 | Registro de usuarios | Permite el registro de productores, comerciantes y transportistas con validación de datos. |
| RF02 | Inicio de sesión | Autenticación mediante correo y contraseña. |
| RF03 | Gestión de perfil | Ver y editar información personal, ubicación y rol. |
| RF04 | Publicación de oferta | Productores registran productos con tipo, cantidad, fecha de cosecha y ubicación. |
| RF05 | Publicación de demanda | Comerciantes publican necesidades con producto, cantidad, fecha y ubicación. |
| RF06 | Matching oferta-demanda | El sistema sugiere coincidencias entre ofertas y demandas. |
| RF07 | Gestión de pedidos | Comerciantes generan pedidos desde ofertas disponibles. |
| RF08 | Aceptación/rechazo de pedidos | Productores aceptan o rechazan pedidos, actualizando su estado. |
| RF09 | Gestión de transporte | Transportistas registran disponibilidad, rutas y capacidad. |
| RF10 | Asignación de transporte | El sistema sugiere transportistas para pedidos confirmados. |
| RF11 | Seguimiento de pedidos | Estado en tiempo real: pendiente → aceptado → en tránsito → entregado. |
| RF12 | Notificaciones | Alertas sobre nuevos pedidos, cambios de estado y coincidencias. |
| RF13 | Historial de transacciones | Consulta de pedidos, ventas y entregas por usuario. |
| RF14 | Sistema de valoraciones | Calificación entre participantes al completar una transacción. |

---

## ⚙️ Requerimientos No Funcionales

| ID | Requerimiento | Descripción |
|----|---------------|-------------|
| RNF01 | Disponibilidad | El sistema debe estar disponible al menos el **99%** del tiempo. |
| RNF02 | Escalabilidad | Soportar crecimiento progresivo de usuarios y datos sin afectar el rendimiento. |
| RNF03 | Usabilidad | Interfaz intuitiva y accesible para usuarios con bajo nivel de alfabetización digital. |
| RNF04 | Rendimiento | Respuesta a operaciones principales en menos de **2 segundos**. |
| RNF05 | Seguridad | Autenticación segura, control de acceso y cifrado de datos. |
| RNF06 | Compatibilidad | Funciona en dispositivos móviles de gama media/baja y navegadores modernos. |
| RNF07 | Localización | Adaptado a contextos rurales: idioma, unidades de medida y baja conectividad. |
| RNF08 | Tolerancia a fallos | Manejo de fallos de red sin pérdida de información, con recuperación de datos. |

---

## 📖 Historias de Usuario

### 🌾 Productor

| ID | Historia | Criterios de Aceptación |
|----|----------|------------------------|
| HU-P01 | Como productor, quiero registrarme en la plataforma para poder ofrecer mis productos y poder venderlos frescos. | - Formulario con datos obligatorios (nombre, correo, contraseña, rol) <br> - El sistema valida que el correo no esté registrado <br> - La cuenta se crea y permite acceso al sistema |
| HU-P02 | Como productor, quiero publicar mis cultivos con fechas estimadas para encontrar compradores. | - Ingreso de tipo, cantidad, fecha de cosecha y ubicación <br> - Validación de campos obligatorios <br> - Publicación visible para otros usuarios |
| HU-P03 | Como productor, quiero actualizar mis cantidades disponibles para reflejar cambios en la producción mostrando que tal esta la cosecha actual. | - El usuario puede editar una publicación existente <br> - Los cambios se guardan y actualizan en tiempo real |
| HU-P04 | Como productor, quiero ver solicitudes de compra para decidir a quién vender así siempre tendré para escoger la mejor venta. | - Lista de pedidos con info del comprador, cantidad y fecha <br> - Lista se actualiza automáticamente |
| HU-P05 | Como productor, quiero aceptar o rechazar pedidos según mi capacidad y lo que sea mas efectivo. | - Puede marcar un pedido como aceptado o rechazado <br> - Estado actualizado inmediatamente <br> - El comprador recibe notificación |
| HU-P06 | Como productor, quiero solicitar un transporte para el envío de mis productos a el comprador | - Notificación cuando un comerciante realiza un pedido <br> - Visibles en plataforma y opcionalmente vía push o correo |
| HU-P07 | Como productor, quiero ver mi historial de ventas | - Listado de ventas con producto, cantidad, fecha y comprador <br> - Sin pérdida de información |
| HU-P08 | Como productor, quiero calificar compradores | - Asignar calificación y/o comentario tras una transacción <br> - Calificación asociada al perfil del comprador |
| HU-P09 | Como productor, quiero visualizar compradores cercanos para facilitar la venta | - Lista de comerciantes cercanos ordenados por proximidad <br> - Muestra ubicación y productos de interés de cada uno |

---

### 🛒 Comerciante

| ID | Historia | Criterios de Aceptación |
|----|----------|------------------------|
| HU-C01 | Como comerciante, quiero registrarme para poder comprar productos directamente a productores. | - Registro indicando rol de comerciante <br> - Validación de datos y acceso tras registro exitoso |
| HU-C02 | Como comerciante, quiero publicar mis necesidades para recibir ofertas directamente de los agricultores. | - Registro de producto requerido, cantidad, fecha y ubicación <br> - Validación y publicación en plataforma |
| HU-C03 | Como comerciante, quiero buscar productos disponibles para conseguir productos más frescos. | - Lista de productos disponibles con filtros (tipo, ubicación, fecha) <br> - Resultados relevantes según filtros |
| HU-C04 | Como comerciante, quiero comparar precios entre productores para conseguir lo que mas me potencie y economice mi trabajo. | - Muestra productores cercanos ordenados por proximidad |
| HU-C05 | Como comerciante, quiero ver recomendaciones de productores cercanos buscando la mejor calidad siempre. | - Selecciona una oferta, indica cantidad y condiciones <br> - Pedido registrado y enviado al productor |
| HU-C06 | Como comerciante, quiero generar pedidos fácilmente así pudiendo obtener lo que necesite. | - Muestra estado del pedido (pendiente, aceptado, en tránsito, entregado) <br> - Actualización automática |
| HU-C07 | Como comerciante, quiero comparar precios | - Visualiza múltiples ofertas del mismo producto <br> - Muestra diferencias de precio, ubicación y disponibilidad |

---

### 🚛 Transportista

| ID | Historia | Criterios de Aceptación |
|----|----------|------------------------|
| HU-T01 | Como transportista, quiero registrarme para ofrecer servicios | - Registro con rol de transportista <br> - Validación y acceso tras registro exitoso |
| HU-T02 | Como transportista, quiero publicar mi disponibilidad | - Ingreso de rutas, horarios y capacidad de carga <br> - Información publicada para asignaciones |
| HU-T03 | Como transportista, quiero recibir solicitudes de transporte | - Lista de solicitudes con detalles del pedido, origen y destino |
| HU-T04 | Como transportista, quiero aceptar o rechazar servicios según mi capacidad | - Puede aceptar una solicitud <br> - Sistema asigna al transportista y actualiza el estado |
| HU-T05 | Como transportista, quiero actualizar estado de entrega | - Puede cambiar estado: recogido → en tránsito → entregado <br> - Actualización en tiempo real para todos los involucrados |
| HU-T06 | Como transportista, quiero ver siempre el estado de la entrega | - Visualización del estado actual de pedidos asignados en todo momento |

---

### 🤖 Sistema

| ID | Historia | Criterios de Aceptación |
|----|----------|------------------------|
| HU-S01 | Como sistema, quiero sugerir coincidencias para facilitar ventas | - Analiza oferta y demanda considerando producto, cantidad, ubicación y fechas |
| HU-S02 | Como sistema, quiero enviar notificaciones | - Notificaciones automáticas ante eventos: nuevo pedido, aceptación, rechazo, entrega |
| HU-S03 | Como sistema, quiero priorizar por cercanía | - Ordena resultados por distancia usando la ubicación registrada |
| HU-S04 | Como sistema, quiero registrar todas las transacciones para la compra venta | - Almacena comprador, productor, producto, cantidad y fecha <br> - Disponible para consultas y auditoría |
| HU-S05 | Como sistema, quiero mostrar transportistas disponibles para el pedido | - Lista filtrada por ubicación, capacidad y disponibilidad del pedido |

---

### 🔧 Administrador

| ID | Historia | Criterios de Aceptación |
|----|----------|------------------------|
| HU-A01 | Como administrador, quiero gestionar usuarios | - Puede ver, editar o bloquear usuarios <br> - Cambios aplicados inmediatamente |
| HU-A02 | Como administrador, quiero ver reportes | - Reportes de usuarios activos, pedidos y transacciones |
| HU-A03 | Como administrador, quiero generar reportes de uso y peticiones de los clientes | - Reportes con solicitudes, frecuencia de uso y comportamiento <br> - Posibilidad de exportar o visualizar |

<br>

# 📋 Épicas Y Prioridad

| Epicas | Historia de Usuario | Prioridad      |
|----|---------------------|---------|
| De transporte | - HU-PO6 <br>  - HU-S05 <br> - HU-T02 <br> - HU-T03 <br> - HU-T04 <br> - HU-T05 <br> - HU-T06  | - Media <br> - Media <br> - Media <br> - Media <br> - Media <br> - Baja <br> - Baja  |
| De gestion de pedidos | - HU-C05 <br> - HU-C06 <br> - HU-PO4 <br> - HU-PO5 <br> - HU-S04  | - Media <br> - Alta <br> - Alta <br> - Alta <br> - Alta |
| De historial/reportes | - HU-A02 <br> - HU-A03 <br> - HU-P07  | - Baja <br> - Baja <br> - Media |
| De gestion de ofertas | - HU-P02 <br> - HU-P03 <br> - HU-P09  | - Alta <br> - Alta <br> - Media |
| De registro | - HU-P01 <br> - HU-C01 <br> - HU-T01  | - Alta <br> - Alta <br> - Media |

<br>

## Sprint #1

En este sprint se trabajo el apartado de registro de usuario y gestión de oferta manejando un puntaje de esfuerzo de 30, se adelantaron labores de analísis tales como la consolidación de la base de datos y algunos errores a lo largo del proceso.


| Historia de usuario | Prioridad | Valor    | 
|---------------------|-----------|----------|
| HU-P01 | Alta | 5 |
