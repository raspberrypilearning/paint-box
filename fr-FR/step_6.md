## Change la largeur du stylo

Ensuite, tu ajouteras du code pour permettre à la personne utilisant ton programme de dessiner des éléments avec différentes largeurs de stylo.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
lorsque le drapeau est cliqué 
effacer tout
basculer sur le costume (crayon-bleu v)
mettre la couleur du stylo à [# 0035FF]
répéter indéfiniment
aller à (pointeur de souris v)
+ définir la taille du stylo à (largeur :: variables)
si <<mouse down?> et <(souris y) > [-120]>> alors 
  stylo en position d'écriture
  sinon
  relever le stylo
fin
```

\--- /task \---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

\--- task \---

Right-click on the `width`{:class="block3variables"} variable displayed on the Stage, and then click on **slider**.

![screenshot](images/paint-slider.png)

\--- /task \---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can change the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---