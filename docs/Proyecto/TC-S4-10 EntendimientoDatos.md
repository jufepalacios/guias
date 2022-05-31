# **Entendimiento de datos**
## **Objetivo**
- Explorar y analizar fuentes de datos (perfilamiento de datos) relacionadas con el proyecto del curso. 
- Inspeccionar el nivel de calidad de las fuentes de datos provistas.
- Revisar la viabilidad de implementar análisis con fuentes de datos dadas.
## **Instrucciones**

![](./imagenes/S210InfrestructuraVisible.png)

Infraestructura visible de forma conjunta con un grupo de consultores de inteligencia de negocios, ha trabajado en una especificación de los primeros análisis que quiere que usted realice. En esta primera fase, a partir de estos análisis propuestos, la empresa le ha entregado una serie de fuentes de datos y requiere que usted:

1.	Las explore, esto significa realizar el entendimiento de datos y analizar el resultado. 
2.	Valide y documente si es posible realizar los análisis solicitados, si debe hacer ajustes en la forma como han sido planteados o si requiere de información adicional para el desarrollo de los mismos.  

Recuerde que la exploración de los datos depende de los objetivos que tenga el proyecto de analítica. Es así como Infraestructura Visible le comparte los análisis que en este momento está interesada en responder:

1.	Análisis 1: ¿Cuántos pasajeros salieron de Medellín a Cali durante temporadas altas? (e.g., Semana santa). En general quiere aplicar este análisis a diferentes ciudades de Colombia y en diferentes temporadas altas.
2.	Análisis 2: ¿Qué departamento de Colombia tiene mayor número de sillas salientes desaprovechadas en un año o mes de un año específico (e.g, 2015)?
3.	Análisis 3: ¿Qué aeropuerto representa mayor exportación internacional en términos de carga?
4.	Análisis 4: Top 3 de aeropuertos nacionales que podrían reducir su presupuesto en aviones debido a que no transportan un mínimo del 50% de la capacidad que tienen en carga.
5.	Análisis 5: ¿Qué aeropuertos están en centros poblados donde la población de mujeres es mayor a la de hombres, con un PIB superior al promedio del Departamento donde está el centro poblado y donde el número de vuelos por mes de una año particular está por debajo del promedio nacional.?

A partir de lo anterior, los consultores de BI construyeron la siguiente tabla donde se encuentran los análisis identificados y los datos requeridos para lograr los objetivos de esta tarea, cada integrante del grupo debe elegir un análisis distinto para el desarrollo del proyecto a lo largo del curso

| Tema analítico  | Análisis requeridos o inferidos | Categoría del análisis (*)  | Procesos de negocio | Fuentes de datos |
| ------------- | ------------- | ------------- | ------------- | ------------- | 
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 1 <br> a. Visualizar el número de pasajeros transportados (entrantes y salientes) en un rango de fechas. <br> b. Visualizar el número de pasajeros transportados (entrantes y salientes) en un rango de fechas de aeropuertos Internacionales a aeropuertos en Colombia o entre aeropuertos nacionales. <br> c. Visualizar el número de pasajeros transportados (entrantes y salientes) en un rango de fechas por departamento y país  | Tablero de control  | Cobertura, Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 2 <br> Visualizar el número de puestos desaprovechados en un rango de fechas de aeropuertos Internacionales a aeropuertos en Colombia o entre aeropuertos nacionales, los aeropuertos se pueden agrupar por departamento, país, etc  | Tablero de control  | Cobertura, Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 3 <br> Visualizar la carga transportada (entrante y saliente) en un rango de fechas de aeropuertos Internacionales a aeropuertos en Colombia o entre aeropuertos nacionales, los aeropuertos se pueden agrupar por departamento, país, etc  | Tablero de control  | Cobertura, Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 4 <br> Visualizar la carga desaprovechada en un rango de fechas de aeropuertos Internacionales a aeropuertos en Colombia o entre aeropuertos nacionales, los aeropuertos se pueden agrupar por departamento, país, etc  | Tablero de control  | Cobertura, Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 5 <br> Visualizar el porcentaje de cobertura internacional, por rango de fechas, nacional o regional por departamentos de Colombia <br> Supuesto: el radio de cobertura es de 40Km. En caso de tener múltiples coberturas, se utiliza la jerarquía de categoría de cobertura para seleccionar la de mayor categoría. La jerarquía se entiende como Internacional es la de mayor categoría y cubre las demás categorías. En el caso de Nacional, incluye nacional, regional y local, en el caso de Regional solo cubre los vuelos regionales y locales.  | Tablero de control  | Cobertura, Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos, Cobertura por centro poblado  |

*La categoría de análisis posibles son Tableros de control, Análisis OLAP, Aprendizaje automático. En el curso solo vamos a abordar los tableros de control

** Los análisis de la tabla pueden ser agrupaciones de análisis más pequeños o se pueden extender, incluso puede que los análisis no estén completos. Es libre de proponerle nuevos análisis al negocio o complementar los de la tabla como parte de sus conclusiones. Piense en que le beneficiaría más a Infraestructura Visible y en paticular a un usuario que esté interesado en este estilo de análisis.

Para esto el negocio les comenta que los datos son ….. Dichos datos pueden tener errores ya que no han sido utilizados previamente para ser analizados.
1.	Hay información de vuelos y de aeropuertos construidos desde 2013 hasta 2020
2.	Hay X aeropuertos y Y vuelos
3.	El valor máximo de vuelos para un mismo aeropuerto en Colombia es de A

## **Recursos requeridos**
***Datos suministrados***

En el siguiente repositorio puede encontrar los diccionarios de datos y archivos de datos requeridos para el desarrollo de esta tarea, los datos de vuelos comprenden los periodos de tiempo entre 2010 y 2013 y la información de aeropuertos es de todos aquellos construidos antes de 2013 [Click aquí](https://github.com/MIAD-Modelo-Datos/Recursos/tree/main/Infraestructura%20visible/Etapa%201)
-	aeropuertos.csv
-	vuelos.csv 
-	Revise y utilice los archivos que considere necesarios diferentes a los anteriores

***Tecnología***

Recuerde que está el tutorial de “Entendimiento de datos”, que será de utilidad para el uso de la tecnología utilizada en esta tarea.
- JupyterLabs 
- Pyspark


## **Recomendaciones de los entregables**
Incluir en la entrega el enlace (link) de la wiki donde registró lo solicitado en esta tarea con las actividades realizadas dentro de las fechas establecidas
## **Preguntas o más información**
- Las preguntas que surjan en el desarrollo de esta tarea pueden registrarlas en el slack del curso.
- Recuerde que tiene a su disposición el tutorial de Creación y manejo de la Wiki [aquí](https://misovirtual.virtual.uniandes.edu.co/codelabs/wiki-github/index.html?index=..%2F..ETL#0): 
- La forma en que se organicen y aporten al interior del grupo es fundamental para el logro del objetivo del proyecto y será evaluada en la entrega final del proyecto.
