## Kleurpotloden

Laten we verschillende kleurpotloden aan je project toevoegen en de gebruiker de mogelijkheid geven om een kleur te kiezen.

--- task --- Hernoem de `potlood` sprite naar `potlood-blauw`

![hernoem-potlood](images/rename-pencil.png) --- /task ---

--- task --- Rechts-klik op de potlood sprite en dupliceer het '-potlood-blauw' uiterlijk.

![schermafdruk](images/paint-blue-duplicate.png) --- /task ---

--- task --- Hernoem je nieuwe kostuum 'potlood-groen' en kleur het potlood groen.

![schermafdruk](images/paint-pencil-green.png)

--- /task ---

--- task --- Teken twee nieuwe sprites - een blauw vierkant en een groen vierkant. Die zijn bedoeld om te kiezen tussen het blauwe en het groene potlood.

![schermafdruk](images/paint-selectors.png) --- /task ---

--- task --- Hernoem je sprites zodat ze 'blauw' en 'groen' heten

[[[generic-scratch3-rename-sprite]]]

--- /task ---

--- task --- Voeg code toe aan de 'groene' sprite, zodat wanneer op de sprite wordt geklikt het een bericht `zend signaal`{:class="block3events"} "groen" geeft.

![groen vierkant](images/green_square.png)

```blocks3
when this sprite clicked
broadcast (groen v)
```

[[[generic-scratch3-broadcast-message]]] --- /task ---

De potlood sprite moet luisteren naar het "groen" bericht en de kleur van het uiterlijk en het potlood wijzigen in groen.

--- task --- Schakel over naar je potlood sprite. Voeg wat code toe zodat wanneer deze sprite het `groen`{:class="block3events"} signaal ontvangt, deze moet overschakelen naar het groene potlooduiterlijk en de potloodkleur moet veranderen in groen.

![potlood](images/pencil.png)

```blocks3
when I receive [groen v]
switch costume to (potlood-groen v)
set pen color to [#00CC44]
```

Om het potlood op groen te zetten, klik op het gekleurde vierkant in het `zet pen kleur`{:class="block3extensions"} blok, en klik dan op de groene vierkantsprite. --- /task ---

Doe vervolgend hetzelfde voor een potlood met de kleur blauw.

--- task --- Klik op de blauwe vierkantsprite en voeg deze code toe:

![blauw_vierkant](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blauw v)
```

Klik vervolgens op de potlood sprite en voeg deze code toe: ![potlood](images/pencil.png)

```blocks3
when I receive [blauw v]
switch costume to (potlood-blauw v)
set pen color to [#0000ff]
```

--- /task ---

--- task --- Voeg ten slotte deze code toe om de sprite van het potlood te vertellen met welke kleur deze moet te beginnen en om ervoor te zorgen dat het scherm leeg is wanneer je programma start.

![potlood](images/pencil.png)

```blocks3
when flag clicked
+erase all
+switch costume to (potlood-blauw v)
+set pen color to [#0035FF]
forever
  go to (muisaanwijzer v)
if <mouse down?> then
  pen down
  else
  pen up
end
```

--- /task ---

Als je wilt, kunt je met een ander kleurpotlood beginnen.

--- task --- Test je code. Kun je schakelen tussen het blauwe en groene potlood door op de blauwe of groene vierkant te klikken?

![schermafdruk](images/paint-pens-test.png) --- /task ---