## Crayons de couleurs

Ajoutons des crayons de couleurs différentes à votre projet, et permettons à l'utilisateur de choisir entre eux.

+ Cliquez sur votre lutin crayon, cliquez sur «Costumes» et dupliquez votre costume «pencil-blue».

![capture d'écran](images/paint-blue-duplicate.png)

+ Renommez votre nouveau costume «crayon-vert» et colorez le crayon en vert.

![capture d'écran](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Dessinez deux nouveaux lutins - un carré bleu et un carré vert. Vous les utiliserez pour sélectionner le crayon bleu ou le crayon vert.

![capture d'écran](images/paint-selectors.png)

+ Renommez vos lutins pour qu'ils soient appelés "bleu" et "vert"

+ Ajoutez du code au lutin "vert" de sorte que lorsque vous cliquez dessus, il ` diffusera ` {: class = "blockevents"} le message "vert" au lutin crayon, lui disant de changer sa couleur de costume et de stylo.

![Diffuser le message "green"](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Passez à votre lutin crayon. Ajoutez du code afin que lorsque ce lutin reçoit le message ` ` {: class = "blockevents"} vert, il passe au costume vert et change la couleur du stylo au vert.

![Diffuser le message "green"](images/broadcast-green.png)

Pour mettre le stylo du lutin crayon en vert, cliquez sur la case de couleur dans la ` mettre la couleur du stylo ` {: class = "blockpen"} bloc, et cliquez sur le lutin vert pour choisir la même couleur verte que la couleur de votre crayon.

+ Vous pouvez maintenant faire la même chose pour le message bleu. Ajoutez ce code au lutin bleu :

```blocks
quand ce lutin est cliqué
 envoyer à tous [bleu v]
```

ajoutez ce code à votre lutin crayon :

```blocks
quand je reçois [vert v]
 basculer sur costume [crayon-vert v]
 mettre la couleur du stylo à [#00ff00
```

+ Enfin, ajoutez ce code pour indiquer au lutin crayon la couleur de départ et s'assurer que l'écran est vide.

![Crayon de début](images/start-pencil.png)

Nous avons choisi de commencer avec le bleu mais si vous préférez, vous pouvez commencer avec un crayon de couleur différente.

+ Testez votre projet. Pouvez-vous basculer entre les crayons bleus et verts en cliquant sur les lutins carrés bleus ou verts ?

![capture d'écran](images/paint-pens-test.png)