# Lección 5: Estilo Simple

**Objetivo:** Aprender a aplicar estilos CSS básicos para modificar la apariencia de los elementos HTML, incluyendo cómo centrar contenido, cambiar colores y añadir bordes.

---

## Introducción

En la lección anterior, vimos qué es CSS y cómo funcionan los selectores para apuntar a elementos HTML. Ahora, ¡es momento de aplicar estilo!

CSS nos permite tomar la estructura HTML (los "ladrillos") y decorarla (la "pintura y el diseño"). En esta lección, nos enfocaremos en tres tareas de estilo fundamentales que usarás en casi todos los proyectos web.

> 🎨 Piensa en CSS como la pintura, los muebles y la decoración de la casa que construiste con HTML. Hoy aprenderemos a pintar las paredes, centrar los muebles y poner marcos a los cuadros.

---

## 1. Añadir Colores

Dar color es una de las formas más fáciles de cambiar el aspecto de tu sitio. Hay dos propiedades principales que debes conocer:

* `color`: Cambia el color del **texto** dentro de un elemento.
* `background-color`: Cambia el color del **fondo** del elemento.

```html
<div class="caja-colorida">
  <h2>¡Tengo estilo!</h2>
  <p>Este texto es de un color, y el fondo es de otro.</p>
</div>
````

```css
/* Archivo CSS */
.caja-colorida {
  background-color: #f0f8ff; /* Un azul "aliceblue" muy claro */
  color: #333; /* Un gris oscuro para el texto */
}

.caja-colorida h2 {
  color: #0056b3; /* Un azul más oscuro para el título */
}
```

### Formatos de Color Comunes

Puedes especificar colores de varias maneras:

| **Formato** | **Ejemplo**                | **Descripción**                                    |
|-------------|----------------------------|----------------------------------------------------|
| Nombre      | `red`, `blue`, `lightgray` | Nombres de color predefinidos por el navegador.    |
| HEX         | `#FF0000`                  | Código hexadecimal (Rojo, Verde, Azul). Muy común. |
| RGB         | `rgb(255, 0, 0)`           | Valores de Rojo, Verde y Azul (de 0 a 255).        |

-----

## 2\. Añadir Bordes

Los bordes son excelentes para separar visualmente el contenido o agrupar elementos. La propiedad más común es `border`, que es un atajo para tres propiedades:

1.  **Grosor:** El ancho del borde (p. ej., `1px`, `2px`).
2.  **Estilo:** El tipo de línea (p. ej., `solid`, `dashed`, `dotted`).
3.  **Color:** El color del borde (usando cualquier formato de la tabla anterior).

<!-- end list -->

```html
<div class="caja-con-borde">
  <p>Este contenido está en una caja con borde.</p>
</div>
<p class="linea-division">
  Un separador simple.
</p>
```

```css
/* Archivo CSS */
.caja-con-borde {
  /* Grosor | Estilo | Color */
  border: 1px solid black;
  padding: 10px; /* (Extra) Añade espacio para que el texto no toque el borde */
}

.linea-division {
  /* Puedes aplicar bordes a un solo lado */
  border-bottom: 2px dashed #999; /* Borde inferior punteado gris */
}
```

-----

## 3\. Centrar Contenido

Centrar cosas en CSS puede parecer complicado al inicio, porque "centrar" significa dos cosas diferentes: centrar el texto *dentro* de un elemento, o centrar el elemento *completo* en la página.

### Centrar Texto

Para centrar texto (o elementos "en línea" como imágenes) **dentro** de su contenedor, usamos `text-align`.

```html
<h1 class="titulo-centrado">Mi Título Principal</h1>
<p class="parrafo-centrado">
  Todo este párrafo tendrá su texto centrado.
</p>
```

```css
/* Archivo CSS */
.titulo-centrado {
  text-align: center;
}
.parrafo-centrado {
  text-align: center;
}
```

### Centrar un Bloque (como un `div`)

Para centrar un elemento de bloque (como un `<div>` o un `<p>`) **en la página**, el método más común es darle un ancho (`width`) y poner sus márgenes (`margin`) izquierdo y derecho en `auto`.

```html
<div class="caja-centrada">
  <p>¡Este contenedor está centrado en la página!</p>
</div>
```

```css
/* Archivo CSS */
.caja-centrada {
  width: 80%; /* Debe tener un ancho definido */
  
  /* Pone los márgenes superior/inferior en 0 */
  /* y los márgenes izq/der en 'auto' */
  margin: 0 auto;
  
  /* (Opcional) Le ponemos un fondo para verlo mejor */
  background-color: #eee;
}
```

> **Dato:** `margin: 0 auto;` es una de las técnicas más importantes en CSS. Solo funciona en elementos de bloque que tengan un `width` definido.

-----

## 4\. Combinando Todo

Vamos a crear una "tarjeta" simple usando todo lo que aprendimos.

```html
<div class="tarjeta">
  <h2>Tarjeta de Perfil</h2>
  <p>
    Estoy usando colores, bordes y contenido centrado
    para crear este componente.
  </p>
</div>
```

```css
/* Archivo CSS */
.tarjeta {
  /* 1. Centrar el bloque */
  width: 300px;
  margin: 20px auto; /* 20px de margen arriba/abajo, y centrado */

  /* 2. Añadir Bordes */
  border: 1px solid #ccc;

  /* 3. Añadir Colores */
  background-color: #f9f9f9;
  
  /* 1. Centrar el texto (para el h2 y el p) */
  text-align: center;

  /* Extras para que se vea mejor */
  padding: 15px;
}

.tarjeta h2 {
  color: #d9534f; /* Un color rojo/anaranjado */
}
```