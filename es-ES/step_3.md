## Lápices de colores

Ahora vas a añadir diferentes lápices de colores a tu proyecto y permitir que el usuario elija entre los mismos.

\--- task \--- Haz clic en el objeto lápiz, haz clic sobre **Disfraces**, y duplica el disfraz llamado 'lápiz-azul'.

![captura de pantalla](images/paint-blue-duplicate.png) \--- /task \---

\--- task \--- Nombra el nuevo disfraz 'lápiz-verde', y colorea el lápiz de verde.

![Captura de pantalla](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- Dibuja dos nuevos objetos: un cuadrado azul y uno verde. Estos sirven para elegir entre el lápiz azul y el verde.

![screenshot](images/paint-selectors.png) \--- /task \---

\--- task \--- Renombra los nuevos objetos para que se llamen 'azul' y 'verde'

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- Añade algún código al objeto 'verde', de modo que cuando se haga clic en este objeto, se `envía`{:class="block3events"} el mensaje "verde".

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

To set the pencil to colour to green, click the coloured square in the `set pen color`{:class="block3extensions"} block, and then click on the green square sprite. \--- /task \---

Then to a similar thing so that you can switch the pencil colour to blue.

\--- task \--- Click on the blue square sprite and add this code:

![blue_square](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blue v)
```

Then click on the pencil sprite and add this code: ![pencil](images/pencil.png)

```blocks3
when I receive [blue v]
switch costume to (pencil-blue v)
set pen color to [#0000ff]
```

\--- /task \---

\--- task \--- Finalmente, añade este código para indicarle al objeto lápiz con qué color comenzar, y asegurarte de que la pantalla esté limpia cuando comiences.

![pencil](images/pencil.png)

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

\--- /task \---

If you prefer, you can start with a different colour pencil.

\--- task \--- Test your code. Can you switch between the blue and green pencil colours by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png) \--- /task \---