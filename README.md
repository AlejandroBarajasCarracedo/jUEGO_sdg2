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
