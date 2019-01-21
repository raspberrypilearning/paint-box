## Undo mistakes

Понекад се дешавају грешке, па хајде да додамо дугме 'обриши' и дугме за гумицу.

\--- task \--- Add the 'X-block' sprite from the library's letters section. Обоји костим лика у црвено и смањи му величину. Овај лик је дугме 'обриши'.

[[[generic-scratch3-sprite-from-library]]]

![снимак екрана](images/paint-x.png) \--- /task \---

\--- task \--- Add code to the 'X-block' sprite to clear the Stage when the sprite clicked.

![крст](images/cross.png) ![blocks_1545296088_6331482](images/blocks_1545296088_6331482.png) \--- /task \---

Не мораш да користиш блок `разгласи`{:class="block3events"} да би очистио Позорницу, зато што то може да уради блок `обриши све`{:class="block3extensions"}.

Do you see that the pencil sprite includes an eraser costume?

![снимак екрана](images/paint-eraser-costume.png)

Твој пројекат такође има посебан лик гумице.

\--- task \--- Right-click on this eraser sprite and then click on **show**. Твоја позорница би сада требало да изгледа овако:

![снимак екрана](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![гумица](images/eraser.png) ![blocks_1545296089_7129629](images/blocks_1545296089_7129629.png) \--- /task \---

Када оловка прими поруку "гумица", требало би да замени костим оловке са костимом гумице, а боју бојице у белу - исту боју као боју позорнице!

\--- task \--- Додај код за креирање гумице.

\--- hints \--- \--- hint \--- Додај следећи код лику оловке: `Када примим`{:class="block3events"} поруку `гумица`{:class="block3events"} `Замени костим са гумица`{:class="block3looks"} `Нека боја оловке буде`{:class="block3extensions"} бела \--- /hint \--- \--- hint \--- Овде су сви блокови који су ти потребни: ![blocks_1545296090_8068566](images/blocks_1545296090_8068566.png) \--- /hint \--- \--- hint \--- Овако би требало да изгледа код: ![pencil](images/pencil.png) ![blocks_1545296091_9156106](images/blocks_1545296091_9156106.png) \--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Test your project to see if you can clear the Stage and erase pencil lines.

![снимак екрана](images/paint-erase-test.png) \--- /task \---

Постоји још један проблем са оловком - можеш да црташ било где на Позорници, укључујући и близу дугмета 'обриши' и дугмета за гумицу!

![снимак екрана](images/paint-draw-problem.png)

\--- task \--- To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![оловка](images/pencil.png) ![blocks_1545296093_0167773](images/blocks_1545296093_0167773.png) \--- /task \---

\--- task \--- Испробај свој пројекат. You now should not be able to draw near the buttons.

![снимак екрана](images/paint-fixed.png) \--- /task \---