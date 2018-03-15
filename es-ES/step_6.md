## Cambiamos el grosor del lápiz

Vamos a permitir al usuario dibujar usando diferentes tamaños de lápiz.

+ Primero añade una nueva variable llamada `ancho`{:class="blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Añade esta linea *dentro* del bucle `por siempre`{:class="blockcontrol"} del código del lápiz:

```blocks
    fijar tamaño de lápiz a (ancho)
```

La anchura del lápiz se fijará ahora repetidamente con el valor de la variable 'ancho'.

+ Haz clic con el botón derecho en la variable en el escenario y haz en clic en 'slider'.

![screenshot](images/paint-slider.png)

Ahora puedes arrastrar la barra de desplazamiento bajo la variable para cambiar su valor.

![screenshot](images/paint-slider-change.png)

+ Prueba tu proyecto y comprueba si puedes modificar el ancho del lápiz.

![screenshot](images/paint-width-test.png)

Si lo prefieres puedes fijar el valor mínimo y máximo permitido de 'ancho'. To do this, right-click on the variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![screenshot](images/paint-slider-max.png)

Keep testing your 'width' variable until you're happy.