+++
author = "Milad Al Chihabi"
title = "Lo más básico de Java"
date = "2024-11-22"
description = "Pequeña guía de Java para principiantes"
categories = [
    "Programación",
    "Sintaxis",
]
tags = [
    "Java",
    "Programación",
    "Guía"
]
image = "orbtal-media-1td5Iq5IvNc-unsplash.jpg"
+++
## Introducción a Java 
Java es un lenguaje de programación orientado a objetos, multiplataforma y ampliamente utilizado para desarrollar aplicaciones de escritorio, web y móviles.

Java se maneja empleando clases, una clase es una plantilla para crear objetos, si no has entendido nada, lo entiendo, pero para que me entiendas, una clase es ese fragmento de código donde vamos a meter el código que queremos ejecutar.

Una clase tiene un nombre y un nivel de privacidad del que hablaremos más adelante.

Crearemos una clase con un nombre cuya primera letra tiene que estar en mayúsculas, por temas te funcionamiento y practicas correctas de programación. Si queremos que nuestro programa principal este dentro de esta clase, declararemos la función 
`public static void main(String[]){}` y el codigo de nuestro programa irá dentro de los corchetes.

## Salida de Datos
Para poder sacar datos por pantalla, vamos a necesitar usar `System.out.println()`. Dentro de los paréntesis y entre comillas incluiremos el texto a mostrar.

## Hola Mundo
Para crear nuestro programa Hola Mundo, necesitamos crear una clase llamada HolaMundo, para ello, crea un archivo .java en el que declaremos la clase.
```java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("¡Hola mundo!");
    }
}
```
Listo! Ya tenemos nuestro primer programa funcional en Java.

## Variables y Tipos de Datos
En Java tenemos 4 tipos primitivos, es decir, las variables pueden ser:
 - `int` (Enteros)
 - `double` (Decimales)
 - `char` (Caractéres)
 - `boolean` (Booleanos)

Por otro lado tenemos las cadenas de texto, que son Objetos, elemento que explicaremos más adelante.
 - String (Cadenas de texto)

```java
int edad = 30;
double altura = 1.75;
char inicial = 'A';
boolean esEstudiante = true;
String nombre = "Juan";
```

## Operadores
Existen los siguientes operadores:
- Aritméticos: 
    - `+` más
    - `-` menos
    - `*` por
    - `/` entre
    - `%` módulo, es decir, resto de una división
- Relacionales
    - `==` 
    
    Es un operador de comparación, no de asignación, es decir, que `x == 3` no asigna el valor "3" a "x" sino que comprueba si x tiene el valor 3 y devuelve true o false al evaluarlo.
    - `!=`

    Este operador es el inverso al anterior, es decir, que comprueba si dos elementos son diferentes, mientras que el anterior comprueba si son iguales.
    - `<`

    Este operador comprueba si un elemento es menor que otro.
    - `>`

    Este operador comprueba si un elemento es mayor que otro.
    - `<=`

    Este operador comprueba si un elemento es menor o igual que otro.
    - `>=`

    Este operador comprueba si un elemento es mayor o igual que otro.


- Lógicos
    - `&&` corresponde con la Y lógica
    - `||` corresponde con la O lógica
    - `!`  corresponde con la negación lógica
```java
int x = 10;
int y = 5;
boolean resultado = x > y && y < 10;
```

## Estructuras de Control
 - Condicionales: 
    - if
    - else if
    - else.
 - Bucles
    - for
    - while
    - do-while.
```java
if (edad >= 18) {
    System.out.println("Eres mayor de edad.");
} else {
    System.out.println("Eres menor de edad.");
}

for (int i = 0; i < 5; i++) {
    System.out.println("Iteración: " + i);
}
```

## Arrays
Un `array` es una colección de elementos de un mismo tipo, por ejemplo, un array de enteros, o un array de cadenas de texto.

```java
int[] numeros = {1, 2, 3, 4, 5};
```

## Clases y Objetos
Las clases son simplemente plantillas para crear objetos y los objetos son instancias de una clase.

```java
public class Perro {
    String nombre;
    int edad;

    public void ladrar() {
        System.out.println("¡Guau!");
    }
}
```

```java
// Crear un objeto
Perro miPerro = new Perro();
miPerro.nombre = "Fido";
miPerro.ladrar();
```
## Encapsulación

Ocultar la implementación: Hacer los atributos privados y proporcionar métodos públicos (getters y setters) para acceder a ellos.

## Herencia

Crear jerarquías de clases: Una clase puede heredar atributos y métodos de otra clase (clase padre).

```java
public class Animal {
    public void comer() {
        System.out.println("Comiendo...");
    }
}
```

```java
public class Perro extends Animal {
    public void ladrar() {
        System.out.println("¡Guau!");
    }
}
```

```java
public class Gato extends Animal {
    public void ladrar() {
        System.out.println("¡Miau!");
    }
}
```

## Polimorfismo
Múltiples formas: Un mismo método puede tener diferentes implementaciones en clases hijas.

## Abstracción
Clases abstractas e interfaces: Definen un contrato que las clases hijas deben cumplir.

## Excepciones
Manejo de errores: try, catch, finally.

## Entrada/Salida
Leer y escribir datos: Scanner, PrintWriter.

## Colecciones

Listas, conjuntos, mapas: ArrayList, HashSet, HashMap.

## Ficheros
Leer y escribir en archivos: FileReader, FileWriter.
