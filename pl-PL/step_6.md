## Zmień szerokość ołówka

Następnie dodasz kod, aby umożliwić osobie korzystającej z programu rysowanie rzeczy o różnej grubości pisania.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
kiedy kliknięto
usuń wszystkie
zmień kostium na (ołówek-niebieski v)
ustaw kolor pisaka na [#0035FF]
zawsze
idź do (wskaźnik myszy v)
+ustaw rozmiar pisaka na (szerokość :: zmienne)
jeśli <<mouse down?> i <(mysza) > [-120]>> a następnie 
  Połóż pisak
  else
  Podnieś pisak
koniec
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