# Lección 6: Creación de una Página Web Básica

**Objetivo:** Combinar los conocimientos de HTML (estructura, elementos) y CSS (estilos simples) para construir una página web completa y funcional, como una página de perfil personal.

---

## Introducción

¡Es el momento de construir! En las lecciones anteriores, aprendimos a crear la estructura de una página con HTML y a darle estilos básicos con CSS. Ahora, uniremos todo eso para crear nuestra primera página web completa.

Vamos a simular la creación de una "Página de Perfil". Este proyecto simple es perfecto para practicar cómo interactúan HTML y CSS.

> 🏠 Si las lecciones anteriores fueron aprender a hacer ladrillos (HTML) y a pintar (CSS), esta lección es construir tu primera "casa" de un solo cuarto.

---

## Plan del Proyecto: Página de Perfil

Nuestra página de perfil tendrá los siguientes componentes:

1.  Un contenedor principal (una "tarjeta").
2.  Un título principal (p. ej., "Mi Perfil").
3.  Una foto de perfil.
4.  Un párrafo con una breve biografía.
5.  Una lista de pasatiempos.
6.  Un enlace a una red social.

Crearemos dos archivos: `index.html` (para la estructura) y `estilos.css` (para el diseño).

---

## Paso 1: La Estructura (index.html)

Primero, creamos el archivo `index.html`. Fíjate bien en cómo usamos `<div>` para agrupar nuestro contenido en una "tarjeta" y cómo enlazamos nuestra hoja de estilos en el `<head>`.

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mi Página de Perfil</title>
  
  <link rel="stylesheet" href="estilos.css">
  
</head>
<body>

  <div class="tarjeta-perfil">
  
    <h1>Mi Perfil</h1>
    
    <img src="[https://via.placeholder.com/150](https://via.placeholder.com/150)" alt="Foto de perfil">
    
    <h2>Juan Pérez</h2>
    
    <p>
      ¡Hola! Soy un estudiante de desarrollo web aprendiendo
      HTML y CSS. Me apasiona la tecnología y crear cosas nuevas.
    </p>
    
    <h3>Mis Pasatiempos</h3>
    <ul>
      <li>Aprender a programar</li>
      <li>Ver series</li>
      <li>Jugar videojuegos</li>
    </ul>
    
    <a href="httpsPOST://[www.github.com](https://www.github.com)" target="_blank">
      Visita mi GitHub
    </a>
    
  </div> </body>
</html>
````

> **Dato:** Estamos usando una imagen de marcador de posición (`https://via.placeholder.com/150`). ¡Puedes cambiar la URL `src` por un enlace a tu propia foto\!

-----

## Paso 2: El Estilo (estilos.css)

Ahora, creemos el archivo `estilos.css` en la misma carpeta. Aquí es donde aplicamos todo lo que aprendimos en la Lección 5.

Usaremos la clase `.tarjeta-perfil` que definimos en nuestro HTML para darle estilo al contenedor principal.

```css
/* Estilos generales para toda la página */
body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4; /* Un fondo gris claro */
  margin: 20px;
}

/* El contenedor principal de nuestro perfil */
.tarjeta-perfil {
  /* 1. Definimos un ancho */
  width: 500px;
  
  /* 2. Centramos la tarjeta en la página */
  margin: 0 auto;
  
  /* 3. Añadimos color de fondo y borde */
  background-color: #ffffff; /* Fondo blanco */
  border: 1px solid #ccc; /* Borde gris */
  
  /* (Extra) Añadimos una sombra para que "flote" */
  box-shadow: 2px 2px 5px rgba(0,0,0,0.1);
  
  /* (Extra) Añadimos espacio interno */
  padding: 20px;
}

/* Estilo para el título principal */
h1 {
  color: #333;
  text-align: center; /* Centramos el texto */
}

/* Estilo para la imagen */
img {
  /* (Truco) Las imágenes son "en línea", para centrarlas
     las convertimos en "bloque" y usamos el truco del margen */
  display: block;
  margin: 0 auto;
  
  /* (Extra) Hacemos la imagen redonda */
  border-radius: 50%;
}

/* Estilo para el enlace */
a {
  color: #007BFF;
  text-decoration: none; /* Quitamos el subrayado */
}

/* (Extra) Cambia el color del enlace al pasar el mouse */
a:hover {
  color: #0056b3;
  text-decoration: underline; /* Lo volvemos a poner */
}
```

-----

## ¡Tu Primera Página\!

Si abres tu archivo `index.html` en un navegador, ahora deberías ver una página de perfil completa, centrada y con un diseño limpio.

Has combinado con éxito:

* La **estructura** HTML (Lección 2)
* **Elementos comunes** como `h1`, `p`, `img`, `ul`, `a` (Lección 3)
* **Selectores** CSS (Lección 4)
* **Estilos simples** de color, bordes y centrado (Lección 5)

¡Felicidades\! Acabas de crear tu primera página web estática.

-----

### Desafío: Página de Blog

¿Cómo adaptarías esto para una "entrada de blog"?

* El `<h1>` sería el **título del artículo**.
* El `<h2>` podría ser el **autor** o la **fecha**.
* Los `<p>` serían los **párrafos del blog**.
* Podrías tener una `<img>` principal al inicio del artículo.

La estructura es la misma, ¡solo cambia el contenido\!

