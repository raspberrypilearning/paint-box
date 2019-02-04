## Cambiar el ancho del marcador

Luego vas a añadir código para permitir que el usuario de tu programa dibuje cosas con diferentes grosor de marcador.

\--- task \--- Primero, añade una nueva variable llamada `ancho`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]] \--- /task \---

\--- task \--- Añade esta línea **dentro** del bucle `forever`{:class="block3control"} del código del objeto lápiz:

```blocks3
cuando se hace clic en la bandera
borrar todo
cambiar disfraz a (lápiz-azul v)
fijar color de marcador a [#0035FF]
siempre
ir a (cursor del ratón v)
+ fijar grosor del marcador a (ancho:: variables)
if <<mouse down?> and <(mouse y) > [-120]>> then
marcador hacia abajo
else
marcador hacia arriba
fin
```

\--- /task \---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

\--- task \--- Right-click on the `width`{:class="block3variables"} variable displayed on the Stage, and then click on **slider**.

![screenshot](images/paint-slider.png) \--- /task \---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

\--- task \--- Test your project and see if you can add code to adjust the pen width.

![screenshot](images/paint-width-test.png) \--- /task \---