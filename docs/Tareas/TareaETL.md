# Tarea: ETL

# Introducción

**Objetivo**

Realizar un proceso ETL básico en Pyspark

**¿Para qué?**

Practicar lo aprendido en el tutorial de ETL

**¿Qué necesita?**

1. Modelo multidimensional asociado al proceso de movimientos
2. Notebook para trabajar: puede usar la seccion 3 "Espacio para desarrollar la tarea" al final del notebook del tutorial para realizar esta actividad
5. Servidor SQL con base de datos relacional "WWImportersTransactional" y base de datos relacional que corresponde a la bodega de WWI de cada estudiante "Estudiante_i"

# Enunciado
Ahora que sabe cómo realizar un proceso ETL, dado el modelo multidimensional del proceso de negocio de movimientos de inventario realice las siguientes actividades:
1. **Entregable 1 - Diseño del ETL:** Diseñe el ETL para las dimensiones proveedor, tipoTransaccion y para la tabla de hechos. A nivel de la tabla de proveedores incluya la tabla categoriasProveedores donde encuentra información de las categorías.
2. **Entregable 2 - Implementación del ETL:** implementación del proceso ETL para las dimensiones Proveedor, TipoTransaccion y para la tabla de hechos

Note que para este proceso de negocio, las dimensiones Producto, Cliente y Fecha son iguales a las del hecho Orden, este caso se conoce como dimensiones compartidas. Usted debe concentrarse en las dimensiones Proveedor, TipoTransaccion y la tabla de hechos que no existen en la bodega de datos actualmente.

![Modelo movimientos](Img/Modelo%20movimiento.png)


Sobre los resultados del entendimiento de datos, Wide World Importers les comenta lo siguiente:
- Los días de pago no pueden ser negativos no tiene sentido para nuestro negocio. Por favor corregir multiplicando los datos negativos por -1.
- Sobre "La cantidad máxima de productos movidos es 50 millones por viaje", encontramos que efectivamente gracias a los avances ya podemos cargar más que la cantidad de 50 millones por viajes. 
- La falta de datos antes del 2014 es un error de extracción de datos. Los nuevos datos incluyen este año.
- Nuestro análisis concluye que la información que se ha duplicado totalmente no es útil. Por favor no tenerlos en cuenta. 
- "El formato de fechas manejado es YYYY-MM-DD HH:MM:SS si tienen hora, minutos y segundos. De lo contrario el formato es YYYY-MM-DD": En cuanto a formatos de fechas estamos de acuerdo con que los estandarizemos y el formato sea el especificado en la regla de negocio.
- Existen proveedores que tienen 2 filas una con un nombre y otra con el mismo nombre mas un "Inc" o "Ltd". Unimos estos a un solo proveedor dado que se trató de un error de digitación.
- El código postal igual para todos nuestros proveedores es un error que también fue corregido.
- Cantidades negativas significan salidas de productos del inventario
