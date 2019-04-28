## Kleurpotloden

Laten we verschillende kleurpotloden aan je project toevoegen en de gebruiker de mogelijkheid geven om een kleur te kiezen.

\--- task \--- Klik op de potloodsprite, klik op **Uiterlijken** en dupliceer het 'pencil-blue' uiterlijk.

![screenshot](images/paint-blue-duplicate.png) \---/task\---

\--- task \--- Hernoem je nieuwe kostuum 'potlood-groen' en kleur het potlood groen.

![screenshot](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- Teken twee nieuwe sprites - een blauw vierkant en een groen vierkant. Die zijn bedoeld om te kiezen tussen het blauwe en groene potlood.

![screenshot](images/paint-selectors.png) \--- /task \---

Hernoem je sprites zodat ze 'blauw' en 'groen' heten

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- Voeg code toe aan de 'groene' sprite, zodat wanneer op de sprite wordt geklikt het een bericht `zend signaal`{:class="block3events"} "groen" geeft.

![green square](images/green_square.png)

```blocks3
wanneer op deze sprite wordt geklikt
zend signaal (groen v)
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

De potlood sprite moet luisteren naar het "groen" bericht en de kleur van het uiterlijk en potlood kleur wijzigen in groen.

\--- task \--- Schakel over naar je potlood sprite. Voeg wat code toe zodat wanneer deze sprite het `groen` {:class= "blockevents"} signaal ontvangt, deze moet overschakelen naar het groene potlood uiterlijk en de potloodkleur moet veranderen in groen.

![pencil](images/pencil.png)

```blocks3
wanneer ik signaal [groen v] ontvang
verander uiterlijk naar (potlood-groen v)
maak penkleur [#00CC44]
```

Om het potlood op groen te zetten, klik op het gekleurde vierkant in het `zet pen kleur`{:class="block3extensies"} blok, en klik dan op de groene sprite. \--- /task \---

Then to a similar thing so that you can switch the pencil colour to blue.

\--- task \--- Click on the blue square sprite and add this code:

![blue_square](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blue v)
```

Then click on the pencil sprite and add this code: ![pencil](images/pencil.png)

```blocks3
when I receive [blue v]
switch costume to (pencil-blue v)
set pen color to [#0000ff]
```

\--- /task \---

\--- task \--- Finally, add this code to tell the pencil sprite which colour to start with, and to make sure that the screen is clear when your program starts.

![pencil](images/pencil.png)

```blocks3
when flag clicked
+erase all
+switch costume to (pencil-blue v)
+set pen color to [#0035FF]
forever
  go to (mouse pointer v)
if <mouse down?> then
  pen down
  else
  pen up
end
```

\--- /task \---

If you prefer, you can start with a different colour pencil.

\--- task \--- Test your code. Can you switch between the blue and green pencil colours by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png) \--- /task \---