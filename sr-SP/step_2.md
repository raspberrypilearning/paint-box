## Направи оловку

Почни тако што ћеш направити оловку која се може користити за цртање на позорници.

\--- task \--- Отвори Скреч почетни пројекат 'Програм за цртање'.

**На мрежи**: отвори почетни пројекат на [rpf.io/paint-box-on](http://rpf.io/paint-box-on){:target="_blank"}

**Ван мреже**: отвори [почетни пројекат](http://rpf.io/p/en/paint-box-go){:target="_blank"} у уређивачу ван мреже.

Ако је потребно да преузмеш и инсталираш Скреч уређивач ван мреже, можеш га пронаћи на [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

У почетном пројекту, пронаћи ћеш ликове оловке и гумице:

![снимак екрана](images/paint-starter.png) \--- /task \---

\--- task \---

Додај проширење Оловка у свој пројекат.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Додај код лику оловке да `увек`{:class="block3control"} прати стрелицу миша, тако да можеш да црташ:

![оловка](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

\--- /task \---

\--- task \--- Кликни на заставицу, а затим померај стрелицу миша по позорници да провериш да ли твој код функционише. \--- /task \---

Затим, направи да твоја оловка црта `ако је`{:class="block3control"} притиснут тастер миша.

\--- task \--- Додај овај код лику оловке:

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

## title: Да ли ваша оловка не црта из њеног врха?

If the line your pencil draw looks like it is coming from the pencil's middle, you need to change your pencil sprite's so the tip is the sprite's centre.

Click on the pencil sprite, and then click on the **Costumes** tab.

Move the costume's so the tip of the pencil is **just above** the centre.

![Costume center](images/costume-center-annotated.png)

Now move the pencil around on the Stage and draw. The pencil should now draw a line from its tip.

\--- /collapse \---