## Creează un creion

Începe prin a crea un creion pe care să îl poți folosi pentru a desena pe Scenă.

\--- task \--- Deschide proiectul de bază Scratch pentru "Cutia de culori".

**Online**: deschide proiectul de bază de la [rpf.io/paint-box-on](http://rpf.io/paint-box-on){:target="_blank"}

Dacă ai un cont Scratch, poți crea o copie dând click pe **Remix**.

**Offline**: deschide [proiectul de bază](http://rpf.io/p/en/paint-box-go){:target="_blank"} în editorul offline.

Dacă ai nevoie să descarci și să instalezi editorul Scratch offline, îl poți găsi la [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

În proiectul de bază ar trebui să poți vedea personajele pentru creion și radieră:

![captură de ecran](images/paint-starter.png) \--- /task \---

\--- task \---

Adaugă în proiect extensia pentru creion.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Adaugă niște cod personajului pentru creion pentru a face personajul să urmărească `la infinit`{:class="block3control"} cursorul mouse-ului astfel încât să poți desena:

![pencil](images/pencil.png)

```blocks3
când se dă click pe steguleț
la infinit
  mergi la (cursorul mouse-ului v)
sfârșit
```

\--- /task \---

\--- task \--- Fă click pe steguleț și apoi deplasează cursorul mouse-ului prin Scenă pentru a testa dacă funcționează codul tău. \--- /task \---

În continuare, permite creionului să deseneze doar `dacă`{:class="block3control"} butonul mouse-ului este apăsat.

\--- task \--- Adaugă acest cod la personajul creionului tău:

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

\--- task \--- Test your code again. This time, move the pencil around the Stage and hold down the mouse button. Can you draw with your pencil?

![screenshot](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: Does your pencil not draw from its tip?

If the line your pencil draw looks like it is coming from the pencil's middle, you need to change your pencil sprite's so the tip is the sprite's centre.

Click on the pencil sprite, and then click on the **Costumes** tab.

Move the costume's so the tip of the pencil is **just above** the centre.

![Costume center](images/costume-center-annotated.png)

Now move the pencil around on the Stage and draw. The pencil should now draw a line from its tip.

\--- /collapse \---