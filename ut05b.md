---
layout: default
title: UT05. Eventos y formularios (Opcionales)
nav_order: 8
---

# UT05. Eventos y formularios (Opcionales)

### OPT0501: Scroll infinito

**<span style="color: #ED7117">📣 Opcional</span>**

Un efecto que vemos habitualmente en muchas páginas web es el **scroll infinito**, que consiste en ir cargando de forma dinámica los contenidos de la página a medida que se va haciendo scroll.

Para realizar este efecto hay que tener encuenta algunas propiedades del nodo DOM que contiene todo el documento, es decir, el que corresponde a la etiqueta `<html>`. Podemos acceder a este nodo con la propiedad `document.documentElement`. Las propiedades que nos interesan son:

- `element.scrollHeight`: contiene la altura (en píxeles) del contenido del elemento, incluyendo el contenido que no es visible en la pantalla.
- `element.scrollTop`: indica el número de píxeles que el contenido del elemento ha sido desplazado hacia arriba, es decir, la distancia desde el límite superior de un elemento al límite superior de su contenido visible.
- `element.clientHeight`: devuelve la altura del elemento en píxeles.

![Scroll Properties](assets/opt0501/scrollProperties.png)

Teniendo esto en cuenta el proceso es muy sencillo:

- Se carga una parte de la página, por ejemplo, si es un blog tres o cuatro artículos, o si es una galería de imágenes las primeras imágenes.
- Asociamos un *listener* al evento **`scroll`** del objeto `window`
- Cada vez que se activa el evento comprobamos si el usuario está visualizando la parte inferior del documento. Esto lo podemos saber cuando `scrollTop + clientHeight` se esté acercando a `scrollHeight`.
- En ese momento cargamos los siguientes elementos y los añadimos al final de la página, lo que modificará el tamaño de `scrollHeight`, por lo que volvemos a empezar.
- Antes de cargar los siguientes elementos puedes añadir un GIF de carga al final de la página para que el usuario tenga algún tipo de realimentación que le indique que se están cargando más elementos.

![GIF de carga](assets/opt0501/loading.gif)

Ahora pon en práctica esto creando una pequeña página que muestre un scroll infinito. Vamos a suponer que queremos mostrar una **galería de fotos** que se irán mostrando infinitamente a medida que hagamos scroll.

Las fotos las vamos a obtener de [Lorem Picsum](https://picsum.photos/), una página web que permite obtener fácilmente fotos aleatorias para nuestros diseños, simplemente tienes que invocar la URL `https://picsum.photos/X/Y` para obtener una foto aleatoria de X píxeles de ancho e Y píxeles de alto. Si tienes dudas en la propia página web se explica su funcionamiento y las diversas opciones disponibles.

---

### OPT0502: Calculadora

Implementa una **calculadora** que pueda ser manipulada tanto con el teclado como con el ratón. Puedes añadirle todas las funciones que quieras, pero por lo menos debería poder realizar las operaciones básicas de suma, resta, multiplicación y división.

### OPT0503: Caída de letras


