## Barvni svinčniki

Zdaj boste svojemu projektu dodali različne barvne svinčnike in uporabniku omogočili izbiro med njimi.

\--- naloga \--- Kliknite na svinčnik sprite, kliknite na **Kostumi**in podvojite kostum "svinčnik-modra".

![posnetek zaslona](images/paint-blue-duplicate.png) \--- / naloga \---

\--- naloga \--- Poimenujte novi kostum "svinčnik-zelen" in obarvajte zeleno svinčnik.

![screenshot](images/paint-pencil-green.png)

\--- / naloga \---

\--- naloga \--- Narišite dva nova sprita: en modri kvadrat in en zeleni kvadrat. To je za izbiro med modrim in zelenim svinčnikom.

![posnetek zaslona](images/paint-selectors.png) \--- / naloga \---

\--- naloga \--- Preimenujte nove sprite tako, da se imenujejo "modra" in "zelena"

[[[generic-scratch3-rename-sprite]]]

\--- / naloga \---

\--- naloga \--- Dodajte nekaj kode v 'zeleni' sprite, tako da, ko se ta sprite klikne, `odda`{: class = "block3events"} sporočilo "zeleno".

![zeleni kvadrat](images/green_square.png)

```blocks3
ko je ta geslo kliknilo
oddaje (zelena v)
```

[[[generic-scratch3-broadcast-message]]] \--- / naloga \---

Slovnik sprite mora poslušati za "zeleno" sporočilo in spremeniti svoj kostum in barvo svinčnika v odgovor.

\--- naloga \--- Preklopite na vašo sprite. Dodajte nekaj kode, tako da, ko ta sprite prejme oddajo `zeleno`{: class = "block3events"}, preklopi na zeleno pisalo in spremeni barvo peresa na zeleno.

![svinčnik](images/pencil.png)

```blocks3
ko prejmem [zeleno v]
preklopi kostum na (svinčnik-zeleni v)
nastavite barvo peresa na [# 00CC44]
```

Nastavljanje svinčnikom obarva zeleno, kliknite barvni kvadrat v `set barve pero`{: razred = "block3extensions"} blok in nato na zeleni kvadratni Sprite. \--- / naloga \---

Potem na podobno stvar, tako da lahko preklopite barvo svinčnika na modro.

\--- naloga \--- Kliknite na modro kvadratno besedo in dodajte to kodo:

![blue_square](images/blue_square.png)

```blocks3
ko je ta geslo kliknilo
oddaje (modra v)
```

Nato kliknite na svinčnik in dodajte to kodo: ![svinčnik](images/pencil.png)

```blocks3
ko prejmem [modri v]
preklopi kostum na (svinčnik-modri v)
nastavite barvo peresa na [# 0000ff]
```

\--- / naloga \---

\--- naloga \--- Nazadnje dodajte to kodo, da povejte, kaj je treba začeti s sprijemalnikom, in se prepričajte, da je zaslon jasen, ko se program zažene.

![svinčnik](images/pencil.png)

```blocks3
ko zastava kliknili
+ izbrišete vse
+ preklop kostum za (svinčnik, modra v)
+ nastavite barvni svinčnik na [# 0035FF]
večno
  Pojdi na (kazalec miške v)
, če <mouse down?> pa
  pero navzdol
  še
  pen up
konec
```

\--- / naloga \---

Če želite, lahko začnete z drugim barvnim svinčnikom.

\--- naloga \--- Preverite svojo kodo. Ali lahko preklopite med modro in zeleno barvo svinčnika s klikom na modre ali zelene kvadrate?

![posnetek zaslona](images/paint-pens-test.png) \--- / naloga \---