---
title: "Introducción a Python"
autor: "José Juarez"
version: "22/06/26"
---


<!-- Image -->
<br>
   <center>![](https://upload.wikimedia.org/wikipedia/commons/3/31/Python-logo.png){width=300px}</center>
   <center>
      <span class="grey3 size70">Logo de Python. </span>
      <span class="grey3 size50">wikimedia.org</span>
   </center>
<br>



<!-- *** GUIDE START *** -->


### 1. ¿Qué es Python?

Python es un lenguaje de programación muy utilizado en educación, ciencia, automatización, desarrollo web e inteligencia artificial. Se caracteriza por tener una sintaxis sencilla y fácil de leer.


<br>


### 2. Instalación de Python

1. Descargar Python desde el sitio oficial: [https://www.python.org](https://www.python.org)

2. Durante la instalación, marcar la opción:

   **✓ Add Python to PATH**

3. Finalizar la instalación.

Para comprobar que funciona, abrir una terminal y escribir:

```bash
python --version
```

Debería aparecer algo similar a (Python más la versión instalada):

```text
Python 3.14.0
```

<br>

### 3. Uso interactivo del intérprete

Abrir una terminal y escribir:

```bash
python
```

Aparecerá algo parecido a:

```text
>>>
```

Ese símbolo indica que Python está esperando instrucciones.

**Ejemplos**

```python
>>> 2 + 3
5

>>> 10 - 4
6

>>> 5 * 7
35

>>> 20 / 4
5.0
```

Para salir:

```python
exit()
```

<br>

### 4. Operadores básicos

Estos operadores nos permiten hacer operaciones con números:


| Operación      | Operador | Ejemplo |
| -------------- | -------- | ------- |
| Suma           | +        | 2 + 3   |
| Resta          | -        | 8 - 5   |
| Multiplicación | *        | 4 * 6   |
| División       | /        | 10 / 2  |
| Potencia       | **       | 2 ** 3  |
| Resto          | %        | 10 % 3  |

**Ejemplos:**

```python
>>> 2 ** 4
16

>>> 10 % 3
1
```

<br>

### 5. Mostrar resultados con `print`

La función `print()` permite mostrar información en pantalla.

```python
print("Hola")
```

Salida:

```text
Hola
```

También puede mostrar números:

```python
print(5 + 3)
```

Salida:

```text
8
```

### 6. Variables

Las variables permiten guardar información. El nombre de una variable debe comenzar con una letra o `_`. Luego del primer carácter pueden contener letras, números o  `_`.

```python
edad = 16
```

Ahora Python recuerda ese valor.

```python
print(edad)
```

Salida:

```text
16
```

También pueden almacenar textos:

```python
nombre = "Ana"
print(nombre)
```

Salida:

```text
Ana
```

<br>

### 7. Operaciones con variables

```python
a = 10
b = 4

print(a + b)
print(a - b)
print(a * b)
print(a / b)
```

Salida:

```text
14
6
40
2.5
```

<br>


### 8. Hacer programas usando variables

Escribir y ejecutar estos ejemplos de programas según las explicaciones de clase.

**Ejemplos:**

*Programa 1: Saludo*

```python
nombre = "Juan"

print("Hola")
print(nombre)
```


*Programa 2: Suma de dos números*

```python
a = 8
b = 5

resultado = a + b

print(resultado)
```

Salida:

```text
13
```


*Programa 3: Área de un rectángulo*

```python
# Las medidas están en metros

base = 6
altura = 4

area = base * altura

print(f"El área en metros cuadrados es: {area}")
```

Salida:

```text
El área en metros cuadrados es: 24
```

#### Actividad

Haz los siguientes programas, usa variables y muestra los resultados:

**a)** Calcula la velocidad de un vehículo que recorre la distancia de 120 metros en el tiempo de 2 segundos. Muestra el resultado en pantalla con el siguiente formato: La velocidad en metros por segundo es: 2

**b)** Una fábrica produce `p` piezas por hora y se trabaja `h` horas por día. Escribe un programa que calcule la producción diaria para p = 35 y h = 8. Muestra el resultado con una frase como: La producción diaria es de 280 piezas.

**c)** Calcula el perímetro de un cuadrado de lado 8 (metros) y muestra el resultado como una frase.

**d)** En Python las variables pueden ir cambiando de valor. Recuerda que Python analiza y ejecuta siempre desde **arriba** hacia **abajo**. Con esto en mente piensa que muestra en pantalla el siguiente programa:

```python
a = 10
b = 20
a = 30
print(a + b)
```

**e)** Un comerciante compra un producto a 3 USD (dólares) y lo vende a $6000 (pesos). ¿Qué ganancia obtuvo si la cotización del dolar cuando lo comrpó era de 1 USD = 1440 pesos? Usa al menos estas variables: costo_en_dolares, costo_en_pesos y muestra el resultado en pantalla.

**f)** Un tanque contiene `a` litros de agua. Se agregan `b` litros y luego se extraen `c` litros. Escribe un programa que represente la cantidad final de agua. Prueba el programa con distintos valores. Muestra el resultado como una frase.

**g)** Prueba el siguiente programa y escribe una explicación de porqué el programa muestra el resultado 101.

```python
cant = 100
cant = cant + 1
print(cant)
```


> Para aprobar esta guía debes mostrar y explicar al profesor los problemas **f)** y **g)**. 
<!-- *** GUIDE END *** -->


<!-- *** GUIDE AUXILIARY TEMPLATES *** -->


<div hidden>


<!-- Learning objectives very briefly -->
<span class="grey3 size85">.</span>

<!-- Image -->
<br>
   <center>{width=400px}</center>
   <center>
      <span class="grey3 size70">. </span>
      <span class="grey3 size50">Fuente: </span>
   </center>
<br>

<!-- Videos: change XXX to the video-id and put time (seconds) -->
<!-- Yotube with start point -->
👉 [Mira este momento clave en el video](https://www.youtube.com/watch?v=XXX&t=123s)
🎬 [Un fragmento que vale la pena ver](https://www.youtube.com/watch?v=XXX&t=123s)
🔎 [Este detalle del video te va a interesar](https://www.youtube.com/watch?v=XXX&t=123s)
⚡ [Dale play a esta parte y fijate qué pasa](https://www.youtube.com/watch?v=XXX&t=123s)
<!-- Youtubetrimmer with start and end point -->
👉 [Mirá este momento puntual del video](https://youtubetrimmer.com/view/?v=XXX&start=120&end=150&loop=0)
🎬 [Este fragmento explica justo lo que necesitamos](https://youtubetrimmer.com/view/?v=XXX&start=120&end=150&loop=0)
⚡ [Dale play a esta parte y sacá tus conclusiones](https://youtubetrimmer.com/view/?v=XXX&start=120&end=150&loop=0)
🔎 [Fijate qué pasa en este momento](https://youtubetrimmer.com/view/?v=XXX&start=120&end=150&loop=0)

<!-- Visible story or anecdote -->
<span class="grey3 size85">...</span>

<!-- Sections -->
<br><span class="grey3 size70">🔁 Repaso:</span>
<br><span class="grey3 size70">🛠️ Trabajo:</span>
<br><span class="grey3 size70">📘 Teoría:</span>
<br><span class="grey3 size70">✅ Autoevaluación:</span>
<br><span class="grey3 size70">📝 Práctica:</span>
**1.**  **:**
**2.** **:** 

<!-- Solutions -->
<div class="grey3 size70">.</div>


</div>


<!-- Guide style definitions -->
<style>
/* Colors */
.grey1 {color: #b3b3b3;} /* my light-grey */
.grey2 {color: #999999;} /* my middle-grey */
.grey3 {color: #808080;} /* my dark-grey */
.blue1 {color: #6495ed;} /* nvim blue */
.blue2 {color: #276cdf;} /* Andrew Ng Blue */
.sky1 {color: #7dbed8;} /* nvim sky */
.sky2 {color: #27a2db;}   /* my sky */
.green {color: #81b524;} /* my green */
.red1 {color: #ec5469;} /* my coral-red */
.red2 {color: #f44336;} /* my red */
.rose {color: #ec9998:} /* nvim rose */
.gold {color: #df9d43;} /* Andrew Ng gold */
.orange1 {color: #fda556;} /* nvim orange */
.orange2 {color: #ff9505;} /* Andrew Ng orange */
.purple1 {color: #ff40ff;} /* Andrew Ng purple */
.purple2 {color: #d164d7;} /* Andrew Ng purple */
/* Font Size */
.size90 {font-size: 0.9em;}
.size85 {font-size: 0.85em;}
.size80 {font-size: 0.8em;}
.size70 {font-size: 0.7em;}
.size60 {font-size: 0.6em;}
.size50 {font-size: 0.5em;}
/* Document General Font Size */
body {font-size: 1.3em;}
/* Bullet "1." see as "1)" */
ol {list-style-type: decimal;}
ol li::marker {content: counter(list-item) ") ";}
/* Two columns */
.two-columns {
  column-count: 2; /* Number of columns */
  column-gap: 20px;
}
/* Indent the example */
.example {margin-left: 20px;}

/* =========================
   IMPRESIÓN A4 – GUÍAS
   ========================= */
@media print {

  @page {
    size: A4;
    margin: 1.2cm;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
    font-size: 10.5pt;
    line-height: 1.35;
    color: #000;

    column-fill: auto; /* Llena una columna y después la otra*/
    column-count: 2;
    column-gap: 1cm;
  }

  h1 {
    font-size: 14pt;
    margin: 0 0 6pt 0;
  }

  h2 {
    font-size: 12pt;
    margin: 8pt 0 4pt 0;
  }

  h3 {
    font-size: 11pt;
    margin: 6pt 0 3pt 0;
  }

  h1, h2, h3 {
    break-after: avoid;
    break-inside: avoid;
  }

  p {
    margin: 0 0 4pt 0;
    text-align: justify;
    break-inside: avoid;
  }

  ul, ol {
    margin: 0 0 4pt 12pt;
    padding: 0;
  }

  li {
    margin-bottom: 2pt;
  }

  code, pre {
    font-family: "Courier New", Courier, monospace;
    font-size: 9.5pt;
    background: #f2f2f2;
    padding: 1px 3px;
    border-radius: 2px;
  }

  pre {
    padding: 6pt;
    overflow: hidden;
    break-inside: avoid;
  }

  img {
    max-width: 100%;
    height: auto;
    break-inside: avoid;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 9.5pt;
  }

  th, td {
    border: 1px solid #000;
    padding: 3pt;
  }

  nav, footer, .no-print {
    display: none;
  }
}
</style>
<!-- Remember: Use <span> inline and <div> with several lines --->
