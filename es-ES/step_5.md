## Deshacer errores

A veces se comenten errores, así que añade un botón 'limpiar' y un botón borrador.

\--- task \--- Añade el objeto 'X-block' desde la sección de letras de biblioteca. Colorea el disfraz de objeto de rojo y hazlo más pequeño. Este objeto es el botón 'limpiar'.

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png) \--- /task \---

\--- task \--- Añade código al objeto 'X-block' para limpiar el Escenario cuando se haga clic en el objeto.

![cross](images/cross.png) ![blocks_1545296088_6331482](images/blocks_1545296088_6331482.png) \--- /task \---

No necesitas utilizar un `enviar`{:class="block3events"} para limpiar el Escenario, porque el bloque `borrar todo`{:class="block3extensions"} cumple con esa función.

¿Ves que el objeto lápiz incluya un disfraz de borrador?

![screenshot](images/paint-eraser-costume.png)

Tu proyecto también incluye un objeto borrador por separado.

\--- task \--- Haz clic con el botón derecho sobre el objeto borrador y luego haz clic sobre **mostrar**. Aquí se ve cómo debería quedar tu Escenario ahora:

![screenshot](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Añade código al objeto borrador para enviar un `enviar 'borrador'`{:class="block3events"} cuando se hace clic en el objeto borrador.

![eraser](images/eraser.png) ![blocks_1545296089_7129629](images/blocks_1545296089_7129629.png) \--- /task \---

Cuando el objeto lápiz recibe el mensaje 'borrador', debería cambiar su disfraz al borrador y cambiar el color del marcador a blanco, ¡que es del mismo color que el Escenario!

\--- task \--- Añade algo de código para crear un borrador.

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white \--- /hint \--- \--- hint \--- Here are all the blocks you need: ![blocks_1545296090_8068566](images/blocks_1545296090_8068566.png) \--- /hint \--- \--- hint \--- Here is what the code should look like: ![pencil](images/pencil.png) ![blocks_1545296091_9156106](images/blocks_1545296091_9156106.png) \--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Test your project to see if you can clear the Stage and erase pencil lines.

![screenshot](images/paint-erase-test.png) \--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![screenshot](images/paint-draw-problem.png)

\--- task \--- To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![pencil](images/pencil.png) ![blocks_1545296093_0167773](images/blocks_1545296093_0167773.png) \--- /task \---

\--- task \--- Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png) \--- /task \---