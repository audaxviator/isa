# Overview

La idea es que
* entiendas las piezas fundamentales que intervienen en el renderizado de una página web
* puedas usarlas de forma básica
* aprendas a usar [git](https://git-scm.com/) en el proceso: si vas a hacer diseño web, colaborar eficazmente con el resto del equipo es fundamental

Vamos a usar html y css básico por razones didácticas; en un proyecto moderno probablemente usarás algún framework de css y gran parte del html será generado por algún backend existente, pero hace falta saber lo básico para sacarle partido a estas cosas.

Aquí hay preguntas, no soluciones: resolverlas requerirá buscar cosas en google, experimentar y documentarse. Iremos añadiendo ejercicios sobre la marcha.

* [Preliminares](#preliminares)
* [Ejercicios](#ejercicios)
  * [hello git](#hello-git)
  * [hello css](#hello-css)

## Preliminares

Hay un montón de texto escrito en internet sobre esto, así que voy a ser esquemático y proporcionar links. Una página web usa 3 tecnologías complementarias:

* [html](https://en.wikipedia.org/wiki/HTML), que es un lenguaje para definir el contenido de la página web, eg. los párrafos, títulos, imágenes
  ```html
  <h1>Esto es un título</h1>
  <p>Esto es un párrafo</p>
  ```

* [css](https://en.wikipedia.org/wiki/Cascading_Style_Sheets) que es otro lenguaje para definir la *apariencia* del contenido del html: por ejemplo, puedes usar css para decirle que el texto de los títulos sea azul:
  ```css
  h1 {
      color: blue;
  }
  ```
* [javascript](https://en.wikipedia.org/wiki/JavaScript) que es un lenguaje de programación (a diferencia de los anteriores que no son [turing completos](https://en.wikipedia.org/wiki/Turing_completeness)) que puedes usar para manipular la página de forma arbitraria

Las responsabilidades de los 3 se solapan, y han ido evolucionando. Históricamente, html se usaba tanto para definir el contenido como su presentación; ahora se considera buena praxis usar html sólo para definir contenido y delegar la responsabilidad de la presentación al css. Por otra parte, muchos efectos que antes se conseguían programando en javascript ahora se pueden conseguir usando css.

Vamos a centrarnos únicamente en html y css.

## Ejercicios

### hello git

Git [puede resultar complicado al principio](https://xkcd.com/1597/) pero vamos a empezar por donde no cubre:
* crea una cuenta de [github](https://github.com/) si no tienes una ya
* instálate git en tu máquina
* clona este repo usando git
* asegurate de que tienes un editor de texto apropiado para programar: ante la duda, descárgate [atom](https://atom.io/)

Ahora deberías tener una copia de este repo en local, y un editor de texto con el cual abrir los archivos.

### hello css

Contenido en el directorio [hello_css](hello_css)

Mientras sólo usemos html y css, con el editor y el browser como herramienta de trabajo es suficiente: podemos modificar los archivos de html y css en disco, y ver qué resultado tienen nuestras ediciones navegando por nuestro sistema de archivos.

También vamos a introducir [el inspector del browser](https://developers.google.com/web/tools/chrome-devtools?hl=es): esto es super útil:
* puedes inspeccionar la estructura del css y html de la página que estás viendo
* puedes llevar a cabo cambios de forma interactiva y ver cómo quedan: puedes hacer esto en cualquier página!""

El ejercicio:
* Navega en tu browser directorio de `hello_css` en el repo clonado; depende de tu sistema operativo, por ejemplo en el mío que es un mac está en esta ruta: `file:///Users/miguelsimon/isa/hello_css/index.html`
* Abre el inspector del browser e inspecciona
* Usando el inspector, cambia el css de forma interactiva para que el título aparezca en verde
* Usando el editor, cambia el archivo de css para que el texto del párrafo aparezca en rojo
