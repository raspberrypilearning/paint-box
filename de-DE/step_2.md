## Erzeuge einen Stift

Beginnen wir mit einem Buntstift, mit dem wir auf der Bühne zeichnen können.

--- task ---

Öffne das Scratch-Projekt 'Malkasten'.

**Online:** Öffne das Projekt zum Starten [scratch.mit.edu/projects/367782713](https://scratch.mit.edu/projects/367782713){:target="_blank"}

Wenn du bereits einen Scratch-Account besitzt, kannst du dir durch Klick auf **Remix** eine Kopie anlegen.

**Offline**: Öffne das [Start-Projekt](http://rpf.io/p/de-DE/paint-box-go){:target="_blank"} im Offline-Editor.

Wenn du Scratch herunterladen und auf deinem Rechner installieren möchtest, findest du es unter diesem Link: [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

Im Start-Projekt solltest du eine Buntstift- und eine Radierer-Figur sehen:

![Bildschirmfoto](images/paint-starter.png)

--- /task ---

--- task ---

Hinzufügen der Erweiterung Malstift zu deinem Projekt.

[[[generic-scratch3-add-pen-extension]]]

--- /task ---

--- task ---

Füge dem Stift folgenden Code hinzu, damit er dem Mauszeiger `ständig`{:class="blockcontrol"} folgt und du mit ihm malen kannst:

![Buntstift](images/pencil.png)

```blocks3
Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
  gehe zu (Mauszeiger v)
end
```

--- /task ---

--- task ---

Klicke auf die Flagge und bewege die Maus über die Bühne. Sieh, ob der Code richtig arbeitet.

--- /task ---

Als nächstes versuchen wir den Stift nur dann zeichnen zu lassen, `falls`{:class="blockcontrol"} die Maustaste gedrückt wird.

--- task ---

Füge diesen Code deiner Stift-Figur hinzu:

![Buntstift](images/pencil.png)

```blocks3
Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
  gehe zu (Mauszeiger v)
+ falls <Maustaste gedrückt?> , dann 
  schalte Stift ein
  sonst 
  schalte Stift aus
end
```

--- /task ---

--- task ---

Teste deinen Code nochmals. Halte diesmal die Maustaste gedrückt, wenn du die Maus über die Bühne bewegst. Kannst du mit deinem Stift zeichnen?

![Bildschirmfoto](images/paint-draw.png)

--- /task ---

--- collapse ---
---
title: Zeichnet dein Buntstift nicht mit der Spitze?
---

Wenn dein Buntstift nicht mit der Spitze zu zeichnen scheint, sondern mit der Mitte, musst du den Buntstift im Kostüm verschieben.

Klicke auf dei Buntstift-Figur und anschließend auf den **Kostüme** Reiter.

Bewege das Kostüm so, dass die Spitze des Buntstifts **knapp über** dem Zentrum liegt.

![Kostüm-Mitte](images/costume-center-annotated.png)

Bewege nun den Buntstift auf der Bühne und zeichne. Der Buntstift sollte jetzt eine Linie von seiner Spitze aus zeichnen.

--- /collapse ---