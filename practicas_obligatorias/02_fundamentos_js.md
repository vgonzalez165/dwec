---
layout: default
title: UT02. Fundamentos de JavaScript
nav_order: 2
---

# UT02: Fundamentos de JavaScript

## Ejercicios de tipos de datos y operadores

### PR0201: Tipos de datos (I)

Crea un script que solicite al usuario su nombre y su localidad. A continuación, muestra un mensaje que tenga un texto de la forma `"Hola <nombre>, eres de <localidad>"`.

---

### PR0202: Tipos de datos (II)

Crea un script que pida por pantalla al usuario tres datos:

- El nombre
- La nota del primer examen 
- La nota del segundo examen 

A continuación mostrará por pantalla el mensaje `"Hola <nombre>, la nota media de tus exámenes es <nota_media>"` donde `<nota_media>` es la suma de las dos notas introducidas divididas entre dos.

---

### PR0203: Tipos de datos (III)

Crea un script que pida al usuario los siguientes datos, asumiendo en todos los casos que el usuario introducirá un valor numérico:

- Precio por kilo de manzanas
- Cantidad de manzanas
- Precio por kilo de naranjas
- Cantidad de naranjas
- Precio por kilo de plátanos
- Cantidad de plátanos

Cuando el usuario haya introducido todos los datos muestra un mensaje de la forma `"Has comprado un total de <kilos> kilos de fruta y te ha costado <importe_total> euros"`.

---

### PR0204: Tipos de datos y operadores (IV)

Crea un script que pida al usuario el radio de un círculo y muestre por pantalla una cadena de la forma `El perímetro del círculo de radio <radio> es <perímetro> y su área es <área>`.

Recuerda que la fórmula del perímetro de un círculo es `P = 2 · Pi · r` y el del área `A = Pr · r ^ 2`.

---


## Ejercicios de condicionales y bucles

### PR0205: Condicionales y bucles (I)

Crea un script que pida un número por pantalla al usuario, seguirá pidiéndolo hasta que el usuario introduzca un número valido. Cuando el número sea válido mostrará un mensaje diciendo `"Has introducido el número <numero>"`.

---

### PR0206: Condicionales y bucles (II)

Crea un script que solicite un número `n` y un valor `k` y que muestre por la consola los primero `k` elementos de la tabla de multiplicar de `n`.

Por ejemplo, si `n=5` y `k=12` mostraría una salida de la forma:

```
5 * 1 = 5
5 * 2 = 10
5 * 3 = 15
...
5 * 11 = 55
5 * 12 = 60
```

---

### PR0207: Condicionales y bucles (III)

Crea un script que solicite un número al usuario y dibuje en la consola un triángulo con asteriscos cuya base sea el número introducido. Por ejemplo, si el número introducido es `5` la salida será:

```
*
**
***
****
*****
```

---

### PR0208: Condicionales y bucles (IV)

Crea un script que pregunte al usuario su año de nacimiento y según sea le indique a qué generación pertenece teniendo en cuenta la siguiente tabla:

| Fecha de nacimiento | Generación           |
| ------------------- | -------------------- |
| 1994 - 2010         | Generación Z         |
| 1981 - 1993         | Generación Millenial |
| 1969 - 1980         | Generación X         |
| 1949 - 1968         | Baby Boomer          |

Si la fecha de nacimiento es anterior o posterior a las fechas indicadas se le mostrará también un mensaje notificándoselo.

---

### PR0209: Condicionales y bucles (V)

Vamos a crear un script que preguntará al usuario la calle en la que vive y, en función de la calle que sea le recomendará qué linea de autobús tiene que tomar para ir al trabajo. Las diferentes líneas de autobús son:

- *Línea 1*: Calle Los Claveles, Calle El Rosal, Calle Las Hortensias y Calle Las Margaritas
- *Línea 2*: Calle Teleno, Calle Catoute, Calle Peña Ubiña y Calle Vizcodillo
- *Línea 3*: Calle Astorga, Calle La Bañeza y Calle Benavente

Cuando el usuario introduzca la calle se le mostrará un mensaje de la forma `"Tienes que tomar la <linea_bus> para ir desde la <nombre_calle> hasta el trabajo"`.

---

### PR0210: Condicionales y bucles (VI) 

Crea un script que pida al usuario que introduzca 5 números y luego le diga cuál es el mayor y el menor de todos ellos de la forma: `El mayor número es <mayor> y el menor <menor>`.

---

### PR0211: Condicionales y bucles (VII)

Crea un script que pida un número por pantalla al usuario y le diga si es par o impar. Si el usuario introdujera un valor inferior o igual a 0, o un valor no numérico se lo volverá a pedir.

--- 

## Ejercicios de funciones

### PR0212: Funciones (I)

Crea una función `isPrime(n)` que devuelva `true` si el número `n` es primo y `false` en caso contrario. Intégrala en un script que pida un número al usuario y le diga si es primo o no. El script finalizará cuando el usuario introduzca el valor `0`.

---

### PR0213: Funciones (II)

Aprovecha la función del ejercicio anterior para crear un script que pida un valor `k` al usuario y le muestre por la consola los primeros `k` números primos.

---

### PR0214: Funciones (III)

Escribe una función `fact( n )` que calcule el factorial del número `n`.

---

### PR0215: Funciones (IV)

Escribe una función `calc( operador, operando1, operando2 )` que reciba como parámetros una cadena con el operador y dos operandos, y devuelva el resultado de la operación indicada. Debe reconocer por lo menos seis operadores y mostrar un error en caso de invocarla con un operador erróneo. Por ejemplo:

```javascript
calc( 5, 7, '*' );      // 35
calc( 1, 0, '+' );      // 1
calc( 9, 3, '/' );      // 3
```

---

### PR0216: Funciones (V)

Escribe una función `convertToBytes( capacity, from )` que reciba una cantidad y una unidad de medida y lo convierta a bytes. Las unidades de medida serán los múltiplos del byte hasta el Exabyte y en la unidad de medida se reconocerá tanto el nombre de la misma como la abreviatura, los cuales se muestran en la siguiente tabla:

| Unidad de medida  | Abreviatura   |   Número de bytes     |
| ----------------- | ------------- | --------------------- |
| Byte              | B             | 1                     |
| Kilobyte          | KB            | 1.000                 |
| Megabyte          | MB            | 1.000.000             |
| Gigabyte          | GB            | 1.000.000.000         |
| Terabyte          | TB            | 1.000.000.000.000     |
| Petabyte          | PB            | 1.000.000.000.000.000 |
| Exabyte           | EB            | 1.000.000.000.000.000.000 |

Por ejemplo:

```javascript
convertToBytes( 3, 'MB' );          // 3000000
convertToBytes( 5, 'Terabyte' );    // 5000000000000
```

---

### PR0217: Funciones (VI)

Mejora la función anterior para que realice las conversiones entre dos unidades de medida cualquiera. La función se llamará `convertCapacity( n, from, to )`, siendo el parámetro `to` la unidad de medida del valor `n` y `from` la unidad de medida a la que hay que convertirlo.

Ejemplos:

```javascript
convertCapacity( 5, 'GB', 'Megabyte' );     // 5000
convertCapacity( 500, 'B', 'KB' );          // 0.5
```

Aunque hay formas más eficientes de hacerlo, con lo que hemos visto hasta ahora lo más sencillo es convertir el valor pasado a bytes y desde ahí a la unidad de medida de destino.

---

### PR0218: Funciones (VI)

Escribe una función que reciba tres números como parámetros y devuelva verdadero si se puede formar un triángulo con esas medidas. Para ello debes usar el [teorema de la desigualdad triangular](https://es.wikipedia.org/wiki/Desigualdad_triangular), que dice que se puede formar un triángulo siempre que la suma de dos lados del triángulo sea mayor que el tercer lado para cualquier combinación de lados. 

Es decir, para los lados `a`, `b` y `c` se tienen que cumplir las siguientes tres condiciones:

```
a + b > c
a + c > b
b + c > a
```

---

### PR0219: Funciones (VII)

Crea una función `sumOfMults( k, n )` que devuelva la suma de los `k` primeros múltiplos del número `n`.

Ejemplo:

```javascript
sumOfMults( 3, 5 );     // 3*1 + 3*2 + 3*3 + 3*4 + 3*5 -> 45
sumOfMults( 2, 10 );    // 2*1 + 2*2 + 2*3 + ... + 2*10 -> Lo que de...
```

---

### PR0220: Funciones (VIII)

Crea una función `getFibonacciAt( n )` que devuelva el enésimo número de la serie de Fibonacci .

Recuerda que la serie de Fibonacci se define como: 

```javascript
fibonacci(0) = 0;
fibonacci(1) = 1;
fibonacci(n) = fibonacci( n-1 ) + fibonacci( n-2 );
// Por lo tanto la serie será: 0 1 1 2 3 5 8 13 21 34 55 ...
getFibonacciAt( 6 );        // Devuelve 8
```

---

### PR0221: Funciones (IX)

Crea una función `isNumber( str )` que reciba una cadena y devuelva `true` si contiene un número válido.

Ejemplo: 

```javascript
isNumber( '234.43' );       // true
isNumber( 'siete' );        // false
isNumber( '    34 ' );      // true
isNumber( '23a' );          // false
```