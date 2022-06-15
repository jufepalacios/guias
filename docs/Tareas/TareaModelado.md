# Tarea: Modelo dimensional y Base de datos

# Introducción

**Objetivo**

Comprender la relación entre un modelo dimensional y su representación en un modelo relacional, lo que se denomina modelo ROLAP. Adicionalmente, fortalecer la competencia de modelar multidimensionalmente a partir de un caso dado.

**¿Para qué?**

Practicar lo aprendido en el tutorial de modelado de datos y SQL y retomar el lenguaje SQL a nivel de creación de objetivos (DDL - _Data Definition Language_ y DML- _Data Manipulation Language_).

**¿Qué necesita?**

1. MySQL Workbench
2. Modelo multidimensional asociado al proceso de movimientos
3. Acceso al servidor de base de datos 
4. Script SQL <a href='https://github.com/MISW-4402-Analisis-y-Modelado-de-datos/guias/blob/main/docs/Tareas/scriptTarea.sql'>aquí</a>

# Enunciado
Ahora que sabe cómo crear modelos multidimensionales y SQL básico, lo que debe hacer en la primera parte, es crear en una base de datos relacional las tablas que representan un modelo dado, poblarlas y consultarlas. En la segunda parte, va a practicar la competencia de modelar con el caso dado. A continuación encuentra el detalle de las actividades a realizar:  

1.	**MODELO ROLAP**: A partir del requerimiento analítico, modelo multidimensional y sentencias SQL que se muestran más adelante, prepare los siguientes entregables. 
-	**Entregable CREATE**: Defina las sentencias para crear las tablas de cliente y movimiento de acuerdo con el modelo que se presenta.
-	**Entregable INSERT**: Defina las sentencias para la inserción de 5 registros en todas las tablas del modelo multidimensional.
-	**Entregable SELECT**: Defina las sentencias para consultar los datos de manera que le permita resolver el requerimiento analítico. 
-	**Entregable EJECUTAR**: Ejecute las sentencias para crear, insertar y consultar la base de datos que refleje el modelo multidimensional dado y muestre los resultados obtenidos.

| **Tema analítico**                                               | **Análisis requeridos o inferidos**                                                                                                       | **Categoría del análisis (\*)** | **Procesos de negocio** | **Fuentes de datos**                                                    |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------- | ----------------------- | ----------------------------------------------------------------------- |
| **Movimientos en el inventario de WWI** | Visualizar el número de productos que se movieron en el inventario en un rango de fechas por cliente, proveedor, y/o tipo de transacción | Consultas SQL             | Inventario                  | Movimientos, Tipos de transacción, Proveedores, Clientes y Productos  |

![Modelo moimientos](https://github.com/MISW-4402-Analisis-y-Modelado-de-datos/General/blob/main/Tutoriales/Modelado/Modelo%20movimiento.png)


![Sentencias CREATE](https://github.com/MISW-4402-Analisis-y-Modelado-de-datos/General/blob/main/Tutoriales/Modelado/CreateMovimientos.png)


2.	**MODELO MULTIDIMENSIONAL**: Proponga un modelo multidimensional para el siguiente caso:

**SINIESTROS ALPES** 
La secretaria de movilidad de los Alpes lo ha contratado a usted para que lo asesore en la construcción de un almacen de datos (Data Mart), asociado al tema de siniestros (hace referencia a accidentes de tránsito), de la ciudad de los Alpes. Con el fin de validar que este proyecto apoya su plan estratégico, la secretaría, hace énfasis en los siguientes puntos relacionados con su estrategia: 

-	**MISION**: […] como cabeza del sector Movilidad y autoridad de tránsito y transporte, presta servicios, planea y formula las políticas del sector, generando condiciones de movilidad acordes con las necesidades de la población de los Alpes […] 
-	**OBJETIVO**: Uno de sus objetivos es aumentar la cobertura y efectividad de la presencia en vía 
-	**META**: Una de las metas que persigue la secretaría es la reducción de siniestros en los cuales hay muertos. 

Asociado a un siniestro se tiene una descripción del mismo que incluye: Fecha, dirección, causa (exceso de velocidad, alcoholemia, etc.), gravedad (solo daños, con heridos, con muertos) y características del entorno. El entorno hace referencia a elementos como si la vía estaba lisa – porque había llovido, si había cerca un hueco, si es muy oscuro el lugar, entre otros. Adicionalmente, se registra información de los actores involucrados en el mismo, de los cuales se tiene el tipo de documento, número de documento, edad, sexo, tipo de actor (peatón, ciclista, motociclista, pasajero o conductor de carro), y el estado (herido valorado, herido hospitalizado, muerto). Finalmente, se tiene información de los vehículos involucrados de los cuales se tiene la placa, la marca (Renault, Mazda, etc.), la clase (automóvil, bus, buseta, motocicleta) y el servicio (público colectivo, público individual, privado, diplomático). 

Cuando se habla de analizar los siniestros, los expertos en seguridad vial identifican tres perspectivas de análisis: actores involucrados, infraestructura y entorno. La infraestructura corresponde al lugar donde ocurre el accidente y a sus características. Esta información contiene la dirección exacta, la localidad (e.g., Usaquén, chapinero), la Unidad de Planeamiento Zonal (UPZ – área urbana más pequeña que una localidad), y la Zona de Análisis de Transporte (ZAT). Una localidad está compuesta por varias UPZ y una UPZ está compuesta por varias ZAT. Adicionalmente, una dirección, está asociada a un tramo de corredor vial, por ejemplo, para el corredor vial de la Av. Boyacá, el tramo específico (entre calles 134 y 138).  

La Secretaría desea identificar causas de diferentes tipos de siniestros, con el fin de formular políticas que lleven a la reducción de los mismos. En particular se hace preguntas del estilo: ¿Cuáles son las principales causas de los siniestros que ocurren en horas de la noche, donde hay por lo menos una motocicleta involucrada?, ¿Cuáles son las principales causas de siniestros en la Avenida 1ero de mayo (corredor vial)? ¿Qué tipos de actores están involucrados en más siniestros? ¿Cuáles son los actores que más muertes han registrado en los últimos años en siniestros? ¿Cuáles son los días de la semana y horas en los que se producen más siniestros y las características de los mismos? ¿Qué vehículos han estado más involucrados en siniestros y qué características tienen? ¿Hay marcas de carros que están involucradas en mayor número de siniestros? 

### Herramientas de modelado online:
- LucidChart: https://www.lucidchart.com/pages/es
- GenMyModel: https://www.genmymodel.com/
