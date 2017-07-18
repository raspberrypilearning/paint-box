## Making a pencil

Let's start by making a pencil that can be used to draw on the stage.



+ Open the 'Paintbox' Scratch project online at <a href="http://jumpto.cc/paint-go" target="_blank">jumpto.cc/paint-go</a> or download from <a href="http://jumpto.cc/paint-get" target="_blank">jumpto.cc/paint-get</a> and then open if you are using the offline editor.

	You will see pencil and eraser sprites:

	![screenshot](images/paint-starter.png)	

+ As you'll be using the mouse to draw, you'll want the pencil to follow the mouse `forever`{:class="blockcontrol"}. Add this code to your pencil sprite:

	```blocks
		when flag clicked
		forever
		  go to [mouse pointer v]
		end
	```

+ Test out this code by clicking the flag and then moving the mouse around the stage. 

+ Next, let's make your pencil draw `if`{:class="blockcontrol"} the mouse has been clicked. Add this code to your pencil sprite:

	![screenshot](images/paint-pencil-draw-code.png)	

+ Test your code again. This time, move the pencil around the stage and hold down the mouse button. Can you draw with your pencil?

	![screenshot](images/paint-draw.png)
	



