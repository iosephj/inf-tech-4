---
title: "Entrada de datos y conversión de tipos"
autor: "José Juarez"
version: "06/07/26"
---

<!-- *** GUIDE START *** -->

## 1. Programas interactivos

Hasta ahora nuestros programas siempre mostraban información en pantalla.

::: example

Ejemplo:

```python
print("Hola")
print(2 + 3)
```

:::

Pero sería mucho más interesante si el programa pudiera hacer preguntas.

Para eso existe la función `input()`.

::: example

Ejemplo:

```python
nombre = input("¿Cómo te llamas? ")

print("Hola", nombre)
```

:::


Si el usuario escribe:

```
Ana
```

la salida será:

```
Hola Ana
```

### ¿Qué hace `input()`?

La función `input()`:

- 1° muestra un mensaje;
- 2° espera que el usuario escriba;
- 3° guarda lo escrito en una variable.

::: example

Ejemplo:

```python
ciudad = input("¿En qué ciudad vives? ")
```

:::

::: activity

### Actividad

Haz los siguientes programas:

**1)** Escribe un programa que pregunte:

  * nombre
  * apellido
  * edad

  Luego muestra los tres datos.


**2)** Escribe un programa que pregunte:

  * nombre del producto
  * precio
  * cantidad comprada

  Luego muestra un resumen con esos datos y el importe total de la compra. ¿Qué falla produce el programa? Esto vamos a resolverlo en el siguiente punto.

:::

## 2. Todo lo que escribe el usuario es texto

Aunque el usuario escriba:

```
25
```

Python lo guarda como si fuera:

```
"25"
```

Es decir, un texto que en Python se llama **string**.

::: example

Observa:

```python
edad = input("Edad: ")

print(edad)
```

Si escribimos:

```
15
```

la variable contiene el texto `"15"`.

:::

**Importante:** Si intentas hacer una operación matemática con el texto `"15"`, por ejemplo sumarle 1, se produce un error como tuviste en el segundo programa de la actividad anterior. 


### Conversión de tipos

Podemos transformar un texto en un número entero.

::: example

Ejemplo

```python
edad = int(input("Edad: "))
```

Ahora sí funcionará:

```python
print(edad + 1)
```

:::

También podemos transformar un texto a un número con decimales:

::: example

Ejemplo

```python
altura = float(input("Altura: "))
```

si escribes 1.72 lo convertirá al número:

```
1.72
```

**Aclaración:** en Python se usa punto para la coma decimal

:::

::: activity

### Actividad

**1)** Ahora resuelve el 2do programa de la actividad del punto anterior

**2)** Escribe un programa que pregunte:

  * nombre del alumno
  * nota del primer examen
  * nota del segundo examen

  Luego calcula y muestra el promedio de las dos notas.


**3)** Escribe un programa que pregunte:

  * nombre;
  * edad;
  * ciudad.

  Luego muestre un mensaje como:

```
Hola Sofía.
Tienes 16 años.
Vives en Mendoza.
Gracias por usar el programa.
```

**4)** Estudia este resumen y las preguntas para pensar. Luego llama al profesor y cuéntale lo que aprendiste.


| Función   | Convierte a    |
| --------- | -------------- |
| `int()`   | entero         |
| `float()` | número decimal |

**Para pensar**

- **a)** ¿Por qué `input()` devuelve texto?
- **b)** ¿Cuándo es necesario usar `int()`?
- **c)** ¿En qué situaciones usarías `float()`?
- **d)** ¿Qué ocurre si intentas sumar un texto y un número?

:::

> Esta guía se aprueba especialmente con el problema **4)** del punto **2**


<!-- *** GUIDE END *** -->



<!-- *** GUIDE AUXILIARY THINGS *** -->

<!--

● Sections: example, activity. soluciones, img-foot, warning, note

::: example
### Ejemplo: Cálculo de derivadas
Aquí va el contenido de tu ejemplo. Puedes usar Markdown normal adentro.
:::


● Image:

::: figure
![](imagen.png){width=400px}

<small>Pie (Source)</small>
:::

[⌕](../../images/ ) 

● Videos:

 Change XXX to video-id and put time in seconds

 - Yotube with start point: [Mira este momento clave en el video](https://www.youtube.com/watch?v=XXX&t=123s)

 - Youtubetrimmer with start and end point: [Mirá este momento puntual del video](https://youtubetrimmer.com/view/?v=XXX&start=120&end=150&loop=0)

-->
