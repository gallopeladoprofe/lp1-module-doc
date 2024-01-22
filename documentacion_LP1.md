# Borrador LP1

## Capítulo 1 - Javascript
Javascript es un lenguaje de programación que puede ser utilizado tanto en el cliente como en el servidor para aplicaciones. Del lado del servidor está la lógica del *backend* que usualmente corren en computadoras de algún datacenter e interactúa con la base de datos, mientras que el lado del cliente es cuando se está usando algún dispositivo del usuario, a menudo el navegador.

De seguro habrás utilizado alguna funcionalidad escrita en Javascript. Si usaste un navegador web, como Chrome, Firefox, Safari, o Edge, entonces definitivamente lo utilizaste. Javascript está por toda la web. Si hiciste enter a una página web y esta te pregunto por las cookies e hiciste clik para aceptarlas, el popup desapareció. Esto es Javascript funcionando. Y si quiere navegar un sitio web y un sub-menu se abre, eso significa también Javascript. A menudo, cuando filtras productos en un sitio web de compras, esto significa Javascript. ¿Y que hay acerca de los chats que inicias conversando despues de haber permanecido una cierta cantidad de tiempo en un sitio web? Bueno, adivinaste, ¡es Javascript!

Tenemos muchísimas interacciones en un sitio web gracias a Javascript; los botones que estás haciendo click, tarjetas de cumpleaños que estás creando, cosas que estás calculando. Cualquier cosa que requiera mas que un sitio web estático necesita Javascript.

En este capítulo vamos a ver los siguientes temas:
- ¿Por qué debería aprender Javascript?
- Configurar mi entorno de trabajo
- ¿Cómo el navegador entiende Javascript?
- Usando la consola del navegador
- Agregando Javascript a una página web
- Escribiendo código de Javascript

### ¿Por qué debería aprender Javascript?
Hay muchas razones para aprender Javascript. Javascript se originó en 1995, y es considerado un el más ampliamente utilizado. Esto es porque Javascript es el lenguaje que soportan y entienden los navegadores web. Tienes todo lo que necesitas en tu navegador web para interpretar código y un editor de texto.

Es un gran lenguaje para los nuevos en el ambiente, y para los más avanzados desarrolladores que por lo menos sabe algo de Javascript porque en algún momento lo utlizaron. Javascript es una gran decisión para los novatos por muchas razones. La primera es que puedes empezar construyendo bonitas aplicaciones utilizando Javascript más rápido de lo que imaginas. Cuando lleguemos al *capítulo de los loops*, serás capaz de escribir complejos script que interactúan con usuarios. Al final serás capaz de escribir páginas web dinámicas que hacen un montón de cosas.

Javascript puede ser utilizado para escribir diferentes tipos de aplicaciones y scripts. Puede ser utilizado para la programación del navegador web, pero también la capa de lógica que no vemos (como la conexión a la base de datos) de una aplicación puede ser programadam, a traves de juegos, scripts de automatización, y para otros propósitos. Javascript puede ser utilizado con diferentes estilos de programación, el cual quiere decir diferentes formas para estructurar y escribir código. Si nunca escribiste código antes puede que no del todo sea enteramente necesario para este nivel, utilizar la programación (semi) orientado-objeto, funcional, y procedimental, ellos son nada más que diferentes paradigmas de programación.

Hay una tonelada de bibliotecas y frameworks que puedes utilizar una vez que aprendes lo básico de Javascript. Estas bibliotecas y frameworks realmente mejorarán el tiempo de vida de tu software y harán un montón de cosas más fácil y también terminar más con menos tiempo. Ejemplos de estas grandiosas bibliotecas y frameworks son React, Vue.js, jQuery, Angular, y Node.js. No te preocupes de ellas de momento.

Finalmente, mencionaremos la comunidad de Javascript. Javascript es un lenguaje de programación muy popular y mucha gente lo usa. Para alguien que está iniciando no debería de haber ningún problema para quien no pueda encontrar alguna solución en internet.

La comunidad de Javascript es enorme. Los foros de Stack OverFlow contienen un montón de ayuda de todo tipo, también solución a errores. Encontrarás en esa web muchísimas soluciones a problemas comunes y sus trucos.

Si Javascript es tu primer lenguaje de programación, eres nuevo en toda la comunidad, sigue intentando y aprendiendo, pronto entenderás los suficiente.

### Configurar mi entorno de trabajo
Hay muchas manera para configurar tu entorno de trabajo para codificar. Para los nuevos, tu computadora probablemente ya tiene toda las mínimas cosas que necesitarás para codificar Javascript. Recomendamos hacer tu vida más fácil y usar un IDE.

### IDE
Un **Integrated Development Enviroment**(Entorno integrado de desarrollo) es una aplicación especial que es usada para escribir, correr, y hacer debug del código. Tu tan solo pueder abrirlo como cualquier programa. Por ejemplo, para escribir un documento, necesitas abir un programa, seleccionar el archivo correcto, y empezar a escribir. Codificar es similar. Abres el IDE y escribes el código. Si quieres ejecutar código, el IDE a menudo tiene botones especiales para esto. Presionando este botón iniciará el programa dentro del IDE. Para Javascript, podrías encontrarte abriendo el navegador manualmente en ciertos casos sin embargo.

Un IDE hace más cosas sin embargo; *como coloreado y resalte de sintaxis*. Esto significa que ciertos elementos en tu código tendrán cierto color, y puedes verlo fácilmente cuando algo está mal. Otra gran característica es la *autosugerencia*, donde el editor te ayuda con opciones en el lugar donde estás escribiendo código. Esto a menudo es llamado *autocompletado*. Muchos IDEs tienen plugins y otras herramientas especiales que hacen más intuitivo y agradable el trabajo, por ejemplo el **hot reload in the browser**(recarga el navegador en caliente cuando hacemos cambios).

Hay muchos IDEs por ahí y ellos se diferencian en las cosas que tienen para ofrecer. **Utilizaremos [Visual Studio Code](https://code.visualstudio.com/)** para este módulo, pero eso es una preferencia personal. Otros populares también son Atom, Sublime Text, y WebStorm.

Hay muchos IDEs en la Internet pero debes escoger aquellos que soporten la sintaxis Javascript.

### Navegador(Web browser)
También necesitarás un navegador, todos menos Internet Explorer.

### ¿Cómo el navegador entiende Javascript?
*Javascript* es un lenguaje **interpretado**, esto significa que la computadora entiende mientras está ejecutando. Algunos lenguajes pueden ser procesados antes de la ejecución, esto es llamado **compilación**, pero no Javascript. La computadora solamente puede interpretar Javascript al vuelo(en el momento). El "motor(engine)" que entiende Javascript será llamado intérprete.

![image](https://hackmd.io/_uploads/B13O3tTIa.png)


**Una página web no es Javascript**. Las páginas webs está escritas en tres lenguajes: HTML, CSS y Javascript.

**HTML** determina que estará en la página; el contenido de la pagina en él. Si hay un párrafo en la página, el HTML de la página contiene un párrafo. Y si es un heading(encabezado), HTML será usando para agrer un heading y así sucesivamente. Aquí un pequeño ejemplo que creará una página web con un texto ```Hello world``` en él:

```HTML
<html>
    <body>
        Hello world!
    </body>
</html>
```

Luego veremos lo que es el *Document Object Model*, vamos a ver primero un curso rápdio en HTML, no te preocupes si nunca viste algo como esto.

**CSS** es la capa de la página web. Por ejemplo, si el color del texto es azul, esto es realizado por CSS. El Font size(tamaño de fuente), font family(tipo o familia de fuente), y la posición en la página son determinados por CSS. Javascript es la pieza final en este rompecabezas, el cual define *qué puede hacer la página y como interactúa con el usuario o el backend*.

Cuando estamos tratando con Javascript, inevitablemente pasarás por un término muy pronto, **ECMAScript**. Esta es una especificación o estandarización del lenguaje Javascript. El actual estándar es **ECMAScript 6**(también referido como **ES6**). Los navegadores usan esta especificación para soportar Javascript (especialmente en algo llamado **Document Object Model(DOM)**. Javascript tiene muchas implementaciones que podrían diferir ligeramente, pero el ECMAScrip puede ser considerado la especificación básica que lo incluye.

### Usando la consola del navegador
De seguro habrás visto esto antes, o no, pero los navegadores tienen una función incluida. Si pulsas la tecla *F12* sobre una ventana de Windows mientras estás en un navegador, o clic derecho y **Inspeccionar**, se visualizará, algo similar a esto.

Luce así;
![image](https://hackmd.io/_uploads/ByUvMqp8T.png)

Este screenshot contiene múltiples pestañas en la parte de arriba. Ahora estamos mirando la pestaña "element", el cual contiene todo el HTML y CSS (¿recuerdas estos?). Si haces click sobre la pestaña "console", encontrarás al final del panel un lugar para escribir código algo de código directamente. Se podría ver algunas advertencias o mensajes de error en esta pestaña. Esto no es común, y no te preocupes si la página está funcionando.

La consola es usada por los desarrolladores para registrar que está ocurriendo y hacer algo de debug.
Debugging es encontrar el problema cunaod una aplicación no está mostrando el comportamiento deseado. La consola muestra algunas pistas acerca de lo que está ocurriendo y si registrar mensajes sensibles. Esto es de hecho el comando que ahora vamos aprender:

```javascript
console.log("Hello world!");
```

Si haces clic en esta consola, ingresa primero el código de Javascript abajo y luego aprieta *Enter*, esto mostrará una salida de tu código allí dentro. Debería mosrtar algo parecido a lo siguiente:

![image](https://hackmd.io/_uploads/rktgvAAUT.png)

Tú estarías trabajando con la sentencia `console.log()` muchas veces a través del módulo para testear tu código y ver los resultados. También hay otros métodos, como `console.table()`, que crea una tabla cuando es ingresado datos que pueden ser mostrados como tabla. Otro comando es `console.error()`, el cual registra los dtos ingresados, pero con un estilo que muestra advertencia por el hecho de que es un error.

#### Ejercicio 1.1
Trabajando con la consola:
1. Ingresa a la consola del navegador, escribe `4 + 10`, presiona *Enter*. ¿Qué respuesta puedes ver?
2. Utiliza `console.log()`, poniendo un valor dentro del paréntesis. Intenta ingresar tu nombre con comillas (esto de hecho indica que es un texto string).

### Agregando Javascript a una página web
Hay dos formas de enlazar Javascript a una página web. El primer tipo es el de escribir directamente Javascript en el HTML rodeado de dos etiquetas `<script>`. En HTML, la primera etiqueta `<script>`, es para declarar lo que será ejecutado en el script. Luego tenemos el contenido que debería estár dentro de este elemento. Siguiente, cerramos el script con la misma etiqueta, pero precedida de una barra, `</script>`. O puedes enlazar un fichero de Javascript al documento HTML usando la etiqueta script al inicio del head del HTML de la página.

#### Directamente en HTML
Aquí hay un ejemplo de como escribir muy fácil una página web que muestra una ventana emergente(pop-up), diciendo `Hi there!`:

```htmlembedded
<html>
    <script>
        alert("Hi there!");
    </script>
</html>
```

![image](https://hackmd.io/_uploads/HkNEeykw6.png)

![image](https://hackmd.io/_uploads/r1NSgkJwa.png)


El comando `alert` creará una ventana emergente(pop-up) que provee un `mensaje`. Este mensaje está especificado en medio de paréntesis detrás del alert.

Ahora mismo, tenemos el contenido directamente dentro de nuestro las etiquetas `<html>`. Esta no es la mejor práctica. Necesitaremos crear dos elmentos dentro `<html>`, `<head>` y el `<body>`.
En el elemento head, vamos a escribir los metadatos y también utilizaremos esta parte para conectar archivos externos a nuestra HTML. En el body, tenemos el contenido de la página web.

También necesitamos permitir al navegador saber que clase de document estamos trabajando con la declaración `<!DOCTYPE>`. Siempre al inicio del HTML. Ejemplo:

```HTML
<!DOCTYPE html>
<html>

<head>
    <title>Aquí va en la pestaña de tu navegador</title>
</head>

<body>
    El contenido de la página web
    <script>
        console.log("Hi there!");
    </script>
</body>

</html>
```

#### Ejercicio 1.2
Javascript en una página HTML:
1. Inicia el editor de código y crea un archivo HTML.
2. Dentro del archivo, coloca las etiquetas HTML, doctype, HTML, head, y body, luego procede a agregar las etiquetas de script.
3. Coloca algún código de Javascript dentro del script tag. Puedes usar `console.log("¡Hola mundo!")`.

### Enlazando un archivo externo a nuestra página web
También puedes enlazar un archivo a un documento HTML. Esto es considerado una buena práctica, como organiza mejor el código y evitas páginas HTML muy largas, debido a Javascript. Otro de los beneficios es que puede reutilizar el Javascript en otra página web de tu website sin estar copiando y pegando. Decimos que sin tenemos el mismo Javascript en 10 páginas y tu necesitas hacer cambios en el script.
Podrías solamente tener el cambio para un archivo y si lo hiciste de esta manera vamos a mostrarte en este ejemplo:

Primero vamos a crear un archivo de Javascript por separado. Estos archivos deben tener la extensión `.js`.
Lo llamaremos `ch1_alert.js`. Este será el contenido de nuestro archivo:

`alert("Diciendo hola desde un archivo diferente");`

Luego vamos a crear un archivo HTML por separado (usando la extensión `.html` otra vez).
Vamos a poner este contenido:

```HTML
<!DOCTYPE html>
<html>
<body>
    <script type="text/javascript" src="./ch1_alert.js"></script>
</body>
</html>

```

Debes estar seguro de colocar los archivos en la misma ubicación, o sino debes especificar la ruta hacia el archivo de Javascript en tu HTML. Los nombres son *case-sensitive* y deben coincidir exactamente.

Tienes dos opciones. Puedes utilizar una ruta relativa o absoluta. Veamos, tu computadora tiene una *raíz*. Para Linux o MacOS, este es `/`, para Windows, usualmente es `C:/`. La ruta del archivo que inicia desde la raíz es la ruta absoluta. Esta es la forma más fácil de agregar porque funciona en tu computadora. Pero esto tiene trampa: solamente en tu computadora, y si luego este directorio es movido a otro servidor, la ruta absoluta no será valida.

La segunda, y más segura opción es usar rutas relativas. Especificas como obtener el archivo desde el archivo donde estas en ese momento. Y si no estás en el misma carpeta, tendrás solo que insertar el nombre. Si esta no es llamada "ejemplo" que esta dentro de la carpeta donde tu archivo esta, debes especificar `ejemplo/nombreDelArchivo.js`. Y una carpeta, se especifica `../nombreDelArchivo.js`.


![image](https://hackmd.io/_uploads/HJIyjnHwa.png)

![code](https://hackmd.io/_uploads/B1OUo2rPa.png)

Si abres el archivo HTML, esto es lo que se mostrará:

![image](https://hackmd.io/_uploads/rJKc2nBP6.png)

#### Ejercicio 1.3
Enlazando a un archivo de Javascript:
1. Crear un archivo separado llamado `app` con la extensión `.js`.
2. Dentro del archivo`.js`, agrega algo de código de Javascript.
3. Enlaza al `.js` dentro del HTML creado.
4. Abre el HTML dentro de tu navegador y revisa si el código de Javascript se ejecutó apropiadamente.

### Escribiendo código de Javascript
Entonces, ahora que tenemos mucho contexto, ¿cómo es que se escribe código de Javascript?
Hay muchas cosas a tener en mente, tales como formatear el código, usar la sangría, los puntos y comas, y adición de comentarios.

### Formatear código
El código necesita ser bien formateado. Si tienes un archivo muy grande con muchas líneas de código y no apegaste a algunas reglas básicas de formateo, va a ser difíci de entender lo que has escrito. Entonces, ¿qué son las reglas básicas de formateo? Las dos más importantes por ahora son la *sangría y el punto y coma*. También la convención de nombrado.

### Sangría(Indentations) y espacios en blanco (whitespace)
Cuando estás escribiendo código, a menudo una línea de código pertenece a cierto bloque de código(código dentro dos de llaves ´{ como esto }´) o sentencia padre. Si es este caso, das una sangría al c´dogio para estar seguros que se puede ver más fácil que parte es del bloque y cuando un nuevo bloque empieza. No necesitas entender el siguiente código, pero este demuestra la legibilidad con y sin sangría.

Sin nuevas líneas:

```Javascript

let status = "new"; let scared = true; if (status === "new") { console.
log("Bienvenido a Javascript"); if(scared) { console.log("No te preocupes
todo estará bien"); } else { console.log("¡Eres valiente! ¡Lo harás genial!"); } 
} else { console.log("Bienvenido de vuelta, Sé que te gustará"); }

```
 Con nuevas líneas pero sin sangrías:
 
```Javascript
 
let status = "new";
let scared = true;
if (status === "new") { 
console.log("Bienvenido a Javascript"); 
if(scared) { 
console.log("No te preocupes todo estará bien"); 
} else { 
console.log("¡Eres valiente! ¡Lo harás genial!"); 
} 
} else { 
console.log("Bienvenido de vuelta, Sé que te gustará"); 
}
 
```

Con nuevas líneas y sangrías

```Javascript
 
let status = "new";
let scared = true;
if (status === "new") { 
    console.log("Bienvenido a Javascript"); 
    if(scared) { 
        console.log("No te preocupes todo estará bien"); 
    } else { 
        console.log("¡Eres valiente! ¡Lo harás genial!"); 
    } 
} else { 
    console.log("Bienvenido de vuelta, Sé que te gustará"); 
}
 
```

Así como puedes ver, ahora puedes fácilmente distinguir los bloques de código finales. Esto es donde el `if` tiene su correspondiente `}` con el mismo nivel de sangría. En el ejemplo sin sangrías, tendríamos que contar las llaves para determinar cuando el bloque `if` terminaría. Sin embargo esto no es necesario para trabajar código, asegurate de usar la sangría bien. Te lo agradecerás luego.

### Punto y coma (semicolons)
Después de cada sentencia, deberías insertar un punto y coma. Javascript es muy permisivo y entiende muchas situaciones en el cual olvidas una, pero desarrollar es el hábito de agregar una línea después de otra línea. Cuando declaras un bloque de código tal como un `if` o un loop, no debería terminar con un punto y coma. Solamente si son sentencias separadas.

### Comentarios de código
Con los comentarios, puedes decirle al intérprete que ignore algunas líneas del archivo. Ellos no serán ejecutados si son comentados. Esto es a menudo útil para permitir o evitar la ejecución de una parte del código. Esto podría ser una de las siguientes razones:
1. No quieres ejecutar una pieza de código mientras se ejecuta el script, entonces comentas la línea que será ignorada por el intérprete.
2. Metadatos. Agregando un poco de contexto al código, tales como autor, una descripción de qué cubre el archivo.
3. Agregando comentarios para especificar partes del código para explicar que está ocurriendo o porque ciertas opciones fueron hechas.

Hay muchas formas de escribir comentarios. Puedes escribir una *single-line* o un *multi-line* de comentarios. Ejemplo:

```Javascript!

// Soy una single line o comentario de una línea
// console.log("comentario single line, no registrado");

/* Soy una multi-line o comentario de varias líneas. Cualquier cosa que está en medio de la barra
y el asterisco no serán ejecutadas.
console.log("No seré registrado, porque soy un comentario");
*/

```
El precendente fragmento de código, puedes ver ambos estilos de comentarios. El primero es una *single-line*. Esto también es un *inline comment* o comentario de una línea. Cualquier cosas después de `//` en la línea será ignorada. La segunda es la *multiline*; esta es escrita empezando con `/*` y terminando con `*/`.

#### Ejercicio 1.4
Agregando comentarios
1. Agrega una nueva sentencia en tu código de Javascript configurando el valor de una variable. Cubriremos esto en siguientes lecciones, de momento puedes utilizar la siguiente línea: `let a = 10;`
2. Agregar un comentario al final de la sentencia indicando que estás seteando el valor de `10`.
3. Imprime el valor usando `console.log()`. Agrega un comentario explicando que esto hará.
4. Al final de tu código de Javascriptm utiliza un *multi-line comment*. En un script real de producción, podrías usar este espacio para agregar brevemente una reseña.

### Prompt
Otra cosa que nos gustaría mostrar aquí es el promp. Este funciona muy parecido al alert, pero en vez de este, toma valores del usuario. Aprenderemos como guardar variables pronto, y una vez que lo sepamos, podrás guardar el resultado de este prompt y hacer algo con el. Adelántate y cambia el `alert()` por un `prompt()`, por ejemplo:

`prompt("Holis, ¿cómo estas?")`

![code](https://hackmd.io/_uploads/SJzbkVUwa.png)

![code](https://hackmd.io/_uploads/H1LQJN8Pa.png)

![Selección_002](https://hackmd.io/_uploads/S158kN8wp.png)

El valor que se ingresó(cualquier otro valor ingresado) será retornado al script, y puede ser usado en tu código. Esto es genial para obtener entradas del usuario.

### Números randómicos o aleatorios
Para hacer más entretenidos los ejercicios en estas primeras etapas, me gustaría mostrarte como se generan números aleatorios en Javascript. Esta bien si no entiendes bien esta parte y qué está pasando, solamente nos conviene saber que este comando crea un número aleatorio:

`Math.random();`

También se puede hacerlo en la consola y ver el resultado que aparece en la misma:

`console.log(Math.random());`

Este número será decimal entre 0 y 1. Si quisiesemos números entre 0 y 100, podemos multiplicarlo por 100, ejemplo:

`console.log(Math.random() * 100);`

Ejemplo usado en la consola del navegador:

![image](https://hackmd.io/_uploads/Sy9ymVLDT.png)

Y si no queremos que los resultados sean decimales, podemos utilizar el la función `Math.floor` en el, el cual redondeará el valor a un `integer`:

`console.log(Math.floor(Math.random() * 100));`

![image](https://hackmd.io/_uploads/rkw2mN8DT.png)

#### Proyecto 1
#### Creando un archivo HTML y enlazando con un archivo de Javascript
Crear un archivo HTML con su archivo de Javascript por separado. Luego, conecta el archivo de Javascript al archivo de HTML.
1. En el archivo de Javascript, muestrar tu nombre en la consola y agrega un *multi-line* comentario a tu código.
2. Intenta comentar el mensaje de la consola en tu archivo de Javascript para que nada se muestre en la consola.

#### Quiz 1
1. ¿Cuál es la sintaxis HTML para agregar un archivo externo de Javascript?
2. ¿Puedes ejecutar Javascript en un archivo sin la extensión JS en tu navegador?
3. ¿Cómo escribir un *multi-line* comentario en Javascript?
4. ¿Cuál es la mejor forma de remover una línea de código en ejecución que quieres mantener como si fuese un debug?

## Capítulo 2 - Javascript Essentials
En este capítulo vamos a tratar, con bloques esenciales de construcción de Javascript: variables y operadores. Vamos a empezar con las variables, que son, y qué tipos de datos existen. Necesitamos estas estructuras básicas para guardar y trabajar con valores de variables en nuestros scripts, y hacerlos dinámicos.

Una vez hayamos cubeirto las variables, estaremos listos para trabajar con los operadores.
Aritméticos, asignación, condicionales y operadores lógicos que será debatidos en esta etapa. Necesitamos operadores para modificar nuestras variables o para decir algo acerca de ellas. Podremos hacer cálculos basados en factores que el usuario ingresa.

A lo largo de esto, vamos a cubir los siguientes temas:
- Variables
- Tipos de datos primitivos
- Analizando y modificando tipos de datos
- Operadores

### Variables
Las variables son el primer bloque de construcción cuando estás aprendiendo algún lenguaje. *Las variables son valores* en tu código que representan diferentes valores en algún momento del programa.

Un ejemplo de dos variables en un script:

```javascript

primernombre = "Rosa";
x = 2;

```

Y ellas pueden ser representadas con un nuevo valor mientras el código esté en ejecución:

```javascript

primernombre = "Sara";
x = 8;

```

Sin variables, una pieza de código haría exactamente lo mismo en el mismo tiempo cuando es ejecutada. Sin embargo puede seguir siendo útil en algunos casos, puede hacer cosas más potentes trabajando con variables que te permiten hacer diferentes cosas cada vez.

### Declarando variables
Cuando vas a crear variables, debes declararlas primero. Y necesitas una palabra "especial" que es: `let, var` o `const`. Luego vamos a discutir, el uso de esos tres argumentos. La segunda vez que llamas a la variable, solamente usas el nombre existente para asignar un nuevo valor:

```javascript

let primernombre = "Rosa";
primernombre = "Celina"

```

En nuestros ejemplos, asignaremos un valor a nuestras variables en el código. Esto es llamado "hardcoded" o "en duro" desde que el valor definido en tu script lo hiciste tú en vez de que haya sido dinámicamente. Esto es algo que comúnmente no harás muy a menudo, los valores usualmente vienen de cajas de texto que están en alguna página web, algún formulario, datatables, etc. Esto hace a nuestro código adaptable a nueva información, sin tener que reescribir el código.

Hemos solamente establecido como son de poderosas los bloques de construcción de variables en código.  Ahora vamos a *hardcodear* variables en nuestro script, y por lo tanto nuestras varibales no variarán después de codificar cambios en el programa. Sin embargo, pronto vamos aprender a como hacer que nuestras variables tomen valores de otros lugares.

### let, var y const
Una definición de variable consiste en tres partes: una palabra clave que defina-variable(`let`, `var` o `const`), un nombre, y un valor. Empecemos con las diferencias entre `let, var` o `const`.

```javascript

let nr1 = 12;
var nr2 = 8;
const PI = 3.14159;

```

`let` y `var` son usadas por variables que podrían tener un nuevo valor asignado algún lugar en el programa. La diferencia en entre `let` y `var` es compleja. Tiene que con el *contexto*.

`var` tiene algo llamado **global scope** y `let` tiene **block scope**. Global scope o *contexto global* significa que puedes usar las variables definidas con `var` en todo el script. En otras palabas, el Block scope o *contexto de bloque* significa que solamente puedes utilizar variables definidas con `let` en un específico bloque de código en el cual se ha definido. Recuerda que un bloque de código siempre empieza con `{` y termina con `}`.

En otras palabras, `const` es usado por variables que *solamente* serán asignadas **una vez(constante)**, por ejemplo, el valor de pi, el cual no cambia. Si intentas reasignar un valor declarado con `const`, obtendrás un error:

```javascript

const algunaConstante = 3;
algunaConstante = 10,

```

El resultado de esto será:

`Uncaught TypeError: Assignment to constant variable`

Nosotros estaremos usando `let` en la mayoría de los ejemplos.

### Nombrado de variables
Hay algunas convenciones en cuanto al nombrado de variables:
- Las variables empiezan en **minúsculas** y deben ser **descriptivas**. Si algo almacena la edad, no lo llames `x`. Esto es para que cuando leas tu código luego puedas entenderlo y que hiciste solamente leyendo.
- Las variables **no contienen espacios**, pero se puede usar **guión bajo**. Si usas un espacio, Javascript no podrá reconocerlo.

---

Nota: Usaremos camel case. Esto significa que cuando queremos usar múltiples palabras que describen una variable, empezaremos con *minúscula*, luego por cada nueva palabra usaremos la primera letra en *mayúscula*, por ejemplo: `edadDelComprador`.

---

El valor de tus variables pueden ser cualquier cosa.

### Tipos de datos Primitivos
Ahora ya sabes que son las variables y por qué necesitamos de ellas en nuestro código, es tiempo para mirar los diferentes tipos de valores que podemos almacenar en variables. Las variables obtienen un valor asignado. Y estos valores pueden ser de diferentes tipos. Javascript no es exigente en cuanto a tipos. Esto significa que *Javascript determina el tipo basado en el valor*. El tipo no es necesario nombrarlo explícitamente. Por ejemplo, si declara un valor 5, Javascript automáticamente lo definirá como un tipo `number`.

#### String
Un string o cadena es usado para alamcenar valor de texto. Es una secuencia de caracteres. Hay muchas maneras de declarar un string:
- Dobles comillas (double quotes)
- Comillas simples (single quotes)
- Comillas invertidas (backticks): para *template strings* en el cual puedes usar variables directamente en el string

Las comillas simples y dobles puede ser usadas de la misma manera:

```javascript

let singleString = 'Holis';
let doubleString = "¿Cómo estas?";

```
---

Nota: Puedes usar la opción que prefieras, a no ser que estés trabajando en un código donde el cual una de las opciones han sido tomadas. De vuelta, la *consistencia* es la clave.

---

La principal difenncia entre comillas simples y dobles es cuando quieres usar caracteres literales en doble comillas, y viceversa. Si tu quieres declarar un string con comillas simples, el string terminará cuando la última comilla se ponga, no importad si esta a la mitad de la palabra. Por ejemplo:

```javascript

let funActivity = 'Let's learn Javascript';

```

Esta será reconocida como un string, pero luego que, el conjunto de caracteres que siguen no podrán ser interpretadas por Javascript. Sin embargo, si declaras el string usando dobles comillas, no terminará con la última comilla, ejemplo:

```javascript

let funActivity = "Let's learn Javascript";

```

En la misma idea con comillas dobles, el siguiente ejemplo no funcionará:

```javascript

let pregunta = "¿Te gustaría aprender Javascript? "Si!"";

```

Otra vez el compilador no distinguirá entre comillas dobles en un mismo contexto y mostrará un error.

En las comillas invertidas(backticks), puedes apuntar la variable y el valor de la misma será sustituida dentro de la línea, ejemplo:

```javascript

let lenguaje = "Javascript";
let mensaje = `Aprendamos ${lenguaje}`;
console.log(mensaje);

```

Así como puedes ver, especificarás estas variables con bastante e interesante sintaxis, no te sientas intimidado. La razón es que esto simplifica los casos de tener que mezclar las comillas dobles o simples cuando están juntas y así evitamos concatenaciones innecesarias.

### Escapar caracteres
Decimos que queremos tener comillas simples, dobles e invertidas en nuestro string. Podríamos tener un problema, como esto no puede estar listo con los ingredientes que tenemos ahora. Hay un carácter especial que podemos usar para decirle a Javascript, "No tomes el siguiente carácter como normalmente lo haces". Esto es el escapado de caracteres, un *backslash*

En este ejemplo, el *backslash* puede ser usado para asegurar que el intérprete no vea la comilla doble o simple y terminar muy rápido:

```javascript

let str = "Hola, ¿cuál es tu nombre? ¿Es \"Juan\"?";
console.log(str);
let str2 = 'Hola, ¿cuál es tu nombre? ¿Es "Juan"?';
console.log(str2);

```

Este log muestra en la consola:

```
Hola, ¿cuál es tu nombre? ¿Es "Juan"?
Hola, ¿cuál es tu nombre? ¿Es "Juan"?

```

Así como puedes ver, ambos tipos de comillas dentro de los strings fueron mostrado sin errores. Esto es porque el *backslash* antes de la comilla le da un significado diferente. En este caso, el significado es que debería ser un carácter literal en vez de un indicador de fin de la cadena.

El carácter de escape tiene aún más propósitos. Puedes usarlo para crear una punto de ruptura con `\n`, o incluir el *backslash* en el texto con `\\`:

```javascript

let str3 = "Nueva \nlínea";
let str4 = 'Estoy conteniendo un backslash: \\!';
console.log(str3);
console.log(str4);

```

La salida de estas lineas son:

```
Nueva
línea
Estoy conteniendo un backslash: \!
```

### Number
El tipo de dato number es usado para representar, números. En muchos lenguajes, hay una muy clara diferencia entre los tipos numéricos. Los desarrolladores de Javascript decidieron ir por un tipo de dato por todos los números: number. Para ser más precisos, ellos decidieron ir por algo llamado *64-bit floating-point number*. Esto significa que ellos pueden guardar numeros bastante grandes y ambos tanto con signo o sin signo, números con decimales, y más.

Sin embargo, hay diferentes tipos de numeros que pueden ser representados. Primero que todo, integers, por ejemplo: 4 o 89. Pero los tipos de datos numéricos también pueden ser representados por decimales, exponenciaciones, octales, hexadecimales, y números binarios. Ejemplo:

```javascript

let inrNr = 1;
let decNr = 1.5;
let expNr = 1.4e15;
let octNr = 0o10; //la versión decimal sería ser 8
let hexNr = 0x3E8; // la versión decimal sería 1000
let binNr = 0b101; // la versión decimal sería 5

```

No deberías preocuparte acerca de estos últimos tres si no estas familiarizado con ellos. Estos sin sólo diferentes formas de representar números que puedes encontrarte en el amplio campo de la ciencia de la computación. Entonces los integer son números, como:

```javascript

let intNr2 = 3434;
let intNr3 = -111;

```

Y los de punto flotante son números también:

```javascript

let decNr2 = 45.78;

```

Y los números binarios son números también:

```javascript

let binNr2 = 0b100; // sería un 4

```

### BigInt
Los límites de los tipos de datos numéricos son 2<sup>53</sup>-1 y -(2<sup>53</sup>-1). En caso que necesites números más grandes (o más pequeños), BigInt entra en juego. Un tipo de dato BigInt puede ser reconocido por el posfijo `n`;

```javascript

let bigNr = 90071992547409920n;

```

Veamos que pasa si cuando empezamos a hacer cálculos entre nuestro previo número integer, `intNr`, y BigInt, `bigNr`:

```javascript

let resultado = bigNr + intNr;

```

La salida será:

`Uncaught TypeError: Cannot mix BigInt and other types, use explicit conversions`

Un *Typerror!*, es muy claro acerca de lo que esta funcionando mal. No podemos mezclar BigInt con Number para realizar la operación.

### Boolean
El tipo de dato booleano puede almacenar dos valores: `true` o `false`. No hay nada en medio. El booleano es usado muchas veces en el código, especialmente en expresiones de evaluación:

```javascript

let bool1 = false;
let bool2 = true;

```

En el ejemplo anterior, puedes ver las opciones que tenemos para el tipo de dato Boolean. Es usado para situaciones en el cual necesitas almacenar Falso o Verdadero o Prendido o Apagado, Sí o No, etc. Por ejemplo:

```javascript

let estaBorradoElObjeto = false;

```

O, si la luz está prendida o apagada:

```javascript

let luzEstaPrendida = true;

```

Estas variables sugieren respecticamente que el objeto esta borrado o que la luz esta prendida.

### Symbol
Symbol es un nuevo tipo de dato introducido en ES6 (recuerdas que mencionamos sobre ECMA Script 6) o ES6. Symbol puede ser usado cuando ciertas variables no son iguales, a pesar de su valor y tipo sean el mismo. Ejemplo:

```javascript

let str1 = "JavaScript es divertido";
let str2 = "JavaScript es divertido";
console.log("Estas dos variables son lo mismo: ", str1 === str2);

let sym1 = Symbol("JavaScript es divertido");
let sym2 = Symbol("JavaScript es divertido");
console.log("Estas dos variables son lo mismo: ", sym1 === sym2);

```

La salida sera:
```
Estas dos variables son lo mismo: true
Estas dos variables son lo mismo: false
```

En la primera mitad, Javascript concluye que son lo mismo. Ellos tienen el mismo valor, y el mismo tipo. Sin embargo, en la segunda parte, cada *symbol* es *único*.

En JavaScript, el tipo de dato Symbol se utiliza para crear valores únicos e inmutables. Los símbolos son útiles cuando necesitas crear propiedades de objetos que no colisionarán con otras propiedades, ya que cada símbolo es único. Puedes usarlos como claves de propiedades para evitar posibles conflictos en el nombre de las propiedades. Por lo tanto, por más de que contengan el mismo string, no son lo mismo, y la salida es `false` cuando son comparadas.

Por ejemplo:

```javascript!
const sym = Symbol('miSimbolo');

const obj = {
  [sym]: 'Hola, soy un símbolo'
};

console.log(obj[sym]); // Imprime: Hola, soy un símbolo
```

Aquí, Symbol('miSimbolo') crea un símbolo con una descripción opcional ('miSimbolo' en este caso). La descripción no afecta a la unicidad del símbolo; es solo para propósitos descriptivos.

### Undefined
Javascript es un lenguaje muy especial. Este tiene un tipo de dato especial para las variables a las que no se les asigno un valor. Entonces, su tipo de dato es `undefined` o indefinido:

```javascript!
let noasignado;
console.log(noasignado);
```

La salida será:
`Undefined`

Podemos a propósito asignar un valor `undefined`. Esto es importante saber, que es posible, pero es aún más importante saber que asignarlo es una *mala práctica*:

```javascript!
let terribleCosaParaHacer = undefined;
```

Todo bien, es posible hacerlo, pero **no es recomendado**, por un número de razones -por ejemplo, revisar si dos variables tienen lo mismo. Si una variable es `undefined`, y tu variable fue almacenada con `undefined`, ellos serán iguales. Esto es un error por si estás revisando la igualdad, querrías saber si son de hecho iguales, no solamente si son `undefined`. Imagina la mascota de alguien y su apellido podrían ser consideradas iguales, pero en realidad están vacíos.

### null
En este ejemplo, veremos un error que puede resolverse con un tipo primitivo, `null`. `null` es un valor especial por así decirlo, representa una variable vacía o que tiene un valor desconocido. Cuidado con las mayúsculas, es sensible a ellas, siempre en minúsculas:

```javascript!
let vacio = null;
```

Para resolver el error encontrado de una variable con `undefined`, nota que si pones null, no tendrás el mismo problema. Esta es una de las razones del porque es mejor asignar nukk a una variable cuando intentas decir que estará vacía:

```javascript!
let terribleCosaParaHacer = undefined;
let apellido;
console.log("Mismos undefined: ", apellido === terribleCosaParaHacer);

let buenaPractica = null;
console.log("El null: ", apellido === buenaPractica);
```

La salida en consola:
```
Mismos undefined:  true
El null:  false
```

Esto muestra que de forma automática se pueden crear variables undefined, `apellido`, y deliberadamente otra `terribleCosaParaHacer`, son consideradas iguales, lo cual es problemático. Del otro lado, `apellido` y `buenaPractica`, que fueron explícitamente declarados, con null, no son iguales.

### Analizando y modificando tipos de datos
Vimos los tipos de datos primitivos. Hay algunos métodos preconstruidos en Javascript que nos ayudarán a lidiar con algunos problemas relacionados con los primitivos. *Built-in methods* o métodos preconstruidos son piezas lógicas que pueden ser usadas para escribir lógica de Javascript sin tener que reescribirla tu mismo.

Nota: Ya hemos visto un método built-in: `console.log()`

### Trabajando con `typeof` de variables
Especialmente con null y undefined, puede ser difícil determinar cual es el tipo de dato con el que estamos trabajando. Veamos a `typeof`, este retorna el tipo de dato de la variable. Ejemplo:

```javascript!
testVariable = 1;
variableTypeTest1 = typeof testVariable;
variableTypeTest2 = typeof(testVariable);
console.log(variableTypeTest1);
console.log(variableTypeTest2);
```
Como supnes, ambos métodos retornan un `number`. Los paréntesis no son necesarios porque técnicamente, `typeof` es un operador, no un método, diferente de `console.log()` . Pero, a veces podría ser cómodo usarlo con paréntesis porque hace más facil leer tu código, otro ejemplo:

```javascript!
let str = "holis";
let nr = 7;
let bigNr = 1234567891234n;
let bool = true;
let sym = Symbol("único");
let undef = undefined;
let desconocido = null;

console.log("str", typeof str);
console.log("nr", typeof nr);
console.log("bigNr", typeof bigNr);
console.log("bool", typeof bool);
console.log("sym", typeof sym);
console.log("undef", typeof undef);
console.log("desconocido", typeof desconocido);
```

La salida en consola:
```
str string
nr number
bigNr bigint
bool boolean
sym symbol
undef undefined
desconocido object
```

Hay una extraña salida, el que es `null`. Se ve que el `typeof null` retorna un `object`, de hecho, `null` es un primitivo y no un objeto. Este es un bug que estado siempre y no puede ser removido por problemas de compatibilidad hacia atrás.

### Convirtiendo tipos de datos
Las variables en Javascript pueden cambiar de tipos. Algunas veces esto ocurre de forma automática. ¿Qué ocurriría si hacemos lo siguiente?:

```javascript!
let nr1 = 2;
let nr2 = "2";
console.log(nr1 * nr2);
```
Estamos tratando de multiplicar un tipo Number con una variable de tipo String.
Javascript no retorna ningún error (así como otros lenguajes sí lo hacen), pero primero intenta convertir el string a un numérico. Si esto se puede hacer, se ejecuta sin problemas como si se declarasen dos números. En este caso, `console.log()` escribirá en la consola el `4`.

¡Pero esto es peligroso! Intenta adivinar que sucede con lo siguiente:

```javascript!
let nr1 = 2;
let nr2 = "2";
console.log(nr1 + nr2);
```

Esto va mostrar `22`. El signo `+` también es usado para concatenar strings. Por lo tanto, en vez de convertir un string a number, el number pasará a ser un string, luego se concatenará, cosa que no queremos. Por suerte no debemos confiar en este comportamiento cuando se convierten los tipos de datos. Hay funciones preconstruídas que nos ayudarán en este proceso.

Hay tres métodos de conversión: `String(), Number(), Boolean()`. El primero convierte una variable al tipo String. Es mucho más que tomar cualquier valor, incluyendo undefined y null, pone las comillas alrededor de ello.

El segundo intenta convertir una variable a Number. Si no puede hacerlo, lo convertirá a un valor de tipo `Nan`(Not a Number). `Boolean()` convierte una variable a un Boolean. Esto será true para todo excepto para null, undefined, `0`(number), cadena de texto vacía y NaN. Ejemplo:

```javascript!
let nrToStr = 6;
nrToStr = String(nrToStr);
console.log(nrToStr, typeof nrToStr);

let strToNr = "12";
strToNr = Number(strToNr);
console.log(strToNr, typeof strToNr);

let strToBool = "algún string será retornado como true";
strToBool = Boolean(strToBool);
console.log(strToBool, typeof strToBool);
```

Finalmente, la salida en consola será:
```
6 string
12 'number'
true 'boolean'
```

Vamos a probar un poco tu cerebro. ¿Qué piensas que se mostrará aquí?:

```javascript!
let nr1 = 2;
let nr2 = "2";
console.log(nr1 + Number(nr2));
```

#### Ejercicio 2.1
¿Cuales son los tipos de estas variables listadas abajo? Verifica con`typeof` y muestra la salida del resultado en consola:

```javascript!
let str1 = 'Laurence';
let str2 = "Svekis";
let val1 = undefined;
let val2 = null;
let myNum = 1000;
```

### Operadores
Luego de mirar un poco los *data types* y las formas de convertirlos, es tiempo de ver otros bloques de construcción: operadores

### Operadores Aritméticos
Los operadores aritméticos pueden ser usados para trabajar operaciones con números.

### Adición
La adición en Javascript es muy simple, ya lo vimos. Usamos el símbolo `+`:
```javascript!
let nr1 = 12;
let nr2 = 14;
let result = nr1 + nr2;
```

Sin embargo, este operador puede también ser muy práctico concatenando strings, inclusive el espacio:

```javascript
let str1 = "Holis ";
let str2 = "adición";
let result = str1 + str2;
```

En la consola debería verse:
```
26
Hola adición
```
#### Ejercicio 2.2
Crea una variable para tu nombre, otra variable para tu edad, otra variable para saber si sabes codificar o no en Javascript.
Muestra en la consola, con tu nombre, tu edad y si es true/false:

```
Hola, mi nombre es Mike, tengo 25 años y puedo codificiar en Javascript: true
```

### Substracción
La substracción funciona como lo esperaríamos también. Usamos el signo `-`:
```javascript!
let nr1 = 20;
let nr2 = 4;
let str1 = "Holis";
let nr3 = 3;
let result1 = nr1 - nr2;
let result2 = str1 - nr3;
console.log(result1, result2);
```
La salida es:
`16 NaN`
El primer resultado es `16`. Y lo segundo es un resultado interesante. Nos da un`NaN`, no un error, pero la conclusión a esto es que una palabra y un número no pueden substraerse.

### Multiplicación
Podemos multiplicar dos variables numéricas con el `*`. A diferencia de otros lenguajes, no podemos multiplicar exitosamente un número y un string.
El resultado de multiplicar un numérico y otro que no lo es, retorna `NaN`:
```javascript!
let nr1 = 15;
let nr2 = 10;
let str1 = "Hi";
let nr3 = 3;
let result1 = nr1 * nr2;
let result2 = str1 *nr3;
console.log(result1, result2);
```
La consola muestra:
`150 NaN`

### División
La divisón también es una operación directa. Podemos dividir dos números con `/`:

```javascript!
let nr1 = 30;
let nr2 = 5;
let result1 = nr1 / nr2;
console.log(result1);
```
Muestra en consola:
`6`

### Exponenciación
La exponenciación significa que teniendo cierta base numérica a elevar de un exponente, se usa `**`:

```javascript!
let nr1 = 2;
let nr2 = 3;
let result1 = nr1 ** nr2;
console.log(result1);
```

### Módulo
El módulo es la operación en el cual se determina cuanto es el residuo de la división, se usa `%`:

```javascript!
let nr1 = 10;
let nr2 = 3;
let result1 = nr1 % nr2;
console.log(`${nr1} % ${nr2} = ${result1}`);

let nr3 = 8;
let nr4 = 2;
let result2 = nr3 % nr4;
console.log(`${nr3} % ${nr4} = ${result2}`);

let nr5 = 15;
let nr6 = 4;
let result3 = nr5 % nr6;
console.log(`${nr5} % ${nr6} = ${result3}`);
```

El resultado es:

![image](https://hackmd.io/_uploads/rkQGVtVu6.png)

### Operadores unarios: incremento y decremento

```javascript!

let nr1 = 4;
nr1++;
console.log(nr1);

let nr2 = 4;
nr2--;
console.log(nr2);

```

![image](https://hackmd.io/_uploads/Byhj_YEuT.png)


### Prefijos y posfijos
Podemos tener el operador de incremento despues del operando `x++`, en el cual usamos el operador posfijo. También podemos hacerlo antes `++x`, esto es el prefijo.
El postfix o posfijo es ejecutado despues de enviar a la variable el valor:

```javascript!
let nr = 2;
console.log(nr++);
console.log(nr);
```

![image](https://hackmd.io/_uploads/ryvCFFNO6.png)


Con el prefijo, es ejecutado antes de enviarse a la variable:

```javascript!
let nr = 2;
console.log(++nr);
```

![image](https://hackmd.io/_uploads/B1Rz9YV_6.png)


### Combinando operadores
Estos operadores pueden combinarse, y funcionan igual que en matemáticas. Ellos se ejecutan en cierto orden, no necesariamente de izquierda a derecha. Este fenómeno conocido es llamado precedencia de operadores.

| Nombre | Símbolo | Ejemplo |
|--------|---------|---------|
| Agrupación | `(...)` | `(x + y)`|
| Exponenciación | `**` | `x ** y` |
| Prefijos y Posfijos | `--, ++` | `--x, ++y` |
| Multiplicación, división y módulo | `*, /, %` | `x * y, x / y, x % y` |
| Adición y substracción | `+, -` | `x + y, x - y` |

#### Ejercicio 2.3
Investiga y escriba un poco de código para calcular la hipotenusa usando el teorema de Pitágoras, a<sup>2</sup>+b<sup>2</sup> = c<sup>2</sup>

![image](https://hackmd.io/_uploads/SJkwAFVua.png)

[Algunas funciones math](https://www.freecodecamp.org/espanol/news/funciones-math-en-javascript-explicadas/#:~:text=Math%20Sqrt-,La%20funci%C3%B3n%20Math.,n%C3%BAmero%20negativo%2C%20te%20devuelve%20NaN%20)

Puedes usar la función `prompt()` para obtener el valor de a y b.

Imprime en consola el resultado.

### Operadores de asignación
Ya hemos visto un operador de asignación cuando asignábamos valores a las variables. El carácter básico era `=`. También hay otros disponibles.
Por ejemplo:

```javascript!

x += 5; // significa x = x + 5;
x **= 3; // significa x a la potencia de 3

```

En el primer ejemplo declaramos una variable `x`, lo seteamos con `2` como valor inicial:

```javascript!

let x = 2;
x += 2;
console.log(`Resultado de x = ${x}`);

x -= 2;
console.log(`Resultado de x = ${x}`);

x *= 6;
console.log(`Resultado de x = ${x}`);

x /= 3;
console.log(`Resultado de x = ${x}`);

x **= 2;
console.log(`Resultado de x = ${x}`);

x %= 3;
console.log(`Resultado de x = ${x}`);

```

La salida será: 

```
Resultado de x = 4
Resultado de x = 2
Resultado de x = 12
Resultado de x = 4
```

Calcula el resulta de los últimos dos ejercicios y muestra en pantalla.

#### Ejercicio 2.4
Crea variables para tres números: *a, b, c*. Actualiza los valores de esas variables usando los operadores de asignación:
- Suma *b* en *a*
- Divide *a* con *c*
- Reemplaza el valor de *c* con el módulo de *c* y *b*
- Imprimir los tres números en consola

### Operadores de comparación
Los operadores de comparación son un tipo distinto de lo que hemos visto. En estos se manejan booleanos(`true/false`):

#### Igualdad

```javascript!
let x = 5;
let y = "5";
console.log(x == y);
```

El doble operador de igualdad, dos signos iguales, significa que solamente se revisará el *valor y no el tipo de dato*.

El triple operador de igualdad, escrito con tres signos iguales, significa que evaluará el *valor y el tipo de dato* para determinar si ambos son iguales o no.

```javascript!
let x = 5;
let y = "5";
console.log(x === y);
```

### No igual
Not equal es muy similar al igual, es su opuesto, este retorna `true` si dos variables no son iguales:

```javascript!
let x = 5;
let y = "5";
console.log(x != y);
```

Esto mostrará `false`. Si te estabas preguntando que va pasar si usasemos el de doble igualdad:

```javascript!
let x = 5;
let y = "5";
console.log(x !== y);
```

### Mayor que y menor que
El operador de mayor que retorna true si el de la izquierda es mayor que el de la derecha, se usa el carácter `>`:

```javascript!
let x = 5;
let y = 6;
console.log(x > y);
```

Solamente será `true`, si `y` es mayor que `x`. Y como no es `true`, será `false`.

`y` no es mayor que `y`, entonces mostrará `false`:

```javascript!
console.log(y >= y);
```

No debería de sorprenderte en el caso de menor que:

```javascript!
console.log(y < x); // retorna true
```

Pero en el caso de que `y` sea menor que `y`:

```javascript!
console.log(y < y); // retorna false
```

Dará true si aplicamos igualdad:

```javascript!
console.log(y <= y); // retorna false
```

### Operadores lógicos
Cuando quieras comprobar dos condiciones, o necesitas negarlas, los operadores lógicos `and, or, not` entran en acción.

#### And

```javascript!
let x = 1;
let y = 2;
let z = 3;
console.log(x < y && y < z);
```

#### Or

```javascript!
console.log(x > y || y < z);
console.log(x > y || y > z);
```

#### Negación
En algunos casos tenemos que negar un Boolean.

```javascript!
let x = false;
console.log(!x); // retorna true
```

También podemos agrupar:
```javascript!
let x = 1;
let y = 2;
console.log(!(x < y));
```


#### Proyecto 2
#### Convertidor de millas a kilómetros
Crea una variable que contenga un valor en millas, conviértelo a kilómetros, muestra el mensaje en consola del valor en kilómetros, el formato a mostrar será:

`La distancia de 130 Km es igual a 209.2142 millas`

Referencia, 1 milla es igual a 1.60934 kilómetros

#### Calculadora IMC(Índice de masa corporal)
Utilice la siguente fórmula:

![image](https://hackmd.io/_uploads/BJzrlboua.png)

desarrollar un programa que permita ingresar dos valores (peso en Kg) y (altura en metros) utilizando el `prompt()`, realice el cálculo y muestre el resultado en consola:

#### Prueba
1. ¿Qué tipo de dato tiene la siguente variable?
```javascript 
const c = "5";
```
2. ¿Qué tipo de dato tiene la siguente variable?
`const c = 91;`
3. ¿Cuál de los dos es mejor?, línea 1 or línea 2?
```javascript
let empty1 = undefined; //line 1
let empty2 = null; //line 2
```
4. ¿Qué salida producen en consola?
```javascript
let a = "Hello";
a = "world";
console.log(a);
```
5. ¿Qué se mostrará en la consola?
```javascript
let a = "world";
let b = `Hello ${a}!`;
console.log(b);
```
6. ¿Cuál es el valor de a?
```javascript
let a = "Hello";
a = prompt("world");
console.log(a);
```
7. ¿Cuál es el valor de b en la consola?
```javascript
let a = 5;
let b = 70;
let c = "5";
b++;
console.log(b);
```
8. ¿Cuál es el valor de este resultado?
`let result = 3 + 4 * 2 / 8;`
9. ¿Cuál es el valor de total y total2?
```javascript
let firstNum = 5;
let secondNum = 10;
firstNum++;
secondNum--;
let total = ++firstNum + secondNum;
console.log(total);
let total2 = 500 + 100 / 5 + total--;
console.log(total2);
```
10. ¿Qué se mostrará en la consola aquí?
```javascript
const a = 5;
const b = 10;
console.log(a > 0 && b > 0);
console.log(a == 5 && b == 4);
console.log(true ||false);
console.log(a == 3 || b == 10);
console.log(a == 3 || b == 7);
```

## Capítulo 3 - Javascript valores múltiples
Los *data types* básicos ya fueron revisados y ahora es tiempo de mirar algo ligeramente complicado: arrays y objects. En lecciones anteriores, vimos variables que tenían un valor. Para permitir un poco de programación avanzada, objects y arrays pueden contener múltiples valores.

Puedes ver a los objetos como una colección de *propiedades* y *métodos*. Las propiedades pueden puede ser pensadas como variables. Ellas pueden ser simples estructuras de datos como números o strings, pero también otros objetos. Los métodos realizan acciones; ellos contienen cierto número de lines de código que serán ejecutadas cuando son llamadas.

**Un ejemplo de objeto puede un objeto de la vida real, por ejemplo, un perro. El tiene propiedades, como nombre, peso, color y raza.**

También debemos conversar sobre los arrays. **Un array es un tipo de objeto**, que nos permite almacenar múltiples valores. Son parecidos a las listas. Entonces, puedes tener un array de items para comprar de la despensa, el cual contendría los siguientes valores: manzanas, huevos, y pan. Esta lista sería parecida a una variable simple, almacenando múltimples valores.

En este capítulo vamos a ver los siguientes temas:

- Arrays y sus propiedades
- Métodos de los arrays
- Arrays multidimensionales
- Objetos en JavaScript
- Trabajando con objetos y arrays

#### Arrays y sus propiedades
Los arrays son listas de valores. Estos valores pueden ser de cualquier tipo de *data type* y valor. Es a menudo útil para almacenar valores dentro de una variable; por ejemplo, una lista de estudiantes, comestibles, notas. Una vez que empiezas a escribir el script, encontrarás por ti mismo que es necesario usar arrays a menudo; por ejemplo. cuando quieres mantener el seguimiento de lo que el usuario ingresa, o cuando quiere tener una lista de opciones para presentarle al usuario.

#### Creando arrays
Ahora ya sabes que los arrays son geniales, pero hay una manera correcta de hacer y otra mala, te mostraré las dos y me dices cuál esta mal y cuál es la buena:

```javascript
arr1 = new Array("purple", "green", "yellow");
arr2 = ["black", "orange", "pink"];
```

Si adivinaste que la segunda opción, usando corchetes, acertaste. Esta es la mejor y más legible manera de crear un nuevo array. Por otro lado, la primera opción puede hacer cosas inesperadas. Fíjate en las siguientes líneas. ¿Qué opinas que hacen?

```javascript
arr3 = new Array(10);
arr4 = [10];
```

Probablemente, sentiste algo ahí. Ellos no crean un array con el valor, `10`. El segundo, `arr4`, sí lo hace. La primera opción crea un array con 10 valores undefined. Si hacemos console para comprobar:

```javascript
console.log(arr3);
console.log(arr4);
```
Se muestra:
```
[ <10 empty items> ]
[ 10 ]
```

¡Gracias, Javascript! eso ha sido de gran ayuda. A no ser que necesites hacerlo, por favor usa los corchetes.

Como dijimos anteriormente, podemos mezclar los arrays y estos pueden guardar cualquier tipo de variable. Los valores de un array *no son convertidos a ningún tipo de dato*. Javascript simplemente almacena todas las variables con su *propio tipo de dato y valor* en el array:

```javascript
let arr = ["hi there", 5, true];
console.log(typeof arr[0]);
console.log(typeof arr[1]);
console.log(typeof arr[2]);
```

Esto va mostrar en consola:
```
string
number
boolean
```

Algo divertido, el último array que veremos en el caso si definimos una `const`. Puedes cambiar los valores de un array constante :flushed: , pero no puedes cambiar el array en sí mismo :unamused:. Veamos:

```javascript
const arr = ["hi there"];
arr[0] = "new value";
console.log(arr[0]);
arr = ["nope, now you are overwriting the array"];
```

El nuevo valor del primer elemento del array está bien, pero no puedes asignar un nuevo valor a **todo** el array. Veamos en consola:

```
new value
TypeError: Assignment to constant variable.
```

#### Accediendo a los elementos
Los arrays son hermosos porque podemos hacer cosas poderosas con el, siempre y cuando podamos acceder a su contenido. Esto lo haremos por referencia, usando el *índice del array*. Javascript asigna un índice a cada valor del array. El primer valor asignado de la posición 0, el segundo es 1, el tercero 2, etc. Si queremos llamar a un valor en específico, debemos usar el nombre del array y agregarle cochetes con el número del índice en medio.
Veamos:

```javascript
cars = ["Toyota", "Renault", "Volkswagen"];
console.log(cars[0]);
```

Esto debería mostrar en consola `Toyota`, y si hacemos:

`console.log(cars[1]); // muestra Reanult`

Y el 2?:
`console.log(cars[2]); // muestra Volkswagen`

¿Qué pasaría si ponemos un valor más alto que el número de elementos del array?

```javascript
console.log(cars[3]);
console.log(cars[-1]);
```

No hemos asignado un valor al negativo o a un index inexistente, entonces podemos pedirlo, el valor será undefined. Como tal se mostrará indefinido. Javascript no lanzará ningún error por eso.

#### Sobreescribiendo elementos
Los elementos en un array pueden ser sobreescritos. Esto puede ser realizado accediendo a ciertos elementos usando su índice y asignando un nuevo valor:

```javascript
cars[0] = "Tesla";
console.log(cars[0]);
```

Se muestra en consola:

`console.log(cars); // muestra [ 'Tesla', 'Renault', 'Volkswagen' ]`

¿Qué pasa si intentas sobreescribir un elemento que no existe?

`cars[3] = "Kia";`

O incluso un índice negativo:

`cars[-1] = "Fiat";`

Veamos que se muestra en consola:

```
console.log(cars[3]);
console.log(cars[-1]);
```

La salida:
```
Kia
Fiat
```

:satisfied: ¡De repente existen! ¿Cómo esto es posible?

#### La propiedad `length`
Los Arrays tiene una propiedad muy útil: length. Este muestra el número de valores que tiene un Array:

```javascript
colors = ["black", "orange", "pink"]
booleans = [true, false, false, true];
emptyArray = [];
console.log("Length of colors:", colors.length);
console.log("Length of booleans:", booleans.length);
console.log("Length of empty array:", emptyArray.length);
```

Consola:

```
Length of colors: 3
Length of booleans: 4
Length of empty array: 0
```

Pero, ten cuidado que `length` toma el número de elementos de un array, pero también recuerda que los array empiezan en la posición 0. 

Trata de averiguar la salida de esto, que intenta acceder al último elemento del array:

`lastElement = colors[colors.length - 1];`

Bien, recuerdas los index no existentes, veamos este ejemplo:

```javascript
numbers = [12, 24, 36];
numbers[5] = 48;
console.log(numbers.length);
```

El length del array esta solamente contando los integer empezando por el 0 para el más alto índice. Si hay elementos en el medio de una secuencia que no tiene valor, igual será contado. En este caso el length será 6:

`console.log("numbers", numbers);`

La salida:
`numbers [ 12, 24, 36, <2 empty items>, 48 ]`

Porque agregamos un elemento, 48, en el índice 5, entonces se crean dos elementos, en la posición 3 y 4 que contienen elementos vacíos.

#### Ejercicio 3.1
1. Crea un array para usar en tus compras al supermercado, una lista de tres items.
2. Revisa tu lista usando `length`.
3. Actualiza uno de los elementos.
4. Muestra la lista entera en consola

#### Métodos de Array
Ya hemos visto la propiedad `length`. También tenemos otros métodos.
Los *métodos* están en funciones de ciertos objetos. En vez de mantener un valor, como las propiedades, ellas hacen cosas. Esto se cubrirá en el capítulo de funciones.
Por ahora lo que se necesita saber es que puedes llamar a los métodos y funciones, y cuando haces algo de código.

Accidentalmente vimos que podíamos agregar elementos usando nuevos índices. Esta no es la forma apropiada de hacerlo, porque es fácil de cometer errores y accidentalmente sobreescribir algún valor o ignorar cierto índice. La forma correcta de hacerlo es con un método especial. Similarmente, podemos borrar elementos y ordenar los elementos del array.

#### Agregando y reemplazando elementos
Podemos agregar ciertos elementos con el método push `push()`:

```javascript
favoriteFruits = ["grapefruit", "orange", "lemon"];
favoriteFruits.push("tangerine");
```

Los valores agregados estarán al final del array. El método `push` retorna un nuevo `length` del array, en este caso cuatro. Puedes guardar este length en una variable:

`let lengthOfFavoriteFruits = favoriteFruits.push("lime");`

El valor 5 guardado en `lengthOfFavoriteFruits`. Si hacemos console.log de nuestro array, `favoriteFruits`:

`console.log(favoriteFruits);`

Muestra:
`[ 'grapefruit', 'orange', 'lemon', 'tangerine', 'lime' ]`

Eso fue fácil, pero ¿qué pasa si quieres agregar elementos a cierto índice?
Puedes usar el método `splice()`. Este es un poco más difícil:

```javascript
let arrOfShapes = ["circle", "triangle", "rectangle", "pentagon"];
arrOfShapes.splice(2, 0, "square", "trapezoid");
console.log(arrOfShapes);
```

Despues de esto, la salida contendrá:

```javascript
[
'circle',
'triangle',
'square',
'trapezoid',
'rectangle',
'pentagon'
]
```

Así como lo puedes ver, el `square` y el `trapezoid` fueron insertados en el índice 2. El resto del array fue movido a la derecha. El método `splice` toma múltiples parámetros. El primer parámetro, 2 en nuestro caso, es el índice de array sobre el cual queremos empezar a insertar. El segundo parámetro, 0 en nuestro caso, es el número de elementos que queremos eliminar empezando de nuestro previo índice definido. Los parámetros después de, primer 2, `square` y `trapezoid` en nuestro caso.

Veamos otro caso:

```javascript
arrOfShapes.splice(2, 2, "square", "trapezoid");
console.log(arrOfShapes);
```

Esto reemplazaría los elementos `rectangle` y `pentagon` y agrega `trapezoid` en su lugar:
`[ 'circle', 'triangle', 'square', 'trapezoid' ]`

Si incrementamos el segundo parámetro a un número más alto del que dispone nuestro array, esto no afectará el resultado.

```javascript
arrOfShapes.splice(2, 12, "square", "trapezoid");
console.log(arrOfShapes);
```

muestra:

`[ 'circle', 'triangle', 'square', 'trapezoid' ]`

También puedes agregar otro array en tu array. Esto puede hacerse usando el método `concat()`. Esta forma crea un nuevo array que consiste en la *concatenación* de arrays. Los elementos del primer array estarán primeros, y los elementos del argumento de `concat()` serán concatenados al final:

```javascript
let arr5 = [1, 2, 3];
let arr6 = [4, 5, 6];
let arr7 = arr5.concat(arr6);
console.log(arr7);
```

La consola muestra:
`[ 1, 2, 3, 4, 5, 6 ]`

`concat()` puede hacer todavía más cosas! Podemos agregar valores valores también. Podemos agregar un valor o varios valores separados por comas:

```javascript
let arr8 = arr7.concat(7, 8, 9);
console.log(arr8);
```

El nuevo valor del array sera:
`[ 1, 2, 3, 4, 5, 6, 7, 8, 9 ]`

#### Borrando elementos
Hay muchas maneras en el cual se pueden borrar elementos de un array. Removiendo el último elemento con `pop()`:

`arr8.pop();`

La consola muestra:
`[ 1, 2, 3, 4, 5, 6, 7, 8 ]`

Y si quisiésemos borrar el primer elemento, usaremos `shift()`. Esto reducirá todos los índices de una vez:

`arr8.shift();`

El nuevo array será:
`[ 2, 3, 4, 5, 6, 7, 8 ]`

¿Recuerdas `splice()`? Esta es una forma muy especial de usarla también para borrar valores. Especificamos el índice desde donde queremos empezar a borrar, y luego el número de elementos que queremos borrar:

`arr8.splice(1, 3);`

La consola muestra:
`[ 2, 6, 7, 8 ]`

Así como puedes verlo, 3 elementos empezando por la segunda posición de index fueron eliminados. Los valores 3, 4 y 5 se . Si no deseas cambiar ninguno de los siguientes índices, puedes también usar el operador delete. Esto no es un método, pero puedes usar para cambiar el valor en cierta posición del array a undefined:

`delete arr8[0];`

Muestra:
`[ <1 empty item>, 6, 7, 8 ]`

Esto es útil cuando estás confiando sobre un índice o length por alguna razón. Por ejemplo, si estás manteniendo la entrada de un usuario, y quieres determinar el número de entradas del usuario basado en un array que el usuario está ingresando, el borrado decrece el número de inputs.

#### Búsqueda de elementos -  Finding
Si quieres revisar si un valor está presente en un array, puedes usar el método `find()`. Este método funciona un poco diferente. Es de hecho una función. Esta función será ejecutada sobre cada elemento del array hasta que encuentra una coincidencia, y si no, retorna undefined.

No te preocupes si esto es difícil ahora. Vamos a escribir la función en dos formas. De hecho ambas hacen lo mismo, excepto que la primera opción revisa si un elemento es igual a 6, y la segunda si un elemento es igual a 10:

```javascript
arr8 = [ 2, 6, 7, 8 ];
let findValue = arr8.find(function(e) { return e === 6});
let findValue2 = arr8.find(e => e === 10);
console.log(findValue, findValue2);
```

La consola mostrará 6 y undefined porque puede encontrar el elemento que es 6, pero no se puede encontrar el número 10.

Una función puede tomar ciertas entradas. En este caso, toma los elementos del array como input. Cuando el elemento del array es igual a 6 `(findValue)` o 10 `(findValue2)`, retorna el elemento. Mas adelante veremos las funciones.

A menudo, no solamente necesitas encontrar el elemento, pero necesitas saber en qué posición esta. Es puede realizarse con el método `indexOf()`. Este método retorna el índice sobre el valo encontrado. Si un valor existe en un array más de una vez, se retorna la primera ocurrencia. Si el valor no se encuentra, se retorna -1:

```javascript
arr8 = [ 2, 6, 7, 8 ];
let findIndex = arr8.indexOf(6);
let findIndex2 = arr8.indexOf(10);
console.log(findIndex, findIndex2);
```

Entonces, el primero retornará 1 desde que está el index en la posición 6 en el array. El segundo retorna -1 porque no existe 10 en el array.

Si quieres encontrar la siguiente ocurrencia de un número en específico, puedes agregar un segundo argumento a `indexOf()`, especificando desde qué posición debería empezar a buscar:

```javascript
arr8 = [ 2, 6, 7, 8 ];
let findIndex3 = arr8.indexOf(6, 2);
```

En este caso, el valor de `findIndex3` será -1, porque 6 no se puede encontrar empezando por el index 2.

También la última ocurrencia puede ser encontrada. Esto es gracias al método `lastIndexOf()`:

```javascript
let animals = ["dog", "horse", "cat", "platypus", "dog"];
let lastDog = animals.lastIndexOf("dog");
```

El valor de `lastDog` será 4 porque es la última ocurrencia de dog en el array.

### Ordenación - Sorting
También hay métodos para ordenar array. Ordena números de pequeños a grandes y strings de A a la Z. Puedes llamar a `sort()` en un array y ordenar los valores:

```javascript
let names = ["James", "Alicia", "Fatiha", "Maria", "Bert"];
names.sort();
```

La consola muestra:
`[ 'Alicia', 'Bert', 'Fatiha', 'James', 'Maria' ]`

Así como puedes ver, el array ahora está ordenado alfabéticamente. Para números, el ordenamiento es ascendente:

```javascript
let ages = [18, 72, 33, 56, 40];
ages.sort();
```

muestra:
`[ 18, 33, 40, 56, 72 ]`

#### Reversing
Los elementos de un array pueden ser invertidos llamando al método `reverse()`. Este pone el último elemento primero, y el primer elemento al final. No importa si está ordenado o no, solamente invierte el orden:


Antes del reverse():
`[ 'Alicia', 'Bert', 'Fatiha', 'James', 'Maria' ]`

Ahora:

`names.reverse();`

muestra: 
`[ 'Maria', 'James', 'Fatiha', 'Bert', 'Alicia' ]`

Ejercicio 3.2
1. Crear un array vacío para usar en una lista de compras.
2. Agregar `leche, pan, manzanas` a tu lista.
3. Actualizar `pan` con `bananas` y huevos.
4. Remover el último elemento del array y mostrar en consola.
5. Ordenar la lista alfabéticamente
6. Encuentra y muestra la salida del index del valor "leche".
7. Después de `bananas`, agrega `zanahorias` y `lechuga`.
8. Crea una nueva lista conteniendo `jugo` y `pop`.
9. Combina ambas listas, agrega la nueva lista dos veces al final de la primera lista.
10. Obtener el último valor de index de `pop` y muestra en consola.
11. Tu lista final debería verse así: ```["Bananas", "Carrots", "Lettuce", "Eggs", "Milk", "Juice", "Pop", "Juice", "Pop"]```

### Arrays multidimensionales
Establecimos que son los arrays y que pueden contener valores de cualquier tipo. Esto significa que los arrays también pueden contener otros arrays (y de paso, estos arrays... otros arrays). Esto es llamado array multidimensional. Suena complicado, pero es solo un array de arrays: una lista de listas:

```javascript
let someValues1 = [1, 2, 3];
let someValues2 = [4, 5, 6];
let someValues3 = [7, 8, 9];
let arrOfArrays = [someValues1, someValues2, someValues3];
```

Entonces podemos crear un array con arrays existentes. Esto es llamado un array de dos dimensiones. Algo como esto:

`let arrOfArrays2 = [[1, 2, 3], [4, 5, 6], [7, 8, 9]];`

Si quieres acceder a los elementos del array interno, tienes que especificar el index dos veces:

`let value1 = arrOfArrays[0][1];`

Algo más loco:

`arrOfArraysOfArrays = [arrOfArrays, arrOfArrays, arrOfArrays];`


se verá en consola:

```javascript
[
[ [ 1, 2, 3 ], [ 4, 5, 6 ], [ 7, 8, 9 ] ],
[ [ 1, 2, 3 ], [ 4, 5, 6 ], [ 7, 8, 9 ] ],
[ [ 1, 2, 3 ], [ 4, 5, 6 ], [ 7, 8, 9 ] ]
]
```

Podemos probar:

`let middleValue = arrOfArraysOfArrays[1][1][1];`


#### Ejercicio 3.3
1. Crear un array que contenga tres valores, 1, 2, 3.
2. Anidar el array original en un nuevo array, tres veces.
3. Mostrar en pantalla el valor 2 de uno de los arrays en la consola

### Objetos en Javascript
Ahora es momento de aprender otra estructura de datos compleja que puede contener mas de un valor: !objetos! Los objetos son muy útiles y puede ser utilizados para describir cosas de la vida real como también conceptos más complejos y abstractos que permiten flexibilidad en tu código.

Secretamente, ya fuiste introducido a los objetos :smirk:, porque los arrays son un tipo especial de objeto. Los Arrays son objetos con *propiedades indexadas*. Todos los obejtos, también los objetos que veremos, son objetos con propiedades nombradas. Esto significa que un en vez de un index numérico generado automáticamente, vamos a crear un propiedad personalizada y *descriptiva*.

Como podemos ver en el siguiente código, los arrays son definidos por Javascrip siendo de tipo objeto:

```javascript
let arr = [0, 1, 2];
console.log(typeof arr);
```

La salida será:
`Object`

Los *Objetos* no son tan diferentes que los objetos de la vida real. Ellos *tienen(have)* propiedades y *pueden(can)* realizar acciones, métodos. Un objeto es una oportunidad de agrupar múltiples variables dentro de una. Se puede hacer esto con las llaves(`{}`). Veamos al objeto `dog`:

```javascript
let dog = { dogName: "JavaScript",
        weight: 2.4,
        color: "brown",
        breed: "chihuahua",
        age: 3,
        burglarBiter: true
    };
```

Creamos la variable `dog` y la añadimos como objeto. Podemos reconocer que es un objeto mirando sus `{  }`. En medio de las llaves(`curly braces`), vemos un montón de propiedades y sus valores.
Si alguna vez te preguntaste si algo debería ser una propiedad, puedes probar la plantilla en tu pensamiento:

\*nombreobjeto\* tiene un (has a) \*nombreDePropiedad\*

Por ejemplo, un perro tiene un nombre(name), un perro tiene un color, un perro tiene un peso(weight). Esto es ligeramente diferente para las propiedades Boolean, por el cual debes usar "es(is)" o "no es(is not)" en vez de "tiene".

Podemos acceder a las propiedades de este objeto de forma muy similar a como lo haríamos con un array. Esta vez, no vamos a estar usando un index numérico, pero si el nombre de la propiedad, para obtener el valor:

`let dogColor1 = dog["color"];`

Hay otra forma de hacer lo mismo. En vez de utilizar los corchetes(`[]`), podemos utilizar el nombre de la propiedad:

`let dogColor2 = dog.color;`

Esto parece familiar. ¿Recuerdas como obteníamos la propiedad `length` de un array? pues de la misma manera.

### Actualizando objetos
Podemos cambiar el valor de las propiedades de los objetos. Otra vez, esto es similar a un array porque un array es un objeto también, tenemos dos opciones:

```javascript
dog["color"] = "blue";
dog.weight = 2.3;
```
Esto cambió las propiedades de nuestro perrito:dog: chihuahua en Javascript. El color se actualiza a `"blue"` y pierde algo de `weight`, más o menos 0.1, si mostramos en consola:

`console.log(dog);`

Muestra:

```javascript
{
    dogName: 'JavaScript',
    weight: 2.3,
    color: 'blue',
    breed: 'chihuahua',
    age: 3,
    burglarBiter: true
}
```

Esto es fácil de notar que si cambiamos el tipo de dato de una de nuestras propiedades, por ejemplo:

`dog["age"] = "three";`

Esto no es un problema. Javascript lo cambiará por completo, el valor y su tipo en la nueva situación.

Otro elemenot a notar es si ahora usamos el literal string para referirnos a la propiedades del objeto, podemos también trabajar con variables para lograrlo. Por ejemplo:

```javascript
let variable = "age";
console.log(dog[variable]);
```

Esto mostrará `chihuahua`. Y cuando actualizamos el valor accesado por esta manera, es exacatamente como lo haríamos con el literal string:

```javascript
variable = "breed";
console.log(dog[variable]);

dog[variable] = "dalmata";
console.log(dog["breed"]);
```
Mostrará en consola `dalmata`

#### Ejercicio 3.4
1. Crear un nuevo objeto `myCar` de un auto. Agrega algunas propiedades, incluyendo, pero no limitado a, `hacer` y `modelo`y valores típicos de tu auto. Siéntete libre de usar booleanos, strings o númericos.
2. Crear una variable que pueda almacenar el `color`. Esta variable puede ser utilizada por el literal string para referenciar a color de `myCar`. Luego, usa la variable dentro `[]` para asignar un nuevo valor a la propiedad de `myCar`.
3. Utiliza la misma variable y asigna una nueva propiedad string, por ejemplo `enVenta`. Usa los `[]` otra vez para asignar un nuevo valor a `enVenta` para indicar si el auto está disponible para la venta.
4. Muestra en consola el `hacer` y `modelo`.
5. Muestra en consola el valor de `enVenta`.

### Trabajando con objetos y arrays
Cuando trabajamos con objetos y arrays, a menudo estarán combinados.

### Objetos en objetos
Veamos el objeto company(compañía). Esta company tiene un address(dirección). Y este address es otro objeto. Si damos nuestra address estamos usando un objeto dentro de un objeto:
```javascript
let company = { companyName: "Healthy Candy",
                activity: "food manufacturing",
                address: {
                    street: "2nd street",
                    number: "123",
                    zipcode: "33116",
                    city: "Miami",
                    state: "Florida"
                },
                yearOfEstablishment: 2021
            };
```

Así como puedes ver, nuestro objeto `company` tiene un address de tipo objecto. Esto puede ir a niveles mucho más profundos de lo necesario.

Para modificar una de las propiedades de address aqui, podemos hacerlo de las siguientes maneras:

```javascript
company.address.zipcode = "33117";
company["address"]["number"] = "100";
```

### Arrays en objetos
Nuestro objeto company podría tener un rango de actividades en vez de uno. Podemos reemplazar la actividad de nuestro previo ejemplo con un array:

```javascript
company = { companyName: "Healthy Candy",
            activities: ["food manufacturing","improving kids' health", "manufacturing toys"],
            address: {
                street: "2nd street",
                number: "123",
                zipcode: "33116",
                city: "Miami",
                state: "Florida"
            },
            yearOfEstablishment: 2021
        };
```

Hemos usado un array en nuestro objeto company. Puedes simplemente usar el `[]` para obtener el valor de dicho array mencionando primero a la propiedad:

`let activity = company.activities[1];`

Aquí podemos llamar al objeto del cual estamos interesados, luego el array, `activities`, con la referencia para la posición del index, el cual es 1.

### Objetos en arrays
También es posible que en vez de una dirección(address), nuestra company tenga una lista de address. Podemos lograr esto creando un array de objetos. En este caso:

```javascript
let addresses = [{
        street: "2nd street",
        number: "123",
        zipcode: "33116",
        city: "Miami",
        state: "Florida"
    },
    {
        street: "1st West avenue",
        number: "5",
        zipcode: "75001",
        city: "Addison",
        state: "Texas"
    }];
```

Entonces, los arrays pueden ser recuperados con `[]` y luego la propiedad que necesitemos:
`let streetName = addresses[0].street;`

### Objetos en arrays en objetos
Solamente para mostrar que esto también es posible. Vamos a agregar a este array de address de objetos a nuestro objeto company:

```javascript
company = { companyName: "Healthy Candy",
    activities: [ "food manufacturing","improving kids' health","manufacturing toys"],
    address: [{
        street: "2nd street",
        number: "123",
        zipcode: "33116",
        city: "Miami",
        state: "Florida"
        },
        {
        street: "1st West avenue",
        number: "5",
        zipcode: "75001",
        city: "Addison",
        state: "Texas"
    }],
    yearOfEstablishment: 2021
};
```

Y para acceder a uno de ellos:

`let streetName = company.address[0].street;`

Como puede verlo, podemos seguir este orden de manera indefinida para lograr alcanzar el valor que necesitemos

#### Ejercicio 3.5
1. Crear un objeto llamado persona que contenga un array vacío llamado `amigos`.
2. Crear tres variables, cada una conteniendo un objeto, que contiene uno de los primeros nombres, apellidos y ID.
3. Agregar los tres amigos al array `amigos`.
4. Muestra en consola.

#### Proyecto 3
Toma el siguiente array:

```javascript
const theList = ['Laurence', 'Svekis', true, 35, null, undefined,
{test: 'one', score: 55}, ['one', 'two']];
```

Manipula tu array usando varios métodos, tales como `pop(), push(), shift(), unshift()`, y transforma en lo siguiente:

`["FIRST", "Svekis", "MIDDLE", "hello World", "LAST"]`

Puedes tomar los siguientes pasos o adoptar tu solución:
- Remover el primer y último ítem
- Agregar `FIRST` al inicio del array
- Asignar `hello World` para el cuarto valor de item
- Asignar `MIDDLE` para el tercer index
- Add `LAST` a la última posición del array
- Mostrar la salida en consola

##### Catálogo de productos de una compañía
En este proyecto, vas a implementar una estructura de datos para el catálogo de un producto y crear consultas para traer los datos.
1. Crear un array para guardar el inventario que almacena los items
2. Crear tres items, cada uno teniendo como propiedades el nombre, modelo, costo y cantidad
3. Agrega los tres items en el array principal usando un método de array, luego muestra en consola el inventario
4. Accede a ka cabtudad del tercer item, luego muestra en consola. Experimenta agregand y accediento a más elementos dentro de tu estructura de datos

#### Quiz 2
1. ¿Puedes usar `const` para actualizar los valores dentro de un array?
2. ¿Cuál es la propiedad en un array que da el número de items contenidos en un array?
3. ¿Cuál es la salida en consola?: 
```javascript
    const myArr1 = [1,3,5,6,8,9,15];
    console.log(myArr1.indexOf(0));
    console.log(myArr1.indexOf(3));
```
4. ¿Como se puede reemplazar el segundo elemento en un array `myArr = [1,3,5,6,8,9,15]` con el valor 4?
5. ¿Cuál es la salida en consola?
```javascript
const myArr2 = [];
myArr2[10] = 'test'
console.log(myArr2);
console.log(myArr2[2]);
```
6. ¿Cuál es la salida en consola?
```javascript
const myArr3 = [3,6,8,9,3,55,553,434];
myArr3.sort();
myArr3.length = 0;
console.log(myArr3[0]);
```

## Capítulo 4 - Sentencias lógicas
En este capítulo vamos a ver los siguientes temas:

- Sentencias if y else
- else if
- Operadores condicionales ternarios
- sentencias switch

### Sentencias if y else
Podemos tomar decisiones en nuestro código usando if else. Es muy simple con esta plantilla:

**if *algunacondicion* es true, entonces cierta acción pasará, else otra acción pasará**

Por ejemplo, si está lloviendo, abriré el paraguas, sino voy a dejar el paraguas en casa:

```javascript
let rain = true;
if(rain){
    console.log("** Trayendo mi paraguas **");
} else {
    console.log("** Puedo dejar el paraguas en casa **");
}
```

En este caso se mostrará:

`** Trayendo mi paraguas **`

Empezamos con if, después de esto, tenemos el `()`, y escribimos algo dentro de él. Cualquier cosa dentro de ellos será convertido a Boolean**. Si el valor es true, se ejecutará el bloque a continuación.
El siguiente bloque es opcional, el else. Y solamente será ejecutado cuando la expresión del else sea falsa. Si no hay else el programa igual continuará funcionando.

```javascript
if(expression) {
// código asociado del bloque if
// solamente será ejecutado si la expression es true
} else {
// código asociado del bloque else
// no necesitamos el bloque else, es opcional
// solamente será ejecutado si la expression es false
}
```

Otro ejemplo. Si la edad es menor que 18, mostrar en consola que el acceso es prohibido, en caso contrario, la persona podrá entrar:

```javascript
if(age < 18) {
    console.log("Lo siento, pero no puedes entrar si eres menor de 18");
} else {
    console.log("Bienvenido/a!");
}
```

Hay un error común en la codificación del if. Si tengo hecho el siguiente bloque:

```javascript
let hobby = "dancing";
if(hobby = "coding"){
    console.log("** I love coding too! **");
} else {
    console.log("** Can you teach me that? **");
}
```

Mostrará en consola
`** I love coding too! **`

¿Por qué crees que pasa esto?

#### Ejercicio 4.1
1. Crea una variable con un valor Boolean
2. Muesrta el valor de la variable en consola
3. Revisa si la variable está true y si lo es, mostrar un mensaje en consola, usando lo siguiente:
```javascript
if(myVariable){
    //action
}
```
4. Agrega otra sentencia con el `!` en frente de la variable para revisar si la condición `no` es true, y crea un mensaje que mostrar el mensaje en consola. Deberías tener dos sentencias, una con el `!` y otra sin ella. Puedes tambieén agregar un if y else.
5. Cambia la variable por su opuesto para ver el resultado.

### Sentencia else if
Esta es una variación del else, ejemplo:
```javascript
let age = 10;
let cost = 0;
let message;
if (age < 3) {
    cost = 0;
    message = "Access is free under three.";
} else if (age >= 3 && age < 12) {
    cost = 5;
    message ="With the child discount, the fee is 5 dollars";
} else if (age >= 12 && age < 65) {
    cost = 10;
    message ="A regular ticket costs 10 dollars.";
} else {
    cost = 7;
    message ="A ticket is 7 dollars.";
}
console.log(message);
console.log("Your Total cost "+cost);
```

¿Dónde crees que entrará?

Otro ejemplo:
```javascript
if(age < 3){
    console.log("Access is free under three.");
} else if(age < 12) {
    console.log("With the child discount, the fee is 5 dollars");
} else if(age < 65) {
    console.log("A regular ticket costs 10 dollars.");
} else if(age >= 65) {
    console.log("A ticket is 7 dollars.");
}
```

#### Ejercicio 4.2
1. Crear usando `prompt()` para preguntar la edad
2. Convertir la respuesta de prompt a un número
3. Declarar un variable message que sirva para guardar el mensaje en consola para el usuario
4. Si el input edad es igual o mayor a 21, escribir en message "mostrar tu cédula para comprar alcohol"
5. Si el input edad es igual o mayor que 19, escribir en message "mostrar tu cédula pero tienes prohibido comprar alcohol"
6. Poner por defecto un else para escribir en message "la variable no es true"
7. Muestra la respuesta de message en la consola

### Operador condicional ternario
La sintax es asi:

`operand1 ? operand2 : operand3;`

Si operand1 es verdadero entonces se hace operand2, sino se hace operand3

Ejemplo:
`let access = age < 18 ? "prohibido" : "permitido";`

también así:

`age < 18 ? console.log("prohibido") : console.log("permitido");`

#### Ejercicio 4.3
1. Crear un valor Boolean paraun ID
2. Usar el operador ternario, crear una variable message que revisará si su ID es valido y también permitir a una persona en un lugar o no
3. Mostrar el contenido de message en consola

### Sentencia switch
if y else son buenos para evaluar condiciones booleanas. Hay otras formas de hacer lo mismo, pero en algunos casos, es mejor reemplazarlos con un switch.

Ejemplo:

```javascript
if(activity === "Get up") {
    console.log("It is 6:30AM");
} else if(activity === "Breakfast") {
    console.log("It is 7:00AM");
} else if(activity === "Drive to work") {
    console.log("It is 8:00AM");
} else if(activity === "Lunch") {
    console.log("It is 12.00PM");
} else if(activity === "Drive home") {
    console.log("It is 5:00PM")
} else if(activity === "Dinner") {
    console.log("It is 6:30PM");
}
```

Esto podría ser reemplazado por switch:

```javascript
switch(expression) {
    case value1:
        // code to be executed
        break;
    case value2:
        // code to be executed
        break;
    case value-n:
        // code to be executed
        break;
}
```

Ejemplo reescrito:

```javascript
switch(activity) {
    case "Get up":
        console.log("It is 6:30AM");
    break;
    case "Breakfast":
        console.log("It is 7:00AM");
        break;
    case "Drive to work":
        console.log("It is 8:00AM");
        break;
    case "Lunch":
        console.log("It is 12:00PM");
        break;
    case "Drive home":
        console.log("It is 5:00PM");
        break;
    case "Dinner":
        console.log("It is 6:30PM");
        break;
}
```

Mostrará:

`It is 12:00PM`

### El caso default

```javascript
switch(expression) {
    case value1:
        // code to be executed
        break;
    case value2:
        // code to be executed
        break;
    case value-n:
        // code to be executed
    break;
    default:
        // code to be executed when no cases match
        break;
}
```
En default es como el else de if, cuando no se puedan evaluar ninguno de los casos, entra:

Ejemplo:

```javascript
switch(activity) {
    case "Get up":
        console.log("It is 6:30AM");
        break;
    case "Breakfast":
        console.log("It is 7:00AM");
        break;
    case "Drive to work":
        console.log("It is 8:00AM");
        break;
    case "Lunch":
        console.log("It is 12:00PM");
        break;
    case "Drive home":
        console.log("It is 5:00PM");
        break;
    case "Dinner":
        console.log("It is 6:30PM");
        break;
    default:
        console.log("I cannot determine the current time.");
        break;
}
```

Mostrará:
`I cannot determine the current time.`

Ejercicio 4.4
Como vimos al principio, existe la biblioteca `Math.random()` que retorna un número aleatorio en el rango de 0 a 1, incluido el 0 pero no no1. Puedes escalar eso con un rango deseado y el resultado pasarlo por `Math.floor()` para redondear.

Ejemplo:

```javascript
// random number between 0 and 1
let randomNumber = Math.random();
// multiply by 10 to obtain a number between 0 and 10
randomNumber = randomNumber * 10;
// removes digits past decimal place to provide a whole number
randomNumber = Math.floor(randomNumber);
```
En este ejercicio, vamos a crear una Mágica bola 8 con respuestas aleatorias
1. Empieza seteando la variable un valor random. El valor asignado será generando números de 0 a 5, con posibles 6 resultados. Puedes incrementar el valor de este número.(No olvides redondear)
2. Crear una variable respuesta que diga "algo ha ido mal"
3. Crear un prompt que diga "Pregúntame lo que quieras"
4. Crear una variable pregunta y almacena la respuesta del paso 3
5. Crear 6 respuestas usando switch, usa la variable del paso 2
6. Crear una variable salida que diga "Me preguntaste " + pregunta + ". Pienso que la respuesta es " + respuesta
7. Usa template string `${}` en vez de concatenar en el paso 6
8. Mostrar en consola el resultado.

### Combinando casos

```javascript
switch(grade){
    case "F":
    case "D":
        console.log("You've failed!");
        break;
    case "C":
    case "B":
        console.log("You've passed!");
    break;
    case "A":
        console.log("Nice!");
        break;
    default:
        console.log("I don't know this grade.");
}
```

Aunque es más legible usar el if-else:

```javascript
if(grade === "F" || grade === "D") {
    console.log("You've failed!");
} else if(grade === "C" || grade === "B") {
    console.log("You've passed!");
} else if(grade === "A") {
    console.log("Nice!");
} else {
    console.log("I don't know this grade.");
}
```

#### Ejercicio 4.5
1. Crear una variable llamada `prize` y usa un prompt para preguntar al usuario y setear la variable con un número del 0 al 10
2. Convertir la respuesta del prompt a tipo number
3. Crear una variable para usar como salida de mensaje conteniendo el valor "Mi selección es: "
4. Usar el switch (y tu creatividad:stuck_out_tongue_winking_eye:), proveer una respuesta correspondiente al premio dependiendo del número seleccionado
5. Usar el `break` del switch para agregar y combinar premios
6. Mostrar un mensaje de respuesta concatenando el premio

#### Proyecto 4
##### Evaluando el número del juego
Pregunta al usuario para que ingrese un número y revisar si este número es mayo que, igual que, o menor que un número dinámico en tu código. Muestra el resultado del usuario en consola.

#### Juego del "friend checker"
Pregunta al usuario para que ingrese un nombre, usando switch para retornar una confirmación que el usuario es un amigo si el nombre seleccionado es conocido en los casos. Puedes agregar una respuesta por defecto en donde no se sabe que persona es debido a que el nombre es desconocido. Muestra en consola.

#### Juego de "Piedra, papel y tijeras" (Hard level -  inténtalo y pruébate de lo que eres capaz :muscle:)
Este juego es de un jugador contra la computadora, si ambos harán selecciones aleatorias de piedra, papel o tijera (alternativamente puedes crear una versión real). La piedra puede romper la tijera, el papel puede tapar la roca y la tijera cortar el papel. Puedes usar Javascript para crear este juego, aplicando lógica con todo lo aprendido. Este proyecto tiene un poco más de dificultad, aquí te dejo algunas sugerencias:
1. Crear un array conteniendo las variables, piedra, papel y tijeras
2. Setear una variable que genera números aleatorios 0-2 para el jugador y hacer lo mismo para la selección de la computadora. El número representa el index en el array de los 3 items
3. Crear una variable para almacenar la respuesta para el usuario. Este puede mostrar el resultado aleatorio para el jugador y luego el resultado para la computadora, luego el match del item
4. Crear una condición para manejar las selecciones del jugador y computadora. Si ambos son lo mismo, el resultado es un empate
5. Usa condiciones para aplicar la lógica del juego y retornar los resultados correctos
6. Agrega un nuevo mensaje de salida que muestra la selección del jugador versus la computadora y el resultado del juego

#### Quiz
1. ¿Qué se mostrará en la consola?

```javascript
const q = '1';
switch (q) {
    case '1':
        answer = "one";
        break;
    case 1:
        answer = 1;
        break;
    case 2:
        answer = "this is the one";
        break;
    default:
        answer = "not working";
}
console.log(answer);
```

2. ¿Qué se mostrará en la consola?

```javascript
const q = 1;
switch (q) {
    case '1':
        answer = "one";
    case 1:
        answer = 1;
    case 2:
        answer = "this is the one";
    break;
    default:
        answer = "not working";
}
console.log(answer);
```

3. ¿Qué se mostrará en la consola?

```javascript
let login = false;
let outputHolder = "";
let userOkay = login ? outputHolder = "logout" : outputHolder = "login";
console.log(userOkay);
```

4. ¿Qué se mostrará en la consola?

```javascript
const userNames = ["Mike", "John", "Larry"];
const userInput = "John";
let htmlOutput = "";
if (userNames.indexOf(userInput) > -1) {
    htmlOutput = "Welcome, that is a user";
} else {
    htmlOutput = "Denied, not a user ";
}
console.log(htmlOutput + ": " + userInput);
```
5. ¿Qué se mostrará en la consola?

```javascript
let myTime = 9;
let output;
if (myTime >= 8 && myTime < 12) {
    output = "Wake up, it's morning";
} else if (myTime >= 12 && myTime < 13) {
    output = "Go to lunch";
} else if (myTime >= 13 && myTime <= 16) {
    output = "Go to work";
} else if (myTime > 16 && myTime < 20) {
    output = "Dinner time";
} else if (myTime >= 22) {
    output = "Time to go to sleep";
} else {
    output = "You should be sleeping";
}
console.log(output);
```

6. ¿Qué se mostrará en la consola?

```javascript
let a = 5;
let b = 10;
let c = 20;
let d = 30;
console.log(a > b || b > a);
console.log(a > b && b > a);
console.log(d > b || b > a);
console.log(d > b && b > a);
```

7. ¿Qué se mostrará en la consola?

```javascript
let val = 100;
let message = (val > 100) ? `${val} was greater than 100` :
`${val} was LESS or Equal to 100`;
console.log(message);
let check = (val % 2) ? `Odd` : `Even`;
check = `${val} is ${check}`;
console.log(check);
```

## Capítulo 5 - Loops
Estamos empezando a comprender mejor a Javascript. Este capítulo se enfocará en algo muy importante, el control del flujo: loops(bucles). Los loops ejecutan bloques de código un cierto número de veces. Podemos usar loops para hacer muchas cosas, como repetir operaciones cada tanto o iterar sobre datasets, arrays y objetos.

En este capítulo vamos a ver los siguientes temas:
- `while`
- `do while`
- `for`
- `for in`
- `for of`

### while loops
El primer loop que vamos a ver es el **while loop**. Un `while` ejecuta un cierto bloque de código siempre y cuando una expresión sea `true`, ejemplo:

```javascript
while (condition) {
// code that gets executed as long as the condition is true
}
```

Un ejemplo más real:

```javascript
let i = 0;
while (i < 10) {
    console.log(i);
    i++;
}
```

En consola:
```
1
2
3
4
5
6
7
8
9
```

Estos tres pasos está ocurriendo aquí:
1. Se crea la variable `i`, se asigna a `0`;
2. Se inicia el `while` y se verifica si la condición de `i < 10` sea `true`;
3. Si la condición es `true`, el código muestra el valor de `i` en consola, luego se incrementa el valor en `1`;
4. La condición es evaluada de vuelta; 1 sigue siendo menos que 10;
5. La condición es de vuelta `true`, se muestra en consola el valor de `i`, luego se incrementa el valor en `1`;
6. Cuando la variable `i` llegue a `10`, la condición ya no será válida porque `i(10) < 10`, i que vale 10 no es mayor que 10;
7. El bucle termina.

Usando un array:

```javascript
let someArray = ["Mike", "Antal", "Marc", "Emir", "Louiza", "Jacky"];
let notFound = true;
while (notFound && someArray.length > 0) {
    if (someArray[0] === "Louiza") {
        console.log("Found her!");
        notFound = false;
    } else {
        someArray.shift();
    }
}
```

La salida en consola es:
```
Found her!
false
```

¿Por qué crees que el `&& someArray.length > 0` se agregó en la condición del `while`? Si no lo hacemos quedaremos atascados en algo llamado bucle infinito, entonces nos aseguramos que mientras `notFound` sea `true` el array vaya siendo descontado de a uno usando `.shift()`, en algún momento se acabarán los elementos del array o si se encuentra antes un elemento que sea válido en el if, la condición `notFound` sea falsa.

Podríamos seguir haciendo cosas más sofisticadas fácilmente con bucles. Veamos que tan fácil es llenar un array usando la *secuencia de Fibonacci*:

```javascript
let nr1 = 0;
let nr2 = 1;
let temp;
fibonacciArray = [];
while (fibonacciArray.length < 25) {
    fibonacciArray.push(nr1);
    temp = nr1 + nr2;
    nr1 = nr2;
    nr2 = temp;
}
```

En consola:
```
[
0,
1,
1,
2,
3,
5,
8,
13,
21,
34,
55,
89,
144,
233,
377,
610,
987, 1597, 2584, 4181,
6765, 10946, 17711, 28657, 46368
]
```

#### Ejercicio 5.1
En este ejercicio vamos a crear un juego para adivinar el número que toma el ususario y responder basado en qué tan preciso el usuario fue.
1. Crear una variable para almacenar el valor max del número a adivinar.
2. Crear una variable para almacenar un valor random usando `Math.floor(Math.random() * max) + 1`.
3. Si hace falta, mostrar en consola para ver como genera el paso 2.
4. Crear una variable para ser utilizada como seguimiento si la respuesta es correcta o no y setearlo como Boolean false. Podemos actualizarlo a true si el usuario acierta.
5. Usar el `while` para iterar un prompt que pregunte al usuario para que ingrese un número entre 1 y 5, convierta a Number para compararlo con el número random.
6. Dentro del `while`, revisar si está usando una condición si el valor del prompt es igual a la solución. Aplicar la lógica que si el número es correcto, puedes setear el status de true y romper el while. Proveer al jugado alguna pista de como adivinar, si ha sido alto o bajo, e iniciar otro propmt hasta que el usuario haya adivinado correctamente. De esta manera podemos usar un loop para mantener preguntando hasta que la solución sea correcta, y en ese punto poder para la iteración de nuestro código.

### do while
En algunos casos, necesitamos ejecutar el bloque de código almenos una vez. Por ejemplo, si necesitamos validar el input de un usuario, hay que preguntar al menos una vez. Tambié si querer conectarnos a una base de datos o alguno recurso externo. Ejemplo:

```javascript
do {
// code to be executed if the condition is true
} while (condition);
```

Un ejemplo con prompt:

```javascript
let number;
do {
    number = prompt("Please enter a number between 0 and 100: ");
} while (!(number >= 0 && number < 100));
```

La salida será:

```
Please enter a number between 0 and 100: > -50
Please enter a number between 0 and 100: > 150
Please enter a number between 0 and 100: > 34
```

#### Ejercicio 5.2
En este ejercicio vamos a crear un contador básico que incrementa dinámicamente una variable consistiendo en un valor
1. Inicia una variable contado con 0
2. Crear una variable, step, para incrementar tu contador
3. Agrega al `do while`, imprimiento el contador para la consola incrementando el step en cada loop
4. Continuar el loop hasta que el contador sea igual a 100 o mayor a 100.

### for loops
**for loops** son un tipo especial de bucle. La sintaxis podría ser un poco confusa al principio, pero solo al principio. En realidad son muy útiles.

Un ejemplo:

```javascript
for (initialize variable; condition; statement) {
// code to be executed
}
```

Dentro de los paréntesis del `for`, hay tres partes separadas por `;`. Lo primero inicializa las variables que pueden ser usadas dentro del `for loop`. Lo segundo es una condición: si la condición es `true`, entonces el loop continuará. Esta condición será revisada despues de la inicialización de las variables antes de la primera interación (siempre será así cuando la condición evaluada sea `true`). Por último está la sentencia `i++`, esto se ejecutará en cada iteración:
1. Inicialización de variables
2. Revisa la condición
3. Si la condición es `true`, ejecuta el bloque de código. Si la condición es `false`, terminará el loop
4. Se ejecuta la sentencia (la tercera parte, por ejemplo `i++`)
5. Vuelve al paso 2

Un ejemplo:
```javascript
for (let i = 0; i < 10; i++) {
    console.log(i);
}
```

Esto mostrará en consola:

```javascript
[
    0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11,
    12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23,
    24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35,
    36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47,
    48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59,
    60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71,
    72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83,
    84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95,
    96, 97, 98, 99
]
```

También podemos crear un array conteniendo solamente valores pares:
```javascript
let arr = [];
for (let i = 0; i < 100; i = i + 2) {
    arr.push(i);
}
```

Resultando en este array:
```javascript
[
    0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20,
    22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42,
    44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64,
    66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86,
    88, 90, 92, 94, 96, 98
]
```

Muy comúnmente, veras `i++` en la tercera parte del loop, pero toma nota que tu puedes escribir cualquier sentencia aqui. En este caso estamos usando `i = i + 2` para agregar 2 al valor previo cada tanto, creando un array con números pares.

#### Ejercicio 5.3
En este ejercicio vamos a usar un `for loop` para crear un array que almacena objetos. Empezando por crear un array vacío, el bloque de código del loop va crear un objeto que sea insertado en el array.
1. Crear un array vacio `myWork`.
2. Usar el `for loop`, crear una lista de 10 objetos, cada objeto tendra numerado (Lección 1, Lección 2, Lección 3...) con una alternativa `status` que sea `true/false` para cada item indicando si la lección será este año, por ejemplo: `name: "Leccion 1", status: true`
3. Puedes especificar el status usando el operador ternario para revisar si la lección está activa o no.
4. Push del objeto en `myWork`.
5. Mostrar en consola.