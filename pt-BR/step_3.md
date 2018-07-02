## Fazendo um lápis

Vamos começar fazendo um lápis que pode ser usado para desenhar no palco.

+ Abra o projeto 'Paintbox' no Scratch (versão online) em [jumpto.cc/paint-go](http://jumpto.cc/paint-go){:target="_ blank"} ou faça o download de <http://jumpto.cc/paint-get>{:target="_ blank"} e depois abra no editor Scratch versão off-line.

Você verá atores de lápis e borracha:

![screenshot](images/paint-starter.png)

+ Adicione algum código ao ator lápis para que ele siga o mouse `sempre`{:class= "blockcontrol"} para que você possa desenhar:

```blocks
    when flag clicked
    forever
      go to [mouse pointer v]
    end
```

+ Click the flag and then move the mouse around the stage to test whether the code works.

Next, let's make your pencil only draw `if`{:class="blockcontrol"} the mouse has been clicked.

+ Add this code to your pencil sprite:

![screenshot](images/paint-pencil-draw-code.png)

+ Teste seu código novamente. This time, move the pencil around the stage and hold down the mouse button. Você pode desenhar com o seu lápis?

![screenshot](images/paint-draw.png)

## \--- collapse \---

## title: Se você tiver problemas...

If your pencil seems to be drawing the line from the middle of the pencil rather than the tip, you will need to change your costume center.

![Costume center](images/costume-center.png)

The crosshair for the pencil must be placed **just below** the tip of the pencil, not on the tip of the pencil.

A changes in a sprite's 'costume center' isn't registered until another tab is clicked, so click on another costume, or on the 'Scripts' tab to finalise your changes to the costume center.

\--- /collapse \---