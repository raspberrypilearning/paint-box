## Зміна ширини олівця

Let's allow the user to draw using a range of different pencil sizes.

+ Спершу, створіть список, який називається ` width` {: class = "blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Додайте цей рядок *inside* the `forever`{:class="blockcontrol"} цикл коду олівця:

```blocks
    set pen size to (width)
```

The pencil width will now repeatedly be set to the value of the 'width' variable.

+ Right click on the variable display on the stage and click 'slider'.

![screenshot](images/paint-slider.png)

You can now drag the slider below the variable to change its value.

![screenshot](images/paint-slider-change.png)

+ Перевірте свій проект та подивіться, чи можна змінити ширину олівця.

![screenshot](images/paint-width-test.png)

Якщо ви забажаєте, ви можете встановити мінімальне та максимальне значення ширини, яке дозволено. Для цього клацніть правою кнопкою миші на змінну і натисніть "встановити слайдер міні та макс". Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![screenshot](images/paint-slider-max.png)

Keep testing your 'width' variable until you're happy.