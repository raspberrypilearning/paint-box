## Réparer les erreurs

Parfois, des erreurs se produisent, alors ajoutons un bouton "effacer" et une gomme.

+ Ajoutez le luttin 'X-block' - vous le trouverez dans la bibliothèque, dans la catégorie "Lettres". Colorez le costume en rouge. Cela deviendra le bouton "effacer".

![capture d'écran](images/paint-x.png)

+ Ajoutez du code à ce lutin pour effacer la scène lorsqu'il est cliqué.

![Effacer la scène](images/clear-stage.png)

Notez que vous n'avez pas besoin d'envoyer un message pour effacer la scène, vous pouvez simplement utiliser le bloc "effacer tout" de ce lutin.

Vous avez probablement remarqué que votre lutin crayon comprend un costume de gomme :

![capture d'écran](images/paint-eraser-costume.png)

+ Votre projet comprend également un lutin gomme distinct. Faites un clic droit sur ce lutin et choisissez "Montrer". Voici à quoi votre scène devrait ressembler :

![capture d'écran](images/paint-eraser-stage.png)

+ Ajoutez du code au lutin de la gomme, pour indiquer au crayon de passer au costume gomme lorsque le lutin gomme est cliqué.

![Broadcast eraser](images/broadcast-eraser.png)

Lorsque le crayon reçoit le message "gomme", vous pouvez passer du costume crayon au costume gomme, et passer la couleur de crayon à blanc - la même couleur que la scène !

+ Ajoutez du code pour créer la gomme

\--- hints \--- \--- hint \--- Ajoutons un peu de code au lutin crayon : **Quand je reçois ** **gomme** **Basculer sur le costume** gomme **Mettre la couleur du stylo à** blanc \--- /hint \--- \--- hint \--- Voici à quoi devrait ressembler le code du lutin crayon :

```blocks
quand je reçois [gomme v]
basculer sur le costume [gomme v]
mettre la couleur du stylo à [#ffffff]
```

\--- /hint \--- \--- /hints \---

+ Testez votre projet, pour voir si vous pouvez gommer sur la scène et même effacer toute la scène.

![screenshot](images/paint-erase-test.png)

Il y a encore un problème avec le crayon - vous pouvez dessiner n'importe où sur la scène, y compris près des lutins de sélection !

![screenshot](images/paint-draw-problem.png)

Pour résoudre ce problème, dites au crayon de ne dessiner que si vous cliquez sur la souris * et * si la position y de la souris est supérieure à -120 :

![screenshot](images/pencil-gt-code.png)

+ Testez votre projet ; vous ne devriez plus être en mesure de vous rapprocher des lutins de sélection.

![screenshot](images/paint-fixed.png)