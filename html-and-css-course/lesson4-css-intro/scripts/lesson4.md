# Lección 4: Introducción a CSS (Selectores, Propiedades y Diseño)

**Objetivo:** Comprender qué es CSS, cómo se utiliza para dar estilo a una página web, y aprender los conceptos fundamentales de **selectores**, **propiedades** y **valores** para personalizar el color, la fuente y el diseño de los elementos HTML.

---

## Introducción

Si HTML define la **estructura** de una página web, **CSS (Cascading Style Sheets)** se encarga de su **apariencia y diseño visual**.  
CSS permite cambiar colores, fuentes, tamaños, márgenes, posiciones y prácticamente cualquier aspecto estético de los elementos de una página.

> 💡 Piensa en CSS como la pintura, los muebles y la decoración de una casa: el HTML es la estructura, y el CSS la hace atractiva.

---

## ¿Qué es CSS?

CSS (Hojas de Estilo en Cascada) es un lenguaje que describe **cómo se muestran los elementos HTML en pantalla**, en papel o en otros medios.

Puedes agregar CSS de tres formas principales:

1. **En línea (inline):** dentro del atributo `style` de una etiqueta HTML.

   ```html
   <p style="color: blue;">Texto azul</p>
   ```

2. **Interno:** dentro de una etiqueta `<style>` en el archivo `HTML`.

```html
<style>
  p {
    color: blue;
  }
</style>
```

3. **Externo:** en un archivo separado `.css` enlazado al `HTML`.

```html
<link rel="stylesheet" href="estilos.css" />
```

## Estructura de una regla CSS

Cada regla CSS tiene un selector, una o más propiedades, y sus valores:

```css
selector {
  propiedad: valor;
}
```

Ejemplos:

```css
p {
  color: red;
  font-size: 16px;
}
```

Esto indica que todos los párrafos `p` tendrán texto rojo y tamaño de fuente de 16 píxeles.

## Componentes de una regla CSS

| **Elemento** | **Descripción**                                                                 |
| ------------ | ------------------------------------------------------------------------------- |
| Selector     | Indica qué elementos HTML serán afectados (por ejemplo, `p`, `.clase`, `#id`).  |
| Propiedad    | Define qué aspecto se modificará (por ejemplo, `color`, `font-size`, `margin`). |
| Valor        | Especifica cómo se modificará (por ejemplo, `red`, `20px`, `center`).           |

---

## Tipos de selectores CSS

CSS ofrece varios tipos de selectores para aplicar estilos con precisión:

| **Tipo de Selector** | **Ejemplo**      | **Descripción**                                            |
| -------------------- | ---------------- | ---------------------------------------------------------- |
| Etiqueta             | `p { }`          | Selecciona todos los elementos `<p>`.                      |
| Clase                | `.destacado { }` | Selecciona todos los elementos con la clase `"destacado"`. |
| ID                   | `#titulo { }`    | Selecciona el elemento con el identificador `"titulo"`.    |
| Universal            | `* { }`          | Aplica el estilo a todos los elementos de la página.       |
| Descendiente         | `div p { }`      | Afecta solo los `<p>` dentro de un `<div>`.                |

## Propiedades básicas de CSS

La propiedad color cambia el color del texto, y background-color define el color de fondo.

```css
body {
  background-color: #f0f0f0;
  color: #333333;
}
```

## Fuente y texto

Propiedades relacionadas con el texto:

| **Propiedad** | **Ejemplo**                       | **Función**                                   |
| ------------- | --------------------------------- | --------------------------------------------- |
| `font-family` | `font-family: Arial, sans-serif;` | Cambia el tipo de letra.                      |
| `font-size`   | `font-size: 18px;`                | Define el tamaño del texto.                   |
| `font-weight` | `font-weight: bold;`              | Define el grosor de la fuente.                |
| `text-align`  | `text-align: center;`             | Alinea el texto (izquierda, centro, derecha). |
| `line-height` | `line-height: 1.5;`               | Ajusta el espaciado entre líneas.             |

---

## Diseño y espacio

CSS controla el diseño con propiedades de espaciado, tamaño y posición.

| **Propiedad** | **Ejemplo**                | **Función**                      |
| ------------- | -------------------------- | -------------------------------- |
| `margin`      | `margin: 20px;`            | Espacio **fuera** del elemento.  |
| `padding`     | `padding: 10px;`           | Espacio **dentro** del elemento. |
| `border`      | `border: 1px solid black;` | Agrega un borde alrededor.       |
| `width`       | `width: 50%;`              | Define el ancho del elemento.    |
| `height`      | `height: 100px;`           | Define la altura del elemento.   |
