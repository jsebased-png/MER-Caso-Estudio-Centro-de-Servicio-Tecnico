# Caso de Estudio: Centro de Servicio Técnico 

## Objetivo
Diseñar un modelo entidad-relación (MER) que represente el flujo de gestión de garantías en un centro de servicio técnico especializado en electrodomésticos de línea blanca y marrón.

## Entidades principales
- Cliente
- Producto
- OrdenServicio
- Técnico
- Repuesto

## Relaciones
- Cliente solicita OrdenServicio (1:N)
- Producto genera OrdenServicio (1:N)
- Técnico atiende OrdenServicio (1:N)
- OrdenServicio utiliza Repuesto (N:M)

## Construcción del modelo
El diagrama fue realizado en **diagrams.net (draw.io)**, representando entidades, atributos y relaciones con sus respectivas cardinalidades.  
Se exportó en formato PNG y se encuentra en la carpeta `/diagramas`.

## Aplicación práctica
Este modelo permite:
- Registrar clientes y productos con garantía.
- Gestionar órdenes de servicio técnico desde la entrada hasta la salida.
- Asignar técnicos y controlar repuestos utilizados.
- Generar reportes de estado de garantía (vigente, vencida, rechazada).
- Mantener trazabilidad completa de cada producto desde la compra hasta la reparación.
