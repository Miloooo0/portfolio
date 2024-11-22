+++
title = "Markdown"
date = "2024-11-20"
author = "Milad Al Chihabi"

description = "Guia básica de Markdown"
tags = [
    "markdown",
    "css",
    "html",
    "temas",
]
categories = [
    "Temas",
    "Sintaxis",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]
image = "pawel-czerwinski-8uZPynIu-rQ-unsplash.jpg"
+++

Este artículo ofrece un ejemplo de la sintaxis básica de Markdown que se puede utilizar en archivos de contenido de Hugo, una explicación de los recursos que he empleado para desarrollar esta misma página.

## Headings

Los siguientes elementos HTML del `<h1>` a `<h6>` representan seis niveles de encabezados o headers. `<h1>` es el nivel más alto, mientras que `<h6>` es el más bajo.

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Texto en Negrita y Cursiva

Markdown permite dar formato al texto con negrita y cursiva utilizando asteriscos (*) o guiones bajos (_). De modo que la sintaxis para introducir un texto en cursivaa sería:
<br>

`*Texto*` - **Texto en negrita** <br>
`_Texto_` - _Texto en cursiva_ <br>
`***Texto***` - ***Texto en negrita y cursiva***


## Remarcado

Podemos remarcar parte del texto empleando el acento invertido "\`". De modo que si queremos hacer incapié en una palabra o grupo de palabras bastaría con ponerlas entre dos de estos caracteres como en este `ejemplo`.

## Cita
Podemos incluir texto a modo de cita o _blackquote_ incluyendo el carácter "\>" antes de la línea a citar.
> Este es un ejemplo de texto citado.

Además de esto, podemos incluir una atribución de la cita, empleando lo siguiente.
```
> — <cite>Persona citada</cite>
```

## Tablas

Las tablas no forman parte de Markdown como tal pero si que son soportadas por Hugo de forma nativa y se implementan dibujando de manera casi literal las tablas.

   Nombre | Edad
----------|------
 Manuel   | 27
  Milad   | 20

```
    Nombre | Edad
-----------|------
  Manuel   | 27
   Milad   | 20
```
## Bloques de Código con Backticks

Con Markdown, podemos crear bloques de código con el uso de backticks o acentos invertidos,
para ello, basta con poner el texto que queremos que se vea en el bloque de código entre 3 de los mismos. Además, se puede incluir un nombre de idioma para el bloque de código, para ello, basta con
agregarle al final el nombre despues de los primeros acentos, como en el siguiente ejemplo:

\```html codigo```

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Ejemplo</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

## Listas

#### Listas Ordenadas
Se pueden crear listas ordenadas colocando el numero de posición seguido de un punto y el elemento.

1. Crear el Virtual Host en Sites-Available 
2. Activar el Virtual Host con a2ensite
3. Agregar la dirección al archivo hosts del sistema en etc/hosts

#### Listas Independientes del Orden
Se pueden crear listas "desordenadas" colocando asteriscos o guiones antes del texto del elemento.

* Intel i5-8300H
* NVIDIA GeForce GTX 1050
* 16 GB de RAM

#### Listas Anidadas
Se pueden crear listas anidadas colocando asteriscos o guiones antes del texto del elemento y segun la identación,
será un elemento independiente o hijo del anterior.

* Fruta
  * Manzanas
  * Naranjas
  * Platanos
* Basico
  * Leche
  * Pan de Molde

## Otros elementos — abbr, sub, sup, kbd, mark
Todas estas etiquetas se emplean con la siguiente sintaxis:
\<etiqueta>texto\</etiqueta>

Texto abreviado o siglas (abbr): <abbr title="Graphics Interchange Format">GIF</abbr> es un formato gráfico para imágenes y animaciones.

Subíndice (sub): CO<sub>2</sub> 

Superíndice (sup): X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Teclas (kbd): <kbd>CTRL</kbd> + <kbd>F</kbd> para buscar dentro de la página.

Remarcado (mark): Algunos dispositivos emplean la arquitectura <mark>ARM64</mark>.

## Videos de YouTube
Se pueden insertar videos de YouTube con el uso de shortcodes, para ello, basta con poner entre corchetes el nombre del shortcode previamente creado y luego el id del video que queremos insertar.

{{< youtube hjD9jTi_DQ4 >}}

<br>


## Imágenes en línea con enlaces
Usando markdown, podemos insertar imágenes en línea con un enlace a la imagen, para ello, basta con poner el texto que queremos que se vea en el enlace entre corchetes y luego el enlace al archivo de la imagen entre parentesis. En adición se puede incluir despues de este enlace entre parentesis el enlace a la página web.

Este sería el código markdown para insertar una imagen en línea con un enlace a la imagen.

`[![facebookImagen](https://www.almoradi.es/wp-content/uploads/2022/02/Facebook-logo-1.png)](https://www.facebook.com)`

[![facebookImagen](https://www.almoradi.es/wp-content/uploads/2022/02/Facebook-logo-1.png)](https://www.facebook.com)

