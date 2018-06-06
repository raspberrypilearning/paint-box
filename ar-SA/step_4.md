## أقلام ملونة

لنضِف أقلامًا ملوَّنة مختلفة إلى المشروع لنسمح للمستخدم بالاختيار من بينها.

+ انقر فوق كائن القلم الرصاص، ثم انقر فوق 'المظاهر' وضاعف المظهر 'قلم أزرق'.

![screenshot](images/paint-blue-duplicate.png)

+ غيِّر اسم المظهر الجديد إلى 'قلم أخضر'، ولوِّن قلم الرصاص باللون الأخضر.

![screenshot](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ أنشئ كائنَين جديدَين لتستخدمهما في تحديد القلم الأزرق أو الأخضر. سوف تستخدم هذه لتحديد قلم رصاص أزرق أو أخضر.

![screenshot](images/paint-selectors.png)

+ اعد تسمية الكائنين الخاصين بك بالتسمية التالية: "ازرق" و "أخضر"

+ Add some code to the 'green' sprite so that when it is clicked, it will `broadcast`{:class="blockevents"} the message "green" to the pencil sprite, telling it to change its costume and pencil colour.

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

![screenshot](images/paint-pens-test.png)