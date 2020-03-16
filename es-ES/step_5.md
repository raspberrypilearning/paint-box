## Cometiendo errores

A veces se comenten errores, así que añade un botón 'limpiar' y un botón gomadeborrar.

\--- task \---

Añade el objeto ‘X-block’ desde la sección letras de la biblioteca. Colorea el disfraz del objeto de rojo y hazlo más pequeño. Este objeto es el botón 'limpiar'.

[[[generic-scratch3-sprite-from-library]]]

![captura de pantalla](images/paint-x.png)

\--- /task \---

\--- task \---

Añade código al objeto ‘X-block’ para limpiar el Escenario cuando se haga clic en el objeto.

![cruz](images/cross.png)

```blocks3
al hacer clic en este objeto
borrar todo
```

\--- /task \---

No necesitas utilizar un `enviar`{:class="block3events"} para limpiar el Escenario, porque el bloque `borrar todo`{:class="block3extensions"} cumple con esa función.

¿Ves que el objeto lápiz incluye un disfraz de goma de borrar?

![captura de pantalla](images/paint-eraser-costume.png)

Tu proyecto también incluye un objeto gomadeborrar aparte.

\--- task \---

Ve al cajón de las características del objeto (encima de la gomadeborrar) y haz clic sobre (el icono en forma de ojo) **mostrar**. Aquí se ve cómo debería quedar tu Escenario ahora:

![captura de pantalla](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Añade código al objeto gomadeborrar para mandar el mensaje `enviar 'borrador'`{:class="block3events"} cuando se haga clic en el objeto gomadeborrar.

![borrador](images/eraser.png)

```blocks3
al hacer clic en este objeto
enviar (borrador v)
```

\--- /task \---

Cuando el objeto lápiz recibe el mensaje 'borrador', debería cambiar su disfraz al de gomadeborrar y cambiar el color del marcador a blanco, ¡que es del mismo color que el Escenario!

\--- task \---

Añade código para definir la goma de borrar.

\--- hints \--- \--- hint \---

Añade algo de código al objeto lápiz: `al recibir`{:class="block3events"} el mensaje `borrador`{:class="block3events"} `cambiar disfraz a gomadeborrar`{:class="block3looks"} `fijar color de lápiz a`{:class="block3extensions"} blanco

\--- /hint \--- \--- hint \---

Aquí están todos los bloques que necesitas:

```blocks3
fijar color de lápiz a [#FFFFFF]
al recibir [borrador v]

cambiar disfraz a (gomadeborrar v)
```

\--- /hint \--- \--- hint \---

Así es como debería verse tu código:

![lápiz](images/pencil.png)

```blocks3
al recibir [borrador v]
cambia disfraz a (gomadeborrar v)
fijar color de lápiz a [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \---

Prueba tu proyecto para ver si puedes limpiar el Escenario y borrar las líneas del lápiz.

![captura de pantalla](images/paint-erase-test.png)

\--- /task \---

Hay un problema más con el lápiz: puedes dibujar en cualquier lugar del Escenario, ¡incluyendo el espacio cerca de los botones 'limpiar' y gomadeborrar!

![captura de pantalla](images/paint-draw-problem.png)

\--- task \---

Para arreglar esto, cambia el código de modo que el lápiz esté abajo sólo si se hace clic en el ratón **y** la posición `y` del cursor sea mayor que `-120`:

![pencil](images/pencil.png)

```blocks3
al hacer clic en la bandera
borrar todo
cambia disfraz a (lápiz-azul v)
fijar color de lápiz a [#0035FF]
por siempre
ir a (puntero del ratón v)
+si <<mouse down?> y <(mouse y) > [-120]>> entonces 
bajar lápiz
si no
subir lápiz
fin
```

\--- /task \---

\--- task \---

Prueba tu proyecto. Ahora no deberías ser capaz de dibujar cerca de los botones.

![captura de pantalla](images/paint-fixed.png)

\--- /task \---