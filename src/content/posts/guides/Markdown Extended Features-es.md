---
title: Características Extendidas de Markdown
published: 2025-04-25
tags:
  - Guía
toc: false
lang: es
abbrlink: markdown-extended-features
---

Aquí presentamos algunas características extendidas de Markdown compatibles con Retypeset, incluyendo ejemplos de sintaxis y sus efectos estilísticos.

## Leyendas de Figuras

Para crear leyendas automáticas para figuras, utilice la sintaxis estándar de imágenes de Markdown `![alt](src)`. Para ocultar la leyenda, añada un guion bajo `_` antes del texto `alt` o deje el texto `alt` vacío.

### Sintaxis

```
![Descripción de la imagen](https://image.radishzz.cc/image/gallery/06.webp)

![_Descripción de la imagen](https://image.radishzz.cc/image/gallery/06.webp)
```

### Resultado

![Descripción de la imagen](https://image.radishzz.cc/image/gallery/06.webp)

![_Descripción de la imagen](https://image.radishzz.cc/image/gallery/06.webp)

## Bloques de Admonición

Para crear bloques de admonición, utilice la sintaxis de GitHub `> [!TYPE]` o la directiva contenedor `:::type`. Se admiten los siguientes tipos: `note`, `tip`, `important`, `warning` y `caution`.

### Sintaxis

```
> [!NOTE]
> Información útil que los usuarios deben conocer, incluso al leer por encima.

> [!TIP]
> Consejos útiles para hacer las cosas mejor o más fácilmente.

> [!IMPORTANT]
> Información clave que los usuarios necesitan saber para lograr su objetivo.

:::warning
Información urgente que requiere atención inmediata del usuario para evitar problemas.
:::

:::caution
Advierte sobre riesgos o resultados negativos de ciertas acciones.
:::

:::note[TÍTULO PERSONALIZADO]
Esta es una nota con un título personalizado.
:::
```

### Resultado

> [!NOTE]
> Información útil que los usuarios deben conocer, incluso al leer por encima.

> [!TIP]
> Consejos útiles para hacer las cosas mejor o más fácilmente.

> [!IMPORTANT]
> Información clave que los usuarios necesitan saber para lograr su objetivo.

:::warning
Información urgente que requiere atención inmediata del usuario para evitar problemas.
:::

:::caution
Advierte sobre riesgos o resultados negativos de ciertas acciones.
:::

:::note[TÍTULO PERSONALIZADO]
Esta es una nota con un título personalizado.
:::

## Secciones Plegables

Para crear secciones plegables, utilice la sintaxis de directiva contenedor `:::fold[title]`. Haga clic en el título para expandir o contraer.

### Sintaxis

```
:::fold[Consejos de Uso]
El contenido que pueda no interesar a todos los lectores puede colocarse en una sección plegable.
:::
```

### Resultado

:::fold[Consejos de Uso]
El contenido que pueda no interesar a todos los lectores puede colocarse en una sección plegable.
:::

## Diagramas Mermaid

Para crear diagramas Mermaid, envuelva la sintaxis de Mermaid en bloques de código y especifique el tipo de lenguaje como `mermaid`.

### Sintaxis

``````
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
``````

### Resultado

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

## Galerías

Para crear galerías de imágenes, utilice la directiva contenedor `:::gallery`. Desplácese horizontalmente para ver más imágenes.

### Sintaxis

```
:::gallery
![Alpaca](https://image.radishzz.cc/image/gallery/sheep-1.jpg)
![Girando la cabeza](https://image.radishzz.cc/image/gallery/sheep-2.jpg)
![Contacto visual](https://image.radishzz.cc/image/gallery/sheep-3.jpg)
![Alpaca bebé](https://image.radishzz.cc/image/gallery/sheep-4.jpg)
![¡Ay, qué lindo!](https://image.radishzz.cc/image/gallery/sheep-5.jpg)
:::
```

### Resultado

:::gallery
![Alpaca](https://image.radishzz.cc/image/gallery/sheep-1.jpg)
![Girando la cabeza](https://image.radishzz.cc/image/gallery/sheep-2.jpg)
![Contacto visual](https://image.radishzz.cc/image/gallery/sheep-3.jpg)
![Alpaca bebé](https://image.radishzz.cc/image/gallery/sheep-4.jpg)
![¡Ay, qué lindo!](https://image.radishzz.cc/image/gallery/sheep-5.jpg)
:::

## Repositorios de GitHub

Para incrustar repositorios de GitHub, utilice la directiva hoja `::github{repo="owner/repo"}`.

### Sintaxis

```
::github{repo="radishzzz/astro-theme-retypeset"}
```

### Resultado

::github{repo="radishzzz/astro-theme-retypeset"}

## Videos

Para incrustar videos, utilice la directiva hoja `::youtube{id="video-id"}`.

### Sintaxis

```
::youtube{id="9pP0pIgP2kE"}

::bilibili{id="BV1sK4y1Z7KG"}
```

### Resultado

::youtube{id="9pP0pIgP2kE"}

::bilibili{id="BV1sK4y1Z7KG"}

## Spotify

Para incrustar contenido de Spotify, utilice la directiva hoja `::spotify{url="spotify-url"}`.

### Sintaxis

```
::spotify{url="https://open.spotify.com/track/0HYAsQwJIO6FLqpyTeD3l6"}

::spotify{url="https://open.spotify.com/album/03QiFOKDh6xMiSTkOnsmMG"}
```

### Resultado

::spotify{url="https://open.spotify.com/track/0HYAsQwJIO6FLqpyTeD3l6"}

::spotify{url="https://open.spotify.com/album/03QiFOKDh6xMiSTkOnsmMG"}

## Tweets

Para incrustar tweets, utilice la directiva hoja `::tweet{url="tweet-url"}`.

### Sintaxis

```
::tweet{url="https://x.com/hachi_08/status/1906456524337123549"}
```

### Resultado

::tweet{url="https://x.com/hachi_08/status/1906456524337123549"}

## CodePen

Para incrustar demostraciones de CodePen, utilice la directiva hoja `::codepen{url="codepen-url"}`.

### Sintaxis

```
::codepen{url="https://codepen.io/jh3y/pen/NWdNMBJ"}
```

### Resultado

::codepen{url="https://codepen.io/jh3y/pen/NWdNMBJ"}
