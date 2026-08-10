---
title: "Ciclo `for`"
autor: "José Juarez"
version: "09/08/26"
---

<!-- *** GUIDE START *** -->

## 1. Repetir tareas con `for`

Hasta ahora, los programas que escribimos ejecutaban sus instrucciones una vez. Pero muchas veces necesitamos hacer algo varias veces: mostrar varios mensajes, revisar caracteres de un texto, contar elementos o repetir una operación.

En Python podemos utilizar `for` para repetir un bloque de instrucciones.

::: example

**Ejemplo:**


```python
for i in range(5):
    print("Hola")
```

`range(5)` indica que queremos realizar la repetición **5 veces**.

:::

La variable `i` va tomando diferentes valores durante la repetición. Puede usarla o no. En el programa anterior no la usas pero en el de abajo la usas mostrando su valor: 

::: example

**Ejemplo**

```python
for i in range(5):
    print(i)
```

El resultado es:

```text
0
1
2
3
4
```

:::

**Una idea importante:** En Python, la instrucción que pertenece al `for` debe estar con sangría (indentada). Esto indica que instrucciones se repiten.

::: example

**Ejemplo**

```python
for i in range(3):
    print("Hola")
print("Adios")
```
Aquí "Hola" se repite 3 veces por que está dentro del `for` y "Adios" muestra una sola vez por que está fuera del `for`

:::

### Actividades

::: activity

**1)** En la carpeta, sin ejecutar el programa, responde:

```python
for i in range(4):
    print("Python")
```

   - *a.* ¿Cuántas veces aparece `Python`?
   - *b.* ¿Qué valores toma `i`?
   - *c.* ¿Qué ocurriría si `range(4)` fuera `range(7)`?

**2)** Pensar antes de programar: En la carpeta indica si para resolver cada situación utilizarías probablemente un `for`. No es necesario escribir código. Justifica brevemente las respuestas.

   - *a.* Mostrar un mensaje una sola vez.
   - *b.* Mostrar los números del 1 al 20.
   - *c.* Revisar uno por uno los caracteres de una palabra.
   - *d.* Preguntar al usuario una contraseña hasta que sea correcta.

**3)** Hacer un programa que muestre 7 veces la frase "Buen día" y 3 veces la frase "Buenas noches". Utiliza dos `for`.

**4)** Hacer un programa que muestre los números del 0 al 20. Ten en cuenta que `range(20)` empieza en 0 y termina en 19.


## 2. La variable del `for`

La variable utilizada por `for` permite saber en qué repetición estamos.

::: example

**Ejemplo**

```python
for i in range(5):
    print(f"Repetition: {i}")
```

El resultado será:

```text
Repetition: 0
Repetition: 1
Repetition: 2
Repetition: 3
Repetition: 4
```
:::

El nombre `i` no es obligatorio. Podemos utilizar otro nombre:

::: example

**Ejemplo**

```python
for numero in range(5):
    print(numero)
```

:::

Es conveniente elegir nombres que ayuden a entender el programa.

### Actividades

::: activity

**1)** Busca y escribe en la carpeta los significados en español de: range, loop e indentation.

**2)** Hacer un programa que muestre los números del 1 al 30. 

:::

## 3. `for` y decisiones

Un `for` puede contener un `if`.

::: example

Por ejemplo:

```python
for n in range(10):
    if n > 5:
        print(n)
```

El `for` genera los números y el `if` decide cuáles mostrar. El resultado es:

```text
6
7
8
9
```

:::

### Actividad

::: activity

**1)** Modificar el siguiente programa para que muestre solo los números mayores que 10 y menores que 20:

```python
for n in range(30):
    if n > 5:
        if n < 8:
           print(n)
```

**2)** Hacer el programa anterior con un solo if usando el operador lógico `and`. 

**3)** El **resto** de dividir un número par por `2` es siempre cero. En Python puedes usar el operador `%` para encontrar el valor del resto de una división. Por ejemplo `5 % 2` es `1`. Haz un programa que muestre todos los números pares entre 0 y 20. En el programa debe aparacer `range(21)` y un `if`.

:::

::: warning
Esta guía continuará la próxima clase
:::



<div hidden>


## Pensar como dar lo de and y or

## 5. Recorrer una palabra

El `for` no solamente sirve para números.

También podemos recorrer los caracteres de un texto:

```python
palabra = "Python"

for letra in palabra:
    print(letra)
```

El resultado será:

```text
P
y
t
h
o
n
```

En cada repetición, `letra` contiene un carácter diferente.

Esta posibilidad será especialmente importante cuando trabajemos con textos.

### Actividad 6 — ¿Qué hace el programa?

Observa:

```python
texto = "programacion"

for letra in texto:
    if letra == "a":
        print("Found!")
```

Responde:

a. ¿Qué significa `for letra in texto`?

b. ¿Cuántas veces se ejecuta el `if`?

c. ¿Cuántas veces aparecerá `Found!`?

d. ¿Qué ocurriría si cambiamos `"a"` por `"o"`?

---

## 6. Contar mientras recorremos un texto

Podemos utilizar una variable para acumular información.

Por ejemplo:

```python
texto = "banana"
cantidad = 0

for letra in texto:
    if letra == "a":
        cantidad = cantidad + 1

print(cantidad)
```

El programa recorre cada letra y aumenta `cantidad` cada vez que encuentra una `a`.

La variable `cantidad` comienza en cero y va acumulando el resultado.

### Actividad 7 — En carpeta

Analiza el programa anterior y completa la tabla:

| Letra | ¿Es `"a"`? | Valor de `cantidad` |
| ----- | ---------- | ------------------- |
| b     |            |                     |
| a     |            |                     |
| n     |            |                     |
| a     |            |                     |
| n     |            |                     |
| a     |            |                     |

Luego responde:

**¿Por qué `cantidad` debe comenzar en 0?**

---

## 7. Pequeños analizadores

Vamos a construir programas que obtengan información de un texto.

### Actividad 8 — Contar letras

Escribe una función llamada:

```python
def count_letter(texto, letra):
```

Debe recibir un texto y una letra y devolver cuántas veces aparece esa letra.

Por ejemplo:

```python
resultado = count_letter("banana", "a")
print(resultado)
```

debe mostrar:

```text
3
```

Prueba también con:

```python
count_letter("programacion", "o")
count_letter("Python", "x")
count_letter("abracadabra", "a")
```

No utilices todavía métodos especiales para contar. El objetivo es practicar `for`.

---

### Actividad 9 — Buscar una letra

Escribe una función:

```python
def contains_letter(texto, letra):
```

Debe devolver `True` si la letra aparece en el texto y `False` si no aparece.

Por ejemplo:

```python
contains_letter("Python", "y")
```

debe devolver:

```text
True
```

y:

```python
contains_letter("Python", "z")
```

debe devolver:

```text
False
```

**Desafío:** intenta resolverlo recorriendo el texto con `for`.

---

## 8. Separar los programas en funciones

Hasta ahora, probablemente teníamos varios ejercicios dentro del mismo archivo.

Por ejemplo:

```python
print("Ejercicio 1")

# programa...

print("Ejercicio 2")

# programa...
```

Al ejecutar el archivo, todos los ejercicios se ejecutan.

Podemos comenzar a organizarlos de otra manera:

```python
def ejercicio_1():
    print("Hola")


def ejercicio_2():
    for i in range(5):
        print(i)


def ejercicio_3():
    print("Otro ejercicio")


ejercicio_2()
```

En este caso, solamente se ejecuta `ejercicio_2()`.

Las demás funciones están definidas, pero no son llamadas.

Para ejecutar otro ejercicio podemos cambiar:

```python
ejercicio_2()
```

por:

```python
ejercicio_1()
```

### Actividad 10 — Organizar

Toma dos ejercicios anteriores y colócalos en funciones diferentes.

Por ejemplo:

```python
def ejercicio_1():
    ...


def ejercicio_2():
    ...


ejercicio_1()
```

Deja solamente **una llamada activa** al final del programa.

Para probar otro ejercicio, comenta la llamada anterior y descomenta la nueva:

```python
# ejercicio_1()
ejercicio_2()
```

Por ahora no es necesario profundizar en cómo funcionan las funciones. Las utilizaremos principalmente para mantener ordenados nuestros programas.

---

## 9. Proyecto: una primera herramienta para textos

Nuestro proyecto final será un programa capaz de analizar textos, pero no queremos que sea solamente una colección de estadísticas.

Por ahora vamos a construir pequeñas herramientas que puedan formar parte de ese programa.

### Actividad 11 — Detector de caracteres

Diseña una función que reciba un texto y una letra.

El programa debe recorrer el texto y mostrar un mensaje cada vez que encuentre esa letra.

Por ejemplo, para:

```text
Texto: computadora
Letra: o
```

podría mostrar:

```text
Found: o
Found: o
```

Luego modifica el programa para que, además, indique **en qué posición** encontró cada aparición.

No hace falta que el resultado tenga todavía el formato definitivo del proyecto.

---

## 10. Actividad lúdica — El texto secreto

Vamos a utilizar el `for` para construir una pequeña herramienta.

Un jugador escribe una palabra o frase. El programa debe recorrerla y producir una nueva versión siguiendo una regla.

Por ejemplo, una regla podría ser:

> Cada vez que aparezca la letra `a`, reemplazarla por `@`.

Para:

```text
banana
```

el resultado sería:

```text
b@n@n@
```

### Consigna

Diseña una función que reciba un texto y produzca una versión modificada siguiendo una regla que ustedes mismos definan.

Algunas posibilidades:

* cambiar determinadas letras por símbolos;
* destacar determinadas letras;
* eliminar determinadas letras;
* duplicar determinadas letras;
* convertir algunas letras en mayúsculas.

La regla debe poder explicarse claramente en una oración.

**Importante:** no es necesario resolverlo utilizando métodos de strings que todavía no vimos. El objetivo principal es practicar el recorrido carácter por carácter con `for`.

---

## 11. Desafío

Escribe una función que reciba un texto y determine cuál de estas categorías corresponde:

* contiene la letra `a`;
* contiene la letra `e`;
* contiene ambas;
* no contiene ninguna.

Por ejemplo:

```text
"casa" → contiene a
"verde" → contiene e
"pared" → contiene ambas
"ritmo" → ninguna
```

Intenta resolverlo utilizando:

* `for`;
* `if` / `elif` / `else`;
* variables booleanas.

No hace falta utilizar funciones o métodos que todavía no hayamos estudiado.

---

## 12. Para pensar

Hasta ahora utilizamos `for` para recorrer números y textos.

Responde en tu carpeta:

1. ¿Qué problema resuelve un `for`?

2. ¿Qué diferencia hay entre:

```python
for i in range(5):
```

y:

```python
for letra in texto:
```

3. ¿Qué función cumple la indentación?

4. ¿Qué ocurre si colocamos el `print` fuera del bloque del `for`?

5. ¿Por qué recorrer caracteres de un texto puede ser útil para nuestro proyecto?

6. ¿Qué cosas interesantes podríamos detectar en un texto además de contar letras?

Anota al menos **tres ideas**. No tienen que ser estadísticas: pueden ser reglas, juegos, patrones, mensajes ocultos o cualquier otra cosa que pueda hacer que el análisis resulte interesante.

Creo que hay una decisión pedagógica importante acá: **no convertiría esta guía en una introducción general a `range`**. Lo usaría como puerta de entrada, pero rápidamente pasaría a `for letra in texto`, porque ahí aparece una conexión natural con el proyecto.

También me parece acertado introducir ya `def ejercicio_1()` / `ejercicio_2()` aunque todavía no desarrolles "Funciones" como tema 7. Es una herramienta organizativa: los chicos pueden tener 8–10 ejercicios en el mismo `.py` sin que todos se ejecuten cada vez.

Y la actividad **"El texto secreto"** me parece especialmente útil para lo que venís buscando: empieza a darle al analizador una dimensión lúdica sin obligarte todavía a decidir cuál será el juego final.



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
![](imagen.png){width=400px}

<small>Pie (Source)</small>
:::

[⌕](../../images/ ) 

● Videos:

 Change XXX to video-id and put time in seconds

 - Yotube with start point: [Mira este momento clave en el video](https://www.youtube.com/watch?v=XXX&t=123s)

 - Youtubetrimmer with start and end point: [Mirá este momento puntual del video](https://youtubetrimmer.com/view/?v=XXX&start=120&end=150&loop=0)

-->
