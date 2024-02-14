# Ejercicio de reflexión sobre los mapas de densidad que hemos generado


> + **_Versión_**: 2023-2024
> + **_Asignatura (titulación)_**: Ciclo de gestión del dato: ecoinformática (máster conservación, gestión y restauración de la biodiversidad. UGR).
> + **_Autor_**: Curro Bonet-García y María Suárez Muñoz (bv2sumum@uco.es)



## Objetivos del ejercicio

Esta actividad tiene los siguientes objetivos de aprendizaje:

+ Entrenar la capacidad de comparar con criterio distintas formas de representar en el espacio una variable ambiental concreta.
+ Mejorar la capacidad de cuestionar la validez de un mapa en función de factores relacionados con la ecología de la variable representada. 
+ Aprender que completar un flujo de trabajo satisfactoriamente no tiene por qué implicar que el resultado sea válido desde un punto de vista ecológico.
+ Evaluar una parte del conocimiento adquirido en el "tema" de caracterización de la densidad de los pinares de repoblación.

## Tareas a realizar

Para satisfacer los objetivos anteriores deberás reflexionar sobre los dos mapas de densidad que hemos obtenido y sobre otro que no hemos visto en clase. Lee atentamente el siguiente texto que describe los mapas anteriores. Recuerda que [aquí](https://rawcdn.githack.com/aprendiendo-cosas/TP_densidad_pinar_ecoinf_UGR/2023-2024/guion_densidad_pinares.html) puedes ver el guión que describe cómo obtuvimos dos de los tres mapas de densidad comentados. 

A partir de un inventario forestal (en el que se expresa la densidad en árboles/superficie) hemos obtenido dos mapas diferentes usando distintas metodologías:

Mediante imputación hemos asignado a todos los polígonos del mismo estrato la densidad promedio de todas las parcelas que hay en dicho estrato. De esta forma podemos asignar valores de densidad a los polígonos en los que no haya caído ninguna parcela de inventario. La siguiente imagen muestra el resultado obtenido en una zona concreta de Sierra Nevada. La línea roja representa el límite norte del espacio protegido (descarga [aquí](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2023-2024/geoinfo/pnatural_23030.zip) el fichero de formas con los límites de Sierra Nevada). [Aquí](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2023-2024/geoinfo/densidad_pinar_x_estratos.tif) puedes descargar la capa de densidad obtenida de esta forma.

![image](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2023-2024/imagenes/imputacion.jpeg)



Además, mediante la técnica de interpolación más sencilla (IDW), obtuvimos otro mapa de densidad de los pinares de repoblación. En este caso asumimos que la densidad de un punto en el que no hay inventarios depende de la densidad de los puntos que tenga más cerca. La siguiente imagen muestra el resultado obtenido. Y [aquí](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2023-2024/geoinfo/densidad_pinar_interpolada.tif) puedes descargar la capa de densidad obtenida de esta forma. 

![image](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2023-2024/imagenes/interpolacion.jpeg)

Al margen de las dos capas anteriores os paso [aquí](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2023-2024/geoinfo/TCD_pines.tif) otro mapa que muestra la densidad de los pinares de Sierra Nevada. En esta ocasión se ha obtenido mediante teledetección. En este mapa la densidad se expresa en porcentaje de cobertura del suelo, no en árboles por superficie como en los casos anteriores. Esta capa procede de un producto generado para toda Europa por el programa [Copernicus](https://www.copernicus.eu/en). [Aquí](https://land.copernicus.eu/pan-european/high-resolution-layers/forests/tree-cover-density/status-maps/tree-cover-density-2018) tienes el enlace de descarga. Y [aquí](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2023-2024/biblio/Forest_Technical_Specs_Public_v11.pdf) un informe que detalla la metodología que han seguido para generar el mapa. Mira la página 7 del informe para saber cómo se ha calculado la densidad del bosque. La siguiente imagen muestra el aspecto de la densidad según este producto en una porción de nuestra zona de estudio.

![image](https://github.com/aprendiendo-cosas/A_densidad_pinar_ecoinf_UGR/raw/2023-2024/imagenes/teledeteccion.jpeg)

Una vez que hayas visto las capas y hayas pensado un poco sobre el asunto, deberás de contestar a las siguientes preguntas de manera justificada. No es necesario que te extiendas demasiado. Un par de folios es más que suficiente. Sube el archivo en formato editable (no pdf, por favor) al classroom. De esa forma podré comentar tu trabajo más fácilmente.

+ Sobre el mapa "imputado":
  + ¿Qué ventajas tendría usarlo para nuestro objetivo?.  Descríbelas brevemente.
  + ¿Qué desventajas o problemas puedes identificar?. Descríbelas brevemente.
  + Propón alguna forma de minimizar las desventajas de este mapa.
+ Sobre el mapa interpolado:
  + ¿Qué ventajas tendría usarlo para nuestro objetivo?.  Descríbelas brevemente.
  + ¿Qué desventajas o problemas puedes identificar?. Descríbelas brevemente.
  + Propón alguna forma de minimizar las desventajas de este mapa.
+ Sobre el mapa de Copernicus:
  + ¿Qué ventajas tendría usarlo para nuestro objetivo?.  Descríbelas brevemente.
  + ¿Qué desventajas o problemas puedes identificar?. Descríbelas brevemente.
  + Propón alguna forma de minimizar las desventajas de este mapa.
+ ¿Cuál de los tres mapas usarías para tu trabajo? Justifica tu respuesta.



## Evaluación
Esta tarea no lleva asociado un proceso de calificación. Es decir, no tendrás una nota numérica. Sí habrá evaluación. Es decir, leeré vuestras aportaciones y trataré de hacer comentarios constructivos que pongan de manifiesto en qué medida (en mi opinión) habéis adquirido las competencias que nos planteamos en clase.

