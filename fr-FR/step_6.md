## Changer l'épaisseur du trait

Permettons à l'utilisateur de dessiner en utilisant une gamme de largeurs de traits différentes.

+ D'abord, ajoutez une nouvelle variable appelée `largeur` {:class="blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Ajoutez cette ligne *à l'intérieur* de la boucle `pour toujours ` {: class = "blockcontrol"} du code du lutin crayon :

```blocks
    mettre la taille du stylo à (largeur)
```

L'épaisseur du trait du stylo sera maintenant toujours liée à la valeur de la variable 'largeur'.

+ Right click on the variable display on the stage and click 'slider'.

![screenshot](images/paint-slider.png)

You can now drag the slider below the variable to change its value.

![screenshot](images/paint-slider-change.png)

+ Test your project, and see if you can modify the pencil width.

![screenshot](images/paint-width-test.png)

If you prefer, you can set the minimum and maximum value of 'width' that's allowed. To do this, right-click on the variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![screenshot](images/paint-slider-max.png)

Keep testing your 'width' variable until you're happy.