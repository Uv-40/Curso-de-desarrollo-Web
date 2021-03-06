<div align="center">
  <h1> Curso de Desarrollo Web Online</h1>
  <p> El contenido de este documento son los apuntes realizados del curso de desarrollo web online dictado por @Leonidas Esteban en @Platzi.</p>
</div>

# Tabla de contenido
- [HTML](#HTML)
    - [DOM](#DOM)
    - [Etiquetas](#etiquetas)
    - [Atributos HTML](#atributos-HTML)
    - [Formularios HTML](#Formularios-HTML)
    - [Navegacion entre secciones](#Navegacion-entre-secciones)
    - [Formas de agregar estilos a HTML](#formas-de-agragar-estilos-a-html)
    - [Reglas selectores declaraciones y css](#Reglas-selectores-declaraciones-y-css)
    - [Los estilos incluidos por el navegador](#Los-estilos-incluidos-por-el-navegador)
    
- [Estilos y CSS](#estilos-y-css)
    - [Unidades de medida y colores](#unidades-de-medida-y-colores)
    - [Introducción a la Programación Dinámica](#Introducción-a-la-Programación-Dinámica)
    - [Optimización de Fibonacci](#Optimización-de-Fibonacci)
   
# HTML

## DOM

## etiquetas

## Formularios HTML

Los formularios en HTML son una unidad para manejar información y permite del envio de información a dueño de web site.

Partes del formulario:
1. Ingreso de datos y modelación de los datos (clase 10)
2. Envío de datos y almacenamiento de los mismos, poner la seguridad y temas sensibles de la información.
 
Los fomularios se crean con la etiqueta '<form></form>'
las esntradas de datos se definen con la etqiqueta '<input></input>' 
   Atributos de input:
     - type="" es el tipo de dato que recoge el campo rn el formulario
     - Placeholder="" es el mensaje que aparece dentro del campo de input
     - Value="" este atributo se puede usar en vez del placeholder para dejar un formato del dato que se debe ingresar ej: @gmail.com
     - Label="" Este genera un texto indicativo al lado del campo para el input ( el label es muy usado cuando se usa un checkbox de input)
El boton se genera con la etiqueta '<button></button>'
 
 ```HTML
<section>
      Sección contacto
      <form action="/Suscripcion/">
        <h3>¿Creamos algo juntos?</h3>
        <input type="email" placeholder="Déjame tu email" />
        <button>Enviar</button>
      </form>
</section>

```

## Navegacion entre secciones

La navegación entre secciones es el enlazamiento de información a otras páginas web o a una seccion dentro de nuestro mismo sitio web.

Los enlaces se agregan con un atributo de la etiqueta llamado id="", este atributo se agrega en la etiqueta ej: <seccion id="" y por otro lado debe haber un href que nos permita general el origen del enlace, en la etiqueta href="#se coloca el id generado en la etiqueta seccion".

```HTML
<li>
  <a href="#portafolio">Portafolio</a>
</li>
<section id="portafolio">
</section>

```

Si el enlace se quiere hacer a otra página en la etiqueta hash se pone un slash y el nombre de la pagina a direccionar ej: /portafolio/index.html

### Enlace externo

Mediante un etiqueta anchor '''<a  ->< / a >''' y el atributo href="" se pone la url de la página a la que queremos que nos dirija y el atributo target="_blank permite que el enlace se abra en una nueva pestaña si no se usa esta etiqueta en enlace recarga en la misma página la direeción"
 
```HTML
<a href="https://www.youtube.com/watch?v=5f5Ig_U2Bpk&t=11s" target="_blank">Ver platica </a>
```

## Formas-de-agragar-estilos-a-html

Hay tres formas para incluir estilos que definan la apariencia de tu html:

- Estilos en línea: se definen directamente en el elemento html que quieres estilizar, se agregan con el atributo style. No es para nada recomendado ya que Html sirve para definir la estructura y semántica del código y no el aspecto visual, aquí estaríamos mezclando todo.
- Estilos con el tag Style: regularmente este tag se incluye dentro de la etiqueta head del html. Utiliza una etiqueta style. Separa en cierto modo, de una forma menos sucia (por decirlo así). Esta forma sigue sin ser la más recomendada porque seguimos mezclando lo que es el aspecto visual con la estructura y semántica del código.
- Estilos enlazados desde un archivo css externo: utilizando la etiqueta link que nos permite enlazar recursos externos. Utilizando un archivo CSS externo al documento HTML. Esta es la forma más recomendada porque estamos separando totalmente la estructura y semántica con el aspecto visual.

A CSS, se le llama hojas de estilos en cascada porque los estilos que se definen para una página, se van aplicando de arriba hacia abajo, y de lo más general a lo más particular, teniendo prioridad lo más particular. Esto es, los estilos que prevalecen son los que han sido definidos en línea, luego los que fueron definidos mediante la etiqueta style en la cabeza o cuerpo del html, y por último los estilos definidos en archivos externos enlazados con la etiqueta link. Esta prioridad se puede alterar al usar el modificador **!important"" en la definición de algún estilo en particular, aunque esto no es recomendado.


## Reglas selectores declaraciones y css

  - selectores: se usan para identificar un elemento de HTML y poder asignarle un estilo con css(Header, footer, body etc).
      - Selector de etiqueta: utiliza la etiqueta para colocarle un estilo a todo el contenido de la etiqueta.
      - Selector descendente: se debe colocar toda la ruta de etiquetas hasta llegar a la que queremos aplicar algún estilo.
      - Selector de clase: se le asigna una clase a las etiquetas que quemeros seleccionar con css y permite que esta calse aplique a multiples etiquetas
      - Selector de id: se le asigna el id a una etiqueta pero el id si es unico entonces solo se le podria generar un estilo para ese único id
  - declaraciones: son las acciones que se van a realizar con el selector.
  - propiedades: son los atributos que usaremos con el selector.
  - valores: son los inputs que reciben las propiedades.

![reglacss](https://user-images.githubusercontent.com/25805919/102266095-fb54be80-3ee5-11eb-94d9-b02b4ac24a54.png)

# Estilos y css

## Unidades de medida y colores

En css los colores se pueden representar de 3 formas:
  - **Palabras clave:** son atajos con los nombre de los colores (se limta a algunos colores)
  - **Usando hexadecimales o rgb, rgba:** cuando se quiere llegar a colores exactos se utiliza este método.
  - **Usando hls() hlsa():**
  
La unidad de medida por excelencia en el mundo digital son los **pixeles**, un pixel es la menor unidad homogenea de color que forma parte de una imagen digital. los pixeles tambien sirven para **asignar** tamaño a imágenes, texto, bordes, dimensiones, márgenes y rellenos.
