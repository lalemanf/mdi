# 1.Introducción al HTML y CSS

## Qué es HTML

- Es un lenguaje de programación basado en etiquetas
- Se utiliza para elaborar páginas web
- El contenido se pone entre etiquetas como:
    * h1~h6 (para títulos)
    * p (para párrafos)
    * b o strong (para texto en negrita)
    * i (para texto en cursiva)
    * u (para texto subrayado)
    * a (para poner un enlace a otro sitio o página web)
    * blockquote (para citar texto entre comillas)
    * img (para poner una imagen)
    * table (para crear una tabla)
    * ul (para crear una lista de elementos)
    * ol (para crear una lista de elementos con número)

## Ejemplo de código

```html
<h1>Bienvenid@s a mi página web</h1>

<p>Ésto es un párrafo donde meto el <b>texto</b> que <i>yo quiera</i> mostrar en la página</p>

<p>Pero <b><i>¿qué es HTML?</i></b></p>

<blockquote>HTML, siglas en inglés de 
    <a href="https://es.wikipedia.org/wiki/HTML">HyperText Markup Language</a> (‘lenguaje de marcado de hipertexto’), hace referencia al lenguaje de marcado para la elaboración de páginas web.</blockquote>
```
<div style="border: solid 1px; padding: 10px;margin: 20px 0;">
    <h1 style="border: 0;">Bienvenid@s a mi página web</h1>
    <p>Ésto es un párrafo donde meto el <b>texto</b> que <i>yo quiera</i> mostrar en la página</p>
    <p>Pero <b><i>¿qué es HTML?</i></b></p>
    <blockquote>HTML, siglas en inglés de <a href="https://es.wikipedia.org/wiki/HTML" target="_blank">HyperText Markup Language</a> (‘lenguaje de marcado de hipertexto’), hace referencia al lenguaje de marcado para la elaboración de páginas web.</blockquote>
</div>

<div style="display:block;page-break-before:always;"></div>

# Qué es CSS

- Un lenguaje de diseño gráfico para dar formato a los documentos HTML
- Cascading Style Sheets (Hojas de Estilo en Cascada)
- Básico y muy usado en páginas web
- Puede venir declarado de 3 formas distintas:
    * dentro del atributo style de cualquier etiqueta HTML ```<h1 style="color: blue;">Título de color azul</h1>```
    * entre ```<style></style>``` dentro del documento HTML
    * en un archivo aparte que vinculamos dentro de ```<head></head>``` de esta manera ```<link rel="stylesheet" href="estilo.css">```

## Estructura del código CSS

El código CSS está formado por un conjunto de **selectores** que dentro tienen **propiedades** declarativas para establecer el formato a nuestro documento HTML.

Existen 3 tipos de selectores:
- Selector de etiqueta => Utiliza el mismo nombre que la etiqueta HTML

```css
h1 {
    color: red;
    font-size: 34px;
    margin: 10px 5px 10px 5px;
}
```

- Selector de identificador => Utiliza el atributo *id* dentro de una etiqueta html, como por ejemplo ```<h1 id="titulo">Hola Mundo</h1>```:

```css
#titulo {
    color: red;
    font-size: 34px;
    margin: 10px 5px 10px 5px;
}
```
- Selector de clase o *class* => Utiliza el atributo class dentro de una etiqueta html, como por ejemplo ```<h1 class="mi-titulo">¡Hola Mundo!</h1>```:

```css
.mi-titulo {
    color: red;
    font-size: 34px;
    margin: 10px 5px 10px 5px;
}
```

## Propiedades CSS más usadas

- **color** => Establece el color del texto y sus valores pueden ir en nombre de color en inglés (red, blue, green, yellow, aquamarine...) o en hexadecimal #66ccff

- **font-size** => Establece el tamaño del texto en píxeles (12px)
- **margin** => Define un espacio alrededor de un elemento de bloque representado en píxeles por 4 valores (arriba derecha abajo izquierda)
- **background-color** => Pone un color de fondo, ya sea en inglés o en hexadecimal.
- **font-family** => Define el tipo de letra que se va a utilizar (verdana, arial, helvetica, san-serif...)
- **border** => Pintamos un borde alrededor del elemento diciéndole qué grosor en píxeles y de qué color lo queremos (en inglés o hexadecimal)

> Para más información acerca de las propiedades CSS más usadas podéis visitar <a href="https://www.eniun.com/resumen-tabla-propiedades-css-valores/" target="_blank">esta lista</a> con ejemplos de código.

<div style="display:block;page-break-before:always;"></div>

# Actividades

101. Descárgate el archivo "plantilla.html" y crea una página web con el texto que tú quieras pero utilizando las 7 primeras etiquetas que hemos visto, es decir:

    h1~h6 (para títulos)
    p (para párrafos)
    b o strong (para texto en negrita)
    i (para texto en cursiva)
    u (para texto subrayado)
    a (para poner un enlace a otro sitio o página web)
    blockquote (para citar texto entre comillas)

> Guarda este archivo como **101plantillaHTML.html**

102. Una vez creado el archivo **101plantillaHTML.html** agrégale estilo CSS utilizando las propiedades que hemos visto en los apuntes añadiendo el atributo *style* a los elementos que tú quieras pero usando, al menos 1 vez, todas estas propiedades de CSS:

    color (para cambiarle el color al texto)
    font-size (para cambiar el tamaño del texto)
    background-color (para cambiar el color de fondo a la etiqueta body)
    border (para añadir borde)

Un ejemplo sería

```html
<p style="color: blue; border: solid 2px black">Esto es un texto de color azul con un borde de 2 píxeles y de color negro</p>
``` 

> Guarda este archivo como **102plantillaHTMLconCSS.html**