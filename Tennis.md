# Kata Tennis

## Enunciado

Esta kata trata de modelar un partido de tenis :).

La forma de llevar el tanteo en tenis puede ser complicado, por este motivo la ATP nos ha contratado para construir un marcador que sea capaz de mostrar el resultado actual de un partido.

Nuestro trabajo consiste en escribir un programa "TennisGame" que contenga la lógica del sistema de tanteo y que muestre el resultado correcto en formato de texto para mostrarlo en las pantallas.

Cuando un jugador gane un punto, el programa contendrá un método al que se le podrá llamar para poder indicarle qué jugador ha sido el ganador del punto. Además, el sistema recibirá llamadas de las pantallas a un método "score()" que devolverá cuál es el resultado actual. Este método debería devolver un texto con el resultado.

Este es un resumen explicamos cómo funciona el tanteo en tenis, pero si necesitas más información puedes visitar el siguiente
[enlace](https://en.wikipedia.org/wiki/Tennis#Scoring):

Un juego se gana cuando uno de los jugadores gana al menos 4 puntos en total y al menos dos puntos más que el oponente.
El tanteo parcial se lleva de una manera un tanto (¡BOOM!) "especial": respectivamente "Love", "Fifteen", "Thirty", y "Forty".
Si al menos cada uno de los jugadores ha ganado 3 puntos y el resultado está empatado, el resultado es "Deuce".
Si al menos cada uno de los jugadores ha ganado 3 puntos y uno de lo jugadores tiene un punto más que su rival, el resultado del juego es "Advantage" para el jugador que va en cabeza.
Sólo necesitas reportar el resultado del juego actual. Este es un primer desarrollo, por lo tanto, ahora los sets y juegos quedan fuera del contexto. ¡Más vale!

## Requerimientos
Escribe un programa para manejar cada uno de los siguientes requerimientos de puntuación de dos jugadores del juego de tennis.

```
Los jugadores deben poder ganar puntos.
El juego debe terminar con un ganador.
Debes de manejar la casuística de "iguales"
Después de terminar el juego, debe determinarse quién es el ganador.
Debe ser posible obtener la puntuación de cualquier de los jugadores en cualquier momento del partido.
```

## Créditos

[Kata original](http://www.solveet.com/exercises/Kata-Tennis/13)
[Kata tennis refactoring] (https://github.com/emilybache/Tennis-Refactoring-Kata)
