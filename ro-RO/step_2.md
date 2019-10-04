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

![creion](images/pencil.png)

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

![creion](images/pencil.png)

```blocks3
când se dă click pe steguleț
la infinit
  mergi la (cursorul mouse-ului v)

+ dacă <butonul mouse-ului e apăsat?> atunci
  stilou jos
  altfel
  stilou sus
sfârșit
```

\--- /task \---

\--- task \--- Testează-ți din nou codul. De data aceasta, deplasează creionul prin Scenă și ține apăsat butonul mouse-ului. Poți desena cu creionul?

![captură de ecran](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: Creionul tău nu desenează cu vârful?

Dacă linia desenată de creionul tău pare să pornească din mijlocul creionului, va trebui să modifici personajul creionului astfel încât vârful său să fie centrul personajului.

Fă click pe personajul creionului, apoi click pe categoria **Costume**.

Deplasează costumul astfel încât vârful creionului să fie **deasupra** centrului.

![Galeria de costume](images/costume-center-annotated.png)

Acum deplasează creionul prin scenă și desenează. Acum creionul ar trebui să deseneze din vârful său.

\--- /collapse \---