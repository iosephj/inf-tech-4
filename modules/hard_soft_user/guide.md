---
tit|le: "Componentes de los sistemas informáticos"
autor: "José Juarez"
version: "12/04/26"
---


<!-- Image -->
<br>
   <center>![](https://imgs.search.brave.com/X9tP8QhFI-tS9wMWz40ojzkBGa4RGon55SZ3liNn5pM/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9kaWdp/dGFsZWsuY29tL3dw/LWNvbnRlbnQvdXBs/b2Fkcy8yMDI0LzA5/L3NvZnR3YXJlLXkt/aGFyZHdhcmUucG5n){width=400px}</center>
   <center>
      <span class="grey3 size70">Hardware - Software - Users. </span>
      <span class="grey3 size50">Fuente: digitalek.com</span>
   </center>
<br>



<!-- *** GUIDE START *** -->

### 1. ¿Qué es un sistema informático?

Un sistema informático es un conjunto de elementos que trabajan juntos para procesar información.

Está formado por:

- **Hardware**: partes físicas (lo que se puede tocar)
- **Software**: programas (lo que da instrucciones)
- **Usuario**: quien utiliza el sistema

🔹 Idea clave: *ninguno funciona solo, siempre trabajan juntos.*


#### Actividad 1

<span class="grey3 size50">Conexión con Inglés</span>

Aprende el significado y pronunciación de "hard" y "soft". Luego copia la siguiente frase en la carpeta pero completando las palabras que faltan.

*Hardware come from _____ (physical parts) and software _____ from "soft" (intangible instructions). _____ work with users to operate a computer system.*


<br>


### 2. Reconociendo un sistema informático

Observa un dispositivo digital o una computadora que utilices habitualmente (puede ser una PC, notebook, tablet o celular).

Respondé:

- ¿Qué partes del dispositivo podés identificar como hardware?
- ¿Qué programas o aplicaciones utilizas en ese dispositivo (software)?
- ¿Qué periféricos de entrada y salida intervienen cuando lo usas (teclado, mouse, pantalla, parlantes, etc.)?
- ¿Cómo circula la información cuando realizás una acción simple, como escribir un mensaje o abrir un programa?

**Ejemplo:**

Enviar un mensaje por WhatsApp

- Hardware: celular, pantalla, batería
- Software: aplicación WhatsApp, sistema operativo
- Usuario: la persona que escribe y envía


#### Actividad 2

Identificá los componentes:

1. Imprimir un archivo
2. Ver un video en YouTube
3. Escribir un texto

**Respuesta (autocorrección):**

<details>
<summary>Ver respuestas</summary>

1. Hardware: impresora, PC  
   Software: programa de impresión  
   Usuario: quien imprime  

2. Hardware: celular/PC  
   Software: navegador/app  
   Usuario: quien mira  

3. Hardware: teclado, monitor  
   Software: procesador de texto  
   Usuario: quien escribe  

</details>


<br>


### 3. Hardware

El hardware se puede clasificar según su función:

- **Entrada**: teclado, mouse
- **Salida**: monitor, impresora
- **Procesamiento**: CPU
- **Almacenamiento**: disco, pendrive


#### Actividad 3

Haz un esquema de los componentes principales del hardware usando la aplicación Paint. Para esto:

a) Copia la imagen de abajo (por ejemplo con la tecla "Imprimir Pantalla") y pégala en Paint.

b) Arréglala de modo que quede limpia y de tamaño adecuado.

c) Agrega los nombres de cada componente numerado tanto en español como en inglés. Por ejemplo: **(1)** Pantalla / Screen.

<!-- Image -->
<br>
   <center>![](intro_computers_hard_external1_400px.png){width=500px}</center>
   <center>
      <span class="grey3 size50">Fuente: internet</span>
   </center>
<br>

<span class="red1 size70">**Importante** debes mostrar la pantalla con la tarea hecha en tiempo de clase, es una de las condiciones para aprobar esta unidad.</span>


<br>


### 4. Software

El software indica qué hacer al hardware.

Tipos:

- **Sistema operativo**: controla el equipo (Windows, Android)
- **Aplicaciones**: programas que usamos (Word, navegador)

El software funciona como por capas, por ejemplo la capa que comanda más directamete el usuario es la capa de aplicaciones como se muestra abajo.

<!-- Image -->
<br>
   <center>![](intro_computers_soft_schemme_800px__wikimedia_commons__con_atrib.png){width=400px}</center>
   <center>
      <span class="grey3 size50">Fuente: internet</span>
   </center>
<br>


#### Actividad 4

**a)** Haz un dibujo en la carpeta como el anterior pero poniendo los nombres en español.

**b)** Investiga y escribe brevemente en tres reglones las formas de interactuar con el sistema operativo que tiene el usuario. En tu explicación tienen que aparecer las frases: "interfaz gráfica" y "intérprete de comando".


<br>


### 5. Complemento histórico

La máquina analítica de Babbage (siglo XIX) es considerada la primera computadora programable. 

#### Actividad 5

Investiga y escribe sobre la máquina analítica de Babbage.


<br>


### 6. Introducción a CMD y PowerShell

En Windows existen herramientas llamadas **intérpretes de comandos** o **terminales**, que permiten interactuar con la computadora escribiendo órdenes en texto. Dos de las más usadas son el **CMD (Símbolo del sistema)** y **PowerShell**.

El **CMD** es más antiguo y sencillo. Permite realizar tareas básicas como navegar entre carpetas, copiar archivos o ejecutar programas.

El **PowerShell** es más moderno y potente. Además de ejecutar comandos similares al CMD, puede trabajar con objetos, automatizar tareas y administrar el sistema de manera más avanzada.

Aprender a usar la terminal ayuda a comprender mejor cómo funciona el sistema operativo y permite realizar tareas de forma rápida y eficiente.

#### Actividad 6

Estos son algunos comandos básicos

| Comando | Función                            |
| ------- | ---------------------------------- |
| `dir`   | Muestra archivos y carpetas        |
| `cd`    | Cambia de carpeta                  |
| `mkdir` | Crea una carpeta                   |
| `cls`   | Limpia la pantalla                 |
| `echo`  | Muestra texto                      |
| `type`  | Muestra el contenido de un archivo |

**Ejercicios de práctica:**

**a)** Abrir la terminal

1. Abrir CMD o PowerShell.
2. Escribir:

```bash
echo Hola mundo
```

3. Presionar Enter. (Siempre se presiona Enter luego de cada comando)

**b)** Ver contenido de una carpeta

1. Escribir:

```bash
dir
```

2. Observar los archivos y carpetas que aparecen.
3. Ahora abre el explorador de archivos y busca la carpeta "Mis documentos". Escribe cmd en la barra de direcciones del explorador y se abrirá el terminal en esa ubicación, verás algo como: `C:\Users\User\Documents>` donde user es el nombre del usuario.
4. Pon `dir` y presiona Enter para ver el contenido de la carpeta

<div hidden>
También puedes abrir CMD directamente sobre una carpeta específica haciendo:

Shift + clic derecho en una carpeta → “Abrir terminal aquí”
o escribiendo cmd en la barra de direcciones del Explorador de archivos.
</div>

**c)** Crear una carpeta y un archivo

1. Abre CMD o PowerShell en "Mis Documentos" como en el punto anterior. Luego creas una carpeta llamada `practica` con `mkdir` (Siempre presiona :

```bash
mkdir practica
```

2. Verificar que se haya creado usando `dir`.

3. Crear un archivo de texto llamado test.txt:

```bash
echo Este es un archivo de testeo > test.txt
```

4. Mostrar el contenido del archivo:

```bash
type texto.txt
```

**d)** Ejercicio Opcional

1. Copiar el archivo:

```bash
copy test.txt copia.txt
```

2. Verificar con `dir`.
3. Abrir el archivo con "Bloc de Notas" y agregarle un renglón con el siguiente texto: "Hola, este es otro renglón". Luego guardar y cerrar.
4. Mostrar el contenido del archivo nuevamente con `type`


<!-- *** GUIDE END *** -->


<!-- *** GUIDE AUXILIARY TEMPLATES *** -->


<div hidden>


<!-- Learning objectives very briefly -->
<span class="grey3 size85">.</span>

<!-- Image -->
<br>
   <center>![](){width=400px}</center>
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
.orange2 {color: #ff9505;} /*Andrew Ng orange */
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
</style>
<!-- Use <span> inline and <div> with several lines --->
