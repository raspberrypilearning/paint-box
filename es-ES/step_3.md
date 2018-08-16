## Hacer un lápiz

Comencemos haciendo un lápiz que se pueda usar para dibujar en el escenario.

+ Abre el projecto 'Paintbox' de Scratch online en [jumpto.cc/paint-go](http://jumpto.cc/paint-go){:target="_blank"} o descárgalo primero de <http://jumpto.cc/paint-get>{:target="_blank"} y ábrelo luego en tu editor offline.

Verás figuras de lápiz y de goma de borrar:

![screenshot](images/paint-starter.png)

+ Añade algo de código a la figura del lápiz para que siga el movimiento del ratón `por siempre`{:class="blockcontrol"} para que puedas dibujar:

```blocks
    al presionar bandera verde
por siempre 
  ir a [puntero del ratón v]
end
```

+ Haz clic en la bandera y luego mueve el ratón por el escenario para comprobar si el código funciona.

Next, let's make your pencil only draw `if`{:class="blockcontrol"} the mouse has been clicked.

+ Add this code to your pencil sprite:

![screenshot](images/paint-pencil-draw-code.png)

+ Test your code again. This time, move the pencil around the stage and hold down the mouse button. Can you draw with your pencil?

![screenshot](images/paint-draw.png)

## \--- collapse \---

## title: If you're having problems...

If your pencil seems to be drawing the line from the middle of the pencil rather than the tip, you will need to change your costume center.

![Costume center](images/costume-center.png)

The crosshair for the pencil must be placed **just below** the tip of the pencil, not on the tip of the pencil.

A changes in a sprite's 'costume center' isn't registered until another tab is clicked, so click on another costume, or on the 'Scripts' tab to finalise your changes to the costume center.

\--- /collapse \---