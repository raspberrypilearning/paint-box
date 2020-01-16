## Làm bút chì

Bắt đầu bằng cách làm một cây bút chì mà bạn có thể sử dụng để vẽ trên Sân khấu.

\--- task \---

Open the 'Paint box' Scratch starter project.

**Online**: open the starter project at [rpf.io/paint-box-on](http://rpf.io/paint-box-on){:target="_blank"}

If you have a Scratch account you can make a copy by clicking **Remix**.

**Offline**: open the [starter project](http://rpf.io/p/en/paint-box-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

In the starter project, you should see pencil and eraser sprites:

![screenshot](images/paint-starter.png)

\--- /task \---

\--- task \---

Add the Pen extension to your project.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Add some code to the pencil sprite to make the sprite follow the mouse pointer `forever`{:class="block3control"} so that you can draw:

![pencil](images/pencil.png)

```blocks3
khi cờ nhấp
mãi mãi
  đi đến (con trỏ chuột v)
kết thúc
```

\--- /task \---

\--- task \---

Click the flag and then move the mouse pointer around the Stage to test whether your code works.

\--- /bài tập \---

Next, make your pencil only draw `if`{:class="block3control"} the mouse button is being clicked.

\--- task \---

Add this code to your pencil sprite:

![pencil](images/pencil.png)

```blocks3
khi cờ nhấp
mãi mãi
  đi tới (con trỏ chuột v)

+ nếu <mouse down?> thì
  bút xuống
  khác
  bút lên
kết thúc
```

\--- /task \---

\--- task \---

Test your code again. This time, move the pencil around the Stage and hold down the mouse button. Can you draw with your pencil?

![screenshot](images/paint-draw.png)

\--- /task \---

## \--- sự sụp đổ \---

## tiêu đề: Bút chì của bạn không rút ra từ đầu của nó?

If the line your pencil draw looks like it is coming from the pencil's middle, you need to change your pencil sprite's so the tip is the sprite's centre.

Click on the pencil sprite, and then click on the **Costumes** tab.

Move the costume's so the tip of the pencil is **just above** the centre.

![Costume center](images/costume-center-annotated.png)

Now move the pencil around on the Stage and draw. The pencil should now draw a line from its tip.

\--- /collapse \---