## Lo que necesitarás

Comienza haciendo un lápiz que puedes utilizar para dibujar en un Escenario.

\--- task \---

Abre el proyecto inicial de Scratch 'Caja de lápices'.

**Online**: open the starter project at [rpf.io/paint-box-on](https://rpf.io/paint-box-on){:target="_blank"}

Si tienes una cuenta de Scratch puedes hacer una copia haciendo clic en **Reinventar**.

**Offline**: open the [starter project](https://rpf.io/p/en/paint-box-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}

En el proyecto de inicio, deberías ver los objetos lápiz y gomadeborrar:

![captura de pantalla](images/paint-starter.png)

\--- /task \---

\--- task \---

Añade la extensión de lápiz a tu proyecto.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Añade algo de código al objeto lápiz para hacer que siga al ratón `siempre`{:class="block3control"} y así puedas dibujar:

![lápiz](images/pencil.png)

```blocks3
al hacer click en la bandera
por siempre
 ir a (puntero del ratón v)
fin
```

\--- /task \---

\--- task \---

Haz clic en la bandera y luego mueve el puntero del ratón alrededor del Escenario para probar si tu código funciona.

\--- /task \---

Luego, haz que tu lápiz sólo dibuje `si`{:class="block3control"} si se mantiene presionado el botón del ratón.

\--- task \---

Añade este código a tu objeto lápiz:

![lápiz](images/pencil.png)

```blocks3
al hacer clic en la bandera
por siempre
ir a (puntero del ratón v)

+si<mouse down?>entonces
bajar lápiz
si no
subir lápiz
fin
```

\--- /task \---

\--- task \---

Vuelve a probar tu código. Esta vez, mueve el lápiz alrededor del Escenario y mantén presionado el botón del ratón. ¿Puedes dibujar con tu lápiz?

![captura de pantalla](images/paint-draw.png)

\--- /task \---

## \--- collapse \---

## title: ¿Tu lápiz no dibuja desde la punta?

Si la línea que tu lápiz dibuja parece que saliera del medio de tu lápiz, necesitas cambiar el objeto lápiz para que la punta sea el centro del objeto.

Haz clic en el objeto lápiz, y luego haz clic sobre la pestaña **Disfraces**.

Mueve la pestaña de disfraces para que la punta del lápiz esté **justo encima** del centro.

![Centro de disfraces](images/costume-center-annotated.png)

Ahora mueve el lápiz alrededor del Escenario y dibuja. El lápiz ahora debería dibujar una línea desde su punta.

\--- /collapse \---