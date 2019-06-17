## Bút chì màu

Bây giờ bạn sẽ thêm bút chì màu khác nhau vào dự án của bạn và cho phép người dùng lựa chọn giữa chúng.

\--- task \--- Rename the `pencil` sprite to `pencil-blue`

![rename-pencil](images/rename-pencil.png) \--- /bài tập \---

\--- task \--- Right click on the pencil sprite, and duplicate the 'pencil-blue' costume.

![screenshot](images/paint-blue-duplicate.png) \--- /task \---

\--- task \--- Name the new costume 'pencil-green', and colour the pencil green.

![screenshot](images/paint-pencil-green.png)

\--- /bài tập \---

\--- task \--- Draw two new sprites: one blue square and one green square. These are for choosing between the blue and green pencil.

![screenshot](images/paint-selectors.png) \--- /task \---

\--- task \--- Rename the new sprites so that they are called 'blue' and 'green'

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- Add some code to the 'green' sprite so that when this sprite is clicked, it `broadcasts`{:class="block3events"} the message "green".

![green square](images/green_square.png)

```blocks3
khi sprite này nhấp
phát (green v)
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

The pencil sprite should listen for the "green" message and change its costume and pencil colour in response.

\--- task \--- Switch to your pencil sprite. Add some code so that when this sprite receives the `green`{:class="block3events"} broadcast, it switchs to the green pencil costume and changes the pen colour to green.

![pencil](images/pencil.png)

```blocks3
khi tôi nhận được [xanh v]
trang phục chuyển sang (bút chì xanh v)
đặt màu bút thành [# 00CC44]
```

To set the pencil to colour to green, click the coloured square in the `set pen color`{:class="block3extensions"} block, and then click on the green square sprite. \--- /task \---

Then to a similar thing so that you can switch the pencil colour to blue.

\--- task \--- Click on the blue square sprite and add this code:

![blue_square](images/blue_square.png)

```blocks3
khi sprite này nhấp
phát (màu xanh v)
```

Then click on the pencil sprite and add this code: ![pencil](images/pencil.png)

```blocks3
khi tôi nhận được [blue v]
trang phục chuyển sang (bút chì màu xanh v)
đặt màu bút thành [# 0000ff]
```

\--- /task \---

\--- task \--- Finally, add this code to tell the pencil sprite which colour to start with, and to make sure that the screen is clear when your program starts.

![pencil](images/pencil.png)

```blocks3
khi lá cờ nhấp
+ xóa tất cả
+ chuyển trang phục để (v bút chì màu xanh)
+ thiết bút màu để [# 0035FF]
mãi mãi
  đi tới (con trỏ chuột v)
nếu <mouse down?> sau đó
  bút xuống
  khác
  bút lên
kết thúc
```

\--- /task \---

If you prefer, you can start with a different colour pencil.

\--- task \--- Test your code. Can you switch between the blue and green pencil colours by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png) \--- /task \---