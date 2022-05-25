# **Tarea: Crear un tablero de control**
## **Introducción**
### Objetivo
- Construir un tablero de control a partir de los datos almacenados en una base de datos relacional con el esquema ROLAP.

¿Para qué?
- Visualizar los resultados del proyecto de datos y facilitar la interacción de los tomadores de decisiones

¿Qué necesita?
    
    1. Google data studio: https://datastudio.google.com

    2. Acceso al servidor de base de datos
## **Enunciado**

World Wide Importers está muy interesado en resolver el siguiente requerimiento analítico por medio del uso de tableros de control


| **Tema analítico**                                               | **Análisis requeridos o inferidos**                                                                                                       | **Categoría del análisis (\*)** | **Procesos de negocio** | **Fuentes de datos**                                                    |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------- | ----------------------- | ----------------------------------------------------------------------- |
| **Movimientos en el inventario de WWI** | Visualizar el número de productos que se movieron en el inventario en un rango de fechas por cliente, proveedor, y/o tipo de transacción | Consultas SQL             | Inventario                  | Movimientos, Tipos de transacción, Proveedores, Clientes y Productos  |


Es así como lo contrató una vez más para desarrollar los siguientes entregables.


2.	Implementar uno de los análisis propuestos por el cliente. En este punto debe agrupar más de dos de los análisis propuestos, que considere de forma conjunta, aportan al análisis global que se quiere realizar.
    - Explicar cómo el resultado del análisis soporta los objetivos de la organización de análisis. Defina la organización a la cual va a orientar los análisis.
    - Describir dos decisiones o acciones que puede tomar un analista en el negocio con la información brindada en el análisis implementado. 
    - Indicar 2 nuevas preguntas que son posibles de contestar con el tablero de control construido.
3.	Enriquecer el análisis e incluir KPIs que considere pueden ser útiles para tomadores de decisión que lo utilicen. 
4.	Preparar un video de máximo 5 minutos, para la junta directiva de la empresa donde presente la solución propuesta en esta etapa del proyecto. 

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

## **Preguntas o más información**
- Las preguntas que surjan en el desarrollo de esta tarea pueden registrarlas en el slack del curso
- Recuerde que tiene a su disposición el tutorial de Creación y manejo de la Wiki [aquí](https://misovirtual.virtual.uniandes.edu.co/codelabs/wiki-github/index.html?index=..%2F..ETL#0): 
