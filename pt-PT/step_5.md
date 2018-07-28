## Cometer erros

Às vezes erros acontecem, vamos então adicionar um botão 'limpar' e uma borracha.

+ Adiciona o actor 'X-block' - podes encontrá-lo na biblioteca, na seção de letras. Pinta o traje de vermelho. Este actor vai ser o botão 'limpar'.

![screenshot](images/paint-x.png)

+ Adiciona código a este actor para limpar o palco quando for clicado.

![Clear stage](images/clear-stage.png)

Toma nota de que não precisas de difundir uma mensagem para limpar o palco, podes simplesmente usar o bloco 'apaga tudo do palco' deste actor.

Provavelmente notaste que o teu actor de lápis inclui um traje de borracha:

![screenshot](images/paint-eraser-costume.png)

+ O teu projeto também inclui separadamente um actor borracha. Clica com o botão direito neste actor e escolhe "mostra-te". Aqui está como o teu palco deve ficar:

![screenshot](images/paint-eraser-stage.png)

+ Adicione código ao actor borracha para dizer ao lápis para mudar para uma borracha quando o actor for clicado.

![Broadcast eraser](images/broadcast-eraser.png)

Quando o lápis recebe a mensagem "borracha", podes trocar o traje de lápis para a borracha e mudar a cor do lápis para branco - a mesma cor do palco!

+ Adiciona algum código para criar a borracha

\--- hints \--- \--- hint \--- Adiciona algum código ao actor lápis: **Quando receberes a mensagem ** 'borracha' **Muda o teu traje para** 'borracha' **Altera a cor da tua caneta ** para 'branco' \--- /hint \--- \--- hint \--- Aqui está como o código dentro to actor lápis deve ficar:

```blocks
quando receberes a mensagem [borracha v] 
muda o teu o traje para [borrachal v] 
altera a cor da tua caneta para [# FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Testa o teu projeto, para ver se podes limpar e apagar no palco.

![screenshot](images/paint-erase-test.png)

Há mais um problema com o lápis - podes desenhar em qualquer lugar do palco, inclusive perto dos ícones de seleção!

![screenshot](images/paint-draw-problem.png)

Para corrigir isso, diz ao lápis para apenas desenhar se o rato for clicado * e * se a posição y do rato for maior que -120:

![screenshot](images/pencil-gt-code.png)

+ Testa o teu projeto; agora já nāo deves conseguir desenhar perto dos blocos de seleção.

![screenshot](images/paint-fixed.png)