# DETECCION-MASCARILLA
Programa de deteccion de mascarilla complimentado con Arduiono. Este programa se encarga de detectar si tu rostro lleva mascarilla o no (con OpenCv yMediapipe).
Para ello primero hay que entrenarlo y para ello hay que tener una carpeta con varias caras de personas random con mascarilla por un lado y por otro lado sin mascarilla.
El entrenamiento de imagenes (train.py) genera un archivo .xtml
Una vez hecho esto se empieza con la deteccion de la cara mediante la videocamara (Mediapipe) y se indica si lleva mascariila o no (CV2)

![Captura1](https://user-images.githubusercontent.com/111430658/187037520-b591fbe8-6d8a-4b3d-a2f4-b166e22539e3.png)

![Captura2](https://user-images.githubusercontent.com/111430658/187037523-9aba1e1a-d7fb-41c9-b0b4-d8c827f76288.png)

Una vez explicada la parte de python, es el turno de la parte de arduino. Lo primero es el montaje del arduino con sus leds.
Programaremos el programa de tal forma que cuando el programa de python le diga a arduino si lleva mascarilla o no (eso será posible gracias a la entrada del monitor serie que puede ser o "p" o "n")
se encienda el led azul o verde.

![ESQUEMA ARDUINO](https://user-images.githubusercontent.com/111430658/187037555-8cd21240-fcbb-4eac-b2ac-5549254f8102.PNG)

Los leds nos van mostrar si nuestra mascarilla esta puesta o no.

CON MASCARILLA:
![CON MASCARILLA ARDUINO](https://user-images.githubusercontent.com/111430658/187037709-264c2ed4-63b3-475e-b148-851e5c5b36f3.jpg)

SIN MASCARILLA:
![SIN MASCARILLA ARDUINO](https://user-images.githubusercontent.com/111430658/187037710-04f184e2-82f3-4677-bf7f-4a0999838031.jpg)
