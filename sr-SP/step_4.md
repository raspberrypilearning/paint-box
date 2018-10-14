## Бојице

Хајде да у твој пројекат додамо бојице различитих боја и омогућимо кориснику да изабере ону коју жели.

+ Кликни на лик оловке, затим кликни на 'Костими' и умножи костим 'бојица-плава'.

![слика екрана](images/paint-blue-duplicate.png)

+ Преименуј нови костим у 'бојица-зелена' и обоји бојицу у зелено.

![слика екрана](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Нацртај два нова лика: плави квадрат и зелени квадрат. Користићеш их да одабереш плаву или зелену бојицу.

![слика екрана](images/paint-selectors.png)

+ Преименуј их тако да се зову 'плава' и 'зелена'.

+ Додај код лику 'зелена' тако да, када се кликне на њега он `разгласи`{:class="blockevents"} поруку "зелена" лику бојице, говорећи му да промени свој костим и боју бојице.

![Broadcast green](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Switch to your pencil sprite. Add some code so that when this sprite receives the `broadcast`{:class="blockevents"} green, it should switch to the green pencil costume and change the pen colour to green.

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

We chose to start with blue but if you prefer, you can start with a different colour pencil.

+ Test out your project. Can you switch between blue and green pens by clicking on the blue or green square sprites?

![слика екрана](images/paint-pens-test.png)