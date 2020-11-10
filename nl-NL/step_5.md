## Fouten repareren

Soms maak je fouten, dus laten we een knop 'wissen' en een gum toevoegen.

\--- task \---

Voeg de sprite 'Block-X' toe uit de Letters-sectie in de bibliotheek. Kleur het sprite-uiterlijk rood en maak het een beetje kleiner. Dit wordt de knop 'wissen'.

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png)

\--- /task \---

\--- task \---

Voeg code toe aan de 'Wissen' sprite om het speelveld te wissen wanneer op de sprite wordt geklikt.

![kruis](images/cross.png)

```blocks3
wanneer op deze sprite wordt geklikt
wis alles
```

\--- /task \---

Je hoeft geen `zend signaal`{:class="block3events"} te gebruiken om het speelveld te wissen, omdat het `wis alles`{:class="block3extensions"} blok dat werk doet.

Zie je dat de potlood sprite een gum uiterlijk bevat?

![screenshot](images/paint-eraser-costume.png)

Je project bevat ook een afzonderlijke gumsprite.

\--- task \---

Click on this eraser sprite and then select **show**.

![screenshot](images/show-eraser.png)

Here is how your Stage should look now:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
wanneer op deze sprite wordt geklikt
zend signaal (gum v)
```

\--- /task \---

When the pencil sprite receives the 'eraser' message, it should switch its costume to the eraser and switch the pen colour to white, which is the same colour as the Stage!

\--- task \---

Add some code to create the eraser.

\--- hints \--- \--- hint \---

Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

\--- /hint \--- \--- hint \---

Here are all the blocks you need:

```blocks3
maak penkleur [#FFFFFF]
wanneer ik signaal [gum v] ontvang

verander uiterlijk naar (gum v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
wanneer ik signaal [gum v] ontvang
verander uiterlijk naar (gum v)
maak penkleur [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \---

Test your project to see if you can clear the Stage and erase pencil lines.

![screenshot](images/paint-erase-test.png)

\--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![screenshot](images/paint-draw-problem.png)

\--- task \---

To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![pencil](images/pencil.png)

```blocks3
wanneer groene vlag wordt aangeklikt
wis alles
verander uiterlijk naar (potlood-blauw v)
maak penkleur [#0035FF]
herhaal
 ga naar (muisaanwijzer v)
+als <muis ingedrukt?> en <(muis y)> [-120]>> dan
pen neer
anders
pen op
end
```

\--- /task \---

\--- task \---

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---