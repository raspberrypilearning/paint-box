## Lápis coloridos

Vamos adicionar lápis de cor diferentes ao teu projeto e permitir ao utilizador escolher entre eles.

\--- task \---

Renomeia o ator ` lápis ` como ` lápis-azul `

![renomear lápis](images/rename-pencil.png)

\--- /task \---

\--- task \---

Clica com o botão direito do rato no ator lápis e duplica o traje de 'lápis azul'.

![captura de ecrã](images/paint-blue-duplicate.png)

\--- /task \---

\--- task \---

Renomeia o teu novo traje para 'lápis-verde' e pinta o lápis de verde.

![captura de ecrã](images/paint-pencil-green.png)

\--- /task \---

\--- task \---

Desenha dois novos actores: um quadrado azul e um quadrado verde. Estes atores vão ser usados para escolher entre o lápis azul e o verde.

![captura de ecrã](images/paint-selectors.png)

\--- /task \---

\--- task \---

Renomeia os teus actores para que sejam chamados de "azul" e "verde"

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \---

Adiciona código ao actor vermelho para que, quando o actor for clicado, ele `difunda a mensagem`{:class="block3events"} 'vermelho' ao personagem actor".

![quadrado verde](images/green_square.png)

```blocks3
quando alguém clicar em ti
difunde a mensagem (green v)
```

[[[generic-scratch3-broadcast-message]]]

\--- /task \---

O ator lápis deve ouvir a mensagem "verde" e mudar o seu traje e cor do lápis em resposta.

\--- task \---

Muda para o teu actor de lápis. Acrescenta-lhe código para que quando este actor receber a mensagem` verde ` {: class = "blockevents"}, ele mude para o traje de lápis verde e mude a cor da caneta para verde.

![lápis](images/pencil.png)

```blocks3
quando receberes a mensagem [green v]
muda o teu traje para (pencil-green v)
altera a cor da tua caneta para [#00CC44]
```

Para definir o lápis como verde, clicano quadrado colorido em ` definir cor da caneta ` {: class = "block3extensions"} e clica no ator quadrado verde.

\--- /task \---

Depois, faz o mesmo para mudar a cor do lápis para azul.

\--- task \---

Clica no ator quadrado azul e adiciona este código:

![quadrado azul](images/blue_square.png)

```blocks3
quando alguém clicar em ti
difunde a mensagem (azul v)
```

A seguir, clica no lápis e adiciona este código:

![lápis](images/pencil.png)

```blocks3
quando receberes a mensagem [blue v]
muda o teu traje para (pencil-blue v)
altera a cor da tua caneta para [#0000ff]
```

\--- /task \---

\--- task \---

Finalmente, acrescenta este código para informar o actor lápis sobra a cor com que deve começar e assegurar que o ecrã está limpo quando o programa começar.

![lápis](images/pencil.png)

```blocks3
quando alguém clicar na bandeira verde
apaga tudo do palco
muda o teu traje para (pencil-blue v)
altera a cor da tua caneta para [#0035FF]
repete para sempre 
  vai para (mouse pointer v)
  se <o botão do rato está pressionado>, então 
    baixa a tua caneta
  senão, 
    levanta a tua caneta
  end
end
```

\--- /task \---

Se preferires, podes começar com um lápis de cor diferente.

\--- task \---

Testa o teu código. Consegues alternar entre canetas azuis e verdes clicando nos actores quadrado azul ou verde?

![captura de ecrã](images/paint-pens-test.png)

\--- /task \---