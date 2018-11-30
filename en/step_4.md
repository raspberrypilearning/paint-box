## Making mistakes

Sometimes mistakes happen, so let's add a 'clear' button and an eraser.

+ Add the 'X-block' sprite - you will find it in the library, in the letters section. Colour the costume in red. This will become the 'clear' button.

![screenshot](images/paint-x.png)

+ Add code to this sprite to clear the stage when it's clicked.

![Clear stage](images/clear-stage.png)

Notice that you don't need to send a message to clear the stage, you can just use the clear block from this sprite.

You have probably noticed that your pencil sprite includes an eraser costume:

![screenshot](images/paint-eraser-costume.png)

+ Your project also includes a separate eraser sprite. Right click on this sprite and choose 'show'. Here is how your stage should look:

![screenshot](images/paint-eraser-stage.png)

+ Add code to the eraser sprite, to tell the pencil to switch to an eraser when the sprite is clicked.

![Broadcast eraser](images/broadcast-eraser.png)

When the pencil receives the "eraser" message, you can switch the pencil costume to the eraser, and switch the pencil colour to white - the same colour as the stage!

+ Add some code to create the eraser

--- hints ---
--- hint ---
Add some code to the pencil sprite:
**When I receive** the **eraser** message
**Switch to costume** eraser
**Set pen color** to white
--- /hint ---
--- hint ---
Here is how the code inside the pencil sprite should look:
```blocks
when I receive [eraser v]
switch costume to [eraser v]
set pen color to [#FFFFFF]
```
--- /hint ---
--- /hints ---

+ Test your project, to see if you can clear and erase on the stage.

![screenshot](images/paint-erase-test.png)

There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

![screenshot](images/paint-draw-problem.png)

To fix this, tell the pencil only to draw if the mouse is clicked _and_ if the y-position of the mouse is greater than -120:

![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

![screenshot](images/paint-fixed.png)
