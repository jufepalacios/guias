# Tarea: ETL

# Introducción

**Objetivo**

Realizar un proceso ETL básico en Pyspark

**¿Para qué?**

Practicar lo aprendido en el tutorial de ETL

**¿Qué necesita?**

1. Modelo multidimensional asociado al proceso de movimientos
2. Notebook para trabajar: puede usar la seccion 3 "Espacio para desarrollar la tarea" al final del notebook del tutorial para realizar esta actividad
5. Servidor SQL con base de datos relacional "WWImportersTransactional" y base de datos relacional que corresponde a la bodega de WWI "WWImportersDWH"

# Enunciado
Ahora que sabe cómo realizar un proceso ETL, dado el modelo multidimensional del proceso de negocio de movimientos de inventario 
1. **Entregable 1 - Diseño del ETL:** Diseñe el ETL para las dimensiones proveedor, tipoTransaccion y para la tabla de hechos
2. **Entregable 2 - Implementación del ETL:** implementación del proceso ETL para las dimensiones Proveedor, TipoTransaccion y para la tabla de hechos

Note que para este proceso de negocio, las dimensiones Producto, Cliente y Fecha son iguales a las del hecho Orden, este caso se conoce como dimensiones compartidas. Usted debe concentrarse en las dimensiones Proveedor, TipoTransaccion y la tabla de hechos que no existen en la bodega de datos actualmente.

![Modelo movimientos](https://github.com/MISW-4402-Analisis-y-Modelado-de-datos/General/blob/main/Tutoriales/Modelado/Modelo%20movimiento.png)


Sobre los resultados del entendimiento de datos Wide World Importers les comenta
- 2 para proveedor: explicitas para hacer transformaciones
- B
- C
- D
- E
- F
