## Deshacer errores

A veces se comenten errores, así que añade un botón 'limpiar' y un botón borrador.

\--- task \--- Añade el objeto 'X-block' desde la sección de letras de biblioteca. Colorea el disfraz de objeto de rojo y hazlo más pequeño. Este objeto es el botón 'limpiar'.

[[[generic-scratch3-sprite-from-library]]]

![captura de pantalla](images/paint-x.png) \--- /task \---

\--- task \--- Añade código al objeto 'X-block' para limpiar el Escenario cuando se haga clic en el objeto.

![cruz](images/cross.png) ![blocks_1545296088_6331482](images/blocks_1545296088_6331482.png) \--- /task \---

No necesitas utilizar un `enviar`{:class="block3events"} para limpiar el Escenario, porque el bloque `borrar todo`{:class="block3extensions"} cumple con esa función.

¿Ves que el objeto lápiz incluya un disfraz de borrador?

![captura de pantalla](images/paint-eraser-costume.png)

Tu proyecto también incluye un objeto borrador por separado.

\--- task \--- Haz clic con el botón derecho sobre el objeto borrador y luego haz clic sobre **mostrar**. Aquí se ve cómo debería quedar tu Escenario ahora:

![captura de pantalla](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Añade código al objeto borrador para enviar un `enviar 'borrador'`{:class="block3events"} cuando se hace clic en el objeto borrador.

![borrador](images/eraser.png) ![blocks_1545296089_7129629](images/blocks_1545296089_7129629.png) \--- /task \---

Cuando el objeto lápiz recibe el mensaje 'borrador', debería cambiar su disfraz al borrador y cambiar el color del marcador a blanco, ¡que es del mismo color que el Escenario!

\--- task \--- Añade algo de código para crear un borrador.

\--- hints \--- \--- hint \--- Añade algo de código al objeto lápiz: `Cuando recibo`{:class="block3events"} el mensaje `borrador`{:class="block3events"} `Cambia al disfraz borrador`{:class="block3looks"} `fijar color de marcador`{:class="block3extensions"} a blanco \--- /hint \--- \--- hint \--- Aquí están todos los bloques que necesitas: ![blocks_1545296090_8068566](images/blocks_1545296090_8068566.png) \--- /hint \--- \--- hint \--- Aquí está lo que el código debería decir: ![pencil](images/pencil.png) ![blocks_1545296091_9156106](images/blocks_1545296091_9156106.png) \--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Evalúa tu proyecto para ver si puedes limpiar el Escenario y borrar las líneas del lápiz.

![captura de pantalla](images/paint-erase-test.png) \--- /task \---

Hay un problema más con el lápiz: puedes dibujar en cualquier lugar del Escenario, ¡incluyendo el espacio cerca de los botones 'limpiar' y borrador!

![captura de pantalla](images/paint-draw-problem.png)

\--- task \--- Para arreglar esto, cambia el código de modo que el marcador esté sólo abajo si se hace clic en el ratón **y** la posición del cursor del ratón `y` sea mayor que `120`:

![lápiz](images/pencil.png) ![blocks_1545296093_0167773](images/blocks_1545296093_0167773.png) \--- /task \---

\--- task \--- Evalúa tu proyecto. Ahora no deberías ser capaz de dibujar cerca de los botones.

![captura de pantalla](images/paint-fixed.png) \--- /task \---