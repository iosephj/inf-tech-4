---
title: "Generador de historias locas"
autor: "José Juarez"
version: "15/11/26"
---

<!-- *** GUIDE START *** -->


## Consigna

¡Llegó el momento de mostrar con humor lo que aprendiste de Python! Tu misión es programar un generador de historias locas que le pida palabras al usuario de forma desordenada y luego arme un relato humorístico único.

Abajo de la historia loca se muestra el siguiente informe:

~~~
Análisis de la historia loca:

- Cantidad de palabras: _____
- Cantidad total de vocales: [___, ___, ___, ___, ___, ___]
~~~

Se cuentan tanto las vocales mayúsculas como minúsculas. Los resultados se presentan como una lista en donde el primer número de la lista es la cantidad de "a" o "A" que aparecen en el texto, el segundo elemento es la cantidad de "e" o "E", y así sucesivamente.


**Requisitos obligatorios:**

1. Usar **`input()`** para pedir al menos 4 palabras distintas (ej: un sustantivo, un adjetivo, un verbo, un lugar).
2. Utilizar **f-strings** (`f"..."`) para insertar las palabras dentro de tu historia loca predefinida.
3. Usar "solo" los recursos aprendidos para calcular lo pedido en el informe, por ejemplo no puedes usar `split` para armar una lista con las palabras del texto. Puedes hacer la parte del análisis como una o varias funciones aparte.

**Ejemplo**

Se muestra aquí un ejemplo no completo con dos palabras:

::: example

```python
print("--- ¡Mini Historias locas! ---")

# Pedir las palabras
animal = input("Ingresa un animal: ")
lugar = input("Ingresa un lugar: ")

# Insertarlas en la frase
historia = f"Un día, un {animal} decidió irse de vacaciones a {lugar}. ¡Qué locura!"

# Mostrar historia
print("\nHistoria loca:")
print(historia)

# Calcular y mostrar lo pedido en el informe
#  - Resolver esto aquí.
#  - También puedes hacerlo como una o varias funciones aparte y llamarlas
#    desde aquí. Esto tiene más puntaje.

```

:::

**Sugerencias:**

- Puedes considerar que la cantidad de palabras está relacionada con la cantidad de espacios vacíos "  " que hay en el texto.
- Una forma de hacer la lista de vocales es armar una lista inicial como `vocal = [0, 0, 0, 0, 0]`. Luego con un bucle recorres el texto y cada vez que encuentras una "a" o "A" haces `vocal[0] = vocal[0] + 1`

**PLUS**: Si quieres un desafío de mayor altura puedes calcular la palabra más larga de la historia y agregarla en el informe. Si hay muchas palabras más largas basta con poner una de ellas.


---

::: warning
**Criterio de aprobación:** Esta guía es para los que aspiran a una buena nota. Se aprueba mostrando y explicando el programa y respondiendo las preguntas que te hagan.
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
