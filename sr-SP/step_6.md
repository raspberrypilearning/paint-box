## Промена дебљине оловке

Хајде да омогућимо кориснику да црта користећи оловке различитих дебљина.

+ Прво додај нову променљиву која ће се звати `дебљина`{:class="blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Додај ову наредбу *унутар* петље `понављај`{:class="blockcontrol"} у коду оловке:

```blocks
    нека дебљина оловке буде (дебљина)
```

Дебљина оловке сада ће бити увек постављена на вредност променљиве 'дебљина'.

+ Кликни десним тастером миша на променљиву приказану на позорници и кликни на 'клизач'.

![слика екрана](images/paint-slider.png)

Сада можеш да помераш клизач испод променљиве да промениш њену вредност.

![слика екрана](images/paint-slider-change.png)

+ Test your project, and see if you can modify the pencil width.

![слика екрана](images/paint-width-test.png)

If you prefer, you can set the minimum and maximum value of 'width' that's allowed. To do this, right-click on the variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![слика екрана](images/paint-slider-max.png)

Настави да испробаваш променљиву 'дебљина' док не будеш задовољан/а.