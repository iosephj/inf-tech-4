---
title: "Condicionales (if - else)"
autor: "José Juarez"
version: "13/07/26"
---

<!-- *** GUIDE START *** -->

## 1. Repaso de inglés

### Actividad

Resuelve estas actividades en la carpeta:

::: activity

1) Une cada palabra con su significado.

```
  if          verdadero

  false       si

  else        falso

  true        si no
```

2) Lee el siguiente texto y completa los espacios usando las palabras: **if – hungry – rains – umbrella – home – true – false**

Every morning I look outside. **If** it **____________**, I take an **____________**. If the weather is good, I walk to school. If I am **____________**, I eat breakfast before leaving **____________**. A condition can be **____________** or **____________**. We use the same idea when we write programs in Python.

:::


## 2. Tomar decisiones con "if"

Hasta ahora todos nuestros programas ejecutaban siempre las mismas instrucciones.

Pero muchas veces queremos que el programa decida qué hacer, por jemplo: 

* Si el alumno aprobó, mostrar un mensaje.
* Si una persona es mayor de edad, permitir el ingreso.

Para eso usamos `if`.

### La estructura básica

```python
if condición:
    instrucciones
```

Si la condición es verdadera (`True`), las instrucciones se ejecutan.

Si la condición es falsa (`False`), se omiten.


::: example

**Ejemplo**

```python
edad = int(input("Edad: "))

if edad >= 18:
    print("Eres mayor de edad.")
```

Si el usuario escribe 20 la condición `edad >= 18` es verdadera y etonces aparece `Eres mayor de edad`.

Si escribe 15 la condición es falsa y el el programa no imprime el mensaje.

:::

### Las condiciones

Una condición produce solamente dos resultados posibles.

* `True`
* `False`

::: example

Ejemplos:

`10 > 5` da como resultado `True`

`3 > 8` da como resultado `False`

:::

Recuerda los operadores que se usan para comparar:


| Operador | Significado       |
| -------- | ----------------- |
| ==       | igual que         |
| !=       | distinto de       |
| >        | mayor que         |
| <        | menor que         |
| >=       | mayor o igual que |
| <=       | menor o igual que |


### Actividad

::: activity

1) Escribe un programa que pregunte e ingrese la edad. Si la persona tiene 18 años o más, mostrar: `Puede votar.`
2) Escribe un programa que pregunte e ingrese un número entero. Si el número es positivo, mostrar: `El número es positivo`.
3) Pide ingrasar la temperatura. Si es mayor que 30 grados, mostrar: `Hace mucho calor.`
4) **Sistema de ingreso a una competencia:** Escribe un programa que pregunte:

* nombre del participante;
* edad;
* promedio escolar.

El programa debe hacer lo siguiente:

* Si la persona tiene **16 años o más** y su promedio es **7 o mayor**, mostrar: `Felicitaciones, puedes inscribirte`

* Si no cumple la condición, el programa no debe mostrar ese mensaje.

Además, siempre debe mostrar al final: `Gracias por utilizar el sistema.`

:::


## 3. El uso de else

Cuando la condición es falsa y queremos tomar acciones hay que usar `else`

::: example

**Ejemplo**

```python
edad = int(input("Edad: "))

if edad >= 18:
    print("Eres mayor de edad.")

else:
    print("Eres menor de edad")
```

Aquí si el usuario escribe 15 la condición es falsa y el el programa imprime el mensaje: `Eres menor de edad`.

:::

### Actividades

::: activity

1) Pide un número e indica si es positivo o negativo. Se supone que nunca se ingresa el cero que no es ni positivo ni negativo.
2) Pide dos números. Indica cuál de los dos es mayor.
3) Pide la nota de un examen. Si la nota es 7 o mayor, mostrar: `Aprobado`. En caso contrario: `Desaprobado`
4) Pide la contraseña. La contraseña correcta es: `python123`. Si coincide, mostrar: `Acceso permitido`. Si no coincide: `Acceso denegado`
5) **Sistema de acceso a un torneo escolar:** Escribe un programa que solicite:

* Nombre del participante.
* Edad.
* Promedio general.
* ¿Presentó la autorización? (responder **si** o **no**).

El participante podrá inscribirse **únicamente si**:

* tiene **16 años o más**, **y**
* su promedio es **7 o superior**, **y**
* presentó la autorización.

Si cumple todas las condiciones, mostrar:

```
¡Felicitaciones, [nombre]!
Tu inscripción fue aceptada.
```

En caso contrario, mostrar:

```
Lo sentimos, no cumples los requisitos para participar.
```

Al finalizar, el programa debe imprimir:

```
Gracias por utilizar el sistema.
```

::: warning
Para aprobar esta guía de deben mostrar todos las actividades y explicar este último problema.
:::

:::





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
