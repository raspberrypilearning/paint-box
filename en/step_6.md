## Changing the pencil width

Let's allow the user to draw using a range of different pencil sizes.

--- task ---
First, add a new variable called `width`{:class="blockdata"}.

[[[generic-scratch-add-variable]]]
--- /task ---

--- task ---
Add this line _inside_ the `forever`{:class="blockcontrol"} loop of the pencil's code:

```blocks
when flag clicked
clear
switch costume to [pencil-blue v]
set pen color to [#0035FF]
forever
go to [mouse pointer v]
+set pen size to (width)
if <<mouse down?> and <(mouse y) > [120]>> then 
  pen down
  else
  pen up
end
```
--- /task ---

The pencil width will now repeatedly be set to the value of the 'width' variable.

--- task ---
Right click on the variable display on the stage and click 'slider'.

![screenshot](images/paint-slider.png)
--- /task ---

You can now drag the slider below the variable to change its value.

![screenshot](images/paint-slider-change.png)

--- task ---
Test your project, and see if you can modify the pencil width.

![screenshot](images/paint-width-test.png)
--- /task ---

If you prefer, you can set the minimum and maximum value of 'width' that's allowed. To do this, right-click on the variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![screenshot](images/paint-slider-max.png)

Keep testing your 'width' variable until you're happy.
