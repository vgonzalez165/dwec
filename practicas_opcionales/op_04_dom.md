---
layout: default
title: UT04. Document Object Model. DOM (Opcionales)
nav_order: 24
---

# UT04. Document Object Model. DOM (Opcionales)

## OPT0401: Frutería App (II)

**<span style="color: #ED7117">📣 Opcional</span>**

Vamos a seguir trabajando con la frutería con la que empezamos en la anterior práctica y, en esta ocasión, vamos a añadir un carrito de la compra.

El resultado final debe ser algo parecido a lo que se muestra en el siguiente vídeo:

<video width="640" controls>
    <source src="../assets/videos/fruteria_01.mp4" type="video/mp4">
    Tu navegador no soporta la reproducción de vídeo
</video>

Como vas a ver cuando te pongas con ello aquí se complica todo un poco más. Algunos consejos o pautas de lo que tienes que realizar:

- Asumimos que cada vez que se pulsa el botón *Añadir* añade 1 kg de producto a la cesta de la compra. Si se quieren comprar varios kilos hay que pulsar varias veces y no se pueden comprar fracciones de kilo.
- Necesitarás un array global que almacene la cesta de la compra. Cada elemento de este array corresponderá a cada producto comprado por lo que pueden ser objetos con la misma estructura que los del array `Products` añadiéndole una propiedad con la cantidad de producto comprado.
- Tienes que añadir un *listener* a cada botón que lanzará una función que se puede llamar, por ejemplo, `addToCart(event)`. Esta función tiene que saber qué producto hemos comprado (recuerda que solo recoge información del elemento que disparó el evento), por lo que a cada botón deberás añadir un atributo `data-id` que almacene la fruta a la que corresponde.
- Para actualizar la cesta de la compra, una buena opción será crear una función `renderCart` o como quieras llamarla, que redibuje la cesta completa a partir del array con la compra. Esta función la puedes invocar cada vez que un usuario añada un producto a la compra.


## OPT0402: Frutería App (III)

**<span style="color: #ED7117">📣 Opcional</span>**

Seguimos trabajando con la app de la frutería. En el apartado anterior has creado una cesta de la compra en la que puedes añadir productos cada vez que le damos al botón *Añadir* de un producto, pero siempre una única unidad. 

Vamos a mejorarla añadiendo dos nuevas funcionalidades:

- **Añadir la cantidad que queramos de un producto**: para conseguir este objetivo utilizaremos una **ventana modal** en la que se mostrará un mensaje indicando el producto que vamos a añadir al carrito y un cuadro de texto que permita al usuario seleccionar la cantidad de producto que se va a añadir al carrito de la compra.
- **Eliminar objetos del carrito**: tal como tenemos ahora la aplicación podemos agregar nuevos productos al carrito, pero no podemos eliminar los que hayamos agregado previamente. Para solucionar esto vamos a insertar un botón en cada producto del carrito de forma que, cuando el usuario pulse dicho botón, se elimine el producto correspondiente.

