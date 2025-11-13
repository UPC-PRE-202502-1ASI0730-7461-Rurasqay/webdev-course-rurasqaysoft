# Lección 3: Elementos HTML Comunes

**Objetivo:**  
Aprender a utilizar los elementos más comunes de HTML, como **encabezados, párrafos, listas, imágenes y enlaces**, para estructurar el contenido de una página web de forma clara y ordenada.

---

## Introducción

Una vez que conoces la estructura básica de un documento HTML, el siguiente paso es aprender los **elementos fundamentales** que permiten dar forma al contenido.  
HTML ofrece distintas etiquetas para mostrar texto, imágenes, enlaces y listas.  
Cada una cumple una función específica dentro del documento.

> 💡 Piensa en estos elementos como los muebles de una casa: cada uno tiene su lugar y propósito, pero juntos crean un espacio funcional.

---

## Encabezados (`<h1>` a `<h6>`)

Los encabezados se utilizan para **definir títulos y subtítulos** dentro de una página web.  
Van desde `<h1>` (más importante) hasta `<h6>` (menos importante).

```html
<h1>Encabezado principal</h1>
<h2>Subtítulo</h2>
<h3>Encabezado de tercer nivel</h3>
```

| Etiqueta        | Descripción                                                                     |
| :-------------- | :------------------------------------------------------------------------------ |
| `<h1>`          | Título principal del documento. Solo debería usarse una vez por página.         |
| `<h2>`          | Subtítulo o sección principal.                                                  |
| `<h3>` a `<h6>` | Subniveles de encabezado, usados para organizar jerárquicamente la información. |

## Párrafos (`<p>`)

Los párrafos son la base del texto en HTML.
Se usan para agrupar bloques de texto dentro del contenido.

```html
<p>
  Este es un párrafo de ejemplo. Los párrafos ayudan a organizar el texto y
  hacerlo más legible.
</p>
```

## Listas (`<ul>`, `<ol>`, `<li>`)

Las listas permiten organizar información en forma de ítems.

### Lista desordenada (`<ul>`)

Usa viñetas para mostrar elementos sin un orden específico.

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

### Lista ordenada (`<ol>`)

Muestra elementos numerados.

```html
<ol>
  <li>Inicio</li>
  <li>Desarrollo</li>
  <li>Conclusión</li>
</ol>
```

## Imágenes (`<img>`)

La etiqueta `<img>` permite insertar imágenes dentro de la página.

```html
<img src="imagen.jpg" alt="Descripción de la imagen" />
```

| Atributo           | Descripción                                                              |
| :----------------- | :----------------------------------------------------------------------- |
| `src`              | Indica la ubicación o ruta de la imagen.                                 |
| `alt`              | Proporciona una descripción alternativa (importante para accesibilidad). |
| `width` / `height` | Ajustan el tamaño de la imagen (opcional).                               |

## Enlaces (`<a>`)

Los enlaces conectan una página con otra o con un recurso externo.

```html
<a href="https://www.wikipedia.org" target="_blank">Ir a Wikipedia</a>
```

| Atributo          | Descripción                                           |
| :---------------- | :---------------------------------------------------- |
| `href`            | Dirección del enlace o destino (URL).                 |
| `target="_blank"` | Abre el enlace en una nueva pestaña.                  |
| `title`           | Texto que aparece al pasar el cursor sobre el enlace. |