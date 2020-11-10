## Spremeni širino pisala

Dodaj kodo, ki omogoča osebi, ki uporablja tvoj program, da riše s pisali različnih debelin.

\--- task \---

Najprej dodaj novo spremenljjivko z imenom `širina`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Dodaj to vrstico **znotraj** zanke `ponavljaj`{:class="block3control"}, v kodo figure svinčnika:

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

Širina peresa se sedaj ponavljajoče nastavlja na vrednost spremenljivke `širina`{:class="block3variables"}.

\--- task \---

Z desno tipko klikni na spremenljivko `širina`{:class="block3variables"}, ki je prikazana na odru in nato klikni na **drsnik**.

![posnetek zaslona](images/paint-slider.png)

\--- /task \---

Zdaj lahko premikaš drsnik pod spremenljivko in s tem spreminjaš vrednost spremenljivke.

![posnetek zaslona](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can change the pen width.

![posnetek zaslona](images/paint-width-test.png)

\--- /task \---