## Spremeni širino pisala

Zdaj boš dodal kodo, ki omogoča osebi, ki uporablja tvoj program, da riše s pisali različnih debelin.

\--- task \--- Najprej dodaj novo spremenljjivko z imenom `širina`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]] \--- /task \---

\--- task \--- Dodaj to vrstico **znotraj** zanke `ponavljaj`{:class="block3control"}, v kodo figure svinčnika:

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

\--- naloga \--- desno miškino tipko kliknite spremenljivko `širina`{: class = "block3variables"}, ki je prikazana na stopnji, in nato kliknite **drsnik**.

![posnetek zaslona](images/paint-slider.png) \--- / naloga \---

Zdaj lahko povlečete drsnik, ki je viden pod spremenljivko, da spremenite vrednost spremenljivke.

![posnetek zaslona](images/paint-slider-change.png)

\--- naloga \--- Preizkusite svoj projekt in preverite, ali lahko dodate kodo za prilagoditev širine peresa.

![posnetek zaslona](images/paint-width-test.png) \--- / naloga \---