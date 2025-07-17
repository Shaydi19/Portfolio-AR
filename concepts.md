# Realidad aumentada

## ¿Qué es la Realidad Aumentada?
Es el mecanismo por el cual se agrega metadada a la realidad. A través de video o fotos, se pueden agregar objetos virtuales y cuadros de datos de posición, información adicional a la realidad misma.
``` R+ ```
## ¿Qué es A-Frame?
Es un framework web orientado a la construcción de Realidad Virtual y Realidad Aumentada. 

## ¿Cómo se crean las escenas?
Con la etiqueta <a-scene> y los atributos necesarios, ya sea para usar la webcam o visualizar controles.

## Cámara con A-Frame
La cámara dentro de un entorno A-frame es el punto de vista desde el que se quiere proyectar la escena en A-Frame. Tiene características como el FOV y el Zoom.

## Componente A-Frame arjs
AR.js es una biblioteca orientada a la realidad aumentada en tres partes:
Marcadores, Posicionamiento global y seguimiento de imágenes. Se importa el componente desde la escena una vez cargada la biblioteca.

## AR basado en marcador:
Un marcador es una imagen preestablecida para que sea detectada por la cámara del dispositivo y que mande llamar metainformación, ya sea texto, imágenes, audios o video. Idealmente, es más sencillo para las cámaras y el procesamiento digital de imágenes que los marcadores sean monocromáticos.
### Tipos de marcadores que soporta ARJS
- Marcadores Hiro y Kanji: Estos markers vienen del japonés, se utiliza el kanji "Persona" y el romanji "Hiro" para la detección monocromática. Son marcadores con bordes negros grandes y de alto contraste. Son tradicionalmente usados para primeras pruebas o con cámaras de resolución baja.

- Marcador de patrón: Es como los marcadores anteriores, solo que no tienen un significado implícito, sino bloques cuadrados para ser detectados en diferentes posiciones.

- Marcador de código de barras: Es un marcador con una información de hasta 64 bits.

## AR sin marcador
Es la integración de información basado en características obtenidas de alguna otra manera, por ejemplo:

- Basado en ubicación: Toma el geoposicionamiento de la cámara, que dado un marcador, se pueda mostrar e interactuar con él.

- Basado en Reconocimiento corporal: Es el seguimiento de las extremidades y de las expresiones faciales para ser usadas como comandos. Puedes detectar una sonrisa, abrir la boca, parpadear o el seguimiento de la vista para hacer scroll o dar clic o lanzar algún comportamiento. Además, de que puedes leer gestos como extender la mano, pulgar hacia arriba o pellizcar con algún dedo para marcar alguna posición en la cámara. Puedes dar seguimiento a las lineas del cuerpo para dar movimiento a modelos 3d o validar datos en algún juego de baile.



## Seguimiento de imágenes basado en AR

A través de la marcación de un objeto en algún frame, se puede hacer el seguimiento de los objetos a través de diferentes frames. En combinación con bibliotecas de clasificación de imágenes, se pueden hacer conteo de cosas, como de personas que pasan por una puerta, carros en una avenida, selección de verduras o clasificación de objetos en una linea de producción.

