## Wat heb je nodig

Laten we beginnen met het maken van een potlood dat kan worden gebruikt om op het speelveld te tekenen.

\--- task \--- Open het "Paint box" start project.

**Online** open het online start project op [rpf.io/paint-box-on](http://rpf.io/paint-box-on){:target="_ blank"}

**Offline**: open het [startproject](http://rpf.io/p/en/paint-box-go){:target="_ blank"} in de offline editor.

Als je de Scratch offline editor wilt downloaden en installeren dan kan je die vinden op [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

In het startersproject zou je een potlood- en een gumsprite moeten zien:

![screenshot](images/paint-starter.png) \--- /task \---

\--- task \----

Voeg de Pen-uitbreiding toe aan je project.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Voeg wat code toe aan de potlood sprite om ervoor te zorgen dat deze de muis altijd volgt met een `herhaal`{:class="blockcontrol"} blok, zodat je kunt tekenen:

![pencil](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

\--- /task \---

\--- task \--- Click the flag and then move the mouse pointer around the Stage to test whether your code works. \--- /task \---

Next, make your pencil only draw `if`{:class="block3control"} the mouse button is being clicked.

\--- task \--- Add this code to your pencil sprite:

![pencil](images/pencil.png)

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

\--- task \--- Test your code again. This time, move the pencil around the Stage and hold down the mouse button. Kun je met je potlood tekenen?

![screenshot](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: Does your pencil not draw from its tip?

If the line your pencil draw looks like it is coming from the pencil's middle, you need to change your pencil sprite's so the tip is the sprite's centre.

Click on the pencil sprite, and then click on the **Costumes** tab.

Move the costume's so the tip of the pencil is **just above** the centre.

![Costume center](images/costume-center-annotated.png)

Now move the pencil around on the Stage and draw. The pencil should now draw a line from its tip.

\--- /collapse \---