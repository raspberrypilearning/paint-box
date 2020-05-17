## Виправ хиби

Інколи трапляються хиби, тому додай кнопки очистки та гумки.

\--- task \---

Додай спрайт "Block-X" із розділу літер в бібліотеці. Зафарбуй образ спрайта в червоний колір і зроби його трохи меншим. Цей спрайт буде кнопкою очистки.

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png)

\--- /task \---

\--- task \---

Додай код до спрайта "Block-X", щоб очищувати Сцену, коли на нього клацають.

![cross](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- /task \---

Тобі не треба використовувати `оповіщення`{:class="block3events"} для очищення сцени, тому що блока `очистити все`{:class="block3extensions"} достатньо.

Ти помітив (-ла), що спрайт олівця містить образ гумки?

![screenshot](images/paint-eraser-costume.png)

Твій проєкт також містить окремий спрайт гумки.

\--- task \---

Вибери спрайт гумки і клацни **показати** (іконка із оком). Ось як тепер має виглядати твоя Сцена:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Додай код до спрайту гумки, щоб здійснювати `оповіщення "гумка"`{:class="block3events"}, коли на нього клацають.

![eraser](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

\--- /task \---

Коли спрайт олівця отримує повідомлення "гумка", він має змінювати свій образ на гумку і перемикати колір малювання на білий, який є кольором Сцени!

\--- task \---

Додай код для програмування гумки.

\--- hints \--- \--- hint \---

Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

\--- /hint \--- \--- hint \---

Here are all the blocks you need:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \---

Test your project to see if you can clear the Stage and erase pencil lines.

![screenshot](images/paint-erase-test.png)

\--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![screenshot](images/paint-draw-problem.png)

\--- task \---

To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![pencil](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
  go to (mouse pointer v)
+if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \---

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---