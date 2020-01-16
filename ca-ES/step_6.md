## Canvieu l'amplada del llapis

A continuació, s’afegirà un codi per permetre a la persona que utilitza el vostre programa dibuixar coses amb diferents amplades de llapis.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
quan es fa clic a la bandera
esborrar tots els
vestit de canvi a (llapis blau v)
establir el color del llapis a [# 0035FF]
per sempre
anar a (punter del ratolí v)
+ establir la mida del llapis a (ample :: variables)
si <<mouse down?> i <(ratolí i) > [-120]>> i 
  penals a
  més,
  penals fins al final

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

Test your project and see if you can add code to adjust the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---