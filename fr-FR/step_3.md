## Crayons de couleurs

Tu vas maintenant ajouter des crayons de couleurs différents à ton projet et permettre à l'utilisateur de les choisir.

\--- task \--- Renomme le costume `crayon` en `crayon bleu`

![renommer-crayon](images/rename-pencil.png) \--- /task \---

\--- task \--- Fait un clic droit sur le sprite crayon et duplique le costume "crayon bleu".

![capture d'écran](images/paint-blue-duplicate.png) \--- /task \---

\--- task \--- Nomme le nouveau costume 'crayon-vert' et colorie le crayon en vert.

![capture d'écran](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- Dessine deux nouveaux sprites: un carré bleu et un carré vert. Ceux-ci sont pour choisir entre le crayon bleu et vert.

![capture d'écran](images/paint-selectors.png) \--- /task \---

\--- task \--- Renomme les nouveaux sprites pour qu'ils s'appellent 'bleu' et 'vert'

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- Ajoute du code au sprite 'vert' afin que, lorsque ce sprite est cliqué, il `diffuse`{:class="block3events"} le message "vert".

![carré vert](images/green_square.png)

```blocks3
quand ce sprite est cliqué 
envoyer à tous (vert v)
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

Le sprite crayon devrait écouter le message "vert" et modifier son costume et sa couleur de crayon en réponse.

\--- task \--- Bascule vers ton sprite crayon. Ajoute du code de sorte que lorsque ce sprite reçoit la diffusion `vert`{:class="block3events"}, il passe au costume de crayon vert et change la couleur du stylo en vert.

![crayon](images/pencil.png)

```blocks3
quand je reçois [vert v]
basculer sur le costume (crayon-vert v)
mettre la couleur du stylo à [#00CC44]
```

Pour permettre au crayon de colorier en vert, clique sur le carré coloré dans le bloc `définir la couleur du crayon`{class:"block3extensions"}, et ensuite clique sur le sprite carré vert. \--- /task \---

Reproduis les mêmes étapes afin de pouvoir changer la couleur du crayon en bleu.

\--- task \--- Clique sur le sprite carré bleu et ajoute ce code:

![carré_bleu](images/blue_square.png)

```blocks3
quand ce sprite est cliqué 
envoyer à tous (bleu v)
```

Clique ensuite sur le sprite crayon et ajoute ce code: ![crayon](images/pencil.png)

```blocks3
quand je reçois [bleu v]
basculer sur le costume (crayon-bleu v)
mettre la couleur du stylo à [#0000ff]
```

\--- /task \---

\--- task \--- Enfin, ajoute ce code pour indiquer au sprite crayon quelle couleur avec laquelle commencer et pour t'assurer que l'écran est clair quand ton programme démarre.

![crayon](images/pencil.png)

```blocks3
lorsque le drapeau est cliqué 
+ effacer tout
+ basculer sur le costume (crayon-bleu v)
+ mettre la couleur du crayon à [#0035FF]
répéter indéfiniment
  allez à (pointeur de souris v)
si <mouse down?> alors
  stylo en position d'écriture
  sinon
  relever le stylo
fin
```

\--- /task \---

Si tu préfères, tu peux commencer avec un crayon de couleur différente.

\--- task \--- Teste ton code. Peux-tu basculer entre les couleurs de crayon bleu et vert en cliquant sur les sprites carrés bleus ou verts?

![capture d'écran](images/paint-pens-test.png) \--- /task \---