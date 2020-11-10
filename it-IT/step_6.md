## Cambiare lo spessore della penna

Ora aggiungerai il codice per consentire all'utente del tuo programma di disegnare usando diversi spessori di penna.

\--- task \---

Per prima cosa, aggiungi una nuova variabile chiamata `spessore`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Aggiungi questa riga **dentro** il ciclo `per sempre`{:class="block3control"} del codice dello sprite matita:

```blocks3
quando si clicca sulla bandiera verde
pulisci
passa al costume (matita-blu v)
porta colore penna a [#0035FF]
per sempre 
  raggiungi (puntatore del mouse v)
  + porta dimensione penna a (spessore :: variables)
  se <<mouse down?> e <(y del mouse) > [-120]>> allora 
    penna giù
  altrimenti 
    penna su
  end
end
```

\--- /task \---

Lo spessore della penna ora viene ripetutamente impostata sul valore della variabile `spessore`{:class="block3variables"}.

\--- task \---

Fare clic con il pulsante destro del mouse sulla variabile `spessore`{:class="block3variables"} visualizzata sullo stage e quindi fai clic su **cursore**.

![screenshot](images/paint-slider.png)

\--- /task \---

Ora puoi trascinare il cursore che è visibile sotto la variabile per cambiare il suo valore.

![screenshot](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can change the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---