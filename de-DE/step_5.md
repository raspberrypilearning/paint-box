## Fehler ausbessern

Manchmal passieren Fehler, lass uns also einen 'Löschen'-Knopf und einen Radierer hinzufügen.

--- task ---

Füge die 'x-block' aus dem Buchstabenbereich der Bibliothek hinzu. Färbe das Kostüm rot ein und mache es etwas kleiner. Dieses Kostüm wird unser ‘Löschen’-Knopf.

[[[generic-scratch3-sprite-from-library]]]

![Screenshot](images/paint-x.png)

--- /task ---

--- task ---

Füge Code zur 'Block-X' Figur hinzu, um die Bühne zu löschen, wenn die Figur angeklickt wurde.

![Kreuz](images/cross.png)

```blocks3
Wenn diese Figur angeklickt wird
lösche alles
```

--- /task ---

Beachte, dass du gar keine `Nachricht an alle senden`{:class="block3events"} musst um die Bühne zu löschen, es genügt der `lösche alles`{:class="block3extensions"} Block, der diese Aufgabe übernimmt.

Du hast vielleicht schon bemerkt, dass die Buntstift-Figur auch ein Radier-Kostüm enthält?

![Screenshot](images/paint-eraser-costume.png)

Dein Projekt enthält auch eine eigene Radier-Figur.

--- task ---

Klicke mit der rechten Maustaste auf diese Radierer-Figur und klicke anschließend auf **zeigen**. So sollte deine Bühne jetzt aussehen:

![Screenshot](images/paint-eraser-stage.png)

--- /task ---

--- task ---

Füge der Radierer-Figur Code hinzu, um die Nachricht `'radieren' an alle senden`{:class="block3events"} wenn sie angeklickt wird.

![Radierer](images/eraser.png)

```blocks3
Wenn diese Figur angeklickt wird
sende (radieren v) an alle
```

--- /task ---

Wenn der Buntstift die 'radieren'-Nachricht empfängt, musst du das Buntstift-Kostüm zu “Radierer” ändern und die Buntstiftfarbe auf weiß ändern - die Farbe der Bühne!

--- task ---

Füge Code hinzu um den Radierer zu schaffen.

--- hints ---
 --- hint ---

Füge der Buntstift-Figur Code hinzu: `Wenn ich empfange`{:class="block3events"} die `radieren`{:class="block3events"} Nachricht `Wechsel zu Radierer Kostüm`{:class="block3looks"} `Setze Stiftfarbe auf`{:class="block3extensions"} weiß.

--- /hint --- --- hint ---

Hier sind alle Blöcke die du brauchst:

```blocks3
setze Stiftfarbe auf [#FFFFFF]

Wenn ich [radieren v] empfange

wechsle zu Kostüm (Radierer v)
```

--- /hint --- --- hint ---

So sollte dein Code aussehen:

![Buntstift](images/pencil.png)

```blocks3
Wenn ich [radieren v] empfange
wechsle zu Kostüm (Radierer v)
setze Stiftfarbe auf [#FFFFFF]
```

--- /hint ------ /hints --- --- /task ---

--- task ---

Teste dein Projekt und schau, ob du radieren kannst und die Bühne löschen.

![Screenshot](images/paint-erase-test.png)

--- /task ---

Es gibt noch ein Problem mit dem Buntstift - du kannst auf der ganzen Bühne zeichnen, auch im Bereich der Auswahlsymbole!

![Screenshot](images/paint-draw-problem.png)

--- task ---

Um das zu beheben, ändere den Code, damit der Stift nur dann unten ist, wenn die Maus gedrückt wird **und** die `y` Position des Mauszeigers größer als `-120` ist:

![Buntstift](images/pencil.png)

```blocks3
Wenn die grüne Flagge angeklickt
lösche alles
wechsle zu Kostüm (Stift-blau v)
setze Stiftfarbe auf [#0035FF]
wiederhole fortlaufend 
  gehe zu (Mauszeiger v)
+falls <<Maustaste gedrückt?> und <(Maus y-Position) > [-120]>> , dann 
  schalte Stift ein
  sonst 
  schalte Stift aus
end
```

--- /task ---

--- task ---

Teste dein Projekt. Du solltest jetzt nicht mehr in der Nähe der Auswahlsymbole zeichnen können.

![Screenshot](images/paint-fixed.png)

--- /task ---