## Coloured pencils

Let's add different coloured pencils to your project, and allow the user to choose between them.

--- task ---
Click on your pencil sprite, click 'Costumes' and duplicate your 'pencil-blue' costume.

![screenshot](images/paint-blue-duplicate.png)
--- /task ---

--- task ---
Rename your new costume 'pencil-green', and colour the pencil green.

![screenshot](images/paint-pencil-green.png)

--- /task ---

--- task ---
Draw two new sprites - one blue square and one green square. You will use these to select the blue or green pencil.

![screenshot](images/paint-selectors.png)
--- /task ---

--- task ---
Rename your sprites so that they are called 'blue' and 'green'

[[[generic-scratch-rename-sprite]]]

--- /task ---

--- task ---
Add some code to the 'green' sprite so that when it is clicked, it will `broadcast`{:class="blockevents"} the message "green" to the pencil sprite, telling it to change its costume and pencil colour.

![green square](images/green_square.png)
```blocks
when this sprite clicked
broadcast [green v]
```

[[[generic-scratch-broadcast-message]]]
--- /task ---

--- task ---
Switch to your pencil sprite. Add some code so that when this sprite receives the `broadcast`{:class="blockevents"} green, it should switch to the green pencil costume and change the pen colour to green.

![pencil](images/pencil.png)

```blocks
when I receive [green v]
switch costume to [pencil-green v]
set pen color to [#00CC44]
```

To set the pencil to colour to green, click the coloured box in the `set pen color`{:class="blockpen"} block, and click on the green sprite to choose the same colour green as your pencil colour.
--- /task ---

--- task ---
You can now do the same for the blue pencil icon: add this code to the blue square sprite:

![blue_square](images/blue_square.png)
```blocks
when this sprite clicked
broadcast [blue v]
```

...and add this code to the pencil sprite:
![pencil](images/pencil.png)
```blocks
when I receive [blue v]
switch costume to [pencil-blue v]
set pen color to [#0000ff]
```
--- /task --- 

--- task ---
Finally, add this code to tell the pencil sprite which colour to start with, and make sure that the screen is clear.

![pencil](images/pencil.png)
```blocks
when flag clicked
+clear
+switch costume to [pencil-blue v]
+set pen color to [#0035FF]
forever
  go to [mouse pointer v]
if <mouse down?> then
  pen down
  else
  pen up
end
```
--- /task ---

We chose to start with blue but if you prefer, you can start with a different colour pencil.

--- task ---
Test out your project. Can you switch between blue and green pencils by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png)
--- /task ---

