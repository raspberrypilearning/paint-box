## Ustvari svinčnik

Začni z izdelavo svinčnika, ki ga lahko uporabiš za risanje po odru.

--- task ---

Odpri začetni projekt 'Barvice'

**S povezavo:** odpri nov spletni Scratch projekt na [rpf.io/paint-box-on](https://rpf.io/paint-box-on){:target="_blank"}

Če imaš Scratch uporabniški račun, lahko ustvariš kopijo s klikom na **Predelaj**.

**Brez povezave** : odpri začetni projekt [ ](https://rpf.io/p/sl-SI/paint-box-go){:target="_blank"} v namiznem urejevalniku.

Če želiš prenesti in namestiti Namizni Scratch, ga lahko najdeš na [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}

V začetnem projektu bi moral videti figuri svinčnika in radirke:

![posnetek zaslona](images/paint-starter.png)

--- /task ---

--- task ---

Projektu dodaj razširitev Svinčnik.

[[[generic-scratch3-add-pen-extension]]]

--- /task ---

--- task ---

Figuri svinčnika dodaj kodo, ki bo omogočila, da figura sledi kazalcu miške in da se to `ponavlja` {:class="block3control"}, tako da lahko rišeš:

![svinčnik](images/pencil.png)

```blocks3
ko je kliknjena zelena zastavica
ponavljaj
pojdi na (kazalcu miške v)
konec
```

--- /task ---

--- task ---

Klikni zastavico in premikaj kazalec miške po odru, da vidiš ali tvoja koda deluje.

--- /task ---

Nato poskrbi, da bo tvoj svničnik risal le, `če`{:class="block3control"} je pritisnjena tipka na miški.

--- task ---

Figuri svinčnika dodaj to kodo:

![svinčnik](images/pencil.png)

```blocks3
ko je kliknjena zelena zastavica
ponavljaj
  pojdi na (kazalcu miške v)
+ če <je miškin gumb pritisnjen?> potem 
  spusti pero
  sicer
  dvigni pero
konec
```

--- /task ---

--- task ---

Ponovno preizkusi kodo. Tokrat premikaj svinčnik po odru in hkrati drži pritisnjeno tipko miške. Ali lahko s svojim svinčnikom sedaj rišeš?

![posnetek zaslona](images/paint-draw.png)

--- /task ---

--- collapse ---
---
title: Ali tvoj svinčnik ne riše s konico?
---
Če je videti, da tvoj svinčnik ne riše s konico, temveč črta prihaja iz sredine svinčnika, moraš figuri svinčnika določiti, da bo konica središče figure.

Klini na figuro svinčnika, nato pa klikni na zavihek **Videzi**.

Premakni videz, tako da bo konica svinčnika **tik nad vrhom** centra.

![Sredina videza](images/costume-center-annotated.png)

Sedaj premikaj svinčnik po odru in riši. Svinčnik bi sedaj moral risati črto iz konice.

--- /collapse ---
