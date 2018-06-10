## Кольорові олівці

Давайте додамо до вашого проекту різні кольорові олівці та дозволимо користувачеві обирати палітру.

+ Натисніть на свій олівець "Образи" та скопіюйте "олівець-синій".

![скріншот](images/paint-blue-duplicate.png)

+ Перейменуйте ваш новий образ «зелений олівець» і замалюйте олівцем такого самого кольору.

![скріншот](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Намалюйте два нових олівця- один блакитний квадрат і один зелений. Ви використовуватимете їх для вибору синього або зеленого олівця.

![скріншот](images/paint-selectors.png)

+ Перейменуйте свої олівця так, щоб оди називався "голубий", а інший "зелений",

+ Додайте код до "зелений олівець" зправа так, щоб, коли його натиснули, він передав` перейшов на` (: class = "blockevents") повідомлення "зелений" до олівця,таким чином, змінюючи образ та колір олівця.

![Broadcast green](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Переключіться на ваш олівець. Add some code so that when this sprite receives the `broadcast`{:class="blockevents"} green, it should switch to the green pencil costume and change the pen colour to green.

![Broadcast green](images/broadcast-green.png)

To set the pencil to colour to green, click the coloured box in the `set pen color`{:class="blockpen"} block, and click on the green sprite to choose the same colour green as your pencil colour.

+ You can now do the same for the blue pencil icon: add this code to the blue square sprite:

```blocks
when this sprite clicked
broadcast [blue v]
```

...and add this code to the pencil sprite:

```blocks
when I receive [blue v]
switch costume to [pencil-blue v]
set pen color to [#0000ff]
```

+ Finally, add this code to tell the pencil sprite which colour to start with, and make sure that the screen is clear.

![Start pencil](images/start-pencil.png)

Ми вирішили розпочати з синього кольору, але, якщо захочете, ви можете почати з іншого кольору.

+ Перевірте ваш проект. Ви можете переключитися між синім та зеленим ручками, натискаючи сині або зелені квадратні спрайти.

![screenshot](images/paint-pens-test.png)