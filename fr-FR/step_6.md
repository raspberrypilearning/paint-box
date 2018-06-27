## Changer l'épaisseur du trait

Permettons à l'utilisateur de dessiner en utilisant une gamme de largeurs de traits différentes.

+ D'abord, ajoutez une nouvelle variable appelée `largeur` {:class="blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Ajoutez cette ligne *à l'intérieur* de la boucle `pour toujours ` {: class = "blockcontrol"} du code du lutin crayon :

```blocks
    mettre la taille du stylo à (largeur)
```

L'épaisseur du trait du stylo sera maintenant toujours liée à la valeur de la variable 'largeur'.

+ Faites un clic droit sur l'affichage de la variable "largeur" sur la scène et cliquez sur "potentiomètre".

![capture d'écran](images/paint-slider.png)

Vous pouvez maintenant faire glisser le curseur sous la variable pour changer sa valeur.

![capture d'écran](images/paint-slider-change.png)

+ Testez votre projet et voyez si vous pouvez modifier l'épaisseur du trait du crayon.

![capture d'écran](images/paint-width-test.png)

Si vous préférez, vous pouvez définir la valeur minimale et maximale de «largeur» autorisée. Pour ce faire, cliquez à nouveau sur la variable avec le bouton droit de la souris et cliquez sur "Définir le min et le max du curseur". Définissez les valeurs minimum et maximum de votre variable à quelque chose de plus judicieux, comme 1 et 20.

![screenshot](images/paint-slider-max.png)

Continuez à tester votre variable "largeur" ​​jusqu'à ce que vous soyez satisfait.