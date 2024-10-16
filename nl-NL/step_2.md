## Een potlood maken

Laten we beginnen met het maken van een potlood dat kan worden gebruikt om op het speelveld te tekenen.

--- task --- Open het "Paint box" start project.

**Online** open het start project op [rpf.io/paint-box-on](https://rpf.io/paint-box-on){:target="_blank"}

Als je een Scratch-account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline**: open het [start project](https://rpf.io/p/nl-NL/paint-box-go){:target="_blank"} in de offline editor.

Als je de Scratch offline editor wilt downloaden en installeren dan kan je die vinden op [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}

In het start project zou je een potlood- en een gum-sprite moeten zien:

![schermafdruk](images/paint-starter.png) --- /task ---

--- task ---

Voeg de Pen-uitbreiding toe aan je project.

[[[generic-scratch3-add-pen-extension]]]

--- /task ---

--- task ---

Voeg wat code toe aan de potlood-sprite om ervoor te zorgen dat deze de muis altijd volgt met een `herhaal`{:class="block3control"} blok, zodat je kunt tekenen:

![potlood](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (muisaanwijzer v) 
end
```

--- /task ---

--- task --- Klik op de vlag en verplaats de muisaanwijzer vervolgens door het werkgebied om te testen of je code werkt. --- /task ---

Laat vervolgens je potlood alleen tekenen `als`{:class="block3control"} als de muisknop wordt ingedrukt.

--- task --- Voeg deze code toe aan je potlood sprite:

![potlood](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (muisaanwijzer v)
+ if <mouse down?> then
  pen down
  else
  pen up
end
```

--- /task ---

--- task --- Test je code opnieuw. Verplaats deze keer het potlood in het speelveld en houd de muisknop ingedrukt. Kun je met je potlood tekenen?

![schermafdruk](images/paint-draw.png) --- /task ---

--- collapse ---
---
title: Trekt je potlood de lijn niet vanaf de punt?
---

Als de lijn die je potlood tekent eruit ziet alsof deze uit het midden van het potlood komt, moet je je potlood sprite veranderen, zodat de punt het midden van de sprite is.

Klik op de potlood sprite en klik vervolgens op de **Uiterlijken** tab.

Verplaats het hele uiterlijk zodat de punt van het potlood zich **net boven** het midden bevindt.

![Middelpunt uiterlijk](images/costume-center-annotated.png)

Beweeg nu het potlood in het speelveld en teken. Het potlood moet nu een lijn trekken vanaf de punt.

--- /collapse ---
