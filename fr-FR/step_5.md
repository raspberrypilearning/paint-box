## Annule les erreurs

Parfois, des erreurs se produisent, alors ajoute un bouton "effacer" et un bouton gomme.

--- task --- Ajoute le sprite "Bloc-X" à partir de la section des lettres de la bibliothèque. Colorie le costume du sprite en rouge et rend-le un peu plus petit. Ce sprite est le bouton "effacer".

[[[generic-scratch3-sprite-from-library]]]

![capture d'écran](images/paint-x.png) --- /task ---

--- task --- Ajoute du code au sprite "Bloc-X" pour effacer la scène lorsque tu as cliqué sur le sprite.

![traverser](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

--- /task ---

Tu n'as pas besoin d'utiliser un `envoi à tous`{:class="block3events"} pour effacer la scène, car le bloc `effacer tout`{:class="block3extensions"} fait déjà cette action.

Vois-tu que le sprite crayon comprend un costume gomme?

![capture d'écran](images/paint-eraser-costume.png)

Ton projet comprend également un sprite gomme séparé.

--- task --- Fait un clic droit sur ce sprite gomme, et ensuite clique sur **afficher**. Voici à quoi devrait ressembler ta scène:

![capture d'écran](images/paint-eraser-stage.png) --- /task ---

--- task --- Ajoute du code au sprite gomme pour envoyer un `un envoi à tous "gomme"`{:class="block3events"} lorsque le sprite gomme est cliqué.

![gomme](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (gomme v)
```

--- /task ---

Lorsque le sprite crayon reçoit le message "gomme", il devrait changer son costume en gomme et changer la couleur du crayon en blanc, qui est la même couleur que la scène!

--- task --- Ajoute du code pour créer la gomme.

--- hints ---
 --- hint --- Ajoute du code au sprite crayon: `quand je reçois`{:class="block3events"} le message `gomme`{:class="block3events"} `basculer sur le costume gomme`{:class="block3looks"} `mettre la couleur du stylo`{:class="block3extensions"} sur blanc
--- /hint ---
 --- hint --- Voici tous les blocs dont tu as besoin:

```blocks3
set pen color to [#FFFFFF]
when I receive  [gomme v]

switch costume to (gomme v)
```

--- /hint --- --- hint --- Voici à quoi devrait ressembler le code: ![crayon](images/pencil.png)

```blocks3
when I receive [gomme v]
switch costume to (gomme v)
set pen color to [#FFFFFF]
```

--- /hint ------ /hints --- --- /task ---

--- task --- Teste ton projet pour voir si tu peux effacer la scène et effacer les lignes au crayon.

![capture d'écran](images/paint-erase-test.png) --- /task ---

Il y a encore un problème avec le crayon: tu peux dessiner n’importe où sur la scène, y compris près des boutons "effacer" et gomme!

![capture d'écran](images/paint-draw-problem.png)

--- task --- Pour résoudre ce problème, modifie le code afin que le stylo soit en position d'écriture uniquement si tu cliques sur la souris **et** que la position `y` du pointeur de la souris est supérieure à `-120`:

![crayon](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
  go to (pointeur de la souris v)
+if <<mouse down?> and <(souris y) > [-120]>> then 
  pen down
  else
  pen up
end
```

--- /task ---

--- task --- Teste ton projet. Tu ne devrais plus pouvoir dessiner près des boutons.

![capture d'écran](images/paint-fixed.png) --- /task ---
