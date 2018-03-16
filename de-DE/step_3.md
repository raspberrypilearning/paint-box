## Einen Stift machen

Beginnen wir mit einem Stift, mit dem wir auf der Bühne zeichnen können.

+ Scratch kann entweder online bei [jumpto.cc/paint-go{:target="_blank"}](http://jumpto.cc/paint-go) verwendet werden, oder unter [http://jumpto.cc/paint-get{:target="_blank"}](http://jumpto.cc/paint-get) heruntergeladen und offline benutzt werden.

You will see pencil and eraser sprites:

![screenshot](images/paint-starter.png)

+ Add some code to the pencil sprite to make it follow the mouse `forever`{:class="blockcontrol"} so that you can draw:

```blocks
    when flag clicked
    forever
      go to [mouse pointer v]
    end
```

+ Click the flag and then move the mouse around the stage to test whether the code works.

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