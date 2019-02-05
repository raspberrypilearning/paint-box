## Deshacer errores

A veces se comenten errores, así que añade un botón 'limpiar' y un botón borrador.

\--- task \--- Añade el objeto 'X-block' desde la sección de letras de biblioteca. Colorea el disfraz de objeto de rojo y hazlo más pequeño. Este objeto es el botón 'limpiar'.

[[[generic-scratch3-sprite-from-library]]]

![captura de pantalla](images/paint-x.png) \--- /task \---

\--- task \--- Añade código al objeto 'X-block' para limpiar el Escenario cuando se haga clic en el objeto.

![cross](images/cross.png)

```blocks3
cuando se hace clic en este objeto
borrar todo
```

\--- /task \---

No es necesario utilizar un `enviar`{:class="block3events"} para limpiar un Escenario, porque el bloque `borrar todo`{:class="block3extensions"} cumple esa función.

¿Ves que el objeto lápiz incluye un disfraz de borrador?

![screenshot](images/paint-eraser-costume.png)

Tu proyecto también incluye un objeto borrador por separado.

\--- task \--- Haz clic con el botón derecho sobre el objeto borrador y luego haz clic sobre **mostrar**. Aquí está cómo debería quedar el Escenario ahora:

![screenshot](images/paint-eraser-stage.png) \--- /task \---

Añade código al objeto borrador para enviar un `enviar 'borrador'`{:class="block3events"} cuando se hace clic en el objeto borrador.

![eraser](images/eraser.png)

```blocks3
cuando se hace clic en este objeto
enviar (borrador v)
```

\--- /task \---

Cuando el objeto lápiz reciba el mensaje 'borrador', ¡debería cambiar su disfraz al de borrador y cambiar el color del marcador a blanco, que es el mismo color que el Escenario!

\--- task \--- Añade algo de código para crear el borrador.

\--- hints \--- \--- hint \--- Añade algo de código al objeto lápiz: `Cuando reciba`{:class="block3events"} el mensaje `borrador`{:class="block3events"} `Cambia a borrador de disfraz`{:class="block3looks"} `Fija el color del marcador`{:class="block3extensions"} a blanco \--- /hint \--- \--- hint \--- Aquí están todos los bloques que necesitas:

```blocks3
fijar el color del marcador a [#FFFFFF]
cuando reciba [borrador v]

cambia el disfraz a (borrador v)
```

\--- /hint \--- \--- hint \--- Aquí está cómo debería lucir el código: ![pencil](images/pencil.png)

```blocks3
cuando reciba [borrador v]
cambia disfraz a (borrador v)
fija el color del marcador a [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Test your project to see if you can clear the Stage and erase pencil lines.

![screenshot](images/paint-erase-test.png) \--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![screenshot](images/paint-draw-problem.png)

\--- task \--- To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![pencil](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
  go to (mouse pointer v)
+if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \--- Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png) \--- /task \---