## Greške

Ponekad se dešavaju greške, pa ćemo dodati dugme 'obriši' i gumicu.

+ Dodaj lik 'X-block' - naći češ ga u biblioteci (library), u odjeljku Slova (letters). Oboji kostim u crveno. To će biti dugme 'obriši'.

![snimak ekrana](images/paint-x.png)

+ Dodaj kôd ovom liku da očisti pozornicu kada se na njega klikne.

![Čista pozornica](images/clear-stage.png)

Primijeti da nije potrebno slati poruku za čišćenje pozornice, pošto možeš da koristiš blok očisti (clear) ovog lika.

Vjerovatno primjećuješ da tvoj lik olovke ima kostim gumice:

![snimak ekrana](images/paint-eraser-costume.png)

+ Tvoj projekat takođe ima poseban lik gumice. Klikni desnim tasterom miša na njega i izaberi 'show' (prikaži). Tvoja pozornica bi trebalo da izgleda ovako:

![snimak ekrana](images/paint-eraser-stage.png)

+ Dodaj kôd liku gumice koji će olovci reći da se zamijeni sa gumicom kada se klikne na lik.

![Poruka za gumicu](images/broadcast-eraser.png)

Kada olovka dobije poruku "gumica", možeš kostim olovke zamijeniti kostimom gumice, a boju olovke promijeniti u bijelu - boju jednaku boji pozornice!

+ Dodaj kôd za keiranje gumice

\--- hints \--- \--- hint \--- Dodaj kôd liku olovke: **Kada dobijem** (when I receive) poruku **gumica** **Promijeni kostim** (switch to costume) u gumica **Postavi boju olovke** (set pen color) u bijela \--- /hint \--- \--- hint \--- Ovako bi trebalo da izgleda kôd u liku olovke:

```blocks
when I receive [gumica v]
switch costume to [gumica v]
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Isprobaj svoj projekat da provjeriš da li možeš da brišeš na pozornici.

![snimak ekrana](images/paint-erase-test.png)

Postoji još jedan problem sa olovkom - možeš da crtaš bilo gdje na pozornici, uključujući i dio sa ikonama za izbor!

![snimak ekrana](images/paint-draw-problem.png)

Da bismo to popravili, treba da kažeš olovci da crta samo ako se klikne mišem *i* ako je y-pozicija miša veća od -120:

![snimak ekrana](images/pencil-gt-code.png)

+ Isprobaj svoj projekat; sada ne bi trebalo da možeš da crtaš u blizini blokova za izbor.

![snimak ekrana](images/paint-fixed.png)