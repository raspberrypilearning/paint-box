## Change the pen width

Next you will add code to allow the person using your program to draw things with different pen widths.

\--- task \---

首先，添加一个名为 `width`{:class="block3variables"}的新变量。

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

将此行 **添加到** `永久的`{:class="block3control"}循环的铅笔精灵的代码中：

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
go to (mouse pointer v)
+set pen size to (width :: variables)
if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

\--- /task \---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

\--- task \---

右键单击舞台上显示的 `宽`{:class="block3variables"}变量，然后单击 **滑块**。

![screenshot](images/paint-slider.png)

\--- /task \---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can change the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---