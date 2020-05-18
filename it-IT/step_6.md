## Cambiare lo spessore della penna

Ora aggiungerai il codice per consentire all'utente del tuo programma di disegnare usando diversi spessori di penna.

--- task ---

Per prima cosa, aggiungi una nuova variabile chiamata `spessore`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

Aggiungi questa riga **dentro** il ciclo `per sempre`{:class="block3control"} del codice dello sprite matita:

```blocks3
when flag clicked
erase all
switch costume to (matita-blu v)
set pen color to [#0035FF]
forever
go to (mouse pointer v)
+set pen size to (spessore :: variables)
if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

--- /task ---

Lo spessore della penna ora viene ripetutamente impostata sul valore della variabile `spessore`{:class="block3variables"}.

--- task ---

Fare clic con il pulsante destro del mouse sulla variabile `spessore`{:class="block3variables"} visualizzata sullo stage e quindi fai clic su **cursore**.

![screenshot](images/paint-slider.png)

--- /task ---

Ora puoi trascinare il cursore che è visibile sotto la variabile per cambiare il suo valore.

![screenshot](images/paint-slider-change.png)

--- task ---

Testa il progetto e vedi se riesci a modificare lo spessore della matita.

![screenshot](images/paint-width-test.png)

--- /task ---