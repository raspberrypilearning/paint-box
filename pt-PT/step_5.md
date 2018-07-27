## Cometer erros

Às vezes acontecem erros, então vamos adicionar um botão 'limpar' e uma borracha.

+ Adiciona o actor 'X-block' - podes encontrá-lo na biblioteca, na seção de letras. Pinta o traje de vermelho. Este actor vai ser o botão 'limpar'.

![screenshot](images/paint-x.png)

+ Adiciona código a este actor para limpar o palco quando for clicado.

![Clear stage](images/clear-stage.png)

Toma nota de que não precisas de difundir uma mensagem para limpar o palco, podes simplesmente usar o bloco 'apaga tudo palco' deste actor.

Provavelmente notaste que o teu actor de lápis inclui um traje de borracha:

![screenshot](images/paint-eraser-costume.png)

+ O teu projeto também inclui separadamente um actor borracha. Right click on this sprite and choose 'show'. Here is how your stage should look:

![screenshot](images/paint-eraser-stage.png)

+ Add code to the eraser sprite, to tell the pencil to switch to an eraser when the sprite is clicked.

![Broadcast eraser](images/broadcast-eraser.png)

When the pencil receives the "eraser" message, you can switch the pencil costume to the eraser, and switch the pencil colour to white - the same colour as the stage!

+ Add some code to create the eraser

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: **When I receive** the **eraser** message **Switch to costume** eraser **Set pen color** to white \--- /hint \--- \--- hint \--- Here is how the code inside the pencil sprite should look:

```blocks
when I receive [eraser v]
switch costume to [eraser v]
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Test your project, to see if you can clear and erase on the stage.

![screenshot](images/paint-erase-test.png)

There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

![screenshot](images/paint-draw-problem.png)

To fix this, tell the pencil only to draw if the mouse is clicked *and* if the y-position of the mouse is greater than -120:

![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

![screenshot](images/paint-fixed.png)