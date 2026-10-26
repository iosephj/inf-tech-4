---
title: "Funciones"
autor: "José Juarez"
version: "26/10/26"
---

<!-- *** GUIDE START *** -->

## Contenidos

<details>

<summary>**1. ¿Para qué sirven las funciones?**</summary>

## 1. ¿Para qué sirven las funciones?

Cuando escribimos un programa, podemos encontrarnos con instrucciones que realizan una tarea determinada. Por ejemplo, contar cuántas letras tiene una palabra, calcular un puntaje o mostrar un mensaje.

Si el programa crece, escribir todas las instrucciones una detrás de otra puede volverlo difícil de leer y modificar.

Las **funciones** permiten agrupar instrucciones que realizan una tarea y darles un nombre. Después, podemos utilizar ese nombre para ejecutar las instrucciones cuando las necesitemos.

Observá el siguiente programa:

```python
print("Welcome to the text game!")
print("Welcome to the text game!")
print("Welcome to the text game!")
```

El mensaje se repite tres veces. Podemos organizarlo mediante una función:

```python
def mostrar_bienvenida():
    print("Welcome to the text game!")

mostrar_bienvenida()
mostrar_bienvenida()
mostrar_bienvenida()
```

Analicemos las partes:

- `def` indica que estamos definiendo una función.
- `mostrar_bienvenida` es el nombre que elegimos para la función.
- Los paréntesis `()` aparecen después del nombre.
- Las instrucciones que pertenecen a la función se escriben con sangría.
- `mostrar_bienvenida()` es una llamada a la función: hace que se ejecuten sus instrucciones.

**Importante:** definir una función no significa ejecutarla. Las instrucciones se ejecutan cuando llamamos a la función.

### Actividades

::: activity

**a)** **Programar.** Hacer el ejemplo en Python, prueba de llamar a la función distintas cantidades de veces.

**b)** **En carpeta.** Respondé con tus palabras:

- *b1.* ¿Qué problema puede aparecer cuando un programa tiene muchas instrucciones repetidas?
- *b2.* ¿Qué significa definir una función?
- *b3.* ¿Qué diferencia hay entre definir una función y llamarla?
- *b4.*  ¿Para qué sirve la sangría dentro de una función?

<div hidden>
**3. En carpeta.** Vocabulario en inglés.** Completá el diálogo con las palabras del recuadro. Cada palabra se utiliza una sola vez.

`call — define — function — repeat`

**Alex:** I need to show the same message several times. Should I copy the instruction?

**Sam:** Not necessarily. You can create a __________ that contains the instruction.

**Alex:** How do I create it?

**Sam:** You use `def` to __________ the function.

**Alex:** And how do I execute it?

**Sam:** You __________ it by writing its name followed by parentheses.

**Alex:** Great! Now I can __________ the task without copying the instructions.
</div>


**c)** **En carpeta.** Observá el programa:

```python
def mostrar_mensaje():
    print("Find the hidden word!")

print("The game starts.")
mostrar_mensaje()
print("Good luck!")
```

- *c1.* ¿Qué sucedería si elimináramos la línea `mostrar_mensaje()`?
- *c2.* Modificá el programa para que el mensaje de la función aparezca dos veces.

**d) Programación.** Copia el programa del punto anterior en el IDLE. Ejecútalo. Agrega otra función inventada por vos con otro mensaje que aparezca abajo de "Find the hidden world"

:::

</details>

Esta guía continuará.


<div hidden>

---
---

# Guía de aprendizaje: Funciones en Python
**4.º año de secundaria — Programación**

## 1. ¿Para qué sirven las funciones?

Cuando escribimos un programa, podemos encontrarnos con instrucciones que realizan una tarea determinada. Por ejemplo, contar cuántas letras tiene una palabra, calcular un puntaje o mostrar un mensaje.

Si el programa crece, escribir todas las instrucciones una detrás de otra puede volverlo difícil de leer y modificar.

Las **funciones** permiten agrupar instrucciones que realizan una tarea y darles un nombre. Después, podemos utilizar ese nombre para ejecutar las instrucciones cuando las necesitemos.

Observá el siguiente programa:

```python
print("Welcome to the text game!")
print("Welcome to the text game!")
print("Welcome to the text game!")
```

El mensaje se repite tres veces. Podemos organizarlo mediante una función:

```python
def mostrar_bienvenida():
    print("Welcome to the text game!")

mostrar_bienvenida()
mostrar_bienvenida()
mostrar_bienvenida()
```

Analicemos las partes:

- `def` indica que estamos definiendo una función.
- `mostrar_bienvenida` es el nombre que elegimos para la función.
- Los paréntesis `()` aparecen después del nombre.
- Las instrucciones que pertenecen a la función se escriben con sangría.
- `mostrar_bienvenida()` es una llamada a la función: hace que se ejecuten sus instrucciones.

**Importante:** definir una función no significa ejecutarla. Las instrucciones se ejecutan cuando llamamos a la función.

### Actividades

**1. En carpeta.** Respondé con tus palabras:

a. ¿Qué problema puede aparecer cuando un programa tiene muchas instrucciones repetidas?

b. ¿Qué significa definir una función?

c. ¿Qué diferencia hay entre definir una función y llamarla?

d. ¿Para qué sirve la sangría dentro de una función?

**2. En carpeta.** Un compañero afirma: «Si escribo una función, Python ejecuta inmediatamente todo lo que contiene».

¿Es correcta su afirmación? Explicá por qué y utilizá el ejemplo de la bienvenida para justificar tu respuesta.

**3. En carpeta. Vocabulario en inglés.** Completá el diálogo con las palabras del recuadro. Cada palabra se utiliza una sola vez.

`call — define — function — repeat`

**Alex:** I need to show the same message several times. Should I copy the instruction?

**Sam:** Not necessarily. You can create a __________ that contains the instruction.

**Alex:** How do I create it?

**Sam:** You use `def` to __________ the function.

**Alex:** And how do I execute it?

**Sam:** You __________ it by writing its name followed by parentheses.

**Alex:** Great! Now I can __________ the task without copying the instructions.

**4. En carpeta.** Observá el programa:

```python
def mostrar_mensaje():
    print("Find the hidden word!")

print("The game starts.")
mostrar_mensaje()
print("Good luck!")
```

a. ¿Qué aparece en pantalla?

b. ¿Cuántas veces se ejecuta el contenido de `mostrar_mensaje`?

c. ¿Qué sucedería si elimináramos la línea `mostrar_mensaje()`?

d. Modificá el programa para que el mensaje de la función aparezca dos veces, sin copiar su contenido.

**5. Programación.** Creá un archivo llamado `funciones.py` en IDLE.

Escribí una función llamada `mostrar_reglas()` que muestre tres reglas de un juego de palabras. Después, llamá a la función para que aparezcan las reglas en pantalla.

Las reglas pueden ser inventadas por vos.

---

## 2. Funciones que reciben datos

Una función puede necesitar información para realizar su tarea. Por ejemplo, para saludar a una persona, necesitamos conocer su nombre.

Podemos escribir:

```python
def saludar(nombre):
    print(f"Hello, {nombre}!")

saludar("Sofia")
saludar("Lucas")
```

El resultado será:

```text
Hello, Sofia!
Hello, Lucas!
```

En este ejemplo, `nombre` es un **parámetro**. Es una variable que recibe el dato que le proporcionamos al llamar a la función.

Cuando escribimos `saludar("Sofia")`, el texto `"Sofia"` se utiliza como valor del parámetro `nombre` durante esa llamada.

También podemos usar funciones que reciban números:

```python
def mostrar_puntaje(puntos):
    print(f"Your score is {puntos}.")

mostrar_puntaje(10)
mostrar_puntaje(25)
```

La misma función permite mostrar distintos puntajes sin modificar su definición.

Una función puede recibir más de un dato:

```python
def mostrar_palabra(palabra, puntos):
    print(f"The word '{palabra}' is worth {puntos} points.")

mostrar_palabra("robot", 5)
mostrar_palabra("planet", 10)
```

Los argumentos se escriben en el mismo orden que los parámetros correspondientes.

### Actividades

**6. En carpeta.** Observá la siguiente función:

```python
def mostrar_pista(palabra):
    print(f"Clue: the word is {len(palabra)} letters long.")
```

a. ¿Cuál es el nombre de la función?

b. ¿Cuál es su parámetro?

c. ¿Qué información necesita para mostrar una pista?

d. ¿Qué ocurriría si la llamáramos con `mostrar_pista("school")`?

**7. En carpeta.** Analizá las llamadas a esta función:

```python
def calcular_puntos(aciertos, bonus):
    print(aciertos * 10 + bonus)

calcular_puntos(3, 5)
calcular_puntos(2, 0)
calcular_puntos(4, 10)
```

a. Predecí qué resultado produce cada llamada.

b. ¿Qué función cumple cada parámetro?

c. ¿Por qué no es necesario escribir tres funciones diferentes?

**8. En carpeta. Vocabulario en inglés.** Leé el diálogo y completá los espacios con las palabras del recuadro.

`argument — input — parameter — value`

**Mia:** My function needs a word to analyze. How can I give it that information?

**Leo:** You can use a __________ in the function definition.

**Mia:** Is the word I provide when I call the function also called a parameter?

**Leo:** The actual data you provide is an __________, also called an argument in this context.

**Mia:** So the parameter receives the __________ provided by the argument?

**Leo:** Exactly! The function uses that information as its __________.

**9. Programación.** Escribí una función llamada `mostrar_palabra(palabra)` que reciba una palabra y muestre:

- La palabra recibida.
- La cantidad de letras que tiene.
- Una invitación a descubrir una pista.

Llamá a la función al menos tres veces con palabras diferentes.

Por ejemplo, podés utilizar palabras relacionadas con animales, tecnología o deportes.

**10. Programación.** Creá una función llamada `comparar_palabras(palabra1, palabra2)` que reciba dos palabras y muestre ambas en una misma oración.

Por ejemplo, al llamarla con `"gato"` y `"perro"`, debería mostrar:

```text
The words are gato and perro.
```

Probá la función con tres pares de palabras diferentes.

---

## 3. Funciones que devuelven un resultado: `return`

Hasta ahora, las funciones que escribimos mostraban información en pantalla mediante `print`. Sin embargo, hay situaciones en las que necesitamos que una función calcule un resultado para que otra parte del programa pueda utilizarlo.

Para eso usamos `return`.

Observá el siguiente ejemplo:

```python
def contar_letras(palabra):
    return len(palabra)

cantidad = contar_letras("aventura")

print(cantidad)
```

El programa muestra:

```text
8
```

La función `contar_letras` recibe una palabra y devuelve la cantidad de caracteres que tiene. El resultado se guarda en la variable `cantidad`.

La instrucción `return` devuelve el resultado al lugar desde el que se llamó a la función. Además, finaliza la ejecución de esa llamada.

### Diferencia entre `print` y `return`

Observá los dos ejemplos:

```python
def contar_a(palabra):
    print(palabra.count("a"))
```

```python
def obtener_cantidad_a(palabra):
    return palabra.count("a")
```

La primera función muestra un resultado, pero no lo devuelve para que podamos guardarlo en una variable.

La segunda función devuelve el resultado, por lo que podemos utilizarlo en otras operaciones.

Por ejemplo:

```python
cantidad = obtener_cantidad_a("banana")
print(cantidad + 2)
```

El resultado será `5`, porque `"banana"` contiene tres letras `a` y luego sumamos dos.

**Para recordar:**

- `print`: muestra información en pantalla.
- `return`: devuelve un resultado que el programa puede utilizar.

No todas las funciones necesitan devolver un resultado. Algunas solo realizan una tarea, como mostrar un mensaje.

### Actividades

**11. En carpeta.** Explicá la diferencia entre `print` y `return`. Para justificar tu respuesta, indicá en cuál de los siguientes casos resulta más conveniente utilizar cada uno:

a. Mostrar las reglas de un juego.

b. Calcular la cantidad de letras de una palabra para utilizarla después.

c. Mostrar un mensaje de bienvenida.

d. Calcular el puntaje de una ronda para sumarlo al puntaje total.

**12. En carpeta.** Analizá el programa y respondé:

```python
def doble(numero):
    return numero * 2

resultado = doble(7)
print(resultado)
print(doble(4))
```

a. ¿Qué aparece en pantalla?

b. ¿Qué valor se guarda en `resultado`?

c. ¿Cuántas veces se llama a la función?

d. ¿Por qué se puede utilizar `doble(4)` directamente dentro de `print`?

**13. En carpeta.** Un alumno escribió:

```python
def sumar(a, b):
    print(a + b)

resultado = sumar(3, 4)
print(resultado + 10)
```

El alumno espera que el programa muestre `17`, pero el programa no funciona como espera.

a. Explicá qué problema tiene.

b. Modificá la función para que el resultado de la suma pueda guardarse en `resultado`.

c. ¿Qué diferencia hay entre mostrar el resultado de una suma y devolverlo?

**14. Programación.** Creá una función llamada `contar_vocales(texto)` que reciba un texto y devuelva cuántas vocales contiene.

Podés utilizar un ciclo `for` y una condición `if` dentro de la función.

Después, llamá a la función con distintos textos y mostrá los resultados.

Por ejemplo, con el texto `"hola mundo"`, la función debería devolver `4`.

**15. Programación.** Creá una función llamada `calcular_puntaje(palabra)` que devuelva un puntaje según la cantidad de letras de una palabra.

La regla será sencilla: cada letra vale 2 puntos.

Después, utilizá el resultado para mostrar un mensaje como el siguiente:

```text
The word "planet" earns 12 points.
```

Probá la función con diferentes palabras.

---

## 4. Dividir un problema en varias funciones

La principal ventaja de las funciones aparece cuando un programa tiene varias tareas relacionadas entre sí.

Imaginemos un juego en el que el participante debe descubrir una palabra secreta. El programa necesita:

- Mostrar las instrucciones.
- Contar las letras de una palabra.
- Calcular el puntaje.
- Mostrar el resultado.

Podemos organizar el código en distintas funciones:

```python
def mostrar_instrucciones():
    print("Guess the secret word!")

def contar_letras(palabra):
    return len(palabra)

def calcular_puntaje(palabra):
    return contar_letras(palabra) * 2

def mostrar_resultado(palabra):
    puntos = calcular_puntaje(palabra)
    print(f"The word has {contar_letras(palabra)} letters.")
    print(f"You earn {puntos} points.")

mostrar_instrucciones()
mostrar_resultado("robot")
```

En este programa, cada función tiene una responsabilidad concreta.

Además, una función puede llamar a otra. Por ejemplo, `mostrar_resultado` utiliza `calcular_puntaje` y `contar_letras`.

Esto permite construir programas más grandes a partir de tareas pequeñas.

No es necesario que cada función tenga una sola línea, ni que todos los programas estén divididos en una gran cantidad de funciones. La idea es separar las tareas que conviene identificar y reutilizar.

### Actividades

**16. En carpeta.** Analizá el programa anterior.

a. ¿Qué función muestra las instrucciones?

b. ¿Qué función devuelve la cantidad de letras?

c. ¿Qué función calcula el puntaje?

d. ¿Qué función se encarga de mostrar el resultado final?

e. Si quisiéramos cambiar la regla de puntaje para que cada letra valiera 5 puntos, ¿qué función habría que modificar?

f. ¿Por qué esta organización facilita los cambios?

**17. En carpeta.** Leé el siguiente programa:

```python
def sumar(a, b):
    return a + b

def multiplicar_por_dos(numero):
    return sumar(numero, numero)

resultado = multiplicar_por_dos(6)
print(resultado)
```

a. Seguí la ejecución paso a paso y predecí el resultado.

b. ¿Qué función llama a otra función?

c. ¿Por qué `multiplicar_por_dos` no necesita realizar directamente la operación `numero * 2`?

d. ¿Qué ventaja tiene reutilizar una función ya escrita?

**18. En carpeta. Vocabulario en inglés.** Leé el diálogo y completá los espacios.

`debug — function — maintain — task`

**Nora:** My program has 150 lines, and it is becoming difficult to understand.

**Ethan:** You should divide it into smaller parts. Each __________ can perform a specific __________.

**Nora:** Will that help me find mistakes?

**Ethan:** Yes. It can make it easier to __________ your code.

**Nora:** And what happens when I need to change something?

**Ethan:** Organized code is usually easier to __________.

**19. Programación.** Vamos a construir un pequeño analizador de palabras.

Creá las siguientes funciones:

- `contar_letras(palabra)`: devuelve la cantidad de letras de una palabra.
- `contar_vocales(palabra)`: devuelve la cantidad de vocales.
- `calcular_puntaje(palabra)`: devuelve el doble de la cantidad de letras.

Después, escribí una parte principal del programa que solicite una palabra al usuario y muestre:

- La palabra ingresada.
- Su cantidad de letras.
- Su cantidad de vocales.
- El puntaje obtenido.

Utilizá las funciones para obtener los resultados, en lugar de repetir las operaciones en la parte principal del programa.

**20. Programación.** Mejorá el analizador de palabras anterior incorporando una función llamada `mostrar_informe(palabra)`.

Esta función debe utilizar las otras funciones para mostrar toda la información de la palabra.

La parte principal del programa debería quedar sencilla: solicitar una palabra y llamar a `mostrar_informe`.

Pensá qué instrucciones deberían estar dentro de cada función para que el programa quede organizado.

---

## 5. Las funciones como herramientas para construir un proyecto

Un programa puede crecer poco a poco. No hace falta resolver todo el problema de una sola vez: podemos construir y probar cada función por separado.

En el proyecto final vamos a desarrollar un analizador de textos con una propuesta lúdica. En lugar de limitarse a contar letras o palabras, el programa podrá proponer desafíos, encontrar palabras interesantes, generar pistas o calcular puntajes.

Para comenzar, vamos a trabajar con un texto corto.

### Actividades

**21. En carpeta. Diseño del programa.**

Imaginá que estás diseñando un juego en el que el usuario introduce una oración y recibe un desafío relacionado con ella.

Proponé al menos cuatro funciones que podría tener el programa. Para cada una, escribí:

- El nombre de la función.
- Qué tarea realizaría.
- Qué información necesitaría recibir.
- Qué resultado debería devolver, si corresponde.

Por ejemplo:

`contar_palabras(texto)`: recibe un texto y devuelve la cantidad de palabras.

Podés inventar tus propias funciones y desafíos.

**22. Programación. Primer prototipo del analizador.**

Creá un programa que solicite al usuario una oración y la analice.

El programa deberá tener, como mínimo, estas funciones:

- `contar_palabras(texto)`: devuelve la cantidad de palabras.
- `contar_vocales(texto)`: devuelve la cantidad de vocales.
- `obtener_palabra_larga(texto)`: devuelve la palabra más larga del texto.

Para esta última función, podés utilizar `split()` para obtener una lista de palabras y un ciclo `for` para recorrerla. Si hay varias palabras con la misma longitud máxima, alcanza con devolver una de ellas.

En la parte principal del programa, solicitá el texto y mostrá los resultados utilizando las funciones.

**23. Programación. Convertimos el análisis en un juego.**

Ahora vamos a agregar una propuesta lúdica al analizador.

Elegí una de estas opciones:

**Opción A. Palabra misteriosa**

El programa muestra la cantidad de letras de una palabra del texto y el usuario debe adivinar cuál es. Podés seleccionar una palabra y mostrar una pista antes de solicitar la respuesta.

**Opción B. Desafío de vocales**

El programa pide al usuario que adivine cuántas vocales contiene el texto. Después, muestra la respuesta correcta y otorga puntos si acertó.

**Opción C. Cazador de palabras largas**

El programa invita al usuario a encontrar una palabra que tenga al menos cierta cantidad de letras. Después, comprueba la respuesta y comunica si cumple la condición.

Organizá el programa utilizando funciones. Podés reutilizar las que ya escribiste en las actividades anteriores.

**24. Reflexión final. En carpeta.**

Respondé las siguientes preguntas:

a. ¿Qué ventajas tiene dividir un programa en funciones?

b. ¿En qué se diferencian un parámetro y un argumento?

c. ¿Cuál es la diferencia entre `print` y `return`?

d. ¿Por qué una función puede llamar a otra?

e. Si tu analizador de textos creciera y tuviera muchas funciones, ¿cómo te ayudaría esta organización a encontrar errores y agregar nuevas características?

f. ¿Qué función nueva agregarías al juego para hacerlo más interesante?

### Para recordar

- Una función agrupa instrucciones que realizan una tarea.
- `def` permite definir una función.
- El nombre seguido de paréntesis permite llamarla.
- Los parámetros reciben información.
- `return` devuelve un resultado que puede utilizarse en otras operaciones.
- Una función puede llamar a otras funciones.
- Dividir un programa en tareas pequeñas facilita su lectura, modificación y reutilización.

**La idea principal es que un programa bien organizado no es solamente un programa que funciona: también es un programa que podemos comprender, modificar y ampliar.**





---
---

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
