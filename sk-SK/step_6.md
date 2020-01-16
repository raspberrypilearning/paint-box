## Zmena hrúbky ceruzky

Teraz pridáš scenár, ktorý umožní osobe používajúcej tvoj projekt kresliť čiary s rôznou hrúbkou ceruzky.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
pri kliknutí na ⚑
zmaž
zmeň kostým na (ceruzka-modrá v)
nastav farbu pera na [#0035FF]
opakuj stále 
  skoč na (myš v)
 +nastav hrúbku pera na (hrúbka :: variables)
  ak <<stlačené tlačidlo myši?> a <(myš y) > [-120]>> 
    pero zapni
  inak 
    pero vypni
  end
end
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