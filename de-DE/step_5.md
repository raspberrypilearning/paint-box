## Fehler ausbessern

Manchmal passieren Fehler, lass uns also einen 'Löschen'-Knopf und einen Radierer hinzufügen.

\--- task \---

Füge die 'x-block' aus dem Buchstabenbereich der Bibliothek hinzu. Färbe das Kostüm rot ein und mache es etwas kleiner. Dieses Kostüm wird unser ‘Löschen’-Knopf.

[[[generic-scratch3-sprite-from-library]]]

![Screenshot](images/paint-x.png)

\--- /task \---

\--- task \---

Füge Code zur 'Block-X' Figur hinzu, um die Bühne zu löschen, wenn die Figur angeklickt wurde.

![Kreuz](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- /task \---

Beachte, dass du gar keine `Nachricht an alle senden`{:class="block3events"} musst um die Bühne zu löschen, es genügt der `lösche alles`{:class="block3extensions"} Block, der diese Aufgabe übernimmt.

Du hast vielleicht schon bemerkt, dass die Buntstift-Figur auch ein Radier-Kostüm enthält?

![Screenshot](images/paint-eraser-costume.png)

Dein Projekt enthält auch eine eigene Radier-Figur.

\--- task \---

Click on this eraser sprite and then select **show**.

![Screenshot](images/show-eraser.png)

Here is how your Stage should look now:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (radieren v)
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
set pen color to [#FFFFFF]
when I receive [radieren v]

switch costume to (Radierer v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
when I receive [radieren v]
switch costume to (Radierer v)
set pen color to [#FFFFFF]
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
when flag clicked
erase all
switch costume to (Buntstift-blau v)
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

\--- task \---

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---