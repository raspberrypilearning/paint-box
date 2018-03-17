## Stiftbreite ändern

Geben wir dem Anwender die Möglichkeit verschieden dicke Stifte zu benutzen.

+ Füge zuerst eine neue Variable namens `Dicke`{:class='blockvariable':} hinzu.

[[[generic-scratch-add-variable]]]

+ Füge diese Zeile *innerhalb* der `wiederhole fortlaufend`{:class='blockcontrol':} Schleife ein:

```blocks
    set pen size to (Dicke)
```

Die Stift-Dicke wird nun immer wieder auf den Wert der 'Dicke'-Variablen gesetzt.

+ Klicke auf die Variablen-Anzeige auf der Bühne und klicke auf 'Schieberegler'.

![screenshot](images/paint-slider.png)

Jetzt kannst du den Schieberegler unter der Variablen ziehen, um den Wert zu verändern.

![screenshot](images/paint-slider-change.png)

+ Teste dein Projekt und sieh, ob du die Stift-Dicke verändern kannst.

![screenshot](images/paint-width-test.png)

Wenn du möchtest, kannst du die erlaubten Mindest- und Maximal-Werte festlegen. Dazu klickst du nochmals rechts auf die Variable und klickst auf 'Reglerbereich festlegen'. Setze die Mindest- und Maximal-Werte auf passendere wie 1 und 20.

![screenshot](images/paint-slider-max.png)

Teste deine Dicken-Variable bis du zufrieden bist.