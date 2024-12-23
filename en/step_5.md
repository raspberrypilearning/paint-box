## Change the pen width

Make the lines you draw thicker or thinner.

--- task ---

Add a new variable called `width`{:class="block3variables"}. Make sure it is set to 'all sprites'

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

Add this line __inside__ the `forever`{:class="block3control"} loop of the pencil sprite's code:

![pencil](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
go to (mouse pointer v)
+set pen size to (width :: variables)
if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

--- /task ---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

--- task ---

Right-click on the `width`{:class="block3variables"} variable displayed on the Stage, and then click on **slider**.

![screenshot](images/paint-slider.png)

--- /task ---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

--- task ---

Test your project and see if you can change the pen width.

![screenshot](images/paint-width-test.png)

--- /task ---
