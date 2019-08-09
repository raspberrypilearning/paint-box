## Fare errori

A volte capita di sbagliare, quindi aggiungi un pulsante 'cancella' e un pulsante gomma.

\--- task \--- Aggiungi lo sprite 'X-block' dalla sezione delle lettere della libreria. Colora il costume dello sprite in rosso e rendilo un po' più piccolo. Questo sprite è il pulsante 'cancella'.

[[[generic-scratch3-sprite-from-library]]]

![schermata](images/paint-x.png) \--- /task \---

\--- task \--- Aggiungi il codice allo sprite 'X-block' per cancellare il quadro quando si fa clic sullo sprite.

![attraversare](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- /task \---

Non è necessario utilizzare una `trasmissione`{: class = "block3events"} per cancellare il quadro, perché il `cancella tutto il blocco`{: class = "block3extensions"} svolge già questa funzione.

Vedi che lo sprite matita include un costume da cancellare?

![screenshot](images/paint-eraser-costume.png)

Il tuo progetto include anche uno sprite per selezionare la gomma.

\--- task \--- Fare clic con il tasto destro su questo sprite della gomma e quindi fare clic su **show**. Il tuo quadro dovrebbe apparire così:

![schermata](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Aggiungi il codice allo sprite della gomma per inviare una `trasmissione 'gomma'`{: class = "block3events"} quando si fa clic sullo sprite della gomma.

![gomma per cancellare](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

\--- /task \---

Quando lo sprite della matita riceve il messaggio 'eraser', dovrebbe passare al costume gomma e cambiare il colore della penna in bianco, che è dello stesso colore del quadro!

\--- task \--- Aggiungi del codice per creare la gomma.

\--- suggerimenti \--- \--- suggerimento \--- Aggiungi un codice allo sprite matita: `Quando ricevo`{: class = "block3events"} il `eraser`{: class = "block3events"} messaggio `Passa a gomma da cancellare`{: class = "block3looks"} `Imposta colore penna`{: class = "block3extensions"} a bianco \--- / suggerimento \--- \--- suggerimento \--- Ecco tutti i blocchi che ti servono:

```blocks3
imposta il colore della penna a [#FFFFFF]
quando ricevo [eraser v]

cambia costume in (gomma v)
```

\--- / suggerimento \--- \--- suggerimento \--- Ecco come dovrebbe apparire il codice: ![matita](images/pencil.png)

```blocks3
quando ricevo [eraser v]
passa costume a (gomma v)
imposta colore penna a [#FFFFFF]
```

\--- / suggerimento \--- \--- / suggerimenti \--- \--- / compito \---

\--- task \--- Metti alla prova il tuo progetto per vedere se è possibile ripulire il quadro e cancellare le linee di matita.

![screenshot](images/paint-erase-test.png) \--- /task \---

C’è ancora un problema con la matita: puoi disegnare dappertutto sul quadro, anche vicino alle icone selezionatrici!

![screenshot](images/paint-draw-problem.png)

\--- task \--- Per risolvere il tutto, modifica il codice in modo che la penna sia abbassata solo se si fa clic con il mouse **e** la posizione `y` del puntatore del mouse è maggiore di `-120`:

![matita](images/pencil.png)

```blocks3
quando si fa clic sul flag
cancella tutto
passa al costume (matita-blu v)
imposta il colore della penna su [# 0035FF]
per sempre
  vai a (puntatore del mouse v)
+ se <<mouse down?> e <(mouse y) > [-120]>> quindi 
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \--- Metti alla prova il tuo progetto. Ora non dovresti essere in grado di disegnare accanto ai pulsanti.

![schermata](images/paint-fixed.png) \--- /task \---