## Desfazer erros

Às vezes, erros acontecem, então vamos adicionar um botão 'limpar' e uma borracha.

\--- task \--- Adicione o ator 'X-block' da seção de letras da biblioteca. Pinte o traje do ator de vermelho e torne-o um pouco menor. Este ator vai ser o botão 'limpar'.

[[[generic-scratch3-sprite-from-library]]]

![capturas de tela](images/paint-x.png) \--- /task \---

\--- task \--- Adicione código ao ator 'X-block' para limpar o palco quando o ator for clicado.

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

\--- task \--- Clique com o botão direito do mouse no ator borracha e clique em **mostrar**. Aqui está como seu palco deve ficar:

![captura de tela](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Adicione código ao ator borracha para enviar uma `transmissão 'borracha'`{:class="block3events"} quando o ator borracha é clicado.

![borracha](images/eraser.png)

```blocks3
quando este ator for clicado
transmita (eraser v)
```

\--- /task \---

Quando o ator lápis recebe a mensagem 'borracha', deveria trocar a fantasia para a borracha e mudar a cor do lápis para branco, que é a mesma cor do palco!

\--- task \--- Adicione algum código para criar a borracha.

\--- hints \--- \--- hint \--- Adicione algum código ao ator lápis: `Quando eu receber`{:class="block3events"} a mensagem `borracha`{:class="block3events"} `Mudar para fantasia de borracha`{:class="block3looks"} `Definir cor da caneta`{:class="block3extensions"} para branco \--- / hint \--- \--- hint \--- Aqui estão todos os blocos que você precisa:

```blocks3
mude a cor da caneta para [#FFFFFF]

quando eu receber [eraser v]

mude para a fantasia (eraser v)
```

\--- /hint \--- \--- hint \--- Aqui está como seu código deve parecer: ![lápis](images/pencil.png)

```blocks3
quando eu receber [eraser v]
mude para a fantasia (eraser v)
mude a cor da caneta para [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Teste seu projeto para ver se você consegue limpar o palco e apagar as linhas do lápis.

![captura de tela](images/paint-erase-test.png) \--- /task \---

Há mais um problema com o lápis: você pode desenhar em qualquer lugar do palco, inclusive perto dos ícones de limpar e borracha!

![captura de tela](images/paint-draw-problem.png)

\--- task \--- Para corrigir isso, altere o código para que a caneta fique abaixada apenas se o mouse for pressionado **e** a posição `y` do ponteiro do mouse é maior que `-120`:

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

\--- task \--- Teste seu projeto. Agora você não deve conseguir desenhar perto dos botões.

![capturas de tela](images/paint-fixed.png) \--- /task \---