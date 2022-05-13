# Tarea: Crear tablero de control

## Introducción

**Objetivo**

En este tutorial aprenderá a crear un tablero de control usando Data Studio

**¿Qué construirá?**
- Un tablero de control

**¿Para qué?**

Visualizar los resultados

**¿Qué necesita?**

1. Google data studio: https://datastudio.google.com
2. Acceso al servidor de base de datos

## Enunciado
Dirijase al link de data studio, de click en "USE IT FOR FREE" e inicie sesión en su cuenta gmail.

Luego de click en Informe vacio y diligencie los datos que le solicita asi como preferencias de notificaciones. Ej. Region: Colombia

Cambie el nombre del tablero en la esquina superior izquierda

En la barra de herramientas de clic en añadir datos, en la barra de busqueda que aparece digite mysql y seleccione el conector de MySQL que observa en la siguiente imagen

Autorize el acceso a los datos y configure el  conector de la siguiente manera, use las credenciales de acceso al servidor dadas en la semana 1 del curso y conectese a la base de datos que modela su bodega de datos

Una vez conectado podra ver las tablas disponibles para consultas


Idealmente en las herramientas de visualización quisieramos poder tomar diferentes tablas y obtener lo necesario para las graficas, sin embargo las herramientas del mercado son muy limitadas en cuanto a escalabilidad, manipulación de datos sencilla entre otras. Data Studio en particular no soporta la union de varias tablas por ende es necesario hacer uso de "vistas" SQL o simplemente crear una tabla en la base de datos que tenga la información que deseamos visualizar en Data Studio

De esta manera nos dirijimos a MySQL Workbench y creamos una tabla nueva con todo lo que queremos visualizar 
