+++
author = "Milad Al Chihabi"
title = "Emojis en Hugo"
date = "2024-11-21" 
description = "Guia de uso de Emojis en Hugo"
categories = [
    "Sintaxis"
]
tags = [
    "Emoji",
]
image = "emojis.jpg"
+++

En Hugo se pueden insertar emojis en contenido de Markdown, para ello, hay diversas opciones.

La función [`emojify`](https://gohugo.io/functions/emojify/) puede ser llamada directamente empleando [Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes).

Para habilitar de manera global los emojis solo hay que darle el valor `true` a `enableEmoji` en el archivo toml o yaml del sitio de Hugo y ya estaría configurado para poder usar shortcodes para el uso de emojis en los archivos de contenido. 

<p><span class="nowrap"><span class="emojify">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙊</span> <code>:speak_no_evil:</code></span></p>
<br>
Se recomienda el uso de sitios como [Emoji cheat sheet](http://www.emoji-cheat-sheet.com/) para obtener los códigos de los emojis.
The [Emoji cheat sheet](http://www.emoji-cheat-sheet.com/) is a useful reference for emoji shorthand codes.

***

**Anotación:** Los pasos de arriba habilitan los emojis en el estándar Unicode en Hugo, sin embargo, el renderizado de estos elementos depende del navegador y la plataforma.