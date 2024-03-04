# Introducción a CSS
## Profesor: Lic. Juan José González Ramírez
### Email: juanftp100.edu@gmail.com
### Github: 
- [Repositorio del profe - docencia](https://github.com/gallopeladoprofe)
- [Repositorio del profe - personal](https://github.com/gallopelado)

Aviso: Este documento está en constante actualización, favor dirigirse al email en caso de encontrar errores. Muchas gracias :sunglasses: :stuck_out_tongue_closed_eyes: :heartbeat:. La mayoría de los ejemplos pertenecen a [CSS Tutorial](https://www.w3schools.com/css/default.asp) del inglés.

### ¿Qué es CSS?
CSS es el lenguaje que usamos para estilizar un documento HTML.
CSS describe como los elementos HTML deberían ser mostrados.
Este tutorial va ir de lo básico de CSS a lo avanzado.

#### Ejemplos en cada capítulo
Este tutorial contiene miles de ejemplos de CSS.
En nuestro caso es conveniente crearse un repositorio en Github para ir versionando los avances.

```CSS
body {
  background-color: lightblue; /* cambia de color el fondo del body*/
}

h1 {
  color: white; /* cambia de color de fuente a blanco */
  text-align: center; /* alinea el texto al centro */
}

p {
  font-family: verdana; /* cambia el tipo de fuente del párrafo */
  font-size: 20px; /* cambia el tamaño de la fuente a 20px */
}
```
Ahora veamos el HTML:
```html
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: lightblue;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: verdana;
  font-size: 20px;
}
</style>
</head>
<body>

<h1>My First CSS Example</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

#### Introducción
- CSS es un acrónimo que significa Hoja de estilos cascada (Cascading Style Sheets)
- CSS describe como los elementos HTML son mostrados sobre la pantalla, papel u otro dispositivo multimedia.
- CSS ahorra trabajo. Puede controlar la disposición(*layout*) de múltiples páginas web de una vez.
- Hojas de estilo externas son almacenadas en archivos CSS.

Veamos un ejemplo en línea de [CSS Demo - One HTML Page - Multiple Styles!](https://www.w3schools.com/css/css_intro.asp).

#### ¿Por qué usamos CSS?
CSS se usa para definir estilos para tus páginas web, incluido el diseño, la disposición y variaciones en pantall para diferentes dispositivos y tamaños de pantalla.

#### CSS solucionó un gran problema
HTML nunca tuvo la intención de contener etiquetas para formatear páginas web.
HTML fue creado para describir contenido de una página web, como:
```html
<h1>This is a heading</h1>

<p>This is a paragraph.</p>
```
Cuando las etiquetas como `<font>`, y atributos de color fueron agregadas a la especificación HTML 3.2, empezó la pesadilla para los desarrolladores web.
Desarrollar grandes sitios, donde la fuente y la información de color debían de ser agregadas en cada página, se convirtió en un largo y costoso proceso.

Para solucionar este problema, el consorcio World Wide Web creó CSS.

CSS removió el formateo desde las páginas HTML.

#### CSS ahorra trabajo
La definición de estilos se realizan normalmente en archivos externos con extensión **.css**.
Con un archivo de CSS extenro, puedes cambiar la apariencia de un sitio web modificando en un solo archivo.

#### Sintaxis CSS
Una regla CSS consiste en un selector y una declaración de bloque.
![css syntax](./img/css_syntax.png)

El *selector* marca cual es el elemento HTML al cual quieres darle estilo.
El bloque *declaration* contiene una o más declaraciones separadas por el signo `;`.
Cada declaración de CSS está separada por punto y coma, y los bloques están rodeados de llaves.

Ejemplo:
```css
p {
  color: red;
  text-align: center;
}
```

Ejemplo explicado:
- `p` es un selector en CSS que apunta la etiqueta `<p>` de HTML.
- `color` es una propiedad y `red` es el valor de la propiedad.
- `text-align` es una propiedad y `center` es el valor de la propiedad.

### Selectores en CSS
Un selector en CSS selecciona un(o varios) elemento(os) HTML que quieres darle estilo.

Los selectores son usados para "encontrar" o seleccionar elementos HTML para darles estilo.

Podemos dividirlos en cinco categorías:
- Selectores simples (seleccionar elementos basados en nombre, id, clase).
- Combinator selectors (seleccionan elementos basados en una específica relación entre ellos).
- Pseudo-class selectors (seleccionan elementos basados en un cierto estado).
- Pseudo-elements selectors (seleccionar estilo de una parte de un elemento).
- Attribute selectors (seleccionan elementos basados en un atributo o valor de atributo).

Ejemplo:

Todas las etiquetas `<p>` serán alineadas al centro , y el color de texto será rojo.
```css
p {
  text-align: center;
  color: red;
}
```

#### El selector de id
El selector de id usa el atributo id de un elemento HTML para seleccionarlos.
El id es un elemento único en una página, entonces el id selector es usado para seleccionar un único elemento.
Para seleccionar un elemento que usa id, hay que usar el signo `#` seguido del nombre del id del elemento:

La regla CSS abajo va aplicarse para aquel elemento HTML que tenga el *id="para1"*:
```css
<!DOCTYPE html>
<html>
<head>
<style>
    #para1 {
        text-align: center;
        color: red;
    }
</style>
</head>
<body>

<p id="para1">Hello World!</p>
<p>This paragraph is not affected by the style.</p>

</body>
</html>
```

#### El selector de clase
El selector de clase selecciona un elemento HTML con una clase específica.
Para seleccionar elementos, se utiliza el punto `.` seguido del nombre de la clase.

Ejemplo:
```css
<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<h1 class="center">Red and center-aligned heading</h1>
<p class="center">Red and center-aligned paragraph.</p> 

</body>
</html>

```

También se puede especificar solamente el elemento que tenga esa clase:
```css
p.center {
  text-align: center;
  color: red;
}
```

#### El selector universal
El selector universal es el asterisco (`*`), selecciona todos los elementos de la página:
```css
* {
  text-align: center;
  color: blue;
}
```

#### El selector de grupo
El selector de grupo selecciona todos los elementos HTML con la misma definición de estilo.
Mira el siguiente bloque, h1, h2 y p tienen la misma definición:
```css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

Sería mejor agrupar los selectores, para minimzar el código, ejemplo:
```css
h1, h2, p {
  text-align: center;
  color: red;
}
```

#### Ejercicios de CSS Selectors:
1. Asigna el color de texto rojo, para todos los elementos `<p>`.
2. Asigna el color de texto rojo, para el elemento que tenga un id="para1".
3. Asigna el color de texto rojo, para los elementos con `class="colortext"`.
4. Asigna el color de texto rojo, para todos las etiquetas `<p>` y `<h1>`. Utiliza la agrupación para minimizar código.

#### Todos los selectores simples
| Selector | Ejemplo | Descripción |
|----------|---------|-------------|
| `#id` | #primernombre | Selecciona el elemento con el *id="primernombre"* |
| `.class` | .intro | Selecciona todos los elementos con la clase *class="intro"* |
| `elemento.class` | p.intro | Selecciona solamente `<p>` con la clase *class="intro"* |
| `*` | * | Selecciona todos los elementos |
| `elemento` | p | Selecciona todos los elementos `<p>` |
| `elemento, elemento2,..` | div, p | Selecciona todos los `<div>` y todos los `<p>` |

### Como agregar CSS
Cuando un navegador lee una hoja de estilo, este va a formatear el documento HTML de acuerdo con la información en la hoja de estilos.

#### Hay tres formas de usar CSS
- CSS externo
- CSS interno
- CSS en línea

#### CSS externo
Con una hoja de estilos externa, puedes cambiar la apariencia completa de un website en un solo archivo.
Cada página HTML debe incluir una referencia a la hoja de estilos usando la etiqueta `<link>` en el head.

Ejemplo:
```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="mystyle.css">
  </head>
  <body>

    <h1>Esto es un título grande</h1>
    <p>Un párrafo.</p>

  </body>
</html>
```
[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_howto_external)

Una hoja de estilos externa puede ser escrita con cualquier editor de texto, debe ser guardada con la extensión **.css**.
El fichero **.css** no debería contener ninguna etiqueta HTML.

Ejemplo:
```css
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```
---
**Atención:** No agregar espacios en medio de la propiedad (20) y la unidad (px):
Incorrecto(espacio): `margin-left: 20 px;`
Correcto(espacio): `margin-left: 20px;`
---

#### CSS interno
También puede usarse CSS en un documento HTML.
El css interno se define dentro de la etiqueta `<style></style>` del head.

Ejemplo:
```html
<!DOCTYPE html>
<html>
  <head>
  <style>
    body {
      background-color: linen;
    }

    h1 {
      color: maroon;
      margin-left: 40px;
    }
  </style>
  </head>
  <body>

	<h1>This is a heading</h1>
	<p>This is a paragraph.</p>

  </body>
</html>
```
[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_howto_internal)


#### CSS en línea
El estilo *inline* podría ser aplicado a un elemento.
Para usar el estilo inline, se debe agregar el atributo `style` a un elemento. Este atributo puede contener propiedades CSS.

Ejemplo:
```html
<!DOCTYPE html>
<html>
	<body>

		<h1 style="color:blue;text-align:center;">This is a heading</h1>
		<p style="color:red;">This is a paragraph.</p>

	</body>
</html>
```
[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_howto_inline)

#### Hojas de estilo múltiple
Si algunas propiedades fueron definidas para el mismo selector (elemento) en diferentes hojas de estilo, el valor de la última hoja de estilo leída será usado.

Asumimos que una **hoja de estilos externa** está siendo aplicada al elemento `<h1>`:
```css
h1 {
  color: navy;
}
```

Luego, asumimos que hay **estilos internos** que también modifican al elemento `<h1>`:
```css
h1 {
  color: orange;
}
```

Si el estilo interno es definido **después** de un link externo, el <h1> será orange:
```html
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
	h1 {
	color: orange;
	}
</style>
</head>
```
#### Orden en cascada
¿Cuál será el estilo a usarse cuando hay más de uno en el documento HTML?

Todoslos estilos en una página será interpretados en un nuevo estilo virtual de reglas, donde el número uno tiene la mayor prioridad de todas:
1. Estilo en línea(inline dentro del elemento HTML)
2. Hojas de estilos interna y externa (en la sección del head)
3. Por defecto del navegador

Entonces, un estilo inline tiene la mayor prioridad, y va a sobreescribir estilos internos y externos como también lo que el navegador maneja por defecto.

[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_howto_cascade)

Ejercicio:
Agregar un estilo externo con la URL: "mystyle.css".
```html
<head>

</head>

<body>
  <h1>This is a heading</h1>
  <p>This is a paragraph</p>
  <p>This is a paragraph</p>
</body>
```

### Comentarios en CSS
Los comentarios en CSS no son mostrados en el navegador, pero ellos pueden ayudar a documentar el código fuente.

Los comentarios son usados para explicar código, también para editar.

Los comentarios son ignorados por el navegador.

Un comentario puede ser escrito dentro de las etiquetas `<style>`, empieza con `/*` y termina con `*/`:

Ejemplo:
```css
/* This is a single-line comment */
p {
  color: red;
}
```
[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_comments)

Puedes agregar comentarios donde quieras en el código:
```css
p {
  color: red;  /* Set text color to red */
}
```
[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_comments2)

Incluso en medio del código:
```css
p {
  color: /*red*/blue; 
}
```
[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_comments2_2)

También pueden ocupar múltiples líneas:
```css
/* This is
a multi-line
comment */

p {
  color: red;
}
```
[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_comments3)

#### Comentarios CSS y HTML
Ya sabes que en HTML, los comentarios son `<!--...-->`.

En el ejemplo de HTML:
```html
<!DOCTYPE html>
<html>
	<head>
	<style>
		p {
			color: red; /* Set text color to red */
		}
	</style>
	</head>
	<body>

		<h2>My Heading</h2>

		<!-- These paragraphs will be red -->
		<p>Hello World!</p>
		<p>This paragraph is styled with CSS.</p>
		<p>CSS comments are not shown in the output.</p>

	</body>
</html>
```
[¡Prueba en línea!](https://www.w3schools.com/css/tryit.asp?filename=trycss_comments4)