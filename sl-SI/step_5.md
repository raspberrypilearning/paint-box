## Razveljavitev napak

Včasih pride do napak, zato dodajte gumb »počisti« in gumb za radirko.

\--- task \--- Dodaj figuro 'X-block', ki se nahaja v razdelku Črke iz knjižnice figur. Premineuj to figuro v 'blok x', pobarvaj jo rdeče in jo malo zmanjšaj. To bo gumb, ki 'počisti' risalno površino.

[[[generic-scratch3-sprite-from-library]]]

![posnetek zaslona](images/paint-x.png) \--- /task \---

\--- task \--- Figuri 'blok x' dodaj kodo, ki izbriše vse na odru, kadar kliknemo na njo.

![križ](images/cross.png)

```blocks3
ko kliknemo to figuro
izbriši vse
```

\--- /task \---

Za čiščenje odra ti ni potrebno `objaviti`{: class = "block3events"} sporočila, ker že `izbriši vse`{: class = "block3extensions"} blok opravi to delo.

Si opazil, da figura svinčnika vsebuje tudi videz radirke?

![posnetek zaslona](images/paint-eraser-costume.png)

Tvoj projekt vsebuje tudi ločeno figuro radirke.

\--- task \--- Klikni na figuro radirke in jo prikaži s klikom na **oko** v panoju za urejanje podatkov o figuri. Tukaj lahko vidite, kako naj bo vaš oder videti zdaj:

![posnetek zaslona](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Figuri radirke dodaj kodo, ki `objavi 'radirka'`{:class="block3events"}, kadar kliknemo na figuro radirke.

![radirka](images/eraser.png)

```blocks3
ko kliknemo to figuro
objavi (radirka v)
```

\--- /task \---

Ko figura svinčnika prejme objavljeno sporočilo "radirka", mora preklopiti svoj videz na radirko in preklopiti barvo peresa na belo, kar je barva odra!

\--- task \--- Dodaj kodo, ki ustvari radirko.

\--- namigi \--- \--- namig \--- Dodajte kodo za sprite svinčnika: `Ko prejmem`{: class = "block3events"} `radirke`{: class = "block3events"} message `Preklopi na kostumsko brisalo`{: class = "block3looks"} `Nastavi barvo peresa`{: class = "block3extensions"} na belo \--- / namig \--- \--- namig \--- Tu so vsi bloki, ki jih potrebujete:

```blocks3
nastavite barvo peresa na [#FFFFFF]
ko prejmem kljukico [radirka v]

v (radirka v)
```

\--- / namig \--- \--- namig \--- Tukaj je, kako naj izgleda koda: ![svinčnik](images/pencil.png)

```blocks3
ko prejmem [radirka v]
preklopite kostum na (radirka v)
nastavite barvo peresa na [#FFFFFF]
```

\--- / namig \--- \--- / namigi \--- \--- / naloga \---

\--- naloga \--- Preizkusite svoj projekt, da vidite, če lahko počistite stopnjo in izbrišete črte svinčnika.

![posnetek zaslona](images/paint-erase-test.png) \--- / naloga \---

Še ena težava s svinčnikom: lahko povlečete kjerkoli na odru, tudi blizu "jasnih" in brisalnih gumbov!

![posnetek zaslona](images/paint-draw-problem.png)

\--- naloga \--- Če želite to popraviti, spremenite kodo tako, da je pero le navzdol, če miško kliknete **in** položaj `y` kazalca miške pa je večji od `-120`:

![svinčnik](images/pencil.png)

```blocks3
ko zastave klikne
izbrisali vse
Stikalo noša do (svinčnika-modro V)
set barve svinčnikom [# 0035FF]
veke
  kraju (mouse pointer v)
+ če <<mouse down?> in <(miš y) > [-120]>> potem 
  pero navzdol
  še
  pero do
konca
```

\--- / naloga \---

\--- naloga \--- Preizkusite svoj projekt. Zdaj ne smete risati blizu gumbov.

![posnetek zaslona](images/paint-fixed.png) \--- / naloga \---