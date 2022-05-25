# **Mi primer tablero de control**
## **Objetivo**
- Analizar fuentes de datos (perfilamiento de datos) relacionadas con el proyecto del curso.
- Construir un tablero de control dadas fuentes de datos en formato "csv"  o xls.
## **Instrucciones**

![](./imagenes/S210InfrestructuraVisible.png)


Infraestructura visible de forma conjunta con un grupo de consultores de inteligencia de negocios, siguió trabajando en la especificación de los primeros análisis que quiere que usted realice. En particular, en esta entrega le solicita:
1.	Mejorar el perfilamiento de las fuentes de datos a utilizar. Esta mejora incluye completar o corregir de acuerdo con lo requerido para realizar los análisis propuestos.
2.	Implementar uno de los análisis propuestos por el cliente. En este punto debe agrupar más de dos de los análisis propuestos, que considere de forma conjunta, aportan al análisis global que se quiere realizar.
    - Explicar cómo el resultado del análisis soporta los objetivos de la organización de análisis. Defina la organización a la cual va a orientar los análisis.
    - Describir dos decisiones o acciones que puede tomar un analista en el negocio con la información brindada en el análisis implementado. 
    - Indicar 2 nuevas preguntas que son posibles de contestar con el tablero de control construido.
3.	Enriquecer el análisis e incluir KPIs que considere pueden ser útiles para tomadores de decisión que lo utilicen. 
4.	Preparar un video de máximo 5 minutos, para la junta directiva de la empresa donde presente la solución propuesta en esta etapa del proyecto. 
A continuación, se presentan los análisis propuestos, los datos requeridos y algunas de las preguntas que les gustaría contestar con esos análisis. 

| Tema analítico  | Análisis requeridos o inferidos | Categoría del análisis - Tablero de control, análisis OLAP, Minería de datos   | Procesos de negocio | Fuentes de datos |
| ------------- | ------------- | ------------- | ------------- | ------------- | 
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar el número de pasajeros transportados en un rango de fechas de aeropuertos Internacionales a Colombia   | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos, Aeropuertos Histórico  |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar la carga transportada en un rango de fechas de aeropuertos Internacionales a Colombia    | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos, Aeropuertos Histórico  |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar la carga desaprovechada en un rango de fechas de aeropuertos Internacionales a Colombia     | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos, Aeropuertos Histórico  |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar el número de puestos desaprovechados en un rango de fechas de aeropuertos Internacionales a Colombia      | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos, Aeropuertos Histórico  |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar el número de pasajeros transportados en un rango de fechas de aeropuertos Nacionales de Colombia      | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos, Aeropuertos Histórico  |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar la carga transportada en un rango de fechas de aeropuertos Nacionales de Colombia       | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos, Aeropuertos Histórico  |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar la cantidad de pasajeros salientes y entrantes a través del tiempo por departamentos de Colombia        | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos, Aeropuertos Histórico  |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar la cantidad de carga aérea saliente y entrante a través del tiempo por departamentos de Colombia         | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos, Aeropuertos Histórico  |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar el porcentaje de cobertura Internacional, por rango de fechas, nacional o regional por departamentos de Colombia | Tablero de control  | Cobertura, Tráfico y capacidad de carga aérea en aeropuertos de Colombia |  Aeropuertos, Aeropuertos Histórico, Cobertura por centro poblado   |
| Cobertura y comportamiento de vuelos y aeropuertos en Colombia   | Visualizar la relación entre las características de infraestructura de cada aeropuerto y el número de vuelos | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia   |  Aeropuertos cambios infraestructura  |

Con estos análisis ellos quieren respuestas para:

1. El número de pasajeros transportados en un rango de fechas de aeropuertos Internacionales a Colombia.
2. La carga transportada en un rango de fechas de aeropuertos Internacionales a Colombia.
3. La carga desaprovechada en un rango de fechas de aeropuertos Internacionales a Colombia.
4. El número de puestos desaprovechados en un rango de fechas de aeropuertos Internacionales a Colombia.
5. El número de pasajeros transportados en un rango de fechas de aeropuertos Nacionales de Colombia.
6. La carga transportada en un rango de fechas de aeropuertos Nacionales de Colombia.
7. La cantidad de pasajeros salientes y entrantes a través del tiempo por departamentos de Colombia.
8. La cantidad de carga aérea saliente y entrante a través del tiempo por departamentos de Colombia.

Adicionalmente, están interesados en definir una serie de KPIs (Key Performance Indicator) para revisar el logro de posibles metas de interés para aerolíneas y usuarios entre otros. En este momento no tienen muy claro ese punto, por lo cual le sugieren lo siguiente para su definición:
1. Si el valor está por encima del promedio, asignarle un color verde.
2. Si el valor es el promedio, asignarle un color naranja.
3. Si el valor está por debajo del promedio, asignarle un color rojo.

## **Recursos requeridos**

En el siguiente repositorio puede encontrar los archivos de datos requeridos para el desarrollo de esta tarea, los datos de vuelos comprenden los periodos de tiempo entre 2010 y 2013 y la información de aeropuertos es de todos aquellos construidos antes de 2013 [click aquí](https://github.com/MIAD-Modelo-Datos/Recursos/tree/main/Infraestructura%20visible/Etapa%201)

***Datos suministrados***

- vuelos.csv
- aeropuertos.csv
- Revise y utilice los archivos que considere necesarios diferentes a los anteriores

***Tecnología***

Recuerde que está el tutorial de “Construcción de un tablero de control”, que será de utilidad para el uso de la tecnología utilizada en esta tarea.
- PowerBI
- PySpark

## **Recomendaciones de los entregables**
- Incluir en la entrega la dirección (link) de la wiki donde registró lo solicitado en esta tarea con las actividades realizadas dentro de las fechas establecidas
- Padlet: 
  - Resultados de análisis Grupo X: https://uniandes.padlet.org/miadvirtualmde/ow6uu0ce6b6r0z4 
  - Contraseña: Diríjase a las instrucciones del curso para ver la contraseña

## **Preguntas o más información**
- Las preguntas que surjan en el desarrollo de esta tarea pueden registrarlas en el slack del curso
- Recuerde que tiene a su disposición el tutorial de Creación y manejo de la Wiki [aquí](https://misovirtual.virtual.uniandes.edu.co/codelabs/wiki-github/index.html?index=..%2F..ETL#0): 
