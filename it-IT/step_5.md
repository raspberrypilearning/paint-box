## Fare errori

A volte capita di sbagliare, quindi aggiungi un pulsante "pulisci tutto" e un pulsante gomma.

--- task ---

Aggiungi lo sprite 'X-block' dalla sezione delle lettere della libreria. Colora il costume dello sprite in rosso e rimpiccioliscilo un po'. Questo sprite è il pulsante "pulisci tutto".

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png)

--- /task ---

--- task ---

Aggiungi il codice allo sprite 'X-block' per cancellare completamente lo stage quando lo si clicca.

![croce](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

--- /task ---

Non è necessario `inviare un messaggio`{:class="block3events"} per cancellare lo stage, perché il comando `pulisci`{:class="block3extensions"} svolge già questa funzione.

Hai visto che lo sprite matita include un costume "gomma"?

![screenshot](images/paint-eraser-costume.png)

Il tuo progetto include anche uno sprite per selezionare la gomma.

--- task ---

Fare clic con il tasto sinistro sul costrume "gomma" per **visualizzarlo** nello stage. Il tuo stage dovrebbe apparire così:

![screenshot](images/paint-eraser-stage.png)

--- /task ---

--- task ---

Aggiungi il codice allo sprite gomma per inviare un `messaggio "gomma"`{:class="block3events"} quando si fa clic sullo sprite della gomma.

![gomma per cancellare](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (gomma v)
```

--- /task ---

Quando lo sprite della matita riceverà il messaggio "gomma", passerà al costume "gomma" e cambiarà il colore della penna in bianco, che è lo stesso colore dello stage!

--- task ---

Aggiungi del codice per creare la gomma.

--- hints --- --- hint ---

Aggiungi del codice allo sprite matita: `Quando ricevo`{:class="block3events"} il messaggio `gomma`{:class="block3events"} `Passa al costume gomma`{:class="block3looks"} `Porta colore penna a`{:class="block3extensions"} bianco

--- /hint --- --- hint ---

Ecco tutti i blocchi di codice che ti serviranno:

```blocks3
set pen color to [#FFFFFF]
when I receive [gomma v]

switch costume to (gomma v)
```

--- /hint --- --- hint ---

Ecco come dovrebbe apparire il risultato:

![matita](images/pencil.png)

```blocks3
when I receive [gomma v]
switch costume to (gomma v)
set pen color to [#FFFFFF]
```

--- /hint --- --- /hints --- --- /task ---

--- task ---

Metti alla prova il tuo progetto per vedere se è possibile ripulire lo stage e cancellare i tratti lasciati dalla matita.

![schermata](images/paint-erase-test.png)

--- /task ---

C’è ancora un problema con la matita: puoi disegnare dappertutto sul quadro, anche vicino ai pulsanti per pulire ad alla gomma!

![screenshot](images/paint-draw-problem.png)

--- task ---

Per sistemare il difetto, modifica il codice in modo che la penna sia abbassata solo se si fa clic con il mouse **e** la posizione `y` del puntatore del mouse è maggiore di `-120`:

![matita](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (matita-blu v)
set pen color to [#0035FF]
forever
  go to (mouse pointer v)
+if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

--- /task ---

--- task ---

Prova il tuo progetto. Ora non dovresti essere in grado di disegnare vicino ai pulsanti.

![screenshot](images/paint-fixed.png)

--- /task ---