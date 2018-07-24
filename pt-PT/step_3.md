## Criar um lápis

Vamos começar por criar um lápis que pode ser usado para desenhar no palco.

+ Abre o projeto Scratch 'Paintbox' online em [ jumpto.cc/paint-go ](http://jumpto.cc/paint-go) {: target = "_ blank"} ou faz o download de [ http://jumpto.cc/paint-get ](http://jumpto.cc/paint-get) {: target = "_ blank"} e depois abre-o se estiveres a usar o editor off-line.

Verás os actores lápis e borracha:

![screenshot](images/paint-starter.png)

+ Adiciona código ao actor lápis para que ele siga o rato ` para sempre ` {: class = "blockcontrol"} para que possas desenhar:

```blocks
    Quando alguém  clicar em "bandeira"
    repete para sempre
         vai para [o ponteiro do rato v] 
    fim
```

+ Clica na bandeira e em seguida, move o rato pelo palco para testares se o código funciona.

Em seguida, vamos fazer o teu lápis apenas desenhar ` se ` {: class = "blockcontrol"} o rato for clicado.

+ Adiciona este código ao teu actor lápis:

![screenshot](images/paint-pencil-draw-code.png)

+ Testa o teu código outra vez. Desta vez, move o lápis ao redor do palco enquanto clicas o botão do rato. Podes desenhar com o teu lápis?

![screenshot](images/paint-draw.png)

## \--- collapse \---

## title: Se estás com dificuldades ...

If your pencil seems to be drawing the line from the middle of the pencil rather than the tip, you will need to change your costume center.

![Costume center](images/costume-center.png)

The crosshair for the pencil must be placed **just below** the tip of the pencil, not on the tip of the pencil.

A changes in a sprite's 'costume center' isn't registered until another tab is clicked, so click on another costume, or on the 'Scripts' tab to finalise your changes to the costume center.

\--- /collapse \---