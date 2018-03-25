## Cambiamos el grosor del lápiz

Vamos a permitir al usuario dibujar usando diferentes tamaños de lápiz.

+ Primero añade una nueva variable llamada `ancho`{:class="blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Añade esta linea *dentro* del bucle `por siempre`{:class="blockcontrol"} del código del lápiz:

```blocks
    fija tamaño de lápiz a (ancho)
```

La anchura del lápiz se fijará ahora con el valor de la variable 'ancho'.

+ Haz clic con el botón derecho en la esquina del escenario donde aparece la variable y haz en clic en 'deslizador'.

![screenshot](images/paint-slider.png)

Ahora puedes arrastrar el deslizador debajo de la variable para cambiar su valor.

![screenshot](images/paint-slider-change.png)

+ Prueba tu proyecto y comprueba si puedes modificar el ancho del lápiz.

![screenshot](images/paint-width-test.png)

Si lo prefieres puedes fijar el valor mínimo y máximo permitido de 'ancho'. Para conseguirlo haz clic con el botón derecho en la variable de nuevo y haz clic en "Fijar rango del deslizador". Fija el valor mínimo y máximo de tu variable a algo más normal, como 1 y 20.

![screenshot](images/paint-slider-max.png)

Sigue probando tu variable 'ancho' hasta dejarlo como tu quieras.