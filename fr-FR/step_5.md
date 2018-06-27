## Réparer les erreurs

Parfois, des erreurs se produisent, alors ajoutons un bouton "effacer" et une gomme.

+ Ajoutez le luttin 'X-block' - vous le trouverez dans la bibliothèque, dans la catégorie "Lettres". Colorez le costume en rouge. Cela deviendra le bouton "effacer".

![screenshot](images/paint-x.png)

+ Ajoutez du code à ce lutin pour effacer la scène lorsqu'il est cliqué.

![Clear stage](images/clear-stage.png)

Notez que vous n'avez pas besoin d'envoyer un message pour effacer la scène, vous pouvez simplement utiliser le bloc "effacer tout" de ce lutin.

Vous avez probablement remarqué que votre lutin crayon comprend un costume de gomme :

![screenshot](images/paint-eraser-costume.png)

+ Votre projet comprend également un lutin gomme distinct. Faites un clic droit sur ce lutin et choisissez "Montrer". Voici à quoi votre scène devrait ressembler :

![screenshot](images/paint-eraser-stage.png)

+ Ajoutez du code au lutin de la gomme, pour indiquer au crayon de passer au costume gomme lorsque le lutin gomme est cliqué.

![Broadcast eraser](images/broadcast-eraser.png)

Lorsque le crayon reçoit le message "gomme", vous pouvez passer du costume crayon au costume gomme, et passer la couleur de crayon à blanc - la même couleur que la scène !

+ Add some code to create the eraser

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: **When I receive** the **eraser** message **Switch to costume** eraser **Set pen color** to white \--- /hint \--- \--- hint \--- Here is how the code inside the pencil sprite should look:

```blocks
when I receive [eraser v]
switch costume to [eraser v]
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Test your project, to see if you can clear and erase on the stage.

![screenshot](images/paint-erase-test.png)

There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

![screenshot](images/paint-draw-problem.png)

To fix this, tell the pencil only to draw if the mouse is clicked *and* if the y-position of the mouse is greater than -120:

![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

![screenshot](images/paint-fixed.png)