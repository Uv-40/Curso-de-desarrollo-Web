<div align="center">
  <h1> Curso de Desarrollo Web Online</h1>
  <p> El contenido de este documento son los apuntes realizados del curso de desarrollo web online dictado por @Leonidas Esteban en @Platzi.</p>
</div>

# Tabla de contenido
- [HTML](#HTML)
    - [DOM](#DOM)
    - [Etiquetas](#etiquetas)
    - [Atributos HTML](#atributos-HTML)
    - [Formularios HTML](#formularios-HTML)
    - [Navegación entre secciones](#Navegación-entre-secciones)
- [Programación Dinámica](#Programación-Dinámica)
    - [Introducción a la Programación Dinámica](#Introducción-a-la-Programación-Dinámica)
    - [Optimización de Fibonacci](#Optimización-de-Fibonacci)
   
# HTML

## DOM

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

## Nevgación entre secciones

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
