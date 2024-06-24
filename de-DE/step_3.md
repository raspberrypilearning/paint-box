## Buntstifte

Laß uns deinem Projekt verschiedene Buntstifte hinzufügen, die der Anwender anschließend auswählen kann.

--- task ---

Ändere den Namen des `Buntstift-` Kostüms zu `Stift-blau`

![Buntstift-umbenennen](images/rename-pencil.png)

--- /task ---

--- task ---

Klicke mit der rechten Maustaste im Reiter Kostüme auf das Stift-blau-Kostüm und dupliziere es.

![Screenshot](images/paint-blue-duplicate.png)

--- /task ---

--- task ---

Ändere den Namen des neuen Kostüms in 'Stift-grün' und färbe den Buntstift grün.

![screenshot](images/paint-pencil-green.png)

--- /task ---

--- task ---

Zeichne zwei neue Figuren: ein blaues Quadrat und ein grünes Quadrat. Diese sind für die Auswahl einer Malfarbe für den dem blauen oder grünen Buntstift.

![Screenshot](images/paint-selectors.png)

--- /task ---

--- task ---

Ändere den Namen der neuen Figuren, so dass diese 'blau' und 'grün' heißen

[[[generic-scratch3-rename-sprite]]]

--- /task ---

--- task ---

Füge nun Code zur ‘grün’-Figur hinzu, so dass sie, wenn sie geklickt wird, die Nachricht 'grün' `an alle sendet`{:class="block3events"}.

![gruenes_Quadrat](images/green_square.png)

```blocks3
when this sprite clicked
broadcast (grün v)
```

[[[generic-scratch3-broadcast-message]]]

--- /task ---

Die Buntstift-Figur soll auf die 'grün' Nachricht hören und seine Kostüm-Farbe und Buntstift-Farbe entsprechend ändern.

--- task ---

Schalte zu deiner Stift-Figur. Füge Code hinzu, so dass diese Figur, wenn sie die Nachricht `grün`{:class="block3events"} empfängt, zum Kostum Buntstift-grün wechselt und die Stiftfarbe zu grün ändert.

![Buntstift](images/pencil.png)

```blocks3
when I receive [grün v]
switch costume to  (Stift-grün v)
set pen color to [#00CC44]
```

Um die Zeichenfarbe auf das gleiche Grün wie das Auswahlfeld zu setzen, klicke das farbige Feld in `setze Stiftfarbe auf`{:class="block3extensions"} an, und wähle die entsprechende Farbe aus.

--- /task ---

Nun kannst du das Gleiche machen, um den Buntstift auf blau zu schalten.

--- task ---

Klicke auf das blaue Quadrat und füge diesen Code hinzu:

![blaues_Quadrat](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blau v)
```

Anschließend klicke auf die Buntstift-Figur und füge diesen Code hinzu:

![Buntstift](images/pencil.png)

```blocks3
when I receive [blau v]
switch costume to (Stift-blau v)
set pen color to [#0000ff]
```

--- /task ---

--- task ---

Zum Schluss fügst du noch Code ein, um der Bleistift Figur zu sagen mit welcher Farbe sei anfangen soll uns stell sicher, dass das Programm mit einem leeren Bildschirm beginnt.

![Buntstift](images/pencil.png)

```blocks3
when flag clicked
+erase all
+switch costume to(Stift-blau v)
+set pen color to [#0035FF]
forever
  go to(Mauszeiger v)
if <mouse down?> then 
  pen down
  else
  pen up
end
```

--- /task ---

Wir haben hier blau gewählt, aber du kannst mit jeder anderen Stiftfarbe beginnen, wenn du willst.

--- task ---

Teste deinen Code. Kannst du zwischen den blauen und grünen Buntstiften wechseln, indem du das blaue bzw. grüne Quadrat anklickst?

![Screenshot](images/paint-pens-test.png)

--- /task ---