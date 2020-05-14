## Haz un lápiz

Comienza haciendo un lápiz que puedes utilizar para dibujar en un Escenario.

\--- task \---

Abre el proyecto inicial de Scratch 'Caja de lápices'.

**Online**: abre el proyecto de inicio en [rpf.io/paint-box-on](http://rpf.io/paint-box-on){:target="_blank"}

Si tienes una cuenta de Scratch puedes hacer una copia haciendo clic en **Remix**.

**Offline**: abre el [proyecto de inicio](http://rpf.io/p/en/paint-box-go){:target=_blank"} en el editor offline.

Si necesitas descargar e instalar el editor offline de Scratch, puedes encontrarlo en [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

En el proyecto de inicio, deberías ver los objetos lápiz y borrador:

![captura de pantalla](images/paint-starter.png)

\--- /task \---

\--- task \---

Añadir la extensión de lápiz a tu proyecto.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Añade algo de código al objeto lápiz para hacer que el objeto siga al cursor `forever`{:class="block3control"} así puedes dibujar:

![lápiz](images/pencil.png)

```blocks3
al presionar bandera
por siempre 
  ir a (mouse pointer v)
end
```

\--- /task \---

\--- task \---

Haz clic en la bandera y luego mueve el puntero del ratón alrededor del Escenario para probar si tu código funciona.

\--- /task \---

Luego, haz que tu lápiz sólo dibuje `if`{:class="block3control"} si se mantiene presionado el botón del ratón.

\--- task \---

Añade este código a tu objeto lápiz:

![lápiz](images/pencil.png)

```blocks3
al presionar bandera
por siempre 
  ir a (mouse pointer v)
  + si <mouse down?> entonces 
  +   lápiz abajo
  + si no 
  +   lápiz arriba
  + end
end
```

\--- /task \---

\--- task \---

Vuelve a probar tu código. Esta vez, mueve el lápiz alrededor del Escenario y mantén presionado el botón del ratón. ¿Puedes dibujar con tu lápiz?

![captura de pantalla](images/paint-draw.png)

\--- /task \---

## \--- collapse \---

## title: ¿Tu lápiz no dibuja desde la punta?

Si la línea que tu lápiz dibuja parece que sale desde el medio del lápiz, necesitas cambiar tu objeto lápiz de modo que la punta sea el centro del objeto.

Haz clic sobre el objeto lápiz, y luego haz clic sobre la pestaña **Disfraces**.

Mueve el disfraz para que la punta del lápiz esté **justo encima** del centro.

![Centro de disfraces](images/costume-center-annotated.png)

Ahora mueve el lápiz alrededor del Escenario y dibuja. Ahora el lápiz debería dibujar una línea desde la punta.

\--- /collapse \---