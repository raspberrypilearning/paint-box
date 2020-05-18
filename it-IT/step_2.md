## Di cosa avrai bisogno

Inizia creando la matita necessaria per disegnare sullo stage.

--- task ---

Aprire il progetto bozza di Scratch 'Paint box'.

**Online**: apri il progetto bozza su [scratch.mit.edu/projects/396614712](https://scratch.mit.edu/projects/396614712){:target="_blank"}

Se hai un account su Scratch, puoi farne una copia cliccando su **Remix**.

**Offline**: apri il [progetto bozza](http://rpf.io/p/it-IT/paint-box-go){:target="_blank"} nell'editor offline.

Se hai bisogno di scaricare ed installare l'editor Scratch offline, puoi trovarlo su [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

Nel progetto iniziale, dovresti vedere gli sprite di gomma e matita:

![screenshot](images/paint-starter.png)

--- /task ---

--- task ---

Aggiungi l'estensione Penna al tuo progetto.

[[[generic-scratch3-add-pen-extension]]]

--- /task ---

--- task ---

Aggiungi del codice allo sprite matita per far sì che segua il puntatore del mouse `per sempre`{:class="block3control"} e riesca a disegnare:

![matita](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

--- /task ---

--- task ---

Fai click sulla bandierina e muovi il mouse sullo stage per verificare che il codice funzioni.

--- /task ---

Ora facciamo in modo che la matita disegni solo `se`{:class="blockcontrol"} il mouse è stato cliccato.

--- task ---

Aggiungi questo codice allo sprite della tua matita:

![matita](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
+ if <mouse down?> then
  pen down
  else
  pen up
end
```

--- /task ---

--- task ---

Prova di nuovo il tuo codice. Questa volta, muovi la matita sul quadro tenendo premuto il tasto sinistro del mouse. Riesci a disegnare con la tua matita?

![screenshot](images/paint-draw.png)

--- /task ---

--- collapse ---
---
title: la tua matita non scrive dalla sua punta?
---
Se la linea che disegna la tua matita sembra provenire dal suo centro, devi modificare lo sprite in modo che la punta sia il il suo centro.

Fai clic sullo sprite matita e poi sulla scheda **Costumi**.

Sposta il costume in modo che la punta della matita sia ** appena sopra ** il centro.

![Centro del costume](images/costume-center-annotated.png)

Ora sposta la matita sullo stage e disegna. La matita dovrebbe ora tracciare una linea dalla sua punta.

--- /collapse ---