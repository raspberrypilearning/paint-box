## Matite colorate

Ora aggiungerai al tuo progetto matite di diversi colori e consentirai all'utente di sceglierne una.

--- task ---

Rinomina lo sprite `matita` in `matita-blu`

![rinomina-matita](images/rename-pencil.png)

--- /task ---

--- task ---

Fai clic con il tasto destro del mouse sullo sprite della matita e duplica il costume "matita-blu".

![screenshot](images/paint-blu-duplicate.png)

--- /task ---

--- task ---

Riomina il nuovo costume 'matita-verde' e colora la matita di verde.

![screenshot](images/paint-matita-verde.png)

--- /task ---

--- task ---

Crea due nuovi sprite: un quadrato blu e un quadrato verde. Questi sono per scegliere tra la matita blu e verde.

![screenshot](images/paint-selectors.png)

--- /task ---

--- task ---

Rinominare i nuovi sprite in modo che si chiamino 'blu' e 'verde'

[[[generic-scratch3-rename-sprite]]]

--- /task ---

--- task ---

Aggiungi un po' di codice allo sprite "verde" in modo che, quando questo sprite viene cliccato, `invii il messaggio`{:class="block3events"} "verde".

![quadrato verde](images/green_square.png)

```blocks3
when this sprite clicked
broadcast (verde v)
```

[[[generic-scratch3-broadcast-message]]]

--- /task ---

Lo sprite della matita dovrebbe sentire il messaggio "verde" e cambiare il proprio costume e colore in risposta.

--- task ---

Cambia sprite. Aggiungi del codice in modo che, quando questo sprite riceve il messaggio `verde`{:class="block3events"}, passi al costume della matita verde e cambi il colore della penna in verde.

![matita](images/pencil.png)

```blocks3
when I receive [verde v]
switch costume to (matita-verde v)
set pen color to [#00CC44]
```

Per impostare la matita da colorare in verde, fai clic sul quadratino colorato nel blocco `porta colore penna a`{:class="block3extensions"}, quindi fai clic sullo sprite quadrato verde.

--- /task ---

Quindi procedi in modo simile per cambiare il colore della matita in blu.

--- task ---

Clicca sullo sprite quadrato blu e aggiungi questo codice:

![quadrato_blu](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blu v)
```

Quindi fare clic sullo sprite matita e aggiungere questo codice:

![matita](images/pencil.png)

```blocks3
when I receive [blu v]
switch costume to (matita-blu v)
set pen color to [#0000ff]
```

--- /task ---

--- task ---

Infine, aggiungi questo codice per dire allo sprite della matita con quale colore iniziare e per assicurarti che lo schermo sia pulito all'avvio del programma.

![matita](images/pencil.png)

```blocks3
when flag clicked
+erase all
+switch costume to (matita-blu v)
+set pen color to [#0035FF]
forever
  go to (mouse pointer v)
if <mouse down?> then
  pen down
  else
  pen up
end
```

--- /task ---

Se preferisci, puoi iniziare con una matita di colore diverso.

--- task ---

Prova di nuovo il tuo codice. Riesci a cambiare colore alla matita facendo clic sugli sprite quadrato blu o verde?

![schermata](images/paint-pens-test.png)

--- /task ---