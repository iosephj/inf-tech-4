---
title: "Listas"
autor: "José Juarez"
version: "05/10/26"
---

<!-- *** GUIDE START *** -->

## Contenidos

<details>

<summary>**1. ¿Para qué sirven las listas?**</summary>

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

**a)** Escribir tres situaciones de la vida cotidiana en las que sea necesario guardar varios datos del mismo tipo. Para cada situación, indicar qué podría contener la lista.

**b)** Decidir cuáles de las siguientes variables podrían representarse mejor mediante una lista:

```text
student_name
students
age
temperatures
favorite_color
```

:::

</details>



<details>

<summary>**2. Los elementos de una lista**</summary>

## 2. Los elementos de una lista

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

**a)** Sin ejecutar el programa, escribir qué muestra cada `print`.

```python
colors = ["red", "green", "blue", "yellow"]

print(colors[0])
print(colors[2])
print(colors[3])
```

**b)** ¿Por qué no existe `colors[4]`?

:::

</details>



<details>

<summary>**3. Cambiar elementos**</summary>

## 3. Cambiar elementos

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

**a)** Completar el programa de abajo que resuelve esta consigna: Crear y mostrar esta lista `answers = ["yes", "no", "maybe", "yes"]`. Escribir la instrucción necesaria para reemplazar `"maybe"` por `"unknown"` y para cambiar el último elemento para que la lista quede: `["yes", "no", "unknown", "no"]`.

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

**b)** Hacer un programa llamado "ejercicio_3_2" que haga esta lista y la muestre: `numbers = [10, 20, 30, 40]`. Luego debe modificar el 10 por el 100 y el 30 por el 300. Finalmente mostrar la lista. 

:::

</details>



<details>

<summary>**4. Agregar y contar elementos**</summary>

## 4. Agregar y contar elementos

Podemos agregar un elemento al final de una lista utilizando `append()`:

Ejemplo:

::: example

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

:::

La función `len()` permite conocer la cantidad de elementos:

Ejemplo:

::: example

```python
animals = ["dog", "cat", "horse"]

print(len(animals))
```

El resultado es:

```text
3
```

:::



<div hidden>
```python
words = []

words.append("python")
words.append("list")
words.append("program")

print(words)
```
</div>


### Actividades

::: activity

**a)** Crear un programa que comience con una lista vacía con `words = []`. Luego agregue mediante `append()` cinco palabras relacionadas con programación. Al final, mostrar la lista completa. 

**b)** Recuerda que cada elemento de un lista tiene un índice que empieza en cero. Modificar el programa anterior para mostrar también cada una de las palabras por separado, por ejemplo usando `print(word[0])` para mostrar el primer elemento de la lista y así sucesivamente.

**c)** Prueba mostrar el último elemento de la lista de este modo: `print(word[len(word)-1])`. ¿Porqué funciona? Escríbelo como un comentario en el programa.

:::

</details>



<details>

<summary>**5. Recorrer una lista con `for`**</summary>

## 5. Recorrer una lista con `for`

Una de las principales ventajas de las listas aparece cuando las combinamos con `for`.

Por ejemplo:

::: example

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
:::

Podemos utilizar cualquier nombre de variable:

```python
for word in words:
    print(word)
```

La elección del nombre debería ayudar a comprender qué representa cada elemento.

### Actividades

::: activity

**a)** Dado el siguiente programa modificarlo para que muestre `Hello, Ana. Welcome to programming!` y lo mismo para los otros nombres.

```python
names = ["Ana", "Tom", "Leo"]

for name in names:
    print(f"Hello {name}")
```

**b)** **Buscar información dentro de una lista:** El siguiente programa busca la palabra "python" recorriendo la lista. Revisa los elementos uno por uno y toma una decisión cuando encuentra "python". Modifícalo de modo que busque si están las palabras "pyhon" y "ruby", ambas, en la lista. 

```python
words = ["python", "java", "ruby", "c++"]

for word in words:
    if word == "python":
        print("Python found!")
```

**c)** Hacer un programa que dada la lista `numbers = [4, 7, 2, 7, 9]` busque el `7` y muestre el mensaje `Found 7` cada vez que lo encuentre.

**d)** **Contar elementos que cumplen una condición:** En el programa de abajo el for recorre la lista y cada vez que encuentra el 7 incrementa en 1 la variable `contador`. Modifícalo de modo que cuente las veces que aparece el 9.

```python
numbers = [4, 9, 7, 5, 2, 9, 7, 9]

contador = 0 # Empieza en el valor cero

for number in numbers:
    if number == 7:
        contador = contador + 1 # Se incrementa en 1

print(contador)
```

**e)** El siguiente programa recorre una lista de palabras y usando `len` para calcular la cantidad de letras de una palabra solo muestra las que tienen más de 4 letras. Modíficalo para que muestre las palabras que tienen entre 2 y 4 letras. Es decir debería mostrar: is, easy, to.

```python
text = ["Python", "is", "easy", "to", "learn"]

for word in text:
    if len(word) > 4:
        print(word)
```


**f)** Crear un programa que tenga una lista de al menos 10 palabras. El programa debe recorrer la lista y debe:

- mostrar las palabras que tengan 6 o más caracteres;
- contar cuántas palabras cumplen esa condición;
- mostrar al final: `Cantidad de palabras encontradas: X` donde `X` sea la cantidad encontrada.

**g)** **Desafío:** Crear un programa que tenga una lista de palabras. Pedir al usuario que ingrese una palabra con:

```python
palabra_buscada = input("Enter a word: ")
```

El programa debe recorrer la lista y decir cuántas veces aparece esa palabra.

Por ejemplo, para:

```python
words = ["cat", "dog", "cat", "bird", "cat", "dog"]
```

si el usuario escribe `cat` el programa debe mostrar: `Occurrences: 3`

**Condiciones:** No utilizar herramientas que no hayamos estudiado. Resolverlo utilizando: una lista; `for`; `if`; una variable contador; `input()`; `print()`.

:::

</details>

::: warning
Esta guía se aprueba mostrando los programas, los ejercicios de la carpeta y explicando el problema **f)** del punto 5.
:::

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
