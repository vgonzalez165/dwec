---
layout: default
title: UT03. Objetos y tipos de datos (Opcionales)
nav_order: 4
---

# UT03. Objetos y tipos de datos (Opcionales)


## Prácticas opcionales de cadenas

### PR0312: Cadenas (VI)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `isHeterograma(str)` que devuelva `true` si la cadena pasada como parámetro es un **heterograma** y `false` en caso contrario. 

Un [heterograma](https://es.wikipedia.org/wiki/Heterograma) es una palabra o frase que no tiene ninguna letra repetida.

**Ejemplo**: 

```javascript
isHeterograma('Villabalter');   // false (se repite la a y la l)
isHeterograma('Victor');         // true
``` 

**Fuente**: [CodeWars: Isograms](https://www.codewars.com/kata/54ba84be607a92aa900000f1)

---

### PR0313: Cadenas (VII)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `isIsograma(str)` que devuelva `true` si la cadena `str` es un **isograma**. 

Un [isograma](https://es.wikipedia.org/wiki/Heterograma) es una cadena o frase en el que cada letra aparece repetida el mismo número de veces (un *heterograma* es un caso especial de *isograma* en el que cada letra se repite una vez).

**Ejemplo**: 

```javascript
isIsograma('acondicionar');         // true
isIsograma('papelera escritura');   // true
```

---

### PR0314: Cadenas (VIII)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `isPangrama(str)` que devuelva `true` si la palabra pasada como parámetro es un **pangrama**.

Un [pangrama](https://es.wikipedia.org/wiki/Pangrama) es un texto que usa todas las letras del alfabeto.

**Ejemplo**:

```javascript
isPangrama('El veloz murciélago hindú comía feliz cardillo y kiwi. La cigüeña tocaba el saxofón detrás del palenque de paja.');    // true
isPangrama('Un jugoso zumo de piña y kiwi bien frío es exquisito y no lleva alcohol.');     // true
```

--- 


## Prácticas opcionales de arrays

### PR0321: Arrays (VII)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `getUpperCase( arr )` que reciba como parámetro un arrays con *strings* y devuelve un array que únicamente contenga los *strings* cuyas letras sean todas mayúsculas.

**Ejemplo**:

```javascript
getUpperCase( ['aBc', 'BE', 'hfa', 'AEO'] );        // [ 'BE', 'AEO ]
```

---

### PR0322: Arrays (VIII)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `maxString( arr )` que tome como parámetro un array de *strings* y devuelva la cadena de mayor longitud.

**Ejemplo**: 

```javascript
maxString( ['hola', 'victor', 'villabalter', 'IES'] );      // 'villabalter' 
```

---

### PR0323: Arrays (IX)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `getNames( arr )` que tome como entrada un array de cadenas con nombres (nombre y apellidos) y devuelva un array de objetos de la forma `{ nombre: 'xxx', apellidos: 'yyy zzz' }`. Vamos a suponer que tanto los nombres como cada uno de los apellidos solo tienen una única palabra.

**Ejemplo**:

```javascript
getNames( ['Victor González Rodríguez', 'Pepe Pérez Fernández'] );      // [ { nombre: 'Victor', apellidos: 'González Rodríguez },
                                                                        //   { nombre: 'Pepe', apellidos: 'Pérez Fernández' } ]
```



## Prácticas opcionales de repaso

### PR0331: Repaso (I)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `reverseWords(str)` que tome una cadena `str`como entrada y devuelva la misma cadena invirtiendo el orden de las letras de cada palabra.

Ejemplo: 

```javascript
reverseWords('Hola mundo');      // 'aloH odnum'
reverseWords('IES Villabalter')  // 'SEI retlaballiV'
```

**Fuente**: [CodeWars: Reverse Words](https://www.codewars.com/kata/5259b20d6021e9e14c0010d4)

---

### PR0332: Repaso (II)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `arrayDiff( a, b )` que tome como parámetros dos arrays y devuelva el resultado de eliminar del primero todos los elementos que se encuentren en el segundo.

**Ejemplo**:

```javascript
arrayDiff([1,2],[1]);       // [2]
```

---

### PR0333: Repaso (III)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `digitalRoot(a)` que reciba como parámetro un número y devuelva la suma recursiva de todos sus dígitos. Es decir, sumará sus dígitos y, en caso de que el resultado tenga más de un dígito seguirá sumándolos hasta que el resultado sea un único dígito.

**Ejemplo**:

```javascript
        16  -->  1 + 6 = 7
       942  -->  9 + 4 + 2 = 15  -->  1 + 5 = 6
    132189  -->  1 + 3 + 2 + 1 + 8 + 9 = 24  -->  2 + 4 = 6
    493193  -->  4 + 9 + 3 + 1 + 9 + 3 = 29  -->  2 + 9 = 11  -->  1 + 1 = 2
```

**Fuente**: [CodeWars: Digital Root](https://www.codewars.com/kata/541c8630095125aba6000c00)


---

### PR0334: Repaso (IV)

Desarrolla una función `findNextPower( n, pow)` que, dado un número `n`, devuelva la potencia `pow` de otro número más próxima que sea superior a `n`.

**Ejemplo**:

```javascript
findNextPower( 70, 4 );         // 81, ya que es 81 = 3^4
findNextPower( 12385, 3 );      // 13824
```

**Fuente**: [CodeWars: Find Next Power](https://www.codewars.com/kata/56ba65c6a15703ac7e002075)

---

### PR0335: Repaso (V)

Diseña una función `maxSequence( arr )` que tome un array de enteros (positivos o negativos) como entrada y devuelva el subarray cuya suma sea mayor.

**Ejemplo**:

```javascript
maxSequence([-2, 1, -3, 4, -1, 2, 1, -5, 4])    // Devuelve 6, que es la suma del subarray [4, -1, 2, 1]
```

**Fuente**: [CodeWars: Maximum Subarray Sum](https://www.codewars.com/kata/54521e9ec8e60bc4de000d6c)

--

### PR0336: Repaso (VI)

Crea una función `XO( str )` que tome como parámetro una cadena y devuelva `true` si la cadena tiene el mismo número de `X` que de `O` (sin distinguir entre mayúsculas y minúsculas). La cadena puede tener cualquier otro carácter que se ignorará.

```javascript
XO("ooxx")    // true
XO("xooxx")   // false
XO("ooxXm")   // true
XO("zpzpzpp") // true 
XO("zzoo")    // false
```

**Fuente**: [CodeWars: Exes and Ohs](https://www.codewars.com/kata/55908aad6620c066bc00002a)

--- 

### PR0337: Repaso (VII)

Crea una función `cakes( recipe, ingredients )` donde `recipe` es un objeto con los ingredientes y cantidades que hacen falta para realizar una receta y `ingredients` es otro objeto con los ingredientes que hay disponibles. La función debe devolver un número que corresponderá con el número de recetas que se pueden realizar con los ingredientes disponibles.

```javascript
cakes(  {flour: 500, sugar: 200, eggs: 1},
        {flour: 1200, sugar: 1200, eggs: 5, milk: 200});   // Devuelve 2

cakes(  {apples: 3, flour: 300, sugar: 150, milk: 100, oil: 100}, 
        {sugar: 500, flour: 2000, milk: 2000});     // Devuelve 0
```

**Fuente**: [CodeWars: Pete the Baker](https://www.codewars.com/kata/525c65e51bf619685c000059)