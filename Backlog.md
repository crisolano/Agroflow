# Agroflow

## Stakeholders
- Productor (Agricultores)
- Comerciante
- Transportista
- Administrador

### Enlace Historias de usuario
<a href="https://trello.com/invite/b/69e693841df73bb526e68bdf/ATTI29cdcbf8fc0a7585a1c116a0b63e618cF91A12E6/historias-de-usuario">Historias de usuario</a>

### Requerimientos Funcionales

| ID | Requerimiento Funcional | Descripción |
|----|------------------------|------------|
| RF01 | Registro de usuarios | El sistema debe permitir el registro de productores, comerciantes y transportistas mediante un formulario con validación de datos obligatorios. |
| RF02 | Inicio de sesión | El sistema debe permitir la autenticación de usuarios mediante credenciales válidas (correo y contraseña). |
| RF03 | Gestión de perfil | Los usuarios deben poder visualizar y editar su información personal, incluyendo ubicación y tipo de rol. |
| RF04 | Publicación de oferta | Los productores deben poder registrar productos con información como tipo, cantidad estimada, fecha de cosecha y ubicación. |
| RF05 | Publicación de demanda | Los comerciantes deben poder publicar sus necesidades indicando producto, cantidad requerida, fecha y ubicación. |
| RF06 | Matching oferta-demanda | El sistema debe analizar y sugerir coincidencias entre ofertas de productores y demandas de comerciantes. |
| RF07 | Gestión de pedidos | Los comerciantes deben poder generar pedidos a partir de ofertas disponibles en la plataforma. |
| RF08 | Aceptación/rechazo de pedidos | Los productores deben poder aceptar o rechazar pedidos recibidos, actualizando su estado. |
| RF09 | Gestión de transporte | Los transportistas deben poder registrar su disponibilidad, rutas y capacidad de carga. |
| RF10 | Asignación de transporte | El sistema debe sugerir o asignar transportistas disponibles para pedidos confirmados. |
| RF11 | Seguimiento de pedidos | Los usuarios deben poder consultar el estado de los pedidos en tiempo real (pendiente, aceptado, en tránsito, entregado). |
| RF12 | Notificaciones | El sistema debe enviar notificaciones sobre eventos relevantes como nuevos pedidos, cambios de estado y coincidencias. |
| RF13 | Historial de transacciones | El sistema debe almacenar y permitir la consulta de pedidos, ventas y entregas realizadas por cada usuario. |
| RF14 | Sistema de valoraciones | Los usuarios deben poder calificar a otros participantes después de completar una transacción. |

### Requerimientos No Funcionales

| ID | Requerimiento No Funcional | Descripción |
|----|---------------------------|------------|
| RNF01 | Disponibilidad | El sistema debe estar disponible al menos el 99% del tiempo, garantizando acceso continuo a los usuarios. |
| RNF02 | Escalabilidad | El sistema debe ser capaz de soportar un crecimiento progresivo de usuarios y datos sin afectar el rendimiento. |
| RNF03 | Usabilidad | La interfaz debe ser intuitiva, fácil de usar y accesible para usuarios con bajo nivel de alfabetización digital. |
| RNF04 | Rendimiento | El sistema debe responder a consultas y operaciones principales en un tiempo menor a 2 segundos. |
| RNF05 | Seguridad | El sistema debe proteger la información mediante autenticación segura, control de acceso y cifrado de datos. |
| RNF06 | Compatibilidad | El sistema debe funcionar correctamente en dispositivos móviles de gama media y baja, así como en navegadores modernos. |
| RNF07 | Localización | El sistema debe adaptarse a contextos rurales, incluyendo idioma, unidades de medida y condiciones de conectividad. |
| RNF08 | Tolerancia a fallos | El sistema debe manejar fallos de red o errores sin pérdida de información, permitiendo recuperación de datos. |

### Historias de Usuario + Criterios de Aceptación

| ID | Historia de Usuario | Criterio(s) de Aceptación |
|----|--------------------|--------------------------|
| HU-P01 | Como productor, quiero registrarme para ofrecer mis productos | El usuario puede completar un formulario con datos obligatorios (nombre, correo, contraseña, rol). El sistema valida que el correo no esté registrado previamente. Al finalizar, la cuenta se crea exitosamente y permite el acceso al sistema. |
| HU-P02 | Como productor, quiero publicar mis cultivos para encontrar compradores | El usuario puede ingresar tipo de producto, cantidad estimada, fecha de cosecha y ubicación. El sistema valida que los campos obligatorios no estén vacíos. La publicación queda visible para otros usuarios en el sistema. |
| HU-P03 | Como productor, quiero actualizar mi oferta para reflejar cambios | El usuario puede editar los datos de una publicación existente. El sistema guarda los cambios correctamente y los actualiza en tiempo real. Los cambios se reflejan inmediatamente en las búsquedas. |
| HU-P04 | Como productor, quiero ver pedidos para decidir ventas | El sistema muestra una lista de pedidos asociados a sus productos. Cada pedido incluye información del comprador, cantidad solicitada y fecha. La lista se actualiza automáticamente al recibir nuevas solicitudes. |
| HU-P05 | Como productor, quiero aceptar o rechazar pedidos | El usuario puede seleccionar un pedido y marcarlo como aceptado o rechazado. El sistema actualiza el estado del pedido inmediatamente. El comprador recibe una notificación con la decisión. |
| HU-P06 | Como productor, quiero recibir notificaciones de interés | El sistema envía notificaciones cuando un comerciante realiza un pedido o muestra interés. Las notificaciones son visibles dentro de la plataforma y opcionalmente vía push o correo. |
| HU-P07 | Como productor, quiero ver mi historial de ventas | El sistema muestra un listado de ventas realizadas con detalles (producto, cantidad, fecha, comprador). El usuario puede consultar registros anteriores sin pérdida de información. |
| HU-P08 | Como productor, quiero calificar compradores | El usuario puede asignar una calificación numérica y/o comentario después de una transacción. El sistema guarda la calificación y la asocia al perfil del comprador. |
| HU-P09 | Como productor, quiero visualizar compradores cercanos para facilitar la venta | El sistema muestra una lista de comerciantes cercanos basada en la ubicación del productor. Los resultados se ordenan por proximidad geográfica. El productor puede visualizar información básica de cada comprador (ubicación, productos de interés). |
| HU-C01 | Como comerciante, quiero registrarme para comprar productos | El usuario puede registrarse indicando su rol como comerciante. El sistema valida los datos ingresados y permite el acceso tras completar el registro correctamente. |
| HU-C02 | Como comerciante, quiero publicar mis necesidades | El usuario puede registrar producto requerido, cantidad, fecha y ubicación. El sistema valida los datos y publica la solicitud en la plataforma. |
| HU-C03 | Como comerciante, quiero buscar productos disponibles | El usuario puede visualizar una lista de productos disponibles. Puede aplicar filtros (tipo de producto, ubicación, fecha). El sistema devuelve resultados relevantes según los filtros aplicados. |
| HU-C04 | Como comerciante, quiero ver recomendaciones cercanas | El sistema muestra productores cercanos basándose en la ubicación del usuario. Las recomendaciones se ordenan por proximidad geográfica. |
| HU-C05 | Como comerciante, quiero generar pedidos | El usuario puede seleccionar una oferta y crear un pedido indicando cantidad y condiciones. El sistema registra el pedido y lo envía al productor correspondiente. |
| HU-C06 | Como comerciante, quiero hacer seguimiento de pedidos | El sistema muestra el estado del pedido (pendiente, aceptado, en tránsito, entregado). La información se actualiza automáticamente según cambios en el flujo. |
| HU-C07 | Como comerciante, quiero comparar precios | El sistema muestra múltiples ofertas del mismo producto con sus precios. El usuario puede visualizar diferencias de precio, ubicación y disponibilidad antes de decidir. |
| HU-T01 | Como transportista, quiero registrarme para ofrecer servicios | El usuario puede registrarse seleccionando el rol de transportista. El sistema valida los datos y permite el acceso al finalizar el registro. |
| HU-T02 | Como transportista, quiero publicar mi disponibilidad | El usuario puede ingresar rutas, horarios y capacidad de carga. El sistema valida la información y la publica para asignaciones futuras. |
| HU-T03 | Como transportista, quiero recibir solicitudes | El sistema muestra una lista de solicitudes de transporte disponibles. Cada solicitud incluye detalles del pedido, origen y destino. |
| HU-T04 | Como transportista, quiero aceptar servicios | El usuario puede aceptar una solicitud de transporte. El sistema asigna el transportista al pedido y actualiza el estado del servicio. |
| HU-T05 | Como transportista, quiero actualizar estado de entrega | El usuario puede cambiar el estado del pedido (recogido, en tránsito, entregado). El sistema actualiza la información en tiempo real para todos los involucrados. |
| HU-T06 | Como transportista, quiero actualizar o ver siempre la entrega | El transportista puede visualizar en todo momento el estado actual de los pedidos asignados. El sistema permite actualizar el estado de la entrega en cada etapa del proceso. |
| HU-S01 | Como sistema, quiero sugerir coincidencias para facilitar ventas | El sistema analiza oferta y demanda y muestra coincidencias relevantes. Las coincidencias consideran producto, cantidad, ubicación y fechas. |
| HU-S02 | Como sistema, quiero enviar notificaciones | El sistema genera notificaciones automáticas ante eventos (nuevo pedido, aceptación, rechazo, entrega). Las notificaciones son entregadas de forma oportuna. |
| HU-S03 | Como sistema, quiero priorizar por cercanía | El sistema ordena resultados según la distancia entre usuarios. Se utiliza la ubicación registrada para calcular proximidad. |
| HU-S04 | Como sistema, quiero registrar todas las transacciones para la compra venta | El sistema almacena cada transacción realizada incluyendo datos de comprador, productor, producto, cantidad y fecha. La información queda disponible para consultas futuras y auditoría. |
| HU-S05 | Como sistema, quiero mostrar transportistas disponibles para el pedido | El sistema presenta una lista de transportistas disponibles según ubicación, capacidad y disponibilidad. Los resultados se filtran automáticamente según las necesidades del pedido. |
| HU-A01 | Como administrador, quiero gestionar usuarios | El administrador puede ver, editar o bloquear usuarios. Los cambios se aplican inmediatamente en el sistema. |
| HU-A02 | Como administrador, quiero ver reportes | El sistema genera reportes de uso (usuarios activos, pedidos, transacciones). El administrador puede visualizar y consultar estos datos fácilmente. |
| HU-A03 | Como administrador, quiero generar reportes de uso y peticiones de los clientes | El sistema permite generar reportes detallados que incluyan solicitudes de usuarios, frecuencia de uso y comportamiento en la plataforma. El administrador puede exportar o visualizar estos reportes. |

