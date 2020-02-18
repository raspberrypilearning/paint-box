## Spremeni širino pisala

Dodaj kodo, ki omogoča osebi, ki uporablja tvoj program, da riše s pisali različnih debelin.

--- task ---

Najprej dodaj novo spremenljjivko z imenom `širina`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

Dodaj to vrstico **znotraj** zanke `ponavljaj`{:class="block3control"}, v kodo figure svinčnika:

```blocks3
ko je kliknjena zelena zastavica
izbriši vse
zamenjaj videz na (svinčnik-moder v)
nastavi barvo peresa na [#0035FF]
ponavljaj 
  pojdi na (mouse pointer v)
  + nastavi velikost peresa na (širina :: variables)
  če <<je miškin gumb pritisnjen?> in <(miškin y) > [-120]>> potem 
    spusti pero
  sicer 
    dvigni pero
  end
end
```

--- /task ---

Širina peresa se sedaj ponavljajoče nastavlja na vrednost spremenljivke `širina`{:class="block3variables"}.

--- task ---

Z desno tipko klikni na spremenljivko `širina`{:class="block3variables"}, ki je prikazana na odru in nato klikni na **drsnik**.

![posnetek zaslona](images/paint-slider.png)

--- /task ---

Zdaj lahko premikaš drsnik pod spremenljivko in s tem spreminjaš vrednost spremenljivke.

![posnetek zaslona](images/paint-slider-change.png)

--- task ---

Preizkusi svoj projekt. Ali lahko dodaš kodo, ki spreminja širino pisala.

![posnetek zaslona](images/paint-width-test.png)

--- /task ---