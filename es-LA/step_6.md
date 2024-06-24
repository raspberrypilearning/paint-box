## Cambiar el ancho del lápiz

Luego vas a añadir código para permitir que la persona que use tu programa dibuje cosas con diferentes anchos de lapices.

--- task ---

Primero, añade una nueva variable llamada `ancho`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

Añade esta linea **dentro** del bucle `por siempre`{:class="block3control"} del código del lápiz:

```blocks3
when flag clicked
erase all
switch costume to (lápiz-azul v)
set pen color to [#0035FF]
forever
go to (puntero del ratón v)
+set pen size to (ancho :: variables)
if <<mouse down?> and <(posición y del ratón) > [-120]>> then 
  pen down
  else
  pen up
end
```

--- /task ---

El ancho del lápiz ahora se vuelve repetidamente del valor de la variable `ancho`{:class="block3variables"}.

--- task ---

Haz clic con el botón derecho del ratón sobre la variable `ancho`{:class="block3variables"} que se muestra en el recuadro del Escenario, y luego selecciona la opción **deslizador**.

![captura de pantalla](images/paint-slider.png)

--- /task ---

Ahora puedes arrastrar el deslizador que se ve debajo de la variable para cambiar el valor de la misma.

![captura de pantalla](images/paint-slider-change.png)

--- task ---

Prueba tu programa y mira si puedes añadir código para ajustar el grosor del lápiz.

![captura de pantalla](images/paint-width-test.png)

--- /task ---