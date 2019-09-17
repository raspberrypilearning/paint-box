## 更改笔宽

接下来，您将添加代码以允许使用您的程序的人绘制具有不同笔宽的内容。

\--- 任务 \--- 首先，添加一个名为 `width`{：class =“block3variables”}的新变量。

[[[generic-scratch3-add-variable]]] \--- /任务\---

\--- 任务 \--- 将此行 **添加到** `永久的`{：class =“block3control”}循环的铅笔精灵的代码中：

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

\--- /任务\---

笔宽现在重复设置为 `宽度`{：class =“block3variables”}变量的值。

\--- 任务 \--- 右键单击舞台上显示的 `宽`{：class =“block3variables”}变量，然后单击 **滑块**。

![截屏](images/paint-slider.png) \--- /任务\---

您现在可以拖动变量下方可见的滑块来更改变量的值。

![截屏](images/paint-slider-change.png)

\--- 任务 \--- 测试你的项目，看看你是否可以添加代码来调整笔的宽度。

![截屏](images/paint-width-test.png) \--- /任务\---