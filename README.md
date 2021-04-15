# jUEGO_sdg2
FUNCIONALIDAD SCORES:
EL objetivo es que cuando la pelota rompa un ladrillo, el jugador gane un punto en el acto, pudiendo asi, al llegar a una serie de puntos aumentar
la dificultad del juego con niveles.
· Código:
  - Definimos en sistemLib.h una variable externa global llamada scores, donde se puedan almacenar la puntuación del usuario.
  - Cada vez que la pelota rompa un ladrillo se sumara un punto, esto se hace en la función CompruebaReboteLadrillo de arkanoPiLib.c
  - Cada vez que se inicie el juego o se resetee, la variable scores valdrá 0.
  - Para que el usuario pueda ver su puntuación, se añade a la pantalla una linea llamada SCORES, donde la puntuación se va actualizando conforme
  a la actuación del usuario.
  
  
CAMBIAR EL COLOR DE LA PELOTA:
El objetivo de esta mejora es cambiar el color de la pelota para poder distinguir su trayectoria de una mejor forma. Para ello hemos cambiado el color de la pelota a verde en lugar del color blanco que tenia antes.
Código:
- En pseudowaringPi en el apartado de static int pseudoMatrizColor, tenemos definido de antemano que las dos primeras columnas desde la zona superior sean de color rojo (31), y la última fila de color azul(34)
- Las filas intermedias tenian asignado en primer lugar 0, por tanto, salía de color blanco, y nosotros hemos cambiado ese valor po el número 32 que representa el color verde, de esta forma mientas la pelota se encuentre en esa posición tomará el color verde
