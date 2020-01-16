## Spremeni širino pisala

Dodaj kodo, ki omogoča osebi, ki uporablja tvoj program, da riše s pisali različnih debelin.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
ko kliknemo na zastavico
izbriši vse
zamenja videz na (svinčnik-moder v)
nastavi barvo peresa na [#0035FF]
ponavljaj
  pojdi na (kazalec miške v)
  +nastavi velikost peresa na (širina :: variables)
  if <(je miškin gumb pritisnjen?) in <(miškin y) > [-120]>> potem
    spusti pero
  sicer
    dvigni pero
konec
```

\--- /task \---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

\--- task \---

Right-click on the `width`{:class="block3variables"} variable displayed on the Stage, and then click on **slider**.

![screenshot](images/paint-slider.png)

\--- /task \---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can add code to adjust the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---