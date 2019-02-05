## Deshacer errores

A veces se comenten errores, así que añade un botón 'limpiar' y un botón borrador.

\--- task \--- Añade el objeto 'X-block' desde la sección de letras de biblioteca. Colorea el disfraz de objeto de rojo y hazlo más pequeño. Este objeto es el botón 'limpiar'.

[[[generic-scratch3-sprite-from-library]]]

![captura de pantalla](images/paint-x.png) \--- /task \---

\--- task \--- Añade código al objeto 'X-block' para limpiar el Escenario cuando se haga clic en el objeto.

![cruz](images/cross.png)

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

\--- task \--- Prueba tu proyecto para ver si puedes limpiar el Escenario y borrar las líneas del lápiz.

![screenshot](images/paint-erase-test.png) \--- /task \---

Hay otro problema más con el lápiz: puedes dibujar donde sea en el Escenario, incluyendo el espacio cerca de los botones 'limpiar' y borrar!

![screenshot](images/paint-draw-problem.png)

\--- task \--- Para arreglar esto, cambia el código de modo que el marcador esté abajo sólo si se hace clic en el ratón **y** la posición del cursor `y` es mayor que `-120`:

![pencil](images/pencil.png)

```blocks3
cuando se haga clic en la bandera
borrar todo
cambia disfraz a (lápiz-azul v)
fijar el color del marcador a [#0035FF]
siempre
ir a (cursor del ratón v)
+if <<mouse down?> and <(mouse y) > [-120]>> then 
marcador abajo
o
marcador arriba
fin
```

\--- /task \---

\--- task \--- Prueba tu proyecto. Ahora no deberías ser capaz de dibujar cerca de los botones.

![screenshot](images/paint-fixed.png) \--- /task \---