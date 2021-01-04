## Change the pen width

Next you will add code to allow the person using your program to draw things with different pen widths.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
quando flag for clicado
apague tudo
mude para a fantasia (lapis-azul v)
mude a cor da caneta para [#0035FF]
sempre 
  vá para (ponteiro do mouse v)
  + mude o tamanho da caneta para (espessura :: variables)
  se <<mouse down?> e <(posição y do mouse) > [-120]>> então 
    use a caneta
  senão 
    levante a caneta
  end
end
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

![captura de tela](images/paint-width-test.png)

\--- /task \---