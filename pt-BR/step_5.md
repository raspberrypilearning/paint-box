## Making mistakes

Às vezes, erros acontecem, então vamos adicionar um botão 'limpar' e uma borracha.

+ Add the 'X-block' sprite - you will find it in the library, in the letters section. Colour the costume in red. This will become the 'clear' button.

![screenshot](images/paint-x.png)

+ Adicione o código a este ator para limpar o palco quando for clicado.

![Limpar palco](images/clear-stage.png)

Observe que você não precisa enviar uma mensagem para limpar o palco, você pode simplesmente usar o bloco limpo dele.

You have probably noticed that your pencil sprite includes an eraser costume:

![screenshot](images/paint-eraser-costume.png)

+ Your project also includes a separate eraser sprite. Right click on this sprite and choose 'show'. Aqui está como seu palco deve ficar:

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

\---/hints \--- \--- /hint \---

+ Test your project, to see if you can clear and erase on the stage.

![screenshot](images/paint-erase-test.png)

There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

![screenshot](images/paint-draw-problem.png)

To fix this, tell the pencil only to draw if the mouse is clicked *and* if the y-position of the mouse is greater than -120:

![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

![screenshot](images/paint-fixed.png)