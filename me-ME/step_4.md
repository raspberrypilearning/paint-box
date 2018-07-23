## Olovke u bojama

Dodajmo u tvoj projekat olovke različitih boja i omogućimo korisniku da izabere onu koju želi.

+ Klikni na lik olovke, zatim klikni na 'Costumes' (Kostimi) i umnoži (duplicate) kostim 'olovka-plava'.

![screenshot](images/paint-blue-duplicate.png)

+ Preimenuj novi kostim u 'olovka-zelena' i oboji olovku u zeleno.

![screenshot](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Nacrtaj dva nova lika - plavi kvadrat i zeleni kvadrat. Koristićeš ih da odabereš plavu ili zelenu olovku.

![screenshot](images/paint-selectors.png)

+ Preimenuj likove i daj im imena 'zelena' i 'plava'.

+ Dodaj kôd liku 'zelena' tako da, kada se klikne na njega, `pošalje`{:class="blockevents"} (broadcast) poruku "zelena" liku olovke, govoreći mu da promijeni svoj kostim i boju.

![Broadcast green](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Pređi na lik olovke. Dodaj ovom liku kôd tako da, kada primi `poruku`{:class="blockevents"} zelena, pređe na kostim zelene olovke i promijeni boju olovke u zelenu.

![Broadcast green](images/broadcast-green.png)

Da bismo postavili da olovka boji zelenom bojom, klikni na obojeno polje u bloku `set pen color`{:class="blockpen"} (postavi boju olovke), a zatim klikni na zeleni lik da izabereš zelenu boju za svoju olovku.

+ You can now do the same for the blue pencil icon: add this code to the blue square sprite:

```blocks
when this sprite clicked
broadcast [blue v]
```

...and add this code to the pencil sprite:

```blocks
when I receive [blue v]
switch costume to [pencil-blue v]
set pen color to [#0000ff]
```

+ Finally, add this code to tell the pencil sprite which colour to start with, and make sure that the screen is clear.

![Start pencil](images/start-pencil.png)

We chose to start with blue but if you prefer, you can start with a different colour pencil.

+ Test out your project. Can you switch between blue and green pens by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png)