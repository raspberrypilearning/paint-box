## Change la largeur du stylo

Ensuite, tu ajouteras du code pour permettre à la personne utilisant ton programme de dessiner des éléments avec différentes largeurs de stylo.

--- task --- Premièrement, ajoute une nouvelle variable appelée `largeur`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]] --- /task ---

--- task --- Ajoute cette ligne **à intérieur** de la boucle `répéter indéfiniment`{:class="block3control"} du code du sprite crayon:

```blocks3
when flag clicked
erase all
switch costume to (crayon-bleu v)
set pen color to [#0035FF]
forever
go to (pointeur de souris v)
+set pen size to (largeur :: variables)
if <<souris pressée?> and <(souris y) > [-120]>> then 
  pen down
  else
  pen up
end
```

--- /task ---

La largeur du stylo est maintenant définie à plusieurs reprises sur la valeur de la variable `largeur`{:class="block3variables"}.

--- task --- Fait un clic droit sur la variable `largeur`{:class="block3variables"} affichée sur la scène, puis clique sur **curseur**.

![capture d'écran](images/paint-slider.png) --- /task ---

Tu peux maintenant faire glisser le curseur visible sous la variable pour modifier la valeur de la variable.

![capture d'écran](images/paint-slider-change.png)

--- task --- Teste ton projet et vois si tu peux ajouter du code pour ajuster la largeur du stylo.

![capture d'écran](images/paint-width-test.png) --- /task ---
