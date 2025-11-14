
# Lección 6: Creación de una Página Web Básica

**Objetivo:** Combinar los conocimientos de HTML (estructura, elementos) y CSS (estilos simples) para construir una página web completa y funcional.

---

## Introducción

¡Es el momento de construir! En las lecciones anteriores, aprendimos a crear la estructura de una página con HTML y a darle estilos básicos con CSS. Ahora, uniremos todo eso para crear nuestra primera página web completa.

Vamos a simular la creación de una "Página de Perfil". Este proyecto simple es perfecto para practicar cómo interactúan HTML y CSS.

---

## Plan del Proyecto: Página de Perfil

Nuestra página de perfil tendrá los siguientes componentes:

1.  Un contenedor principal (una "tarjeta").
2.  Un título principal (p. ej., "Mi Perfil").
3.  Un párrafo con una breve biografía.
4.  Una lista de pasatiempos.
5.  Un enlace a una red social.

---

## Paso 1: La Estructura (index.html)

Primero, creamos el archivo `index.html`. Fíjate bien en cómo usamos `<div>` para agrupar nuestro contenido en una "tarjeta" y cómo enlazamos nuestra hoja de estilos.

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
    
    <a href="[https://www.github.com](https://www.github.com)" target="_blank">
      Visita mi GitHub
    </a>
    
  </div> </body>
</html>
````

-----

## Paso 2: El Estilo (estilos.css)

Ahora, aplicamos estilos. Usaremos la clase `.tarjeta-perfil` para darle forma al contenedor.

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
  
  /* (Extra) Añadimos espacio interno */
  padding: 20px;
  
  /* (Extra) Centramos el texto */
  text-align: center;
}

/* Estilo para el título principal */
h1 {
  color: #333;
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

Si abres tu archivo `index.html` en un navegador, ahora deberías ver una página de perfil completa, centrada y con un diseño limpio, sin necesidad de imágenes.

Has combinado con éxito:

* La **estructura** HTML.
* **Elementos comunes** de texto y listas.
* **Selectores** CSS.
* **Estilos simples** de color, bordes y centrado.

<!-- end list -->

