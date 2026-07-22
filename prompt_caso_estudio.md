Caso de Estudio: Centro de Servicio Técnico (Línea Blanca y Marrón)

Objetivo:
Diseñar un modelo entidad-relación (E-R) que represente el flujo de gestión de garantías en un centro de servicio técnico especializado en electrodomésticos de línea blanca (lavadoras, neveras, hornos) y línea marrón (televisores, equipos de sonido, consolas).

Requerimientos:
1. Registrar clientes que solicitan garantía.
2. Asociar productos con sus respectivas marcas y modelos.
3. Gestionar órdenes de servicio técnico (entrada, diagnóstico, reparación, salida).
4. Relacionar técnicos con las órdenes de servicio asignadas.
5. Controlar repuestos utilizados en reparaciones.
6. Generar reportes de estado de garantía (vigente, vencida, rechazada).
7. Permitir trazabilidad de cada producto desde la compra hasta la reparación.

Entidades Principales:
- Cliente (ID_Cliente, Nombre, Teléfono, Dirección, Email)
- Producto (ID_Producto, Categoría, Marca, Modelo, Fecha_Compra, Estado_Garantía)
- OrdenServicio (ID_Orden, Fecha_Entrada, Diagnóstico, Estado, Fecha_Salida)
- Técnico (ID_Técnico, Nombre, Especialidad, Teléfono)
- Repuesto (ID_Repuesto, Nombre, Código, Precio)
- Garantía (ID_Garantía, Fecha_Inicio, Fecha_Fin, Estado)

Relaciones:
- Cliente solicita OrdenServicio (1:N)
- Producto genera OrdenServicio (1:N)
- Técnico atiende OrdenServicio (1:N)
- OrdenServicio utiliza Repuesto (N:M)
