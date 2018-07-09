## Lápis coloridos

Vamos adicionar lápis de cor diferentes ao seu projeto e permitir que o usuário escolha entre eles.

+ Clique no seu lápis (ator), clique em 'Fantasias' e duplique sua fantasia de 'lápis azul'.

![screenshot](images/paint-blue-duplicate.png)

+ Renomeie seu nova fantasia como 'lápis verde' e pinte de verde o lápis.

![screenshot](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Desenhe dois novos atores - um quadrado azul e um quadrado verde. Você os usará para selecionar o lápis azul ou verde.

![screenshot](images/paint-selectors.png)

+ Renomeie seus atores para que eles sejam chamados de "azuis" e "verdes"

+ Adicione algum código ao ator 'verde' para que quando ele for clicado, seja `transmitido`{:class="blockevents"} a mensagem "verde" para o ator lápis, dizendo para mudar a fantasia do lápis e sua cor.

![Broadcast green](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Switch to your pencil sprite. Add some code so that when this sprite receives the `broadcast`{:class="blockevents"} green, it should switch to the green pencil costume and change the pen colour to green.

![Broadcast green](images/broadcast-green.png)

To set the pencil to colour to green, click the coloured box in the `set pen color`{:class="blockpen"} block, and click on the green sprite to choose the same colour green as your pencil colour.

+ You can now do the same for the blue pencil icon: add this code to the blue square sprite:

```blocks
when this sprite clicked
broadcast [blue v]
```

...and add this code to the pencil sprite:

```blocks
when I receive [blue v]
switch costume to [pencil-blue v]
set pen color to [#0000ff]
```

+ Finally, add this code to tell the pencil sprite which colour to start with, and make sure that the screen is clear.

![Start pencil](images/start-pencil.png)

We chose to start with blue but if you prefer, you can start with a different colour pencil.

+ Test out your project. Can you switch between blue and green pens by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png)