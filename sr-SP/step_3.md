## Бојице

Сада ћеш у свој пројекат додати бојице различитих боја и омогућити кориснику да изабере ону коју жели.

\--- task \--- Кликни на лик оловке, а затим на **Костими** и умножи костим 'бојица-плава'.

![снимак екрана](images/paint-blue-duplicate.png) \--- /task \---

\--- task \--- Назови нови костим 'бојица-зелена' и обоји бојицу у зелено.

![снимак екрана](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- Нацртај два нова лика: плави квадрат и зелени квадрат. Они служе за одабир између плаве и зелене оловке.

![снимак екрана](images/paint-selectors.png) \--- /task \---

\--- task \--- Преименуј их тако да се зову 'плава' и 'зелена'

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- Add some code to the 'green' sprite so that when this sprite is clicked, it `broadcasts`{:class="block3events"} the message "green".

![зелени квадрат](images/green_square.png) ![blocks_1545296083_0935004](images/blocks_1545296083_0935004.png)

[[[generic-scratch3-broadcast-message]]] \--- /task \---

The pencil sprite should listen for the "green" message and change its costume and pencil colour in response.

\--- task \--- Врати се на лик оловке. Додај код, тако да, када овај лик прими разглас `зелена`{:class="block3events"}, промени костим у бојица-зелена и боју бојице у зелену.

![оловка](images/pencil.png)

![blocks_1545296084_19679](images/blocks_1545296084_19679.png)

To set the pencil to colour to green, click the coloured square in the `set pen color`{:class="block3extensions"} block, and then click on the green square sprite. \--- /task \---

Then to a similar thing so that you can switch the pencil colour to blue.

\--- task \--- Кликни на плави квадрат и додај следећи код:

![blue_square](images/blue_square.png) ![blocks_1545296085_2853348](images/blocks_1545296085_2853348.png)

Затим кликни на лик оловке и додај следећи код: ![pencil](images/pencil.png) ![blocks_1545296086_3780818](images/blocks_1545296086_3780818.png) \--- /task \---

\--- task \--- На крају, додај овај код да кажеш лику бојице са којом бојом да почне и да екран буде обрисан када се твој програм покрене.

![оловка](images/pencil.png) ![blocks_1545296087_4832299](images/blocks_1545296087_4832299.png) \--- /task \---

Ако желиш, можеш почети са бојицом друге боје.

\--- task \--- Испробај свој код. Можеш ли да мењаш између плаве и зелене бојице када кликнеш на ликове плавог или зеленог квадрата?

![снимак екрана](images/paint-pens-test.png) \--- /task \---