## Mudando a espessura do lápis

Em seguida, você adicionará código para permitir que a pessoa que usa seu programa desenhe coisas com diferentes espessuras de lápis.

\--- task \---

Primeiro, adicione uma nova variável chamada `largura`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Adicione esta linha **dentro** do loop `infinito`{:class="block3control"} do código do ator do lápis:

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

A largura da caneta agora é repetidamente definida para o valor da variável `largura`{:class="block3variables"}.

\--- task \---

Clique com o botão direito na variável `largura` {: class = "block3variables"} exibida no palco e depois clique na **barra deslizante**.

![captura de tela](images/paint-slider.png)

\--- /task \---

Agora você pode arrastar o controle deslizante, que está visível abaixo da variável, para alterar o seu valor.

![captura de tela](images/paint-slider-change.png)

\--- task \---

Teste seu projeto e veja se você consegue adicionar código para ajustar a largura da caneta.

![captura de tela](images/paint-width-test.png)

\--- /task \---