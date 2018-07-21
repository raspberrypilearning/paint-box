## Pravljenje olovke

Počnimo tako što ćemo napraviti olovku koja se može koristiti za crtanje na pozornici.

+ Otvori online Scratch projekat 'Paintbox' na [jumpto.cc/paint-go](http://jumpto.cc/paint-go){:target="_blank"} ili ga preuzmi sa <http://jumpto.cc/paint-get>{:target="_blank"}, a zatim otvori ako koristiš offline editor.

Vidjećeš likove (sprites) olovke i gumice:

![screenshot](images/paint-starter.png)

+ Dodaj kôd liku olovke da napraviš da `uvijek`{:class="blockcontrol"} (forever) prati strelicu miša, tako da možeš da crtaš:

```blocks
    when flag clicked
    forever
      go to [mouse pointer v]
    end
```

+ Klikni na zastavicu, a zatim pomjeraj miša po pozornici da isprobaš da li kôd funkcioniše.

Nakon toga, napravimo da tvoja olovka crta `ako je`{:class="blockcontrol"} (if) pritisnut taster miša.

+ Dodaj ovaj kôd liku olovke:

![screenshot](images/paint-pencil-draw-code.png)

+ Isprobaj svoj kôd još jednom. Ovog puta pomjeraj olovku po pozornici držeći pritisnut taster miša. Možeš li da crtaš svojom olovkom?

![screenshot](images/paint-draw.png)

## \--- collapse \---

## title: Ako imaš problema...

Ako tvoja olovka crta liniju od sredine olovke umjesto vrhom, treba da promijeniš centar svog kostima.

![Costume center](images/costume-center.png)

Krstić za olovku treba da bude postavljen **tačno ispod** vrha olovke, a ne na vrhu olovke.

A changes in a sprite's 'costume center' isn't registered until another tab is clicked, so click on another costume, or on the 'Scripts' tab to finalise your changes to the costume center.

\--- /collapse \---