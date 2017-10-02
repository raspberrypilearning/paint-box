## Making mistakes

Sometimes mistakes happen, so let's add a 'clear' button and an eraser to your project!



+ Let's add a button to clear the stage. To do this, add the 'X-block' letter sprite to the stage, and colour it in red.

	![screenshot](images/paint-x.png)

+ Add code to your new cancel button to clear the stage when it's clicked.

	```blocks
		when this sprite clicked
		clear
	```

	Notice that you don't need to send a message to clear the stage, as any sprite can do it!

+ You have probably noticed that your pencil sprite includes an eraser costume:

	![screenshot](images/paint-eraser-costume.png)
	

+ Your project also includes an eraser selector sprite, right click on it and choose 'show'. This is how your stage should look:

	![screenshot](images/paint-eraser-stage.png)

+ You can then add code to the eraser selector sprite, to tell the pencil to switch to an eraser.

	```blocks
		when this sprite clicked
		broadcast [eraser v]
	```

+ When the pencil receives this message, you can create an eraser by switching the pencil costume to the eraser, and switching the pencil colour to the same colour as the stage!

	```blocks
		when I receive [eraser v]
		switch costume to [eraser v]
		set pen color to [#FFFFFF]
	```

+ Test your project, to see if you can clear and erase on the stage.

	![screenshot](images/paint-erase-test.png)

+ There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

	![screenshot](images/paint-draw-problem.png)

	To fix this, you have to tell the pencil only to draw if the mouse is clicked _and_ if the y-position of the mouse is greater than -120 (`mouse y` statement to look like this:

	![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

	![screenshot](images/paint-fixed.png)



