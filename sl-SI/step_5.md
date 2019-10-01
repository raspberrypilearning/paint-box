## Razveljavitev napak

Včasih pride do napak, zato dodaj gumb »počisti« in gumb za radirko.

\--- task \--- Dodaj figuro 'X-block', ki se nahaja v razdelku Črke iz knjižnice figur. Premineuj to figuro v 'blok x', pobarvaj jo rdeče in jo malo zmanjšaj. To bo gumb, ki 'počisti' risalno površino.

[[[generic-scratch3-sprite-from-library]]]

![posnetek zaslona](images/paint-x.png) \--- /task \---

\--- task \--- Figuri 'blok x' dodaj kodo, ki izbriše vse na odru, kadar kliknemo na njo.

![križ](images/cross.png)

```blocks3
ko kliknemo to figuro
izbriši vse
```

\--- /task \---

Za čiščenje odra ti ni potrebno `objaviti`{: class = "block3events"} sporočila, ker že `izbriši vse`{: class = "block3extensions"} blok opravi to delo.

Si opazil, da figura svinčnika vsebuje tudi videz radirke?

![posnetek zaslona](images/paint-eraser-costume.png)

Tvoj projekt vsebuje tudi ločeno figuro radirke.

\--- task \--- Klikni na figuro radirke in jo prikaži s klikom na **oko** v panoju za urejanje podatkov o figuri. Tukaj lahko vidite, kako naj bo vaš oder videti zdaj:

![posnetek zaslona](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Figuri radirke dodaj kodo, ki `objavi 'radirka'`{:class="block3events"}, kadar kliknemo na figuro radirke.

![radirka](images/eraser.png)

```blocks3
ko kliknemo to figuro
objavi (radirka v)
```

\--- /task \---

Ko figura svinčnika prejme objavljeno sporočilo "radirka", mora preklopiti svoj videz na radirko in preklopiti barvo peresa na belo, kar je barva odra!

\--- task \--- Dodaj kodo, ki ustvari radirko.

\--- hints \--- \--- hint \--- Dodaj nekaj kode figuri svnčnika: `Ko prejme`{:class="block3events"} sporočilo `radirka`{:class="block3events"} `Zamenja videz na radirko`{:class="block3looks"} `Nastavi barvo peresa`{:class="block3extensions"} na belo \--- /hint \--- \--- hint \--- Tu so vsi potrebni bloki:

```blocks3
nastavi barvo peresa na [#FFFFFF]
ko prejmem [radirka v]

zamenjaj videz na (radirka v)
```

\--- /hint \--- \--- hint \--- Tvoja koda bi morala izgledati tako: ![svinčnik](images/pencil.png)

```blocks3
ko prejmem [radirka v]
zamenjaj videz na (radirka v)
nastavi barvo peresa na [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Preizkusi projekt, da vidiš, če lahko počistiš oder in izbrišeš črte svinčnika.

![posnetek zaslona](images/paint-erase-test.png) \--- /task \---

Svinčnik ima še eno težavo: Z njim lahko rišeš kjerkoli po odru, vključno po tistem delu, kjer se nahajata gumba 'radirka' in 'počisti'!

![posnetek zaslona](images/paint-draw-problem.png)

\--- task \--- Da bi to popravil, spremeni kodo na tak način, da je pero spuščeno le kadar je tipka miške pritisnjena **in** je `y` pozicija kazalca miške večji od `-120`:

![svinčnik](images/pencil.png)

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

\--- task \--- Preizkusi svoj projekt. Zdaj bi moralo biti onemogočeno, da bi risal blizu gumbov.

![posnetek zaslona](images/paint-fixed.png) \--- /task \---