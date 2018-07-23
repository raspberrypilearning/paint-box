## Olovke u bojama

Dodajmo u tvoj projekat olovke različitih boja i omogućimo korisniku da izabere onu koju želi.

+ Klikni na lik olovke, zatim klikni na 'Costumes' (Kostimi) i umnoži (duplicate) kostim 'olovka-plava'.

![snimak ekrana](images/paint-blue-duplicate.png)

+ Preimenuj novi kostim u 'olovka-zelena' i oboji olovku u zeleno.

![snimak ekrana](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Nacrtaj dva nova lika - plavi kvadrat i zeleni kvadrat. Koristićeš ih da odabereš plavu ili zelenu olovku.

![snimak ekrana](images/paint-selectors.png)

+ Preimenuj likove i daj im imena 'zelena' i 'plava'.

+ Dodaj kôd liku 'zelena' tako da, kada se klikne na njega, `pošalje`{:class="blockevents"} (broadcast) poruku "zelena" liku olovke, govoreći mu da promijeni svoj kostim i boju.

![Pošalji poruku plava](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Pređi na lik olovke. Dodaj ovom liku kôd tako da, kada primi `poruku`{:class="blockevents"} zelena, pređe na kostim zelene olovke i promijeni boju olovke u zelenu.

![Pošalji poruku zelena](images/broadcast-green.png)

Da bismo postavili da olovka boji zelenom bojom, klikni na obojeno polje u bloku `set pen color`{:class="blockpen"} (postavi boju olovke), a zatim klikni na zeleni lik da izabereš zelenu boju za svoju olovku.

+ Sada možeš da uradiš isto sa ikonom za izbor plave olovke: dodaj ovaj kôd liku plavog kvadrata:

```blocks
when this sprite clicked
broadcast [plava v]
```

...i dodaj sljedeći kôd liku olovke:

```blocks
when I receive [plava v]
switch costume to [olovka-plava v]
set pen color to [#0000ff]
```

+ Na kraju, dodaj sljedeći kôd da kažeš liku olovke sa kojom bojom da započne, kao i da obezbijediš da je ekran očišćen.

![Započni olovku](images/start-pencil.png)

Izabrali smo da započnemo sa plavom bojom, ali možeš da počneš i sa olovkom neke druge boje ako želiš.

+ Isprobaj svoj projekat. Možeš li da zamjenjuješ plavu i zelenu olovku kada klikneš na likove plavog i zelenog kvadrata?

![snimak ekrana](images/paint-pens-test.png)