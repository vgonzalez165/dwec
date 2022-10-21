---
layout: default
title: UT03. Objetos y tipos de datos. Opcionales
nav_order: 4
---

# UT03. Objetos y tipos de datos 

## Prácticas opcionales


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

### PR0331: Prácticas opcionales (I)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `reverseWords(str)` que tome una cadena `str`como entrada y devuelva la misma cadena invirtiendo el orden de las letras de cada palabra.

Ejemplo: 

```javascript
reverseWords('Hola mundo');      // 'aloH odnum'
reverseWords('IES Villabalter')  // 'SEI retlaballiV'
```

**Fuente**: [CodeWars: Reverse Words](https://www.codewars.com/kata/5259b20d6021e9e14c0010d4)

---

### PR0332: Prácticas opcionales (II)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `arrayDiff( a, b )` que tome como parámetros dos arrays y devuelva el resultado de eliminar del primero todos los elementos que se encuentren en el segundo.

**Ejemplo**:

```javascript
arrayDiff([1,2],[1]);       // [2]
```

---

### PR0333: Prácticas opcionales (II)

**<span style="color: #ED7117">📣 Opcional</span>**

Crea una función `digitalRoot(a)` que reciba como parámetro un número y devuelva la suma recursiva de todos sus dígitos. Es decir, sumará sus dígitos y, en caso de que el resultado tenga más de un dígito seguirá sumándolos hasta que el resultado sea un único dígito.

**Ejemplo**:

```javascript
        16  -->  1 + 6 = 7
       942  -->  9 + 4 + 2 = 15  -->  1 + 5 = 6
    132189  -->  1 + 3 + 2 + 1 + 8 + 9 = 24  -->  2 + 4 = 6
    493193  -->  4 + 9 + 3 + 1 + 9 + 3 = 29  -->  2 + 9 = 11  -->  1 + 1 = 2
```

