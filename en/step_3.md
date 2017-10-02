## Making a pencil

Let's start by making a pencil that can be used to draw on the stage.

+ Open the 'Paintbox' Scratch project online at [jumpto.cc/paint-go](http://jumpto.cc/paint-go){:target="_blank"} or download from [http://jumpto.cc/paint-get](http://jumpto.cc/paint-get){:target="_blank"} and then open it if you are using the offline editor.

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
