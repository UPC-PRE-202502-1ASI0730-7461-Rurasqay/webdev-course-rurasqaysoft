# Lección 2: Estructura HTML Básica

**Objetivo:** Comprender cómo se organiza un documento HTML, qué son las etiquetas, los elementos y los atributos, y cómo estructuran el contenido de una página web.

---

## Introducción

Todo sitio web, sin importar su tamaño o complejidad, comienza con **HTML (HyperText Markup Language)**, el lenguaje que define la **estructura y el contenido** de las páginas web.  
HTML no se encarga de los colores ni del diseño (eso lo hace CSS), sino de describir **qué contiene** la página: textos, imágenes, títulos, listas, enlaces y más.

> 💡 Piensa en HTML como los ladrillos de una casa.

---

## ¿Qué es un documento HTML?

Un documento HTML es un archivo de texto con extensión `.html` que el navegador interpreta para mostrar una página web.

Su estructura básica sigue este formato:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Mi primera página web</title>
  </head>
  <body>
    <h1>¡Hola, mundo!</h1>
    <p>Este es mi primer párrafo en HTML.</p>
  </body>
</html>
```

---

### Estructura de un documento HTML

| **Sección**       | **Descripción**                                                                                                    |
| ----------------- | ------------------------------------------------------------------------------------------------------------------ |
| `<!DOCTYPE html>` | Le indica al navegador que el documento usa **HTML5**, la versión actual del lenguaje.                             |
| `<html>`          | Es el contenedor principal que envuelve todo el contenido de la página.                                            |
| `<head>`          | Contiene información no visible directamente, como el título, los metadatos o enlaces a hojas de estilo (**CSS**). |
| `<title>`         | Define el texto que aparecerá en la pestaña del navegador.                                                         |
| `<body>`          | Contiene todo el contenido visible: encabezados, párrafos, imágenes, listas, enlaces, etc.                         |

> Dato: El navegador necesita que el documento esté correctamente estructurado para interpretarlo bien. Si faltan etiquetas importantes, la página puede no mostrarse correctamente.

---

## ¿Qué son las etiquetas HTML?

Las etiquetas son las piezas fundamentales de HTML.
Cada etiqueta indica el tipo de contenido que contiene.

Una etiqueta se escribe entre los signos `<` y `>` y normalmente se cierra con `</nombre>`.

Por ejemplo:

`<p>Este es un párrafo</p>`

---

## ¿Qué son los elementos HTML?

Un elemento HTML incluye la etiqueta de apertura, el contenido y la etiqueta de cierre.

Ejemplo:

`<p>Hola, soy un elemento HTML completo</p>`

Algunos elementos no necesitan cierre, por ejemplo:

`<img src="foto.jpg" alt="Foto de perfil">`
`<br>`
`<hr>`

> Estos se llaman elementos vacíos, porque no tienen contenido dentro.

## ¿Qué son los atributos HTML?

Los atributos agregan información extra o configuran el comportamiento de una etiqueta.
Se escriben dentro de la etiqueta de apertura, con el formato nombre="valor".

`<a href="https://www.wikipedia.org" target="_blank">Ir a Wikipedia</a>`

| **Atributo**      | **Descripción**                                              |
| ----------------- | ------------------------------------------------------------ |
| `href`            | Indica la dirección del enlace (**URL**).                    |
| `target="_blank"` | Abre el enlace en una nueva pestaña.                         |
| `alt`             | Texto alternativo en imágenes (mejora la **accesibilidad**). |
| `src`             | Fuente o ubicación de un recurso, como una imagen o video.   |
| `title`           | Muestra un texto al pasar el cursor sobre el elemento.       |
