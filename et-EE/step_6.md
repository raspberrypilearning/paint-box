## Muutke pliiatsi laiust

Järgmisena lisate koodi, mis võimaldab teie programmi kasutaval isikul joonistada asju erinevate pliiatsi laiustega.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- / ülesanne \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
kui lipu klõpsamine
kustutab kõik
lüliti kostüümi (pliiats-sinine v)
seadke pliiatsivärviks [# 0035FF]
igavesti
minge (hiirekursor v)
+ seadke pliiatsi suurus (laius :: muutujad)
kui <<mouse down?> ja <(hiir y) > [-120]>> siis 
  pensüstelit alla
  teist
  pensüstelit kuni
otsa
```

\--- / ülesanne \---

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