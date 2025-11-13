# Lección 7: Recomendaciones y Errores Comunes

**Objetivo:** Identificar los errores más frecuentes que cometen los principiantes en HTML y CSS, y aprender buenas prácticas para escribir código limpio y profesional desde el principio.

---

## Introducción

Aprender a programar es como aprender un nuevo idioma: al principio es normal cometer errores gramaticales. En el desarrollo web, un pequeño error de escritura puede hacer que tu página se vea rota o que un estilo no se aplique.

En esta lección final, repasaremos qué **NO** hacer y qué hábitos deberías adoptar para convertirte en un mejor desarrollador.

> 🐛 **Dato:** En programación, a los errores se les llama "bugs" (bichos). ¡Encontrar y arreglar estos bugs es parte del trabajo diario!

---

## 1. Errores Comunes en HTML

### Olvidar cerrar las etiquetas
Es el error número uno. Si abres un `<p>` o un `<div>`, ¡asegúrate de cerrarlo! Si no lo haces, el navegador puede confundirse y desordenar todo el diseño.

* ❌ **Mal:** `<strong>Texto en negrita`
* ✅ **Bien:** `<strong>Texto en negrita</strong>`

### Anidamiento incorrecto
Las etiquetas deben cerrarse en el orden inverso al que se abrieron (como muñecas rusas).

* ❌ **Mal:** `<p>Este texto es <strong>importante</p></strong>`
* ✅ **Bien:** `<p>Este texto es <strong>importante</strong></p>`

### Nombres de archivos con espacios
Nunca uses espacios, tildes o ñ en los nombres de tus archivos o carpetas. Los servidores web pueden tener problemas para leerlos.

* ❌ **Mal:** `mi pagina de perfil.html` / `foto de mis vacaciones.jpg`
* ✅ **Bien:** `mi-pagina-perfil.html` / `foto-vacaciones.jpg`

---

## 2. Errores Comunes en CSS

### Olvidar el punto y coma (`;`)
En CSS, cada propiedad debe terminar con un punto y coma. Si te olvidas de uno, **ninguna de las propiedades que escribas después funcionará**.

```css
/* ❌ Mal: Falta el punto y coma en color */
h1 {
  color: red
  font-size: 20px; /* Esto no funcionará */
}

/* ✅ Bien */
h1 {
  color: red;
  font-size: 20px;
}
````

### Olvidar las unidades de medida

A diferencia de otros programas de diseño, en CSS el número `20` no significa nada por sí solo. Debes especificar si son píxeles (`px`), porcentaje (`%`), etc.

* ❌ **Mal:** `width: 100;`
* ✅ **Bien:** `width: 100px;`

### Confundir Clases (.) con IDs (\#)

Recuerda:

* Usa **clases** (`.boton`) cuando quieras aplicar el estilo a **varios** elementos.
* Usa **IDs** (`#header`) cuando el elemento sea **único** en la página.

-----

## 3\. Buenas Prácticas (Recomendaciones)

### Mantén tu código ordenado (Indentación)

Usa la tecla `Tab` para crear sangrías. Esto hace que sea fácil ver qué etiqueta está dentro de cuál.

**Difícil de leer:**

```html
<div><p>Hola</p><ul><li>Item</li></ul></div>
```

**Fácil de leer:**

```html
<div>
  <p>Hola</p>
  <ul>
    <li>Item</li>
  </ul>
</div>
```

### Usa comentarios

Tanto en HTML como en CSS, puedes dejar notas para ti mismo o para otros.

* HTML: \`\`
* CSS: `/* Estilos para la tarjeta de perfil */`

### Organiza tus archivos

A medida que tengas más archivos, no los tires todos en la misma carpeta. Crea una estructura lógica:

```text
/mi-proyecto
  index.html
  /css
    estilos.css
  /img
    foto.jpg
    logo.png
```

-----

## Conclusión del Curso

¡Felicidades\! Has completado los fundamentos del desarrollo web.

Has aprendido:

1.  Qué es la web y cómo funciona.
2.  A estructurar contenido con **HTML**.
3.  A dar estilo y diseño con **CSS**.
4.  A crear una página desde cero.

**¿Cuál es el siguiente paso?**
La mejor forma de aprender es practicando. Intenta crear una página sobre tu mascota, tu película favorita o tu currículum vitae. ¡El límite es tu imaginación\!