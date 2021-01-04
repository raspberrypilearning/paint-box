## Lápis coloridos

Agora vamos adicionar lápis de cores diferentes ao seu projeto e permitir que o usuário escolha entre eles.

\--- task \---

Clique na aba Fantasias do ator 'lápis'.

Rename the `pencil-a` costume to `pencil-blue`

![renomear lápis](images/rename-pencil.png)

\--- /task \---

\--- task \--- Clique no ator quadrado azul e adicione este código:

Clique com o botão direito na fantasia azul-lápis e selecione **duplicado**.

![screenshot](images/paint-blue-duplicate.png)

\--- /task \---

\--- task \---

Nomeie a nova fantasia 'verde-lápis' e pinte-o de verde-lápis.

![screenshot](images/paint-pencil-green.png)

\--- /task \---

\--- task \---

Draw two new sprites: one blue square and one green square. Estes são para escolher entre o lápis azul e o verde.

![screenshot](images/paint-selectors.png)

\--- /task \---

\--- task \---

Renomeie os novos atores cpara que sejam chamados de 'azul' e 'verde'

Depois, faça o mesmo para mudar a cor do lápis para azul.

\--- /task \---

\--- task \---

Adicione algum código ao ator 'verde' para que quando este ator for clicado, ele `transmita`{: class = "block3events"} a mensagem "verde".

![quadrado verde](images/green_square.png)

```blocks3
quando este ator for clicado
transmita (verde v)
```

\--- task \--- Por fim, adicione este código para informar ao ator do lápis qual cor começar e para garantir que a tela esteja limpa quando o programa for iniciado.

\--- /task \---

The pencil sprite should listen for the "green" message and change its costume and pencil colour in response.

Se preferir, você pode começar com um lápis de cor diferente.

\--- task \--- Mude para o seu ator lápis. Add some code so that when this sprite receives the `green`{:class="block3events"} broadcast, it switchs to the green pencil costume and changes the pen colour to green.

![pencil](images/pencil.png)

```blocks3
quando eu receber [verde v]
mude para a fantasia (pencil-green v)
mude a cor da caneta para [#00CC44]
```

To set the pencil to colour to green, click the coloured square in the `set pen color`{:class="block3extensions"} block, and then click on the green square sprite.

\--- /task \---

Depois, faça o mesmo para mudar a cor do lápis para azul.

\--- task \---

Click on the blue square sprite and add this code:

![blue_square](images/blue_square.png)

```blocks3
quando este ator for clicado
transmita (azul v)
```

Then click on the pencil sprite and add this code:

![pencil](images/pencil.png)

```blocks3
quando eu receber [azul v]
mude para a fantasia (pencil-blue v)
mude a cor da caneta para [#0000ff]
```

\--- /task \---

\--- task \---

\--- task \--- Por fim, adicione este código para informar ao ator do lápis qual cor começar e para garantir que a tela esteja limpa quando o programa for iniciado.

![pencil](images/pencil.png)

```blocks3
quando ⚑ for clicado
+apague tudo
+mude para a fantasia (pencil-blue v)
+mude a cor da caneta para [#0035FF]
sempre 
  vá para (mouse pointer v)
  se <mouse down?> então 
    use a caneta
  senão 
    levante a caneta
  end
end
```

\--- /task \---

Se preferir, você pode começar com um lápis de cor diferente.

\--- task \---

Test your code. Can you switch between the blue and green pencil colours by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png)

\--- /task \---