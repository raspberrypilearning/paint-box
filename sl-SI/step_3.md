## Barvice

Svojemu projektu boše sedaj dodal različne barvne svinčnike in uporabniku omogočil izbiro med njimi.

\--- task \--- Z desno tipko klikni na figuro `svinčnik` in preimenuj videz v `'svinčnik-moder'`

![rename-pencil](images/rename-pencil.png) \--- /task \---

\--- task \--- Z desno tipko klikni na videz 'svinčnik-moder' in ga podvoji.

![screenshot](images/paint-blue-duplicate.png) \--- /task \---

\--- task \--- Poimenuje novi videz 'svinčnik-zelen', in ga obarvaj zeleno.

![screenshot](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- Nariši dve novi figuri: en moder in en zelen kvadrat. Namenjena sta izbiri med modro in zeleno barvico.

![screenshot](images/paint-selectors.png) \--- /task \---

\--- task \--- Preimenuj novi figuri v 'modra' in 'zelena'

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- Figuri 'zelena' dodaj kodo, ki povhzroči, da klik na figuro `objavi`{:class="block3events"} sporočilo 'zelena'.

![green square](images/green_square.png)

```blocks3
ko kliknemo to figuro
objavi (zelena v)
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

Figura svinčnika naj spremlja objave in v primeru prejema sporočila 'zelena' spremeni svoj videz in barvo svinčnika.

\--- task \--- Preklopi na figuro svinčnika. Dodaj kodo, ki bo omogočila, da bo figura `zelena`{:class="block3events"} prejela objavo, preklopila na videz zelene barvice in spremenila barvo svinčnika na zeleno.

![pencil](images/pencil.png)

```blocks3
ko prejmem [zelena v]
zamenjaj videz na (svinčnik-zelen v)
nastavi barvo peresa na [# 00CC44]
```

Da bi spremenil barvo svinčnika na zeleno, najprej klikni na obarvan kvadrat v bloku `nastavi barvo peresa na`, izberi kapaljko in potem klikni na figuro z zelenim kvadratom. \--- /task \---

Then to a similar thing so that you can switch the pencil colour to blue.

\--- task \--- Click on the blue square sprite and add this code:

![blue_square](images/blue_square.png)

```blocks3
ko je ta geslo kliknilo
oddaje (modra v)
```

Then click on the pencil sprite and add this code: ![pencil](images/pencil.png)

```blocks3
ko prejmem [modri v]
preklopi kostum na (svinčnik-modri v)
nastavite barvo peresa na [# 0000ff]
```

\--- /task \---

\--- task \--- Finally, add this code to tell the pencil sprite which colour to start with, and to make sure that the screen is clear when your program starts.

![pencil](images/pencil.png)

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

\--- /task \---

If you prefer, you can start with a different colour pencil.

\--- task \--- Test your code. Can you switch between the blue and green pencil colours by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png) \--- /task \---