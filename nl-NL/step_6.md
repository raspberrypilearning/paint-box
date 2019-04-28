## De potlooddikte wijzigen

Vervolgens kunt je code toevoegen om de persoon die jouw programma gebruikt, toe te staan om dingen te tekenen met verschillende pen breedtes.

\--- task \--- Voeg eerst een nieuwe variabele toe met de naam `breedte`{:class="blockvariable"}.

[[[generic-scratch3-add-variable]]] \--- /task \---

\--- task \--- Voeg deze regel **binnen** het `herhaal`{:class="blockcontrol"} blok van de potloodcode toe:

```blocks3
wanneer groene vlag wordt aangeklikt
wis alles
verander uiterlijk naar (potlood-blauw v)
maak penkleur [#0035FF]
herhaal
 ga naar (muisaanwijzer v)
 set pen size to (breedte :: variables)
 if &lt;<muis ingedrukt> en &lt;(mouse y) &gt; [-120]&gt;&gt; then 
  pen down
  else
  pen up
end
```

\--- /task \---

De pendikte wordt nu herhaaldelijk ingesteld op de waarde van de `breedte` {:class="block3variables"} variabele.

\--- task \--- Klik met de rechtermuisknop op de `breedte`{:class="block3variables"} variabele weergegeven in het speelveld en klik vervolgens op **schuif**.

![screenshot](images/paint-slider.png) \--- /task \---

Je kunt nu de schuifregelaar onder de variabele verslepen om de waarde te wijzigen.

![screenshot](images/paint-slider-change.png)

\--- taak \--- Test je project en kijk of je de pen breedte kunt aanpassen.

![screenshot](images/paint-width-test.png) -- /task \---