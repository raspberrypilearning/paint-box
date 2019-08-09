## Lápices de colores

Ahora vas a añadir diferentes lápices de colores a tu proyecto y permitir que el usuario elija entre los mismos.

\--- task \--- Rename the `pencil` sprite to `pencil-blue`

![rename-pencil](images/rename-pencil.png) \--- / tarea \---

\--- task \--- Right click on the pencil sprite, and duplicate the 'pencil-blue' costume.

![captura de pantalla](images/paint-blue-duplicate.png) \--- / tarea \---

\--- task \--- Nombra el nuevo disfraz 'lápiz-verde', y colorea el lápiz de verde.

![captura de pantalla](images/paint-pencil-green.png)

\--- / tarea \---

\--- task \--- Dibuja dos nuevos objetos: un cuadrado azul y uno verde. Estos sirven para elegir entre el lápiz azul y el verde.

![captura de pantalla](images/paint-selectors.png) \--- / tarea \---

\--- task \--- Renombra los nuevos objetos para que se llamen 'azul' y 'verde'

[[[generic-scratch3-rename-sprite]]]

\--- / tarea \---

\--- task \--- Añade algún código al objeto 'verde', de modo que cuando se haga clic en este objeto, se `envíos`{:class="block3events"} el mensaje "verde".

![cuadrado verde](images/green_square.png)

```blocks3
when this sprite clicked
broadcast (green v)
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

El objeto lápiz debería 'escuchar' los mensajes "verde" y cambiar su disfraz y color de lápiz como respuesta.

\--- task \--- Cambia a tu objeto lápiz. Añade algún código de modo que cuando este objeto reciba el envío `verde`{:class="block3events"}, cambia al disfraz de lápiz verde y cambia el color del marcador a verde.

![lápiz](images/pencil.png)

```blocks3
when I receive [green v]
switch costume to (pencil-green v)
set pen color to [#00CC44]
```

Para fijar el lápiz al color verde, haz clic en el cuadrado de color en el bloque `fijar color del marcador`{:class="block3extensions"}, y luego haz clic sobre el objeto cuadrado verde. \--- / tarea \---

Luego de forma similar de modo que puedes cambiar el color del lápiz a azul.

\--- task \--- Haz clic sobre el objeto cuadrado azul y añade este código:

![cuadrado_azul](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blue v)
```

Luego, haz clic sobre el objeto lápiz y añade este código: ![lápiz](images/pencil.png)

```blocks3
when I receive [blue v]
switch costume to (pencil-blue v)
set pen color to [#0000ff]
```

\--- / tarea \---

\--- task \--- Finalmente, añade este código para indicarle al objeto lápiz con qué color comenzar, y asegurarte de que la pantalla esté limpia cuando comiences.

![lápiz](images/pencil.png)

```blocks3
when flag clicked
+erase all
+switch costume to (pencil-blue v)
+set pen color to [#0035FF]
forever
  go to (mouse pointer v)
if <mouse down?> then
  pen down
  else
  pen up
end
```

\--- / tarea \---

Si prefieres, puedes comenzar con un lápiz de diferente color.

\--- task \--- Prueba tu código. ¿Puedes cambiar entre los colores de lápices azul y verde al hacer clic sobre los objetos cuadrado azul o verde?

![captura de pantalla](images/paint-pens-test.png) \--- / tarea \---