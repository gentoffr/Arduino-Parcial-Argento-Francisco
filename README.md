# Arduino-Parcial-Argento-Francisco
# Descripción.
La segunda parte de este proyecto añade dos slideswitch, asi como un sensor de flexion, el estado inicial de los switches es con el interruptor hacia la izquierda, al presionarse el que se haya a la derecha, el display mostrara los numeros primos, permitiendo mostrar el siguiente o el anterior con los botones, o volver al primer numero primo con el boton del medio.
El switch que se encuentra arriba permite ver que tan flexionado esta el sensor a traves del display.
Cabe destacar que el flexor va de 0 a 180, y esta reescalado para que entre en el display de dos cifras, por lo que el numero mostrado seria el porcentaje de flexion actual.
# Actualizacion
Ahora los el contador vuelve al principio si se pasa de 99 o va al final si baja de 0.
# Funciones
No se añaden nuevas funciones, hay una comentada que era la logica para conseguir los numeros primos en cierto rango, pensaba en pasarle un numero a la funcion, y que esta me devolviera un array con todos los numeros primos desde el 0 hasta el numero ingresado por parametro.
Sin embargo me encontre imposibilitado, pregunte a IAs y todas me pedian que hiciera un <include vector>, cosa que al parecer es imposible en tinkercad, ya que al hacerlo, salta un error que dice "no such file or directory found".
El problema principal de la funcion es a la hora de añadir nuevos elementos al array, realmente no entendia porque no podia, y entre en el servidor oficial de arduino para preguntar, recibiendo esta respuesta:
![image](https://github.com/gentoffr/Arduino-Parcial-Argento-Francisco/assets/129513207/c9ae90e7-ae1b-4b54-9f6b-01473b9b0493)
Traduciendo y resumiendo, se me explico que el soporte para la realocacion de memoria dinamica esta incompleto, por lo que no es buena idea hacer lo que estaba haciendo, al final me conforme con listar los numeros primos a mano.
Para mas informacion ver:
https://www.nongnu.org/avr-libc/user-manual/malloc.html
# Imagen del proyecto
![image](https://github.com/gentoffr/Arduino-Parcial-Argento-Francisco/assets/129513207/ebbb017a-d2fd-43e4-b5d4-edfdc1398073)
# Link de tinkercad
https://www.tinkercad.com/things/03Zr3Z3FwU0?sharecode=8diWDRRaRJHAUIWKdlo-qORdnILWH7Bx8B-o2oxOYIs
