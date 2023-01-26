## Was du brauchen wirst

Beginnen wir mit einem Buntstift, mit dem wir auf der Bühne zeichnen können.

\--- task \---

Öffne das Scratch-Projekt 'Malkasten'.

**Online**: open the starter project at [rpf.io/paint-box-on](https://rpf.io/paint-box-on){:target="_blank"}

Wenn du bereits einen Scratch-Account besitzt, kannst du dir durch Klick auf **Remix** eine Kopie anlegen.

**Offline**: open the [starter project](https://rpf.io/p/en/paint-box-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}

Im Start-Projekt solltest du eine Buntstift- und eine Radierer-Figur sehen:

![Bildschirmfoto](images/paint-starter.png)

\--- /task \---

\--- task \---

Hinzufügen der Erweiterung Malstift zu deinem Projekt.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Füge dem Stift folgenden Code hinzu, damit er dem Mauszeiger `ständig`{:class="blockcontrol"} folgt und du mit ihm malen kannst:

![Buntstift](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

\--- /task \---

\--- task \---

Klicke auf die Flagge und bewege die Maus über die Bühne. Sieh, ob der Code richtig arbeitet.

\--- /task \---

Als nächstes versuchen wir den Stift nur dann zeichnen zu lassen, `falls`{:class="blockcontrol"} die Maustaste gedrückt wird.

\--- task \---

Füge diesen Code deiner Stift-Figur hinzu:

![Buntstift](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)

+ if <mouse down?> then
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \---

Teste deinen Code nochmals. Halte diesmal die Maustaste gedrückt, wenn du die Maus über die Bühne bewegst. Kannst du mit deinem Stift zeichnen?

![Bildschirmfoto](images/paint-draw.png)

\--- /task \---

## \--- collapse \---

## title: Zeichnet dein Buntstift nicht mit der Spitze?

Wenn dein Buntstift nicht mit der Spitze zu zeichnen scheint, sondern mit der Mitte, musst du den Buntstift im Kostüm verschieben.

Klicke auf dei Buntstift-Figur und anschließend auf den **Kostüme** Reiter.

Bewege das Kostüm so, dass die Spitze des Buntstifts **knapp über** dem Zentrum liegt.

![Kostüm-Mitte](images/costume-center-annotated.png)

Bewege nun den Buntstift auf der Bühne und zeichne. Der Buntstift sollte jetzt eine Linie von seiner Spitze aus zeichnen.

\--- /collapse \---