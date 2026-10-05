---
title: "Listas"
autor: "José Juarez"
version: "05/10/26"
---

<!-- *** GUIDE START *** -->

## Contenidos

1. [¿Para qué sirven las listas?](#listas1)
2. [Los elementos de una lista](#listas2)
3. [Cambiar elementos](#listas3)


## 1. ¿Para qué sirven las listas? {#listas1}

Hasta ahora trabajamos con variables que contienen un dato:

```python
name = "Sofia"
age = 16
```

Pero muchas veces necesitamos guardar **varios datos relacionados**. Por ejemplo, los nombres de los integrantes de un curso:

```python
students = ["Sofia", "Mateo", "Juan", "Valentina"]
```

Una lista se escribe entre corchetes `[` `]` y sus elementos se separan mediante comas.

Una lista puede contener números:

```python
grades = [7, 8, 6, 10, 9]
```

o textos:

```python
words = ["computer", "program", "list", "data"]
```

También puede contener datos de distintos tipos:

```python
data = ["Sofia", 16, 8.5]
```

## Actividad

::: activity

Resolver en la carpeta, sin programar.

**1)** Escribir tres situaciones de la vida cotidiana en las que sea necesario guardar varios datos del mismo tipo. Para cada situación, indicar qué podría contener la lista.

**2)** Decidir cuáles de las siguientes variables podrían representarse mejor mediante una lista:

```text
student_name
students
age
temperatures
favorite_color
```

:::

[↑ Volver al contenido](#contenidos)


## 2. Los elementos de una lista {#listas2}

Los elementos de una lista tienen una posición.

::: example

Por ejemplo:

```python
animals = ["dog", "cat", "horse", "cow"]
```

Las posiciones comienzan en **0**:

| Índice | Elemento  |
| -----: | --------- |
|      0 | `"dog"`   |
|      1 | `"cat"`   |
|      2 | `"horse"` |
|      3 | `"cow"`   |

:::

Para acceder a un elemento usamos su índice:

```python
print(animals[0])
```

produce:

```text
dog
```

También podemos guardar un elemento en una variable:

```python
animal = animals[2]
print(animal)
```

### Actividad

::: activity

Hacer en carpeta.

**1)** Sin ejecutar el programa, escribir qué muestra cada `print`.

```python
colors = ["red", "green", "blue", "yellow"]

print(colors[0])
print(colors[2])
print(colors[3])
```

**2)** ¿Por qué no existe `colors[4]`?

:::

[↑ Volver al contenido](#contenidos)


## 3. Cambiar elementos {#listas3}

Las listas son modificables.

::: example

Por ejemplo:

```python
colors = ["red", "green", "blue"]

colors[1] = "yellow"

print(colors)
```

Ahora la lista es:

```text
["red", "yellow", "blue"]
```

:::

Podemos cambiar un elemento indicando su índice y asignándole un nuevo valor.

### Actividad

::: activity

Programar en la computadora

**1)** Completar el programa de abajo que resuelve esta consigna: Crear y mostrar esta lista `answers = ["yes", "no", "maybe", "yes"]`. Escribir la instrucción necesaria para reemplazar `"maybe"` por `"unknown"` y para cambiar el último elemento para que la lista quede: `["yes", "no", "unknown", "no"]`.

```python
# Ponemos un nombre al programa usando def:
def ejercicio_3_1():
    answers = ["yes", "no", "maybe", "yes"]
    print(answers)
    answers[2]="unknown"
    # Completarlo ...


# Llamamos al programa por su nombre para ejecutarlo:
ejercicio_3_1()
``` 

**2)** Hacer un programa llamado "ejercicio_3_2" que haga esta lista y la muestre: `numbers = [10, 20, 30, 40]`. Luego debe modificar el 10 por el 100 y el 30 por el 300. Finalmente mostrar la lista. 

:::

[↑ Volver al contenido](#contenidos)

<div hidden>

## 4. Agregar elementos

Podemos agregar un elemento al final de una lista utilizando `append()`:

```python
animals = ["dog", "cat"]

animals.append("horse")

print(animals)
```

Resultado:

```text
["dog", "cat", "horse"]
```

Cada vez que usamos `append()`, la lista aumenta.

```python
words = []

words.append("python")
words.append("list")
words.append("program")

print(words)
```

### Actividad 6 — Construir una lista

Crear un programa que comience con una lista vacía:

```python
words = []
```

y agregue mediante `append()` cinco palabras relacionadas con programación.

Al final, mostrar la lista completa.

Después modificar el programa para mostrar también cada una de las palabras por separado.

---

## 5. ¿Cuántos elementos tiene una lista?

La función `len()` permite conocer la cantidad de elementos:

```python
animals = ["dog", "cat", "horse"]

print(len(animals))
```

El resultado es:

```text
3
```

Es importante distinguir:

```python
len(animals)
```

de:

```python
animals[0]
```

El primero indica **cuántos elementos hay**.

El segundo obtiene **un elemento determinado**.

### Actividad 7 — Pensar antes de ejecutar

Indicar el resultado de cada expresión:

```python
words = ["computer", "mouse", "keyboard", "screen"]

len(words)
words[0]
words[3]
```

Luego responder:

1. ¿Cuál es el último índice?
2. ¿Coincide con `len(words)`?
3. ¿Cómo podríamos obtener el último elemento sin escribir directamente su índice?

---

## 6. Recorrer una lista con `for`

Una de las principales ventajas de las listas aparece cuando las combinamos con `for`.

Por ejemplo:

```python
animals = ["dog", "cat", "horse"]

for animal in animals:
    print(animal)
```

El `for` toma cada elemento de la lista y lo guarda temporalmente en la variable `animal`.

El programa muestra:

```text
dog
cat
horse
```

Podemos utilizar cualquier nombre de variable:

```python
for word in words:
    print(word)
```

La elección del nombre debería ayudar a comprender qué representa cada elemento.

### Actividad 8 — Reading code

Sin ejecutar:

```python
names = ["Ana", "Tom", "Leo"]

for name in names:
    print("Hello", name)
```

1. ¿Cuántas veces se ejecuta `print()`?
2. ¿Qué valor tiene `name` en cada repetición?
3. Escribir exactamente qué aparece en pantalla.

Luego modificar el programa para que diga:

```text
Hello, Ana. Welcome to programming!
```

y lo mismo para los otros nombres.

---

## 7. Buscar información dentro de una lista

Podemos combinar listas con `if`.

Por ejemplo:

```python
words = ["python", "java", "ruby", "python"]

for word in words:
    if word == "python":
        print("Python found!")
```

El programa revisa los elementos uno por uno y toma una decisión cuando encuentra `"python"`.

### Actividad 9 — ¿Qué encuentra el programa?

Indicar qué mostrará:

```python
numbers = [4, 7, 2, 7, 9]

for number in numbers:
    if number == 7:
        print("Found 7")
```

Después responder:

* ¿Cuántas veces aparece el mensaje?
* ¿El programa encuentra solamente el primer `7`?
* ¿Qué habría que cambiar para buscar el número `9`?

---

## 8. Contar elementos que cumplen una condición

Una lista y un `for` también permiten contar elementos.

```python
numbers = [4, 7, 2, 7, 9]

count = 0

for number in numbers:
    if number == 7:
        count = count + 1

print(count)
```

La variable `count` funciona como un contador.

Cada vez que encuentra un `7`, aumenta en uno.

### Actividad 10 — Analizar el contador

Sin ejecutar el programa, completar una tabla indicando cómo cambia `count`:

| number | ¿number == 7? | count |
| -----: | :-----------: | ----: |
|      4 |               |       |
|      7 |               |       |
|      2 |               |       |
|      7 |               |       |
|      9 |               |       |

Finalmente indicar qué muestra el programa.

### Actividad 11 — English + programming

Complete:

> A **list** contains several ______.
> Each element has an ______.
> Python starts counting indexes at ______.
> `append()` ______ an element to the list.
> `len()` tells us how ______ elements there are.

Words:

`adds` — `many` — `index` — `elements` — `0`

---

## 9. Las listas y los textos

Una lista también puede contener palabras.

```python
text = ["Python", "is", "easy", "to", "learn"]
```

Podemos recorrerla:

```python
for word in text:
    print(word)
```

Pero también podemos hacer preguntas sobre cada palabra.

Por ejemplo:

```python
for word in text:
    if len(word) > 4:
        print(word)
```

Este programa muestra solamente las palabras que tienen más de cuatro caracteres.

### Actividad 12 — Clasificar palabras

Crear una lista con al menos 8 palabras relacionadas con informática.

Recorrer la lista y mostrar solamente las palabras que tengan más de 5 caracteres.

Después modificar el programa para mostrar solamente las palabras que tengan **5 caracteres o menos**.

---

## 10. Preparando un pequeño analizador

Supongamos que tenemos una lista de palabras obtenidas de un texto:

```python
words = ["python", "is", "a", "programming", "language"]
```

Podemos recorrerla y obtener información.

Por ejemplo, mostrar las palabras largas:

```python
for word in words:
    if len(word) >= 8:
        print(word)
```

Este tipo de procedimiento será importante cuando construyamos programas capaces de analizar textos.

### Actividad 13 — Explorador de palabras

Crear un programa que tenga una lista de al menos 10 palabras.

El programa debe recorrer la lista y:

1. mostrar las palabras que tengan 6 o más caracteres;
2. contar cuántas palabras cumplen esa condición;
3. mostrar al final:

```text
Long words: X
```

donde `X` sea la cantidad encontrada.

No es necesario analizar todavía un texto introducido por el usuario.

La intención es comenzar a construir pequeñas herramientas para obtener información de un conjunto de palabras.

---

## 11. Desafío — El detective de palabras

Crear un programa que tenga una lista de palabras.

El usuario debe ingresar una palabra:

```python
search = input("Enter a word: ")
```

El programa debe recorrer la lista y decir cuántas veces aparece esa palabra.

Por ejemplo, para:

```python
words = ["cat", "dog", "cat", "bird", "cat", "dog"]
```

si el usuario escribe:

```text
cat
```

el programa debe mostrar:

```text
Occurrences: 3
```

### Condición

No utilizar todavía herramientas que no hayamos estudiado.

Resolverlo utilizando:

* una lista;
* `for`;
* `if`;
* una variable contador;
* `input()`;
* `print()`.

---

## 12. Desafío final — Una lista que cuenta una historia

Crear una lista de palabras relacionadas con una pequeña historia.

Por ejemplo:

```python
story = ["robot", "school", "computer", "robot", "teacher", "robot"]
```

El programa debe permitir investigar la historia.

Como mínimo debe:

1. mostrar todas las palabras;
2. indicar cuántas palabras contiene;
3. permitir buscar una palabra;
4. indicar cuántas veces aparece;
5. mostrar las palabras que tengan 6 o más caracteres.

Agregar **una función nueva** que el programa pueda realizar.

Pensar especialmente qué información interesante se puede obtener de una lista de palabras.

### Para pensar

Un analizador de textos no necesariamente tiene que limitarse a decir:

> "El texto tiene 327 palabras."

¿Qué otras preguntas interesantes podríamos hacerle a un texto?

Me gusta especialmente que el **Desafío 1 y el Desafío final ya dejan preparado el camino del proyecto**, sin revelar necesariamente su diseño final. La progresión queda bastante natural: `lista → índice → modificar → append → len → for → if + lista → contador → palabras → análisis`.

También evitaría por ahora `in`, `count()`, `sort()`, slicing, listas anidadas, etc. Aunque sean útiles, **quitarían parte del trabajo que justamente quiero que hagan con `for` + `if` + contador**, que es lo que después necesitarán comprender de verdad.

</div>




<!-- *** GUIDE END *** -->



<!-- *** GUIDE AUXILIARY THINGS *** -->

<!--

● Sections: example, activity. solutions, figure, warning, note

::: example
### Ejemplo: Cálculo de derivadas
Aquí va el contenido de tu ejemplo. Puedes usar Markdown normal adentro.
:::


● Image:

::: figure
![caption](imagen.png){width=400px}

<small>Pie (Source)</small>
:::

[⌕](../../images/ ) 

● Videos:

 Change XXX to video-id and put time in seconds

 - Yotube with start point: [Mira este momento clave en el video](https://www.youtube.com/watch?v=XXX&t=123s)

 - Youtubetrimmer with start and end point: [Mirá este momento puntual del video](https://youtubetrimmer.com/view/?v=XXX&start=120&end=150&loop=0)

-->
