---
layout: default
title: UT07. Solicitudes de red
nav_order: 11
---

# UT07. Solicitudes de red


## PR0701: APIs REST (I)

Crea una página Web que descargue el listado de planetas de la [API de StarWars](https://swapi.dev) y muestre por pantalla una tabla con información de los mismos. Esta información será el nombre del planeta y otras tres o cuatro propiedades que de tu elección.

---

## PR0702: APIs REST (II)

Seguro que te has fijado que en la llamada a la API del ejercicio anterior únicamente te devuelve 10 planetas, aunque hay un total de 60.

Si observas los datos que devuelve verás que hay una propiedad `next` que indica la llamada que hay que realizar para obtener los siguientes 10 planetas.

```json
{
    count: 60, 
    next: "https://swapi.dev/api/planets/?page=2", 
    previous: null, 
    results: [
        {
            name: "Tatooine", 
            rotation_period: "23", 
```

Modifica el ejercicio anterior para que **muestre todos los planetas** en lugar de únicamente los 10 primeros.

---

## PR0703: APIs REST (III)

Ahora modifica la página anterior para que muestre los planetas de 10 en 10 (tal como los devuelve la API), pero que tenga un par de botones para mostrar los siguientes o los anteriores 10 planetas.

---

## PR0704: APIs REST (IV)

Vamos a utilizar ahora la API de [OpenWeather](https://openweathermap.org), por lo que lo primero que necesitarás será crear una cuenta y obtener una API Key para realizar las pruebas.

Vas a crear una página Web que tenga un formulario en el que se pedirán al usuario una longitud y una latitud y muestre cuál es el tiempo actual en dicha posición (es el campo `weather.description` de la respuesta de la API). Este tiempo lo tienes que mostrar en castellano, por lo que debes buscar en la documentación de la API como hacer para obtener la respuesta en este idioma.

**NOTA**: como la página la subirás a GitHub y no es buena idea tener allí las API Keys, añade otro campo al formulario para que el usuario indique la API Key que se utilizará.

---

## PR0705: APIs REST (V)

Ahora que ya sabes como realizar consultas a una API vamos a mejorar el ejercicio anterior para añadir una serie de mejoras a la página anterior.

- En lugar de preguntar por unas coordenadas geográficas, solicita al usuario el nombre de una ciudad. Como se indica en la documentación, puedes saber cuáles son las coordenadas de una ciudad utilizando [Geocoding API](https://openweathermap.org/api/geocoding-api).
- Vamos a mostrar más información del tiempo, en concreto:
  - La descripción en castellano como ya hicimos en el ejercicio anterior.
  - El icono correspondiente al clima actual (la [propia API](https://openweathermap.org/weather-conditions) indica qué icono utilizar en la respuesta)
  - Temperatura
  - Humedad
  - Cantidad de lluvia y nieve en las últimas 3 horas

Utiliza CSS para presentar los datos de una forma más o menos aceptable. Recuerda que en el aula virtual dispones de una serie de páginas web con gran cantidad de iconos que puedes utilizar en tus ejercicios.