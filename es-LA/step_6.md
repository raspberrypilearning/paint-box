## Cambiar el ancho del lápiz

Luego vas a añadir código para permitir que la persona que use tu programa dibuje cosas con diferentes anchos de lapices.

--- task ---

Primero, añade una nueva variable llamada `ancho`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

Añade esta linea **dentro** del bucle `por siempre`{:class="blockcontrol"} del código del lápiz:

```blocks3
al presionar bandera
borrar todo
cambiar disfraz a (lápiz-azul v)
establecer color de lápiz a [#0035FF]
por siempre 
  ir a (mouse pointer v)
  + establecer color de lápiz a (ancho :: variables)
  si <<mouse down?>  y <(posición y del ratón) > [-120]>> entonces 
    lápiz abajo
  si no 
    lápiz arriba
  end
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