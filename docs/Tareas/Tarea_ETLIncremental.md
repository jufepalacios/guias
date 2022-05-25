# **Tarea: Construir un ETL incremental**
## **Introducción**
### **Objetivo**
- Usar PySpark para crear ETLs con historia en los atributos de las dimensiones.  

### **¿Para qué?**
Dentro  de  procesos  de  ETL,  es común  que se  presenten  dimensiones que puedan  presentar cambios a través del tiempo para las cuales es necesario tener un plan de manejo de historia. Por lo tanto, es esencial saber cómo realizar este manejo en las distintas herramientas de ETLs.

### **¿Qué necesita?**
1. Python 3 con pip instalado
2. JupyterLabs
3. Paquetes: Pyspark (3.0.1) y pandas (1.2.1)
5. Servidor SQL con base de datos multidimensional "WWImportersDWH" que contenga la dimension "cliente_Historia"

## **Enunciado**

![](./imagenes/S210InfrestructuraVisible.png)

En esta fase del proyecto, a partir de algunos ejemplos de análisis requeridos, aclaraciones de la organización sobre los datos compartidos inicialmente, de nuevas fuentes de datos proporcionadas, del modelo multidimensional propuesto inicialmente, Infraestructura Visible considera que están listos para iniciar un trabajo en grupos de máximo tres personas para realizar un proceso de ETL incremental con los nuevos datos y con los ajustes que tuvo que hacer al modelo, en particular relacionados con el manejo de historia de los atributos de las dimensiones. El detalle de los productos a entregar, los encuentra en la sección entregables.

A nivel de trabajo en grupo, dada la experiencia que la empresa tiene en este estilo de proyectos, le sugiere lo siguiente:

***Realizar una reunión de inicio*** para definir la forma como se van a organizar.
En particular esta semana en esa reunión deberían:
1.	Registrar el grupo en el excel definido para esta actividad
2.	Definir los canales de comunicación que tendrá el grupo
3.	Compartir lo construido en la primera iteración del curso
4.	Definir la forma de organizarse para las tareas de esta semana de tal manera que todos aporten de forma equitativa al logro de las mismas
5.	Definir por los menos dos espacios adicionales en la semana para ver el avance de las tareas asignadas y hacer ajustes si se requiere
6.	Nombrar un representante por semana, quién debe ser distinto cada nueva semana.

***Nombrar a un representante por semana*** Quien debe estar pendiente de:
1.	Revisar detalladamente lo que se solicita en las entregas de la semana
2.	Hacer un inventario de los recursos existentes para realizar las entregas
3.	Liderar las dos reuniones que se hagan durante la semana
4.	Recopilar las dudas del grupo y socializarlas por slack
5.	Garantizar que las dudas son resueltas por slack o durante la sesión sincrónica
6.	Garantizar que uno de los miembros hace las entregas de la semana

## **Recursos requeridos**
En el siguiente repositorio puede encontrar los archivos de datos requeridos para el desarrollo de esta tarea, los datos de vuelos comprenden los periodos de tiempo entre 2010 y 2016 y la información de aeropuertos es de todos aquellos construidos antes de 2016. Así mismo, Infraestructura visible comenta que la infraestructura de los aeropuertos ha cambiado en los últimos años y esto se ve reflejado en los datos.

Los datos y la información asociada a los mismos está disponible en este [enlace](https://github.com/MIAD-Modelo-Datos/Recursos/tree/main/Infraestructura%20visible/Etapa%201)

***Datos suministrados***
- aeropuertos.csv
- vuelos.csv
- Ajustes a los diccionarios de datos
- Aclaraciones relacionadas con los comentarios realizados en la tarea de perfilamiento de datos.
- Revise y utilice los archivos que considere necesarios diferentes a los anteriores


***Tecnología***

Recuerden que está el tutorial de “[Construcción de ETL con historia](https://www.coursera.org/learn/modelado-de-datos-y-etl/ungradedLab/BqgON/tutorial-construccion-etl-con-historia)” , que será de utilidad para el desarrollo de esta tarea. Este tutorial utiliza la tecnología Pyspark.

Adicionalmente, se le sugiere utilizar una herramienta como [GenMyModel](https://www.genmymodel.com/) para dibujar el modelo y generar las sentencias de creación de la base de datos. Este tipo de herramientas facilita el mantenimiento de los modelos de datos.
## **Recomendaciones de los entregables**

Incluir en la entrega la dirección (link) de la wiki donde registró lo solicitado en esta tarea con las actividades realizadas dentro de las fechas establecidas

## **Preguntas o más información**

- Las preguntas que surjan en el desarrollo de esta tarea pueden registrarlas en el slack del curso
- Recuerde que tiene a su disposición el tutorial de Creación y manejo de la Wiki [aquí](https://misovirtual.virtual.uniandes.edu.co/codelabs/wiki-github/index.html?index=..%2F..ETL#0)
