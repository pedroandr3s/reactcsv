Informe sobre React y Minería de Datos
Descripción del Proyecto
En el contexto de una asignatura relacionada con minería de datos, se nos asignó una tarea que consistía en trabajar con un archivo comprimido (.rar) que contenía 39 archivos CSV. Estos archivos incluían datos sobre pozos registrados durante un periodo de cuatro años, con las siguientes variables:
date: Fecha y hora del registro.
level: Nivel de agua.
temperature: Temperatura registrada.
Los datos se recolectaron cada 15 minutos, lo que generó un volumen significativo de información. La tarea consistía en graficar los datos, pero debido a la cantidad, resultaba difícil interpretarlos. Por ello, se nos solicitó encontrar una forma de reducir la cantidad de datos para facilitar su visualización y análisis.
Solución Implementada
Para resolver este problema, desarrollé una aplicación web utilizando React. La aplicación permite procesar los archivos CSV, reducir la cantidad de datos seleccionando uno cada dos meses, y visualizar los resultados de manera más clara.
Estructura del Proyecto
El proyecto se organizó de la siguiente manera:

csv-processor/
  - package.json
  - public/
    - index.html
  - src/
    - App.js
    - components/
      - CSVProcessor.js
    - styles/
      - CSVProcessor.css
    - utils/
      - csvProcessor.js
    - index.js


Archivos del Proyecto
App.js

components/CSVProcessor.js










styles/CSVProcessor.css







utils/csvProcessor.js














index.js

Resultados

Al interactuar con la opción "Seleccionar archivo" o al arrastrar un archivo, será necesario cargar un archivo en formato RAR que contenga las características date, level y temperature.






Una vez seleccionado el archivo, su nombre aparecerá junto al botón "Seleccionar archivo", y se habilitará el botón "Procesar y descargar".

Tras procesar el archivo, se generará una tabla que mostrará el promedio correspondiente a cada pozo. Además, se abrirá la ubicación donde se guardará el archivo descargado con los resultados de los promedios calculados.

