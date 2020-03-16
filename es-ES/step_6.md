## Cambia el grosor del lápiz

Luego vas a añadir código para permitir que el usuario de tu programa dibuje cosas con diferentes grosores del lápiz.

\--- task \---

Primero, añade una nueva variable llamada `ancho`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Añade esta línea **dentro** del bloque `por siempre` del código del objeto lápiz:

```blocks3
al hacer clic en la bandera
borrar todo
cambiar disfraz a (lápiz-azul v)
fijar color de lápiz a [#0035FF]
por siempre
ir a (puntero del ratón v)
+ fijar tamaño del lápiz a (ancho:: variables)
si <<mouse down?> and <(mouse y) > [-120]>> entonces
bajar lápiz
si no
subir lápiz
fin
```

\--- /task \---

El grosor del lápiz ahora se establece repetidamente en el valor de la variable `ancho` {: class = "block3variables"}.

\--- task \---

Haz clic con el botón derecho del ratón sobre la variable `ancho` {:class="block3variables"} que se muestra en el recuadro del Escenario, y luego selecciona la opción **deslizador**.

![captura de pantalla](images/paint-slider.png)

\--- /task \---

Ahora puedes arrastrar el deslizador que ves debajo de la variable para cambiar el valor de la misma.

![captura de pantalla](images/paint-slider-change.png)

\--- task \---

Prueba tu programa y mira si puedes añadir código para ajustar el grosor del lápiz.

![captura de pantalla](images/paint-width-test.png)

\--- /task \---