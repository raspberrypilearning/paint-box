## Matite colorate

Ora aggiungi al tuo progetto diverse matite colorate e consenti all'utente di scegliere tra loro.

\--- task \--- Rinominare la `matita` sprite in `pencil-blue`

![rinomina-matita](images/rename-pencil.png) \--- /task \---

\--- task \--- Fai clic con il tasto destro del mouse sullo sprite della matita e duplica il costume "blue matita".

![schermata](images/paint-blue-duplicate.png) \--- /task \---

\--- compito \--- Nomina il nuovo costume 'matita-verde', e colora la matita verde.

![schermata](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- Disegna due nuovi sprite: un quadrato blu e uno quadrato verde. Questi sono per la scelta tra la matita blu e verde.

![schermata](images/paint-selectors.png) \--- /task \---

\--- task \--- Rinominare i nuovi sprite in modo che vengano chiamati 'blue' e 'green'

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- \--- compito Aggiungere un po 'di codice per lo sprite 'verde' in modo che quando questo sprite viene cliccato, `trasmissioni`{: class = "block3events"} il messaggio "verde".

![quadrato verde](images/green_square.png)

```blocks3
quando questo sprite ha fatto clic su
broadcast (verde v)
```

[[[generic-scratch3-broadcast-message]]] \--- / compito \---

Lo sprite della matita dovrebbe ascoltare il messaggio "verde" e cambiare il suo costume e il colore della matita in risposta.

\--- compito \--- Passa al tuo sprite matita. Aggiungi del codice in modo che quando questo sprite riceve la trasmissione `verde`{: class = "block3events"}, passa al costume della matita verde e cambia il colore della penna in verde.

![matita](images/pencil.png)

```blocks3
quando ricevo [verde v]
passa costume a (matita-verde v)
imposta colore penna a [# 00CC44]
```

Per impostare la matita da colorare in verde, fai clic sul quadratino colorato nel blocco `set penna colore`{: class = "block3extensions"}, quindi fai clic sullo sprite quadrato verde. \--- /task \---

Quindi a una cosa simile in modo da poter cambiare il colore della matita in blu.

\--- compito \--- Clicca sullo sprite quadrato blu e aggiungi questo codice:

![quadrato_blu](images/blue_square.png)

```blocks3
quando questo sprite ha fatto clic su
broadcast (blu v)
```

Quindi fare clic sullo sprite matita e aggiungere questo codice: ![matita](images/pencil.png)

```blocks3
quando ricevo [blu v]
passa costume a (matita-blu v)
imposta colore penna a [# 0000ff]
```

\--- /task \---

\--- task \--- Infine, aggiungi questo codice per dire allo sprite della matita di quale colore iniziare e per assicurarti che lo schermo sia chiaro all'avvio del programma.

![matita](images/pencil.png)

```blocks3
when flag clicked
+erase all
+switch costume to (pencil-blue v)
+set pen color to [#0035FF]
forever
  go to (mouse pointer v)
if <mouse down?> then
  pen down
  else
  pen up
end
```

\--- /task \---

Se preferisci, puoi iniziare con una matita di colore diverso.

\--- task \--- Verifica il tuo codice. Riesci a passare tra i colori della matita blu e verde facendo clic sugli sprite quadrati blu o verdi?

![schermata](images/paint-pens-test.png) \--- /task \---