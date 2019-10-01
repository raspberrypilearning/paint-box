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

The pencil sprite should listen for the "green" message and change its costume and pencil colour in response.

\--- task \--- Switch to your pencil sprite. Add some code so that when this sprite receives the `green`{:class="block3events"} broadcast, it switchs to the green pencil costume and changes the pen colour to green.

![pencil](images/pencil.png)

```blocks3
ko prejmem [zeleno v]
preklopi kostum na (svinčnik-zeleni v)
nastavite barvo peresa na [# 00CC44]
```

To set the pencil to colour to green, click the coloured square in the `set pen color`{:class="block3extensions"} block, and then click on the green square sprite. \--- /task \---

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