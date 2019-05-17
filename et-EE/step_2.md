## Tee pliiats

Alustage pliiatsi tegemisest, mida saate kasutada etapis.

\--- ülesanne - Avage 'Paint box' Scratch starter projekt.

**Online**: avab starteri projekti aadressil [rpf.io/paint-box-on](http://rpf.io/paint-box-on){: target = "_ blank"}

**Offline**: avage [starteri projekt](http://rpf.io/p/en/paint-box-go){: target = "_ blank"} offline redaktoris.

Kui teil on vaja alla laadida ja installida Scratch offline redaktor, leiad selle aadressil [rpf.io/scratchoff](http://rpf.io/scratchoff){: target = "_ blank"}

Starteriprojektis peaksite nägema pliiatsit ja kustutusseadet:

![ekraanipilt](images/paint-starter.png) \--- / ülesanne \---

\--- ülesanne \---

Lisage oma projektile pliiatsi laiendus.

[[[generic-scratch3-add-pen-extension]]]

\--- / ülesanne \---

\--- ülesanne \---

Lisage pliiatsile mõned koodid, et teha sprite järgige hiirekursorit `igavesti`{: class = "block3control"}, et saaksite joonistada:

![pliiats](images/pencil.png)

```blocks3
kui lipp klõpsas
igavesti
  minge (hiirekursor v)
lõppu
```

\--- / ülesanne \---

\--- ülesanne - Klõpsake lippu ja seejärel liigutage hiirekursorit lava ümber, et kontrollida, kas kood toimib. \--- / ülesanne \---

Järgmisena tehke pliiats ainult juhtida `kui`{: class = "block3control"} hiirenuppu klikitakse.

\--- ülesanne \--- Lisage see kood pliiatsipildile:

![pliiats](images/pencil.png)

```blocks3
kui lipp klõpsas
igavesti
  minge (hiirekursor v)

+, kui <mouse down?> siis
  pliiatsi alla
  muu
  pliiatsi üles
lõppu
```

\--- / ülesanne \---

\--- ülesanne \--- Testige oma koodi uuesti. Seekord liigutage pliiatsit lava ümber ja hoidke hiire nuppu all. Kas saate oma pliiatsiga joonistada?

![ekraanipilt](images/paint-draw.png) \--- / ülesanne \---

## \--- kollaps \---

## pealkiri: Kas teie pliiats ei tõmba oma otsast?

Kui joon, mille sinu pliiats tõmbab, näeb välja nagu see on pliiatsikeskme keskelt, tuleb muuta oma pliiatsitõkke, nii et ots on sprite keskus.

Klõpsake pliiatsilõõtsale ja seejärel klõpsake vahekaardil **Kostüümid**.

Liiguta kostüümi nii, et pliiatsipeal on **on keskelt üle**.

![Kostüümikeskus](images/costume-center-annotated.png)

Nüüd liigutage pliiats ümber laval ja joonistage. Pliiats peaks joonistama joone otsast.

\--- / kollaps \---