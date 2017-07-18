## Changing the pencil width

Let's allow the user to draw using a range of different pencil sizes.



+ First, add a new variable called 'width'. If you're not sure how to do this, the 'Ghostbusters' project will help you.

+ Add this line _inside_ the `forever`{:class="blockcontrol"} loop of your pencil's code:

	```blocks
		set pen size to (width)
	```

	Your pencil width will now repeatedly be set to the value of your 'width' variable.

+ You can change the number stored in this variable by right-clicking on your variable (on the stage) and clicking 'slider'.

	![screenshot](images/paint-slider.png)

	You can now drag the slider below the variable to change its value.

	![screenshot](images/paint-slider-change.png)

+ Test your project, and see if you can modify the pencil width.

	![screenshot](images/paint-width-test.png)

	If you prefer, you can set the minimum and maximum value of 'width' that's allowed. To do this, right-click on your variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

	![screenshot](images/paint-slider-max.png)

	Keep testing your 'width' variable until you're happy.



