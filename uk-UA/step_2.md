## Створи олівець

Почнімо зі створення олівця, яким ти зможеш малювати на Сцені.

\--- task \---

Відкрий початковий проєкт "Набір для малювання" у Скретч.

**Онлайн**: відкрий початковий проєкт на [rpf.io/paint-box-on](http://rpf.io/paint-box-on){:target="_blank"}

Якщо у тебе є обліковий запис Скретч, то ти можеш зробити копію проєкту, натиснувши **Ремікс**.

**Офлайн**: відкрий [початковий проєкт](http://rpf.io/p/en/paint-box-go){:target="_blank"} в офлайн-редакторі.

Якщо тобі треба завантажити та встановити офлайн-редактор Скретч, то ти можеш його знайти на [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

В початковому проєкті ти маєш побачити спрайти олівця та гумки:

![screenshot](images/paint-starter.png)

\--- /task \---

\--- task \---

Додай розширення Олівець до свого проєкту.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Додай код до спрайту олівця, щоб він `завжди`{:class="block3control"} рухався за вказівником мишки, і щоб таким чином можна було малювати:

![pencil](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

\--- /task \---

\--- task \---

Клацни на прапорець і переміщуй вказівник мишки по Сцені для того, щоб перевірити чи працює твій код.

\--- /task \---

Next, make your pencil only draw `if`{:class="block3control"} the mouse button is being clicked.

\--- task \---

Add this code to your pencil sprite:

![pencil](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)

+ if <mouse down?> then
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \---

Test your code again. This time, move the pencil around the Stage and hold down the mouse button. Can you draw with your pencil?

![screenshot](images/paint-draw.png)

\--- /task \---

## \--- collapse \---

## title: Does your pencil not draw from its tip?

If the line your pencil draw looks like it is coming from the pencil's middle, you need to change your pencil sprite's so the tip is the sprite's centre.

Click on the pencil sprite, and then click on the **Costumes** tab.

Move the costume's so the tip of the pencil is **just above** the centre.

![Costume center](images/costume-center-annotated.png)

Now move the pencil around on the Stage and draw. The pencil should now draw a line from its tip.

\--- /collapse \---