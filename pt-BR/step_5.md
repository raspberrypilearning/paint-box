## Undo mistakes

Sometimes mistakes happen, so add a 'clear' button and an eraser button.

\--- task \---

\--- task \--- Adicione o ator 'X-block' da seção de letras da biblioteca. Pinte a fantasia do ator de vermelho e torne-o um pouco menor. Este ator vai ser o botão 'limpar'.

[[[generic-scratch3-sprite-from-library]]]

![captura de tela](images/paint-x.png)

\--- /task \---

\--- task \---

Adicione código ao 'bloco-X' para limpar o palco quando clicar no ator.

![cruz](images/cross.png)

```blocks3
quando este ator for clicado
apague tudo
```

\--- /task \---

Você não precisa usar uma `transmissão`{:class="block3events"} para limpar o palco, porque o bloco `apagar tudo`{:class="block3extensions"} faz isso.

Você vê que o ator lápis inclui uma fantasia de borracha?

![captura de tela](images/paint-eraser-costume.png)

O seu projeto também inclui separadamente um ator borracha.

\--- task \---

Click on this eraser sprite and then select **show**.

![captura de tela](images/show-eraser.png)

Here is how your Stage should look now:

![captura de tela](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
quando este ator for clicado
transmita (eraser v)
```

\--- /task \---

Quando o ator lápis recebe a mensagem 'borracha', deveria trocar a fantasia para a borracha e mudar a cor do lápis para branco, que é a mesma cor do palco!

\--- task \---

Add some code to create the eraser.

\--- hints \--- \--- hint \---

Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

\--- /hint \--- \--- hint \---

Here are all the blocks you need:

```blocks3
mude a cor da caneta para [#FFFFFF]

quando eu receber [eraser v]

mude para a fantasia (eraser v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![lápis](images/pencil.png)

```blocks3
quando eu receber [eraser v]
mude para a fantasia (eraser v)
mude a cor da caneta para [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \---

Test your project to see if you can clear the Stage and erase pencil lines.

![capturas de tela](images/paint-erase-test.png)

\--- /task \---

Há mais um problema com o lápis: você pode desenhar em qualquer lugar do Palco, inclusive próximo aos botões 'limpar' e borracha!

![capturas de tela](images/paint-draw-problem.png)

\--- task \---

To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![lápis](images/pencil.png)

```blocks3
quando flag for clicado
apague tudo
mude para a fantasia (pencil-blue v)
mude a cor da caneta para [#0035FF]
sempre 
 vá para (mouse pointer v)
+se <<mouse down?> e <(posição y do mouse) > [-120]>> então 
 use a caneta
 senão 
 levante a caneta
end
```

\--- /task \---

\--- task \---

\--- task \--- Teste seu projeto. Agora você não deve conseguir desenhar perto dos botões.

![captura de tela](images/paint-fixed.png)

\--- /task \---