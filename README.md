# Arduino-Parcial-Argento-Francisco
Este proyecto consiste en un arduino uno y dos display de 7 segmentos, ademas de 3 botones.
Los display se hayan multiplexados, es decir que sus leds estan unidos, el pin A de uno con el pin A del otro y asi con los demas, esto es necesario ya que no hay suficientes pines como para conectar dos por separado.
Las funciones mas notables del codigo son "prendeCosas" y "printContador", la primera encargandose de gestionar que leds del display se prenderan, y la segunda encargandose de prender y apagar los dos display rapidamente, dando la sensacion de que ambos se hayan prendidos a la vez, ademas de la logica que contiene que permite mostrar por un lado las unidades, y las decenas por el otro.
La funcion comentada era un intento de hacer una funcion reutilizable para usar en lugar de "prendeCosas", consistia en una funcion a la que yo le pasaria un array con los leds a encender, y un loop for se encargaria de prenderlos, despues de investigar un poco, averigue que no es posible pasar arrays a funciones en C++.
El boton mas a la izquierda se encarga de aumentar el contador a mostrar, el del medio decrece el numero, y el tercero lo devuelve a 0.
