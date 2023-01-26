## Ustvari svinčnik

Začni z izdelavo svinčnika, ki ga lahko uporabiš za risanje po odru.

\--- task \---

Odpri začetni projekt 'Barvice'

**Online**: open the starter project at [rpf.io/paint-box-on](https://rpf.io/paint-box-on){:target="_blank"}

Če imaš Scratch uporabniški račun, lahko ustvariš kopijo s klikom na **Predelaj**.

**Offline**: open the [starter project](https://rpf.io/p/en/paint-box-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}

V začetnem projektu bi moral videti figuri svinčnika in radirke:

![posnetek zaslona](images/paint-starter.png)

\--- /task \---

\--- task \---

Projektu dodaj razširitev Svinčnik.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Figuri svinčnika dodaj kodo, ki bo omogočila, da figura sledi kazalcu miške in da se to `ponavlja` {:class="block3control"}, tako da lahko rišeš:

![svinčnik](images/pencil.png)

```blocks3
ko kliknemo na zastavico
ponavljaj
pojdi na (kazalcu miške v)
konec
```

\--- /task \---

\--- task \---

Klikni zastavico in premikaj kazalec miške po odru, da vidiš ali tvoja koda deluje.

\--- /task \---

Nato poskrbi, da bo tvoj svničnik risal le, `če`{:class="block3control"} je pritisnjena tipka na miški.

\--- task \---

Figuri svinčnika dodaj to kodo:

![svinčnik](images/pencil.png)

```blocks3
ko kliknemo na zastavico
ponavljaj
  pojdi na (kazalcu miške v)

+ če <je miškin gumb pritsnjen?> potem
  spusti pero
  sicer
  dvigni pero
konec
```

\--- /task \---

\--- task \---

Ponovno preizkusi kodo. Tokrat premikaj svinčnik po odru in hkrati drži pritisnjeno tipko miške. Ali lahko s svojim svinčnikom sedaj rišeš?

![posnetek zaslona](images/paint-draw.png)

\--- /task \---

## \--- collapse \---

## title: Ali tvoj svinčnik ne riše s konico?

Če je videti, da tvoj svinčnik ne riše s konico, temveč črta prihaja iz sredine svinčnika, moraš figuri svinčnika določiti, da bo konica središče figure.

Klini na figuro svinčnika, nato pa klikni na zavihek **Videzi**.

Premakni videz, tako da bo konica svinčnika **tik nad vrhom** centra.

![Sredina videza](images/costume-center-annotated.png)

Sedaj premikaj svinčnik po odru in riši. Svinčnik bi sedaj moral risati črto iz konice.

\--- /collapse \---