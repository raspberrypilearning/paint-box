## Fazendo um lápis

Vamos começar fazendo um lápis que pode ser usado para desenhar no palco.

+ Abra o projeto 'Paintbox' no Scratch (versão online) em [jumpto.cc/paint-go](http://jumpto.cc/paint-go){:target="_ blank"} ou faça o download de <http://jumpto.cc/paint-get>{:target="_ blank"} e depois abra no editor Scratch versão off-line.

Você verá os atores lápis e borracha:

![screenshot](images/paint-starter.png)

+ Adicione algum código ao ator lápis para que ele siga o mouse `sempre`{:class="blockcontrol"} para que você possa desenhar:

```blocks
    quando clicar em bandeira
    sempre
      vá para [ponteiro do mouse v]
    fim
```

+ Clique na bandeira e, em seguida, mova o mouse pelo palco para testar se o código funciona.

Em seguida, vamos fazer o seu lápis desenhar apenas `se`{:class="blockcontrol"} o mouse foi clicado.

+ Adicione este código ao seu pincel (ator):

![screenshot](images/paint-pencil-draw-code.png)

+ Teste seu código novamente. Desta vez, mova o lápis ao redor do palco e segure o botão do mouse. Você pode desenhar com o seu lápis?

![screenshot](images/paint-draw.png)

## \--- collapse \---

## title: Se você tiver problemas...

Se o seu lápis parece estar desenhando a linha do meio do lápis, não da ponta, você precisará mudar o centro da sua fantasia.

![Centro da fantasia](images/costume-center.png)

A cruz para o lápis deve ser colocada **logo abaixo** da ponta do lápis, não na ponta do lápis.

As mudanças no 'centro das fantasias' de um ator não são registradas até que outra aba seja clicada, então clique em outra fantasia, ou na aba 'Scripts' para finalizar suas mudanças.

\--- /collapse \---