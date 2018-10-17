## Промена дебљине оловке

Хајде да омогућимо кориснику да црта користећи оловке различитих дебљина.

+ Прво додај нову променљиву која ће се звати `дебљина`{:class="blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Add this line *inside* the `forever`{:class="blockcontrol"} loop of the pencil's code:

```blocks
    нека дебљина оловке буде (дебљина)
```

The pencil width will now repeatedly be set to the value of the 'width' variable.

+ Right click on the variable display on the stage and click 'slider'.

![слика екрана](images/paint-slider.png)

You can now drag the slider below the variable to change its value.

![слика екрана](images/paint-slider-change.png)

+ Test your project, and see if you can modify the pencil width.

![слика екрана](images/paint-width-test.png)

If you prefer, you can set the minimum and maximum value of 'width' that's allowed. To do this, right-click on the variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![слика екрана](images/paint-slider-max.png)

Настави да испробаваш променљиву 'дебљина' док не будеш задовољан/а.