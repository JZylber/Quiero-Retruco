# Quiero Retruco

Para armar un juego de truco, nos interesa modelar las cartas y el mazo

## Punto 1: Cartas

Armar un clase `Carta` en donde el constructor tome 2 parámetros: número y palo. Guardar esa información en atributos.
Además, sobreescribir el método `__str__`, que se llama cuando se imprime el objeto o se pasa a str. Hacerlo para que devuelva una representación apropiada del objeto, como "1 de basto".

## Punto 2: Mazo

Armar una clase `Mazo` en donde el constructor **no tome parámetros** pero se incialice con las 40 cartas de baraja española necesarias para jugar al truco.

Además, debe contar con los siguientes métodos:
- `mezclar`: mezcla las cartas que lo conforman.
- `sacar_carta`: saca una carta del tope del mazo, y la devuelve.
- `poner_carta(carta)`: toma una carta y la pone al final del mazo. Pueden asumir que la carta es una que no se encuentra en el mazo.

Por último, al igual que carta, sobreescriban el método `__str__` para que se vean las cartas que componen al mazo. **TIP:** aprovechen que cuando llaman al print() o str() usan el `__str__` de `Carta`.
 
## Punto 3: Manos

Hacer una función que dado un mazo de cartas, y un número de jugadores (entre 2 y 6), reparta del mazo tantas manos como jugadores. Una mano es un conjunto de 3 cartas sacadas del mazo. Entonces, la función debe retornar una lista de manos (lista de listas). ¡No se olviden de mezclar el mazo antes de repartir!

## Punto 4 (EXTRA): Orden

Construir una función, que dadas dos cartas, A y B, devuelva, en términos de la jerarquía de cartas de truco, 1 si A vale más que B, 0 si pardan (empatan) o -1 si B vale más que A.