## Cometer erros

Às vezes acontecem erros, então vamos adicionar um botão 'limpar' e uma borracha.

+ Adiciona o actor 'X-block' - podes encontrá-lo na biblioteca, na seção de letras. Pinta o traje de vermelho. Este actor vai ser o botão 'limpar'.

![screenshot](images/paint-x.png)

+ Adiciona código a este actor para limpar o palco quando for clicado.

![Clear stage](images/clear-stage.png)

Toma nota de que não precisas de difundir uma mensagem para limpar o palco, podes simplesmente usar o bloco 'apaga tudo palco' deste actor.

Provavelmente notaste que o teu actor de lápis inclui um traje de borracha:

![screenshot](images/paint-eraser-costume.png)

+ O teu projeto também inclui separadamente um actor borracha. Clica com o botão direito neste actor e escolhe "mostra-te". Aqui está como o teu palco deve ficar:

![screenshot](images/paint-eraser-stage.png)

+ Adicione código ao actor borracha para dizer ao lápis para mudar para uma borracha quando o actor for clicado.

![Broadcast eraser](images/broadcast-eraser.png)

Quando o lápis recebe a mensagem "borracha", podes trocar o traje de lápis para a borracha e mudar a cor do lápis para branco - a mesma cor do palco!

+ Adiciona algum código para criar a borracha

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