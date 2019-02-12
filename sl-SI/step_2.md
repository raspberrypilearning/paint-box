## Naredi svinčnik

Začnite z izdelavo svinčnika, ki ga lahko uporabite za risanje na odru.

\--- naloga \--- Odprite 'Paint box' projekt zaganjalnika Scratch.

**Online**: odprite starter projekt na [rpf.io/paint-box-on](http://rpf.io/paint-box-on){: target = "_ blank"}

**Offline**: odprite [začetni projekt](http://rpf.io/p/en/paint-box-go){: target = "_ blank"} v urejevalniku brez povezave

Če želite prenesti in namestiti urejevalnik brez povezave Scratch, ga lahko najdete na [rpf.io/scratchoff](http://rpf.io/scratchoff){: target = "_ blank"}

V zagonskem projektu bi morali videti svinčnik in radirke:

![posnetek zaslona](images/paint-starter.png) \--- / naloga \---

\--- naloga \---

Dodajte podaljšek Pen svojemu projektu.

[[[generic-scratch3-add-pen-extension]]]

\--- / naloga \---

\--- naloga \---

Dodajte nekaj kode na sprite svinčnika, da bo sprite sledil kazalcu miške `vedno`{: class = "block3control"}, da boste lahko risali:

![svinčnik](images/pencil.png)

```blocks3
ko je zastavica kliknila
vedno
  pojdi na (kazalec miške v)
konec
```

\--- / naloga \---

\--- naloga \--- Kliknite zastavo in premaknite kazalec miške okrog stopnje, da preverite, ali koda deluje. \--- / naloga \---

Nato naredite svoj svinčnik samo za risanje `če se klikne`{: class = "block3control"} gumb miške.

\--- naloga \--- Dodajte to kodo na svoj sprite:

![svinčnik](images/pencil.png)

```blocks3
ko je zastavica kliknila
vedno
  pojdi na (kazalec miške v)

+ če <mouse down?> potem
  pero navzdol
  drugo
  pero gor
konec
```

\--- / naloga \---

\--- naloga \--- Ponovno preizkusite svojo kodo. Tokrat premaknite svinčnik okoli stopnje in držite gumb miške. Ali lahko narišete s svinčnikom?

![posnetek zaslona](images/paint-draw.png) \--- / naloga \---

## \--- kolaps \---

## title: Ali vaš svinčnik ne črpa iz konice?

Če je črta, ki jo izgleda risba svinčnika, izhajala iz sredine svinčnika, morate spremeniti svoj sprite s svinčnikom, tako da je konica središče za sprite.

Kliknite na sprite svinčnika in nato na kartico **Costumes**.

Premakni kostum tako, da je konica svinčnika **tik nad** središče.

![Kostumni center](images/costume-center-annotated.png)

Zdaj premaknite svinčnik okrog Stage in narišite. S svinčnikom naj zdaj potegne črto od konice.

\--- / strni \---