# Tarea: Entendimiendo de los datos

# Introducción

**Objetivo**

Realizar el proceso de entendimiento de datos de WWImporters a través de perfilamiento general, análisis de reglas de negocio, estadísticos y análisis de calidad de datos.

**¿Para qué?**

Practicar lo aprendido en el tutorial de entendimiento de los datos.

**¿Qué necesita?**

1. Notebook para trabajar: puede usar la seccion 5 "Tarea" al final del notebook del tutorial para realizar esta actividad
2. Acceso a la base de datos WWImportersTransactional

# Enunciado

Ahora que ya aprendió a usar PySpark para exploración y preprocesamiento de datos, lo invitamos a que realice el proceso de entendimiento de datos de la tabla movimientosCopia, que registra el movimiento en inventario de un producto. La empresa no compartió información de las tablas de clientes ni de proveedores. Adicionalmente, el negocio indica que las tablas de categoriasProveedores y TiposTransaccion fueron analizadas previamente, por su grupo de consultores.

En esta actividad le recomendamos revisar el diccionario de datos suministrado y en particular la información relacionada con la tabla **movimientosCopia**. Si tienen alguna duda relacionada con esta tabla deben incluirla en las preguntas o aclaraciones que le entreguen al negocio. En relación a los datos Wide World Importers menciona:

- La cantidad máxima de productos movidos es 50 millones por transacción
- Existen 236.668 movimientos de producto realizados desde 2013
- Los movimientos están relacionados con 228.265 clientes
- El formato de fechas manejado es YYYY-MM-DD HH:MM:SS
- Actualmente tenemos 13 proveedores 

Recuerde:
 - Terminar la actividad con una conclusión e incluir lista de preguntas o aclaraciones para la organización, problemas de calidad y alternativas para la limpieza.
 - Revisar la infografía de entendimiento de datos.
