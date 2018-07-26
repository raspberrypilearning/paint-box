## Lápis coloridos

Vamos adicionar lápis de cor diferentes ao teu projeto e permitir ao utilizador escolher entre eles.

+ Clica no teu actor 'lápis', clica em 'Trajes' e duplica o teu traje de 'lápis-azul'.

![screenshot](images/paint-blue-duplicate.png)

+ Renomeia o teu novo traje para 'lápis-verde' e pinta o lápis de verde.

![screenshot](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Desenha dois novos actores - um quadrado azul e um quadrado verde. Vais usá-los para selecionar o lápis azul ou verde.

![screenshot](images/paint-selectors.png)

+ Renomeia os teus actores para que eles sejam chamados de "azul" e "verde"

+ Adiciona algum código ao actor 'verde' para que quando ele for clicado, seja ` difundida a mensagem` {: class = "blockevents"} "verde" para o actor lápis, dizendo-lhe para mudar as cores de traje e lápis.

![Difundir verde](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Muda para o teu actor de lápis. Adiciona código para que quando este actor receber a `difusão da mensagem ` {: class = "blockevents"} verde, ele mude para o traje de lápis verde e mude a cor da caneta para verde.

![Difundir verde](images/broadcast-green.png)

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