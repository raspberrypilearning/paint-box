## Alterar a largura da caneta

Agora, vais acrescentar código para permitir que a pessoa que usa seu programa desenhe objetos com diferentes larguras de caneta.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
quando alguém clicar na bandeira verde
apaga tudo do palco
muda o teu traje para (pencil-blue v)
altera a cor da tua caneta para [#0035FF]
repete para sempre 
  vai para (mouse pointer v)
  + altera a espessura da tua caneta para (width :: variables)
  se <<o botão do rato está pressionado> e <(o y da posição do rato) > [-120]>> , então 
    baixa a tua caneta
  senão, 
    levanta a tua caneta
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

Test your project and see if you can add code to adjust the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---