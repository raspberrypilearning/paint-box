## Помилки

Іноді помилки трапляються, так що давайте додамо кнопку 'очистити' та гумку.

+ Додайте 'X-block' спрайт - ви зможете знайти його в бібліотеці, в розділі букв. Змініть колір костюма на червоний. Це буде кнопка «Очистити».

![скріншот](images/paint-x.png)

+ Додайте код до цього спрайта, щоб очистити сцену, коли вона натиснута.

![Очистити сцену](images/clear-stage.png)

Зверніть увагу, що вам не потрібно надсилати повідомлення, щоб очистити сцену, ви можете просто використовувати чіткий блок із цього спрайту.

Мабуть, ви помітили, що олівець спрайт включає в себе гумку-костюм:

![скріншот](images/paint-eraser-costume.png)

+ Ваш проект також включає в себе окрему гумку-спрайт. Клацніть правою кнопкою миші на цьому спрайті і виберіть 'Показати'. Ось як повинна виглядати ваша сцена:

![скріншот](images/paint-eraser-stage.png)

+ Add code to the eraser sprite, to tell the pencil to switch to an eraser when the sprite is clicked.

![Broadcast eraser](images/broadcast-eraser.png)

When the pencil receives the "eraser" message, you can switch the pencil costume to the eraser, and switch the pencil colour to white - the same colour as the stage!

+ Додайте деякі коду для створення гумки

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: **When I receive** the **eraser** message **Switch to costume** eraser **Set pen color** to white \--- /hint \--- \--- hint \--- Here is how the code inside the pencil sprite should look:

```blocks
when I receive [eraser v]
switch costume to [eraser v]
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Перевірте свій проект, щоб побачити, чи можна очистити та стерти платформу.

![screenshot](images/paint-erase-test.png)

There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

![screenshot](images/paint-draw-problem.png)

To fix this, tell the pencil only to draw if the mouse is clicked *and* if the y-position of the mouse is greater than -120:

![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

![screenshot](images/paint-fixed.png)