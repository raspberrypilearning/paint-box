## Fouten maken

Soms maak je fouten, dus laten we een knop 'wissen' en een gum toevoegen.

\--- task \--- Voeg de sprite 'Block-X' toe uit Letters bibliotheek. Kleur het sprite-uiterlijk rood en maak het een beetje kleiner. Dit wordt de knop 'Wissen'.

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png) \--- /task \---

\--- taak \--- Voeg code toe aan de 'Wissen' sprite om het speelveld te wissen wanneer op de sprite wordt geklikt.

![cross](images/cross.png)

```blocks3
wanneer op deze sprite wordt geklikt
wis alles
```

\--- /task \---

Je hoeft geen `zend signaal`{:class="block3events"} te gebruiken om het speelveld te wissen, omdat het `wis alles`{:class="block3extensions"} blok dat werk doet.

Zie je dat de potlood sprite een gum uiterlijk bevat?

![screenshot](images/paint-eraser-costume.png)

Je project bevat ook een afzonderlijke gumsprite.

\--- task \--- Klik op de gum sprite en klik vervolgens op het oogje naast **Toon** om deze sprite weer te geven. Hier is hoe je speelveld eruit zou moeten zien:

![screenshot](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Voeg code toe aan de gum prite om een `zend signaal` {:class="block3events"} gum te verzenden wanneer op de gum sprite wordt geklikt.

![eraser](images/eraser.png)

```blocks3
wanneer op deze sprite wordt geklikt
zend signaal (gum v)
```

\--- /task \---

Wanneer het potlood de "gum"-boodschap ontvangt, zou het potlood uiterlijk in de gum moeten veranderen en de potloodkleur in wit moeten veranderen - dezelfde kleur als de achtergrond van het speelveld!

\--- task \--- Voeg een code toe om de gum te maken.

\--- hints \--- \--- hint \--- Voeg een code toe aan de potlood sprite: `Wanneer ik signaal ontvang`{:class="block3events"} `gum`{:class="block3events"} bericht `verander uiterlijk naar gum` {:class="block3looks"} `maak penkleur` {: class = "block3extensions"} wit \--- / hint \--- \--- hint \--- Hier zijn alle blokken die je nodig hebt:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

\--- /hint \--- \--- hint \--- Here is what the code should look like: ![pencil](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Test your project to see if you can clear the Stage and erase pencil lines.

![screenshot](images/paint-erase-test.png) \--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![screenshot](images/paint-draw-problem.png)

\--- task \--- To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![pencil](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
  go to (mouse pointer v)
+if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \--- Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png) \--- /task \---