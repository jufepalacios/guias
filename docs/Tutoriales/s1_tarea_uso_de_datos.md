# Tarea: Uso de tableros de control
Wide World Importers[^1] es un importador y distribuidor de productos de primera categoría, que funciona desde el área de la bahía de San Francisco. Como mayorista, los clientes de WWI son principalmente empresas que revenden a individuos. WWI vende a los clientes de venta al por menor en el Estados Unidos como tiendas especializadas, supermercados, almacenes informáticos, tiendas de atracción turística y otras personas. WWI también vende a otros mayoristas a través de una red de agentes que promocionan los productos en el nombre de WWI. A pesar de que todos los clientes de WWI se basan actualmente en el Estados Unidos, la empresa está intentando impulsar la expansión en otros países. 

WWI compra mercancías de proveedores, incluidos los fabricantes de la novedad y el juguete, y otros mayoristas. Almacenan las mercancías en el almacén de WWI y reordenan a los proveedores según sea necesario para satisfacer los pedidos de los clientes. También compran grandes volúmenes de materiales de embalaje y los venden en cantidades más pequeñas, por comodidad para los clientes. 

Los objetivos de World Wide Importers son:

1. Ofrecer a los clientes productos que deseen cuándo y dónde lo deseen
2. Dar un servicio de calidad que maximice las ganancias por ventas
3. Optimizar el manejo de inventario de los productos

Wide World Importers nos contrata como consultores para hacer un proyecto de analítica 1.0, en el cual quiere entender el comportamiento de los clientes o vendedores a partir de órdenes de venta con el fin de monitorear el logro de los objetivos estratégicos anteriores. Como resultados de la consultoría se tiene:

1. La documentación de los requerimientos analíticos en el siguiente formato

| **Tema analítico**                                               | **Análisis requeridos o inferidos**                                                                                                       | **Categoría del análisis (\*)** | **Procesos de negocio** | **Fuentes de datos**                                                    |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------- | ----------------------- | ----------------------------------------------------------------------- |
| **Comportamiento de clientes a partir de órdenes** **de compra** | Visualizar la cantidad de productos vendidos y el valor total recaudado en un **rango de fechas** por cliente, vendedor, ciudad, producto | Tablero de control              | Ventas                  | Ordenes, detalles de órdenes, clientes, productos, ciudades, vendedores |

2. Los tableros de control construidos con Data Studio: Comportamiento de clientes a partir de órdenes de compra: 

- [1.000 registros](https://datastudio.google.com/reporting/b00690e8-9e3e-47ec-8c2a-5ca0df2bd981)
- [50.000 registros](https://datastudio.google.com/reporting/5714f6b7-da68-47e7-aaf2-43aa86e2e52c)
- [145.000 registros](https://datastudio.google.com/reporting/ed1d3c28-43e5-4d70-ae08-0873b29ee8cb)

Puede usar cualquiera para el desarrollo de la tarea, tenga en cuanta que a mayor número de registros mayor tiempo toman las herramientas para procesar

[^1]: Caso inspirado en: [https://docs.microsoft.com/en-us/sql/samples/wide-world-importers-what-is?view=sql-server-ver15](https://docs.microsoft.com/en-us/sql/samples/wide-world-importers-what-is?view=sql-server-ver15)

# Tablero de control

Según la metodología ASUM-DM, en este tutorial nos concentramos en el uso de un tablero de control que fue la aplicación desplegada en la etapa número 10 (&quot;Despliegue de solución&quot;). Por otra parte, a nivel de arquitectura de componentes estamos en la capa de aplicación y vamos a simular la interacción de un usuario final con dicha aplicación.
![](./img/S1usotablerosImg3.png)
![](./img/S1usotablerosImg2.png)

El tablero consulta los datos de un servidor de base de datos MySQL para resolver las necesidades o requerimientos analíticos. Puede usar filtros sobre clientes, empleados, fechas, ciudades y productos.

# Ejemplo de análisis sobre un tablero de control

La construcción de un tablero de control no es suficiente para generar valor a una organización. Lo recomendado es dar algunas conclusiones que ejemplifiquen el uso del tablero y al mismo tiempo den valor al negocio en forma de hallazgos que soportarán posibles decisiones o acciones. A continuación, se presenta un ejemplo de posible conclusión del tablero.

"Juana Valencia  abogada corporativa de Wide World Importes (perteneciente al área jurídica de la organización) ha iniciado su interacción con el tablero de comportamiento de clientes con el fin de investigar el comportamiento de ventas y su relación con la cantidad de productos vendidos, la tasa de impuesto autorizada por los diferentes estados de EEUU y los vendedores involucrados en dichas ventas. Haciendo uso del tablero y muy enfocada en estados donde la probabilidad de fraude es mayor, encuentra que para el **año 2015 en Willow Valley la cantidad vendida y el valor (U$403,57 -- como se ilustra en la figura ![](./img/S1usotablerosHallazgo.png))**, tomando la tasa de impuesto, no corresponde a lo permitido por la ley local. Lo cual la lleva a identificar **dos empleados relacionados con dichas ventas (Hudson y Kayla)**". Este hallazgo, le permitió a la abogada fortalecer los cargos contra los empleados para iniciar una investigación jurídica que podría significar el hallar una fuga de dinero que corresponde a un 0,01% del total de ventas por año. Una cifra nada despreciable, pero que hasta la actualidad había permanecido oculta por la dificultad de poner a disposición de los abogados este tipo de herramientas que aportan en su eficiencia operativa. De igual manera, con esta identificación pidió la generación de un nuevo tablero de control, con el fin de validar cumplimientos regulatorios. El hallazgo identificado por Juana es de suma importancia para ella y está alineado con una de sus responsabilidades:  "Garantizar el cumplimiento de las regulaciones y las leyes". 

# Ejercicio

Tomando como base el contenido visto en la semana uno sobre metodología, arquitectura, entre otros, el presente documento y los resultados obtenidos de la consultoría, Wide World Importers quiere continuar desarrollando el proyecto, definiendo otros posibles usos del tablero de control ya construido, para lo cual le solicita generar una conclusión de uso como la del ejemplo, en la cual debe incluir:

1. El rol de la organización que se beneficia con el uso de este tablero de control, al igual el área a la que pertenece.
2. Un nuevo hallazgo obtenido al utilizar el tablero de control y evidencia de su identificación en una imágen sobre el tablero de control.
3. La alineación entre el hallazgo y las funciones de ese rol, los objetivos de Wide World Importers o del área a la que pertenece el rol. Si lo considera necesario puede extender el caso para darle sentido, tal como se hizo en el ejemplo.
4. Dos acciones/decisiones posibles que el rol puede tomar usando el hallazgo sobre el tablero de control.

Usted debe entregar un reporte en pdf que contenga lo solicitado.

