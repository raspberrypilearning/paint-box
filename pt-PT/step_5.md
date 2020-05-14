## Desfazer erros

Às vezes acontecem erros, vamos então adicionar um botão 'limpar' e uma borracha.

\--- task \---

Adiciona o ator 'X-block' a partir da secção de cartas da biblioteca. Pinta o traje do ator de vermelho e torna-o um pouco menor. Este actor vai ser o botão 'limpar'.

[[[generic-scratch3-sprite-from-library]]]

![captura de ecrã](images/paint-x.png)

\--- /task \---

\--- task \---

Adiciona código ao ator 'X-block' para limpar o palco quando o ator for clicado.

![cruz](images/cross.png)

```blocks3
quando alguém clicar em ti
apaga tudo do palco
```

\--- /task \---

Não necessitas de usar uma mensagem ` ` {: class = "block3events"} para limpar o palco, porque o bloco ` apaga tudo ` {: class = "block3extensions"} faz esse trabalho.

Estás a ver que o ator lápis inclui um traje de borracha?

![captura de ecrã](images/paint-eraser-costume.png)

O teu projeto também inclui separadamente um actor borracha.

\--- task \---

Clica com o botão direito do rato neste ator borracha e depois em ** mostra **. Aqui está o aspeto com que o teu palco deve ficar:

![captura de ecrã](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Adiciona código ao ator 'borracha' para difundir uma mensagem de ` 'borracha' ` {: class = "block3events"} quando esse ator é clicado.

![borracha](images/eraser.png)

```blocks3
quando alguém clicar em ti
difunde a mensagem (eraser v)
```

\--- /task \---

Quando o lápis recebe a mensagem "borracha", podes trocar o traje de lápis para a borracha e mudar a cor do lápis para branco - a mesma cor do palco!

\--- task \---

Adiciona algum código para criar a borracha.

\--- hints \--- \--- hint \---

Adiciona código ao ator 'lápis': ` Quando eu receber ` {: class = "block3events"} a mensagem ` 'borracha' ` {: class = "block3events"} ` Mudar para traje de borracha ` {: class = "block3looks"} ` Definir cor da caneta ` {: class = "block3extensions"} para branco

\--- /hint \--- \--- hint \---

Aqui estão os blocos de que precisas:

```blocks3
altera a cor da tua caneta para [#FFFFFF]

Quando receberes a mensagem [eraser v]

muda o teu traje para (eraser v)
```

\--- /hint \--- \--- hint \---

Aqui está o aspeto que o teu código deve ter:

![lápis](images/pencil.png)

```blocks3
quando receberes a mensagem [eraser v]
muda o teu traje para (eraser v)
altera a cor da tua caneta para [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \---

Testa o teu projeto para ver se consegues limpar o Palco e apagar as linhas do lápis.

![captura de ecrã](images/paint-erase-test.png)

\--- /task \---

Há mais um problema com o lápis - consegues desenhar em qualquer lugar do palco, inclusive perto dos botões 'limpar' e ' borracha'!

![captura de ecrã](images/paint-draw-problem.png)

\--- task \---

Para o corrigir, altera o código de forma a que a caneta fique em baixo apenas se o rato for clicado ** e ** o ` y ` da posição do ponteiro do rato for maior que ` -120 `:

![lápis](images/pencil.png)

```blocks3
quando alguém clicar na bandeira verde
apaga tudo do palco
muda o teu traje para (pencil-blue v)
altera a cor da tua caneta para [#0035FF]
repete para sempre 
  vai para (mouse pointer v)
  + se <<o botão do rato está pressionado> e <(o y da posição do rato) > [-120]>>, então 
  +   baixa a tua caneta
  + senão, 
  +   levanta a tua caneta
  + end
end
```

\--- /task \---

\--- task \---

Testa o teu projeto. Agora já não deverás conseguir desenhar próximo dos botões.

![captura de ecrã](images/paint-fixed.png)

\--- /task \---