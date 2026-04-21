# Agroflow

## Stakeholders
- Productor (Agricultores)
- Comerciante
- Transportista
- Administrador

### Enlace Historias de usuario
<a href="https://trello.com/invite/b/69e693841df73bb526e68bdf/ATTI29cdcbf8fc0a7585a1c116a0b63e618cF91A12E6/historias-de-usuario">Historias de usuario</a>

### Historias de Usuario + Criterios de Aceptación (con categorización)

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
| HU-C01 | Como comerciante, quiero registrarme para comprar productos | El usuario puede registrarse indicando su rol como comerciante. El sistema valida los datos ingresados y permite el acceso tras completar el registro correctamente. |
| HU-C02 | Como comerciante, quiero publicar mis necesidades | El usuario puede registrar producto requerido, cantidad, fecha y ubicación. El sistema valida los datos y publica la solicitud en la plataforma. |
| HU-C03 | Como comerciante, quiero buscar productos disponibles | El usuario puede visualizar una lista de productos disponibles. Puede aplicar filtros (tipo de producto, ubicación, fecha). El sistema devuelve resultados relevantes según los filtros aplicados. |
| HU-C04 | Como comerciante, quiero ver recomendaciones cercanas | El sistema muestra productores cercanos basándose en la ubicación del usuario. Las recomendaciones se ordenan por proximidad geográfica. |
| HU-C05 | Como comerciante, quiero generar pedidos | El usuario puede seleccionar una oferta y crear un pedido indicando cantidad y condiciones. El sistema registra el pedido y lo envía al productor correspondiente. |
| HU-C06 | Como comerciante, quiero hacer seguimiento de pedidos | El sistema muestra el estado del pedido (pendiente, aceptado, en tránsito, entregado). La información se actualiza automáticamente según cambios en el flujo. |
| HU-C07 | Como comerciante, quiero comparar precios | El sistema muestra múltiples ofertas del mismo producto con sus precios. El usuario puede visualizar diferencias de precio, ubicación y disponibilidad antes de decidir. |
| HU-C08 | Como comerciante, quiero calificar productores | El usuario puede dejar una calificación después de recibir un pedido. El sistema guarda la calificación y la refleja en el perfil del productor. |
| HU-T01 | Como transportista, quiero registrarme para ofrecer servicios | El usuario puede registrarse seleccionando el rol de transportista. El sistema valida los datos y permite el acceso al finalizar el registro. |
| HU-T02 | Como transportista, quiero publicar mi disponibilidad | El usuario puede ingresar rutas, horarios y capacidad de carga. El sistema valida la información y la publica para asignaciones futuras. |
| HU-T03 | Como transportista, quiero recibir solicitudes | El sistema muestra una lista de solicitudes de transporte disponibles. Cada solicitud incluye detalles del pedido, origen y destino. |
| HU-T04 | Como transportista, quiero aceptar servicios | El usuario puede aceptar una solicitud de transporte. El sistema asigna el transportista al pedido y actualiza el estado del servicio. |
| HU-T05 | Como transportista, quiero actualizar estado de entrega | El usuario puede cambiar el estado del pedido (recogido, en tránsito, entregado). El sistema actualiza la información en tiempo real para todos los involucrados. |
| HU-S01 | Como sistema, quiero sugerir coincidencias para facilitar ventas | El sistema analiza oferta y demanda y muestra coincidencias relevantes. Las coincidencias consideran producto, cantidad, ubicación y fechas. |
| HU-S02 | Como sistema, quiero enviar notificaciones | El sistema genera notificaciones automáticas ante eventos (nuevo pedido, aceptación, rechazo, entrega). Las notificaciones son entregadas de forma oportuna. |
| HU-S03 | Como sistema, quiero priorizar por cercanía | El sistema ordena resultados según la distancia entre usuarios. Se utiliza la ubicación registrada para calcular proximidad. |
| HU-A01 | Como administrador, quiero gestionar usuarios | El administrador puede ver, editar o bloquear usuarios. Los cambios se aplican inmediatamente en el sistema. |
| HU-A02 | Como administrador, quiero ver reportes | El sistema genera reportes de uso (usuarios activos, pedidos, transacciones). El administrador puede visualizar y consultar estos datos fácilmente. |