## Hacer un lápiz

Comienza haciendo un lápiz que puedes utilizar para dibujar en un Escenario.

\--- task \--- Abre la 'caja de pintura' del proyecto de inicio de Scratch.

**Online**: abre el proyecto de inicio en[rpf.io/caja de pintura](http://rpf.io/paint-box-on){:target="_blank"}

**Offline**: abre el [proyecto de inicio](http://rpf.io/p/en/paint-box-go){:target=_blank"} en el editor offline.

Si necesitas descargar e instalar el editor offline de Scratch, puedes encontrarlo en [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

En el proyecto de inicio, deberías ver los objetos lápiz y borrador:

![captura de pantalla](images/paint-starter.png) \--- /task \---

\--- task \---

Añade la extensión de marcador a tu proyecto.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Añade algo de código al objeto lápiz para hacer que el objeto siga al cursor `forever`{:class="block3control"} así puedes dibujar:

![lápiz](images/pencil.png)

```blocks3
cuando se haga clic en la bandera
siempre
ir a (cursor del ratón v)
fin
```

\--- /task \---

\--- /task\--- Haz clic en la bandera y luego mueve el cursor alrededor del Escenario para comprobar si tu código funciona. \--- /task \---

Luego, haz que tu lápiz sólo dibuje `if`{:class="block3control"} si se mantiene presionado el botón del ratón.

\--- task \--- Añade este código al objeto de tu lápiz:

![lápiz](images/pencil.png)

```blocks3
cuando se haga clic en la bandera
siempre
ir a (cursor del ratón v)

+if<mouse down?>then
marcador abajo
o
marcador arriba
fin
```

\--- /task \---

\--- task \--- Prueba tu código de nuevo. Esta vez, mueve el lápiz alrededor del Escenario y mantén presionado el botón del ratón. ¿Puedes dibujar con tu lápiz?

![captura de pantalla](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: ¿Tu lápiz no dibuja desde la punta?

Si la línea que tu lápiz dibuja parece que sale desde el medio del lápiz, necesitas cambiar tu objeto lápiz de modo que la punta sea el centro del objeto.

Haz clic sobre el objeto lápiz, y luego haz clic sobre la pestaña **Disfraces**.

Mueve el disfraz para que la punta del lápiz esté **justo encima** del centro.

![Centro de disfraces](images/costume-center-annotated.png)

Ahora mueve el lápiz alrededor del Escenario y dibuja. Ahora el lápiz debería dibujar una línea desde la punta.

\--- /collapse \---