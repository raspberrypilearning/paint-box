## Farbige Stifte

Lass uns Deinem Projekt unterschiedlich farbige Bleistifte hinzufügen und es dem Nutzer so erlauben zwischen Ihnen zu wechseln.

+ Klicke auf Deine Bleistift-Figur, klicke dann auf 'Kostüme' und dupliziere das 'Bleistift-blau'-Kostüm.

	![screenshot](images/paint-blue-duplicate.png)

+ Benenne Dein Kostüm in 'Bleistift-grün' um und füge ihm grün als Farbe hinzu.

	![screenshot](images/paint-pencil-green.png)

+ Erstelle zwei neue Figuren, welche Du benutzen wirst, um eine Farbe auszuwählen.

	![screenshot](images/paint-selectors.png)

+ Wenn das Grün-Auswahl-Symbol angeklickt ist, musst Du der Bleistift-Figur die Nachricht senden (`sende an alle`{:class="blockevents"}), die ihm mitteilt die Bleistiftfarbe in grün umzuwandeln.

Um dies zu tun, füge dem Grün-Auswahl-Symbol diesen Code hinzu:

  ```blocks
      Wenn ich angeklickt werde
      sende [grün v] an alle
  ```
  
Um einen `sende an alle`{:class="blockevents"}-Block zu erstellen, klicke auf den nach unten zeigenden Pfeil und wähle 'Neue Nachricht...' aus.

![screenshot](images/paint-broadcast.png)

Du kannst nun 'grün' eintippen, um Deine neue Nachricht zu erstellen.

![screenshot](images/paint-green-message.png)

+ Du musst Deiner Bleistift-Figur nun mitteilen was zu tu ist, wenn sie diese Nachricht erhält. Füge Deiner Figur diesen Code hinzu:

	```blocks
      Wenn ich [grün v] empfange
      wechsle zu Kostüm [Bleistift-grün v]
      setze Stiftfarbe auf [#00ff00]
	```

Um die Stiftfarbe auf grün zu setzen, klicke die grün gefärbte Box in dem `setze Schriftfarbe auf`{:class="blockpen"}-Block an und klicke anschließend auf das Grün-Auswahl-Symbol.

+ Du kannst nun das Gleiche mit dem blauen Bleistift-Symbol tun, indem Du diesen Code zu der Blau-Auswahl-Figur hinzufügst:

	```blocks
      Wenn ich angeklickt werde
      sende [blau v] an alle
	```

...und indem Du diesen Code zu der Bleistift-Figur hinzufügst:

  ```blocks
      Wenn ich [blau v] empfange
      wechsle zu Kostüm [Bleistift-blau v]
      setze Stiftfarbe auf [#0000ff]
  ```

+ Zuletzt musst Du Deiner Bleistift-Figur sowohl mitteilen, welches Kostüm und welche Stiftfarbe sie wählen soll, als auch den Bildschirm zu leeren, sobald ein neues Projekt begonnen wird. Füge diesen Code an den Anfang des `Wenn die grüne Flagge angeklickt` {:class="blockevents"}-Code des Bleistifts hinzu (vor die `wiederhole fortlaufend`{:class="blockcontrol"}-Schleife):

	```blocks
      wische Malspuren weg
      wechsle zu Kostüm [blau-Bleistift v]
      setze Stiftfarbe auf [#0000ff]
	```

Wenn Du magst, kannst Du auch mit einer anderen Farbe anfangen!

+ Teste Dein Projekt. Kannst Du zwischen dem grünen und dem blauen Stift hin und her wechseln?

	![screenshot](images/paint-pens-test.png)



