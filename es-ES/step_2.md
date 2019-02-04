## Hacer un lápiz

Comienza haciendo un lápiz que puedes utilizar para dibujar en un Escenario.

\--- task \--- Abre la 'caja de pintura' del proyecto de inicio de Scratch.

**Online**: abre el proyecto de inicio en[rpf.io/caja de pintura](http://rpf.io/paint-box-on){:target="_blank"}

**Offline**: abre el [proyecto de inicio](http://rpf.io/p/en/paint-box-go){:target=_blank"} en el editor offline.

Si necesitas descargar e instalar el editor offline de Scratch, puedes encontrarlo en [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

En el proyecto de inicio, deberías ver los sprites del lápiz y el borrador:

![captura de pantalla](images/paint-starter.png) \--- /task \---

\--- task \---

Agrega la extensión de marcador a tu proyecto.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Agrega algo de código al sprite del lápiz para hacer que el sprite siga al cursor `forever`{:class="block3control"} así puedes dibujar:

![lápiz](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

\--- /task \---

\--- /task\--- Haz clic en la bandera y luego mueve el cursor alrededor del Escenario para comprobar si tu código funciona. \--- /task \---

Luego, haz que tu lápiz sólo dibuje `if`{:class="block3control"} si se mantiene presionado el botón del ratón.

\--- task \--- Agrega este código al sprite de tu lápiz:

![pencil](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)

+ if <mouse down?> then
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \--- Test your code again. This time, move the pencil around the Stage and hold down the mouse button. Can you draw with your pencil?

![screenshot](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: ¿Tu lápiz no dibuja desde la punta?

If the line your pencil draw looks like it is coming from the pencil's middle, you need to change your pencil sprite's so the tip is the sprite's centre.

Click on the pencil sprite, and then click on the **Costumes** tab.

Move the costume's so the tip of the pencil is **just above** the centre.

![Costume center](images/costume-center-annotated.png)

Now move the pencil around on the Stage and draw. The pencil should now draw a line from its tip.

\--- /collapse \---