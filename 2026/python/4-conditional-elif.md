---
title: "Condicionales con elif"
autor: "José Juarez"
version: "03/08/26"
---


<!-- *** GUIDE START *** -->



## 1. ¿Qué problema resuelve `elif`?

Hasta ahora sabíamos tomar una decisión con dos posibilidades.

```python
edad = int(input("Edad: "))

if edad >= 18:
    print("Mayor de edad")
else:
    print("Menor de edad")
```

Pero... ¿qué pasa si ahora queremos distinguir **tres** (o más) situaciones?

* Menor de edad.
* Tiene exactamente 18 años.
* Mayor de 18 años.

Una posibilidad es usar `elif` que significa **"else if"**, es decir, **"si no, entonces pregunta esto otro"**.

Permite escribir el programa de una forma más clara.

```python
edad = int(input("Edad: "))

if edad > 18:
    print("Mayor de edad")
elif edad == 18:
    print("Tienes exactamente 18 años")
else:
    print("Menor de edad")
```

### Actividad

::: activity

**1)** Hacer en carpeta: Sin ejecutar el programa, completa la tabla.

```python
if numero < 0:
    print("Negativo")
elif numero == 0:
    print("Cero")
elif numero < 10:
    print("Positivo de un dígito")
else:
    print("Positivo de dos o más dígitos")
```

| `numero` | ¿Qué imprime? |
| -------: | ------------- |
|       -4 |               |
|        0 |               |
|        7 |               |
|       10 |               |
|       25 |               |

**2)** Hacer en carpeta: Lee el código y reescríbelo agregando un elif con tiempo "Very cold" mostrando para este caso el mensaje: "Take a coat".

```python
weather = input("Weather: ")

if weather == "rain":
    print("Take an umbrella")
else:
    print("Enjoy your day")
```

:::


## 2. ¿Cómo trabaja Python?

Python analiza las condiciones **de arriba hacia abajo**.

**1.** ¿Se cumple el `if`?

   - Sí → ejecuta ese bloque y termina.
   - No → continúa.

**2.** ¿Se cumple el `elif`?

   - Sí → ejecuta ese bloque y termina.
   - No → continúa.

**3.** Si ninguna condición fue verdadera, ejecuta el `else`.

::: example

**Ejemplo:**

```python
nota = 8

if nota >= 9:
    print("Excelente")
elif nota >= 7:
    print("Aprobado")
elif nota >= 4:
    print("Recupera")
else:
    print("Desaprobado")
```

Como `nota` vale **8**, Python no ejecuta el primer if sino el primer elif. Los demás `elif` y el `else` se ignoran.

:::

### Actividad

::: activity

**1)** Programar y luego escribir el programa en la carpeta: Modificar el ejemplo para que la nota solo sea excelente si es 10 y para que se apruebe con 6.

**2)** Programar: Una estación meteorológica recibe una palabra. Puede ser

```
soleado
nublado
lluvia
```

Mostrar un consejo diferente para cada caso. Y si escribe otra palabra indicar

```
Dato desconocido
```

**3)** Programar: En un videojuego el jugador tiene una cantidad de vidas. hacer un programa que lea la cantidad de vidas de una variable y luego escriba el mensaje según la tabla de abajo.

* 3 vidas → Excelente
* 2 vidas → Cuidado
* 1 vida → Peligro
* 0 → Game Over

:::

## 3. Pensando en el proyecto final

Queremos construir un programa que lea un texto y pueda decir cosas sobre él. Todavía no sabemos hacerlo completo, pero sí podemos comenzar.

### Actividades

::: activity

**1)** Programar: Pedir una palabra. Si es `hola` mostrar `Saludo detectado`. Si es `chau` mostrar `Despedida detectada`. En otro caso `No reconocida`

**2)** Programar: En el mismo programa anterior agregar la opción de que si la palabra es `feliz` mostrar el mensaje: `Es una emoción`

**3)** Crear un programa que detecte si una frase contiene alguna de estas palabras:

```
hola
gracias
chau
```

**Pista:** investigar el operador

```python
in
```

**4)** Mini desafío en parejas: Cada pareja inventará un pequeño "detector". Ideas:

* Detector de saludos.
* Detector de emociones.
* Detector de palabras escolares.
* Detector de deportes.
* Detector de comidas.
* Detector de animales.

Debe reconocer al menos **cinco palabras** utilizando `if`, `elif` y `else`.

:::

::: warning
Para aprobar esta guía como mínimo debes mostrar la carpeta con los ejercicios pedidos y el programa que hiciste en la actividad 3 del punto 3. Además debes responder las preguntas que te haga el profesor.
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
![](imagen.png){width=400px}

<small>Pie (Source)</small>
:::

[⌕](../../images/ ) 

● Videos:

 Change XXX to video-id and put time in seconds

 - Yotube with start point: [Mira este momento clave en el video](https://www.youtube.com/watch?v=XXX&t=123s)

 - Youtubetrimmer with start and end point: [Mirá este momento puntual del video](https://youtubetrimmer.com/view/?v=XXX&start=120&end=150&loop=0)

-->
