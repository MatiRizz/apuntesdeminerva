# Apuntes de Minerva

Archivo de los textos de filosofía y filosofía del derecho que escribí durante la licenciatura y la maestría, publicados como sitio web para que no se los lleve el olvido.

**[www.apuntesdeminerva.com.ar](https://www.apuntesdeminerva.com.ar)**

> «La lechuza de Minerva solo alza su vuelo al caer el crepúsculo.»
> — G. W. F. Hegel, *Filosofía del derecho*

## Qué hay

Varios textos escritos entre 2018 y 2024, entre monografías y trabajos prácticos de la Licenciatura en Filosofía (UNSAM) y la Maestría en Filosofía del Derecho (UBA). Están ordenados en seis estaciones temáticas que van de Pitágoras a la inteligencia artificial.

Los textos se publican casi como fueron entregados: se corrigieron erratas, tildes y el formato de algunas citas, sin tocar los argumentos.

## Cómo está hecho

El sitio es un único `index.html` con HTML, CSS y JavaScript, sin frameworks, sin dependencias y sin paso de compilación. Lo único externo son las tipografías de Google Fonts: Fraunces, Newsreader, Courier Prime y Caveat.

- Los textos viven en un bloque oculto dentro del mismo HTML (`<div id="archivo">`). Al cargar la página, el script los lee y arma las fichas de cada estación, el índice, el lector, los contadores y los tiempos de lectura.
- La navegación usa rutas en el hash (`#/seccion/…`, `#/texto/…`, `#/indice`), así que cada texto tiene su propio enlace.
- El lector permite cambiar el tamaño de letra y pasar a modo noche (sigue la preferencia del sistema y recuerda la elección). Las notas al pie se abren como ventanas emergentes, y hay un botón para copiar el enlace y otro para pasar al texto anterior o siguiente de la misma estación.
- El índice se puede filtrar por nivel (licenciatura o maestría).
- Las ilustraciones son SVG dentro del HTML y se animan con el scroll. Si el sistema pide reducir el movimiento, las animaciones se desactivan.
- El diseño se adapta a pantallas de celular.

## Publicación

Está alojado en GitHub Pages, con dominio propio registrado en NIC Argentina y DNS gestionado en Cloudflare.

## Estructura

```
index.html            el sitio completo, textos incluidos
favicon.ico           ícono de la pestaña
favicon.svg
apple-touch-icon.png  ícono para la pantalla de inicio del celular
og-imagen.jpg         imagen de la tarjeta al compartir el link
CNAME                 dominio propio para GitHub Pages
```

## Agregar o editar textos

No hace falta tocar el CSS ni el JavaScript. Las partes editables de `index.html` están marcadas con `✎ EDITABLE` y explicadas en comentarios dentro del archivo.

Para sumar un texto alcanza con copiar un bloque `<article class="texto">` y completar la estación (`data-seccion`), el año (`data-anio`), el nivel (`data-nivel`), el título, un resumen y el cuerpo. La numeración, el índice y los contadores se actualizan solos.

## Verlo en local

Basta con abrir `index.html` en el navegador. Las tipografías se cargan desde Google Fonts, así que sin conexión se ven las de reemplazo.

## Licencia

Los textos se publican bajo licencia [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/deed.es): se pueden citar y compartir mencionando la fuente, sin fines comerciales.

## Autor

Matías Rizzuto · [LinkedIn](https://www.linkedin.com/in/matias-rizzuto/)
