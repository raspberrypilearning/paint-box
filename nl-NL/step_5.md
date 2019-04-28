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

\--- task \--- Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

\--- /task \---

When the pencil sprite receives the 'eraser' message, it should switch its costume to the eraser and switch the pen colour to white, which is the same colour as the Stage!

\--- task \--- Add some code to create the eraser.

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white \--- /hint \--- \--- hint \--- Here are all the blocks you need:

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