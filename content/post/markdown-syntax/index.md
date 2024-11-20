+++
title = "Markdown"
date = "2024-11-20"
description = "Guia básica de Markdown"
tags = [
    "markdown",
    "css",
    "html",
    "themes",
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
#### Inline Markdown within tables

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

| A                                                        | B                                                                                                             | C                                                                                                                                    | D                                                 | E                                                          | F                                                                    |
|----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|------------------------------------------------------------|----------------------------------------------------------------------|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit. | Phasellus ultricies, sapien non euismod aliquam, dui ligula tincidunt odio, at accumsan nulla sapien eget ex. | Proin eleifend dictum ipsum, non euismod ipsum pulvinar et. Vivamus sollicitudin, quam in pulvinar aliquam, metus elit pretium purus | Proin sit amet velit nec enim imperdiet vehicula. | Ut bibendum vestibulum quam, eu egestas turpis gravida nec | Sed scelerisque nec turpis vel viverra. Vivamus vitae pretium sapien |

## Code Blocks

#### Code block with backticks

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

#### Code block indented with four spaces

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Code block with Hugo's internal highlight shortcode
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

#### Diff code block

```diff
[dependencies.bevy]
git = "https://github.com/bevyengine/bevy"
rev = "11f52b8c72fc3a568e8bb4a4cd1f3eb025ac2e13"
- features = ["dynamic"]
+ features = ["jpeg", "dynamic"]
```

## List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

* List item
* Another item
* And another item

#### Nested list

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

## Hyperlinked image

[![Google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_light_color_272x92dp.png)](https://google.com)