## Muutke pliiatsi laiust

Järgmisena lisate koodi, mis võimaldab teie programmi kasutaval isikul joonistada asju erinevate pliiatsi laiustega.

\--- ülesanne \--- Esmalt lisage uus muutuja nimega `width`{: class = "block3variables"}.

[[[generic-scratch3-add-variable]]] \--- / ülesanne \---

\--- ülesande \--- Lisage see liin **sees** `igavesti`{: class = "block3control"} lingu pliiatsi sprite koodis:

```blocks3
kui lipu klõpsamine
kustutab kõik
lüliti kostüümi (pliiats-sinine v)
seadke pliiatsivärviks [# 0035FF]
igavesti
minge (hiirekursor v)
+ seadke pliiatsi suurus (laius :: muutujad)
kui <<mouse down?> ja <(hiir y) > [-120]>> siis 
  pensüstelit alla
  teist
  pensüstelit kuni
otsa
```

\--- / ülesanne \---

Pliiasi laius on nüüd korduvalt seatud `muutuja`{: class = "block3variables" väärtusele.

\--- ülesanne \--- Paremklikkige laval `laius`{: class = "block3variables"}, mis on kuvatud laval, ja seejärel klõpsake **liugurit**.

![ekraanipilt](images/paint-slider.png) \--- / ülesanne \---

Muutuja väärtuse muutmiseks saate nüüd muuta muutuja all nähtavat liugurit.

![ekraanipilt](images/paint-slider-change.png)

\--- ülesanne - Testige oma projekti ja vaadake, kas saate lisada pliiatsi laiuse reguleerimiseks koodi.

![ekraanipilt](images/paint-width-test.png) \--- / ülesanne \---