## Razveljavitev napak

Napake se dogajajo, zato dodaj gumb »počisti« in gumb za radirko.

\--- task \---

Dodaj figuro 'X-block', ki se nahaja v razdelku Črke v knjižnici figur. Preimenuj to figuro v 'blok x', pobarvaj jo rdeče in jo malo zmanjšaj. To bo gumb, ki 'počisti' risalno površino.

[[[generic-scratch3-sprite-from-library]]]

![posnetek zaslona](images/paint-x.png)

\--- /task \---

\--- task \---

Figuri 'blok x' dodaj kodo, ki ob kliku nanjo izbriše vse na odru.

![križec](images/cross.png)

```blocks3
ko kliknemo to figuro
izbriši vse
```

\--- /task \---

Za čiščenje odra ti ni potrebno `objaviti`{: class = "block3events"} sporočila, ker že `izbriši vse`{: class = "block3extensions"} blok opravi to delo.

Si opazil, da figura svinčnika vsebuje tudi videz radirke?

![posnetek zaslona](images/paint-eraser-costume.png)

Tvoj projekt vsebuje tudi ločeno figuro radirke.

\--- task \---

Click on this eraser sprite and then select **show**.

![posnetek zaslona](images/show-eraser.png)

Here is how your Stage should look now:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
ko kliknemo to figuro
objavi (radirka v)
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
nastavi barvo peresa na [#FFFFFF]
ko prejmem [radirka v]

zamenjaj videz na (radirka v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
ko prejmem [radirka v]
zamenjaj videz na (radirka v)
nastavi barvo peresa na [#FFFFFF]
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
ko kliknemo na zastavico
izbriši vse
zamenja videz na (svinčnik-moder v)
nastavi barvo peresa na [#0035FF]
ponavljaj
  pojdi na (kazalec miške v)
  +if <(je miškin gumb pritisnjen?) in <(miškin y) > [-120]>> potem
    spusti pero
  sicer
    dvigni pero
konec
```

\--- /task \---

\--- task \---

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---