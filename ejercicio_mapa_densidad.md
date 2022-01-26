# Ejercicio de reflexión sobre los mapas de densidad que hemos generado


> + **_Versión_**: 1.0
> + **_Asignatura (titulación)_**: Ciclo de gestión del dato: ecoinformática (máster conservación, gestión y restauración de la biodiversidad. UGR). Curso 2020-2021
> + **_Autor_**: Curro Bonet-García (fjbonet@uco.es)



## Objetivos del ejercicio

Esta actividad tiene el siguiente objetivo de aprendizaje:

+ Entrenar la capacidad de comparar con criterio distintas formas de representar en el espacio una variable ambiental concreta.
+ Mejorar la capacidad de cuestionar la validez de un mapa en función de factores relacionados con la ecología de la variable representada. 
+ Aprender que completar un flujo de trabajo satisfactoriamente no tiene por qué implicar que el resultado sea válido desde un punto de vista ecológico.

## Tareas a realizar

Para satisfacer los objetivos anteriores deberás reflexionar sobre los dos mapas de densidad que hemos obtenido y sobre otro que no hemos visto en clase. Lee atentamente el siguiente texto que describe los mapas anteriores. Recuerda que [aquí](https://rawcdn.githack.com/aprendiendo-cosas/TP_densidad_pinar_ecoinf_UGR/2021__2022/guion_densidad_pinares.html) puedes ver el guión que describe cómo obtuvimos dos de los tres mapas de densidad comentados. 

A partir de un inventario forestal (en el que se expresa la densidad en árboles/superficie) hemos obtenido dos mapas diferentes usando distintas metodologías:

Mediante imputación hemos asignado a todos los polígonos del mismo estrato la densidad promedio de todas las parcelas que hay en dicho estrato. De esta forma podemos asignar valores de densidad a los polígonos en los que no haya caído ninguna parcela de inventario. La siguiente imagen muestra el resultado obtenido en una zona concreta de Sierra Nevada. La línea roja representa el límite norte del espacio protegido. [Aquí](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2021-2022/geoinfo/densidad_pinar_x_estratos.tif) puedes descargar la capa de densidad obtenida de esta forma.

![image](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2021-2022/imagenes/imputacion.jpeg)



Además, mediante la técnica de interpolación más sencilla (IDW), obtuvimos otro mapa de densidad de los pinares de repoblación. En este caso asumimos que la densidad de un punto en el que no hay inventarios depende de la densidad de los puntos que tenga más cerca. La siguiente imagen muestra el resultado obtenido. Y [aquí](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2021-2022/geoinfo/densidad_pinar_interpolada.tif) puedes descargar la capa de densidad obtenida de esta forma. 

![image](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2021-2022/imagenes/interpolacion.jpeg)

Al margen de las dos capas anteriores os paso aquí otro mapa que muestra la densidad de los pinares de Sierra Nevada. En esta ocasión se ha obtenido mediante teledetección y aquí la densidad se expresa en porcentaje de cobertura del suelo, no en árboles por superficie como en los casos anteriores. Este mapa procede de un producto generado para toda Europa por el programa Copernicus. [Aquí](https://land.copernicus.eu/pan-european/high-resolution-layers/forests/tree-cover-density/status-maps/tree-cover-density-2018) tienes el enlace de descarga. Y aquí un informe que detalla la metodología que han seguido para generar el mapa. Mira la página 7 del informe para saber cómo se ha calculado la densidad del bosque. 

## Evaluación
En la siguiente tabla podéis ver los criterios que se usarán para evaluar este ejercicio. Dicha rúbrica está basada en los pasos que hemos dado para construir la base de datos:

1. Identificación de entidades, atributos de la realidad que queremos modelar, así como las relaciones entre los mismos.
2. Traducción de los elementos anteriores a una estructura interpretable por un gestor de bases de datos relacionales: tablas, campos, relaciones.
