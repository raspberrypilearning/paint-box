## Cometiendo errores

A veces se comenten errores, así que añade un botón 'limpiar' y un botón 'gomadeborrar'.

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

Click on this eraser sprite and then select **show**.

![captura de pantalla](images/show-eraser.png)

Here is how your Stage should look now:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
al hacer clic en este objeto
enviar (borrador v)
```

\--- /task \---

When the pencil sprite receives the 'eraser' message, it should switch its costume to the eraser and switch the pen colour to white, which is the same colour as the Stage!

\--- task \---

Add some code to create the eraser.

\--- hints \--- \--- hint \---

Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

\--- /hint \--- \--- hint \---

Here are all the blocks you need:

```blocks3
fijar color de lápiz a [#FFFFFF]
al recibir [borrador v]

cambiar disfraz a (gomadeborrar v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
al recibir [borrador v]
cambia disfraz a (gomadeborrar v)
fijar color de lápiz a [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \---

Test your project to see if you can clear the Stage and erase pencil lines.

![screenshot](images/paint-erase-test.png)

\--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![screenshot](images/paint-draw-problem.png)

\--- task \---

To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

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

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---