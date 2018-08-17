## Einen Stift machen

Beginnen wir mit einem Stift, mit dem wir auf der Bühne zeichnen können.

+ Öffne das 'Paintbox'-Projekt in Scratch entweder online bei [jumpto.cc/paint-go-de-DE](https://scratch.mit.edu/projects/227798520/#editor){:target="_blank"} oder lade es unter [http://jumpto.cc/paint-get-de-DE](https://github.com/raspberrypilearning/paint-box/raw/master/de-DE/resources/PaintBox.sb2) herunter wenn du den Offline-Editor benutzt.

Bei den Figuren siehst du einen Stift und einen Radierer:

![screenshot](images/paint-starter.png)

+ Füge dem Stift folgenden Code hinzu, damit er der Maus `ständig`{:class="blockcontrol"} folgt und du mit ihm malen kannst:

```blocks
    Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
  gehe zu [mouse pointer v]
end
```

+ Klicke auf die Flagge und bewege die Maus über die Bühne. Sieh, ob der Code richtig arbeitet.

Als nächstes versuchen wir, den Stift nur dann zeichnen zu lassen, `wenn`{:class="blockcontrol"} die Maus geklickt wird.

+ Füge diesen Code deiner Stift-Figur hinzu:

![screenshot](images/paint-pencil-draw-code.png)

+ Teste deinen Code nochmals. Halte diesmal die Maustaste gedrückt, wenn du die Maus über die Bühne bewegst. Kannst du mit deinem Stift zeichnen?

![screenshot](images/paint-draw.png)

--- collapse ---
---
title: Wenn du Probleme hast...
---
Wenn dein Stift nicht mit der Spitze zu zeichnen scheint, sondern mit der Mitte, dann musst du die Kostüm-Mitte ändern.

![Kostüm-Mitte](images/costume-center.png)

Du musst das Fadenkreuz für den Stift **knapp unter** der Spitze des Stifts platzieren, nicht genau auf der Spitze.

Die Änderungen der Kostüm-Mitte einer Figur werden erst wirksam, wenn etwas Anderes angeklickt wird. Klicke also auf ein anderes Kostüm oder auf den 'Skripte'-Reiter um deine Änderungen abzuschließen.

--- /collapse ---
