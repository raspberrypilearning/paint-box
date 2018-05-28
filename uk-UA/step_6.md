## Зміна ширини олівця

Let's allow the user to draw using a range of different pencil sizes.

+ Спершу, створіть список, який називається ` width` {: class = "blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Add this line *inside* the `forever`{:class="blockcontrol"} loop of the pencil's code:

```blocks
    set pen size to (width)
```

The pencil width will now repeatedly be set to the value of the 'width' variable.

+ Right click on the variable display on the stage and click 'slider'.

![screenshot](images/paint-slider.png)

You can now drag the slider below the variable to change its value.

![screenshot](images/paint-slider-change.png)

+ Test your project, and see if you can modify the pencil width.

![screenshot](images/paint-width-test.png)

If you prefer, you can set the minimum and maximum value of 'width' that's allowed. To do this, right-click on the variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![screenshot](images/paint-slider-max.png)

Keep testing your 'width' variable until you're happy.