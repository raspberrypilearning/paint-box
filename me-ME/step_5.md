## Greške

Ponekad se dešavaju greške, pa ćemo u tvoj projekat dodati dugme 'obriši' i gumicu.

+ Dodaj lik 'X-block' - naći češ ga u biblioteci (library), u odjeljku Slova (letters). Oboji kostim u crveno. To će biti dugme 'obriši'.

![screenshot](images/paint-x.png)

+ Dodaj kôd ovom liku da očisti pozornicu kada se na njega klikne.

![Clear stage](images/clear-stage.png)

Primijeti da nije potrebno slati poruku za čišćenje pozornice, pošto možeš da koristiš blok očisti (clear) ovog lika.

Vjerovatno primjećuješ da tvoj lik olovke ima kostim gumice:

![screenshot](images/paint-eraser-costume.png)

+ Tvoj projekat takođe ima poseban lik gumice. Right click on this sprite and choose 'show'. Here is how your stage should look:

![screenshot](images/paint-eraser-stage.png)

+ Add code to the eraser sprite, to tell the pencil to switch to an eraser when the sprite is clicked.

![Broadcast eraser](images/broadcast-eraser.png)

When the pencil receives the "eraser" message, you can switch the pencil costume to the eraser, and switch the pencil colour to white - the same colour as the stage!

+ Add some code to create the eraser

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: **When I receive** the **eraser** message **Switch to costume** eraser **Set pen color** to white \--- /hint \--- \--- hint \--- Here is how the code inside the pencil sprite should look:

```blocks
when I receive [eraser v]
switch costume to [eraser v]
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Test your project, to see if you can clear and erase on the stage.

![screenshot](images/paint-erase-test.png)

There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

![screenshot](images/paint-draw-problem.png)

To fix this, tell the pencil only to draw if the mouse is clicked *and* if the y-position of the mouse is greater than -120:

![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

![screenshot](images/paint-fixed.png)