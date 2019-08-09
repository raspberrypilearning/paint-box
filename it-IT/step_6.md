## Cambia la larghezza della penna

Quindi aggiungerai il codice per consentire alla persona che usa il tuo programma di disegnare cose con diverse larghezze di penna.

\--- task \--- prima cosa, aggiungi una nuova variabile chiamata `width`{: class = "block3variables"}.

[[[generic-scratch3-add-variable]]] \--- / compito \---

\--- task \--- Aggiungi questa riga **dentro** the `forever`{: class = "block3control"} ciclo del codice dello sprite della matita:

```blocks3
quando il flag ha fatto clic su
cancella tutto il costume di
switch su (matita-blu v)
imposta il colore della penna su [# 0035FF]
per sempre
vai a (puntatore del mouse v)
+ imposta la dimensione della penna su (larghezza :: variabili)
se <<mouse down?> e <(mouse y) > [-120]>> quindi 
  penna giù
  altrimenti
  penna su
fine
```

\--- /task \---

La larghezza della penna ora viene ripetutamente impostata sul valore della variabile `width`{: class = "block3variables"}.

\--- task \--- Fare clic con il pulsante destro del mouse sulla variabile `width`{: class = "block3variables"} visualizzata sullo stage, quindi fare clic su **slider**.

![schermata](images/paint-slider.png) \--- /task \---

Ora puoi trascinare il cursore che è visibile sotto la variabile per cambiare il valore della variabile.

![screenshot](images/paint-slider-change.png)

\--- task \--- Testare il progetto e vedere se è possibile aggiungere codice per regolare la larghezza della penna.

![screenshot](images/paint-width-test.png) \--- /task \---