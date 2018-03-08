## Penne colorate

Aggiungiamo diverse penne colorate al tuo progetto, e permettiamo all'utente di scegliere quella che preferisce!

+ Clicca sullo sprite della matita, clicca 'Costumi' e duplica il tuo costume 'matita-blu'.

	![screenshot](images/paint-blue-duplicate.png)

+ Rinomina il tuo nuovo costume 'matita-verde' e colora la matita verde.

	![screenshot](images/paint-pencil-green.png)

+ Crea due nuovi sprite, che userai per selezionare la matita blu o verde.

	![screenshot](images/paint-selectors.png)

+ Quando l'icona verde è cliccata, dovrai `invia a tutti`  {.blockevents} un messaggio allo sprite della matita, dicendo di cambiare costume e colore di matita.

	Per fare ciò, aggiungi prima questo codice all'icona verde.

	```blocks
		quando si clicca questo sprite
		invia a tutti [verde v]
	```

	Per creare il blocco `invia a tutti` {.blockevents}, clicca la freccia in basso e seleziona 'nuovo messaggio...'.

	![screenshot](images/paint-broadcast.png)

	Puoi dunque digitare 'verde' per creare il tuo nuovo messaggio.

	![screenshot](images/paint-green-message.png)

+ Ora dovrai dire allo sprite della matita cosa fare quando riceve il messaggio. Aggiungi questo codice allo sprite della tua matita:

	```blocks
		quando ricevo [verde v]
		passa al costume [matita-verde v]
		usa penna di colore [#00ff00]
	```

	Per fare in modo che la matita colori verde, clicca la casella colorata nel blocco `imposta colore`  {.blockpen}, e clicca sull'icona verde per scegliere il verde come colore della matita.

+ Ora puoi fare la stessa cosa per l'icona della matita blu, aggiungendo questo codice allo sprite selezionatore blu:

	```blocks
		quando si clicca questo sprite
		invia a tutti [blu v]
	```

	...e aggiungi questo codice allo sprite della tua matita:

	```blocks
		quando ricevo [blu v]
		passa al costume [matita-blu v]
		usa penna di colore [#0000ff]
	```

+ Infine, dovrai dire allo sprite della tua matita quale costume e quale colore di matita scegliere quando il progetto è iniziato, e anche di ripulire la schermata. Aggiungi questo codice all'inizio del codice della matita 'quando si clicca la bandiera' {.blockevents} (prima del loop `per sempre` {.blockcontrol}:

	```blocks
		pulisci
		passa al costume [matita-blu v]
		usa penna di colore [#0000ff]	```

	Se preferisci, puoi iniziare con una matita colorata diversa!

+ Prova il tuo progetto. Puoi intercambiare le penne blu e verde?

	![screenshot](images/paint-pens-test.png)



