## Pravljenje olovke

Počnimo tako što ćemo napraviti olovku koja se može koristiti za crtanje na pozornici.

+ Otvori Scratch projekat 'Paintbox' online na [scratch.mit.edu/projects/239832642/](https://scratch.mit.edu/projects/239832642/#editor){:target="_blank"} ili ga preuzmi sa <http://jumpto.cc/paint-get-me-ME>(https://github.com/raspberrypilearning/paint-box/raw/master/me-ME/resources/PaintBox.sb2), a zatim otvori ako koristiš offline editor.

Vidjećeš likove (sprites) olovke i gumice:

![screenshot](images/paint-starter.png)

+ Dodaj kôd liku olovke da `uvijek`{:class="blockcontrol"} (forever) prati strelicu miša, tako da možeš da crtaš:

```blocks
    when flag clicked
    forever
      go to [mouse pointer v]
    end
```

+ Klikni na zastavicu, a zatim pomjeraj miša po pozornici da isprobaš da li kôd funkcioniše.

Nakon toga, napravimo da tvoja olovka crta samo `ako je`{:class="blockcontrol"} (if) pritisnut taster miša.

+ Dodaj ovaj kôd liku olovke:

![screenshot](images/paint-pencil-draw-code.png)

+ Isprobaj svoj kôd još jednom. Ovog puta pomjeraj olovku po pozornici držeći pritisnut taster miša. Možeš li da crtaš svojom olovkom?

![screenshot](images/paint-draw.png)

--- collapse ---
---
title: Ako imaš probleme...
---
Ako tvoja olovka crta liniju svojom sredinom umjesto vrhom, treba da promijeniš centar kostima (costume center).

![Centar kostima](images/costume-center.png)

Krst za centriranje olovke treba da bude postavljen **malo ispod** vrha olovke, a ne na njenom vrhu.

Izmjene u 'centru kostima' lika neće biti registrovane dok se ne klikne na drugu karticu. Klikni na drugi kostim ili na karticu 'Scripts' (Skripte) da dovršiš svoje izmjene u centru kostima.

--- /collapse ---