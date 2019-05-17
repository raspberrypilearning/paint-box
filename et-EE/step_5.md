## Võta vead tagasi

Mõnikord tekivad vead, lisage nupp „selge” ja kustutusklahv.

\--- ülesanne \--- Lisage 'X-block' sprite raamatukogu kirjadest. Värvige Sprite'i kostüüm punaseks ja tee see veidi väiksemaks. See spriit on nupp "selge".

[[[generic-scratch3-sprite-from-library]]]

![ekraanipilt](images/paint-x.png) \--- / ülesanne \---

\--- ülesanne \--- Lisage kood 'X-block' spritile, et eemaldada etapp, kui sprite klõpsas.

![rist](images/cross.png)

```blocks3
kui see sprite klõpsas
kustuta kõik
```

\--- / ülesanne \---

Et eemaldada etapp, ei pea te kasutama `saatet`{: class = "block3events"}, sest `kustutab kõik`{: class = "block3extensions"}, mida see töö teeb.

Kas sa näed, et pliiatsil on ka kustutuskostüüm?

![ekraanipilt](images/paint-eraser-costume.png)

Teie projektis on ka eraldi kustutuskumm.

\--- ülesanne \--- Paremklõpsake sellel kustutuskummil ja seejärel klõpsake **kuva**. Siin on, kuidas teie etapp peaks nüüd vaatama:

![ekraanipilt](images/paint-eraser-stage.png) \--- / ülesanne \---

\--- ülesanne - Lisa kustutuskummile kood, et saata `'kustutaja' eetris`{: class = "block3events"}, kui kustutuskumm on klõpsatud.

![kustutaja](images/eraser.png)

```blocks3
kui see sprite klõpsas
edastust (kustutaja v)
```

\--- / ülesanne \---

Kui pliiatsitõmme saab "kustutuskummi" sõnumi, peaks see oma kostüümi vahetama kustutajaga ja lülitama pliiatsi värvi valgeks, mis on sama värvi kui laval!

\--- task \--- Lisa kustutuskoodi loomiseks mõni kood.

\--- hints \--- \--- vihje \--- Lisage pliiatsile mõni kood: `Kui ma saan`{: class = "block3events"}, siis `kustutaja`{: class = "block3events"} teade `Lülita kostüümide kustutusseadmesse`{: class = "block3looks"} `Seadista pliiatsivärv`{: class = "block3extensions"} kuni valge \--- / vihje \--- \--- vihje \--- Siin on kõik vajalikud plokid:

```blocks3
määrake pliiatsivärviks [#FFFFFF]
kui ma saan [kustutaja v]

lüliti kostüümi (kustutaja v)
```

\--- / vihje \--- \--- vihje \--- Siin näeb kood välja nagu: ![pliiats](images/pencil.png)

```blocks3
kui ma saan [kustutaja v]
lüliti kostüümi (kustutaja v)
seadke pliiatsivärviks [#FFFFFF]
```

\--- / vihje \--- \--- / hints \--- \--- / ülesanne \---

\--- task \--- Testige oma projekti, et näha, kas saate kustutada pliiatsiliinid ja kustutada pliiatsiliinid.

![ekraanipilt](images/paint-erase-test.png) \--- / ülesanne \---

Pliiatsiga on veel üks probleem: sa saad joonistada kõikjal laval, sealhulgas nuppude "selge" ja kustutuskoha lähedal!

![ekraanipilt](images/paint-draw-problem.png)

\--- ülesanne \--- Selle parandamiseks koodi muuta nii, et pliiats on ainult alla, kui hiir on klõpsatud **ja** `y` positsiooni hiirekursori on suurem kui `-120`:

![pliiats](images/pencil.png)

```blocks3
kui lipu klõpsamine
kustutab kõik
lüliti kostüümi (pliiats-sinine v)
määrake pliiatsivärviks [# 0035FF]
igavesti
  minema (hiirekursor v)
+, kui <<mouse down?> ja <(hiir y) > [-120]>> seejärel 
  pensüstelit alla
  muu
  pliiatsi
otsa
```

\--- / ülesanne \---

\--- task \--- Testige oma projekti. Teil ei tohiks nüüd olla võimalik nuppude lähedal.

![ekraanipilt](images/paint-fixed.png) \--- / ülesanne \---