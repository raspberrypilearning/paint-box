## 更改笔尖宽度

有时会发生错误，因此请添加“清除”按钮和橡皮擦按钮。

\--- task \--- 从库的字母部分添加'X-block'精灵。 将精灵的服装涂成红色并使其略小一些。 这个精灵是'清除'按钮。

[[[generic-scratch3-sprite-from-library]]]

![截屏](images/paint-x.png) \--- /task \---

\--- task \--- 添加代码到'X-block'精灵，以便在点击精灵时清除舞台。

![交叉](images/cross.png)

```blocks3
当这个精灵点击
擦除全部
```

\--- /task \---

您不需要使用 `广播`{：class =“block3events”}来清除舞台，因为 `擦除所有`{：class =“block3extensions”}块执行该作业。

你看到铅笔精灵包括橡皮擦服装吗？

![截屏](images/paint-eraser-costume.png)

项目中还包含一个单独的橡皮角色。

\--- task \--- 右键单击此橡皮精灵，然后单击 **show**。 以下是您的舞台现在的样子：

![截屏](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- 当橡皮精灵被点击时，将代码添加到橡皮精灵以发送 `'橡皮擦'广播`{：class =“block3events”}。

![橡皮](images/eraser.png)

```blocks3
当这个精灵点击
广播（橡皮擦v）
```

\--- /task \---

当铅笔精灵收到“橡皮擦”信息时，它应该将其服装切换到橡皮擦并将笔颜色切换为白色，这与舞台颜色相同！

\--- task \--- 添加一些代码来创建橡皮擦。

\---提示\--- \---提示\--- 向铅笔精灵添加一些代码： `当我收到`{：class =“block3events”}时， `橡皮擦`{：class =“block3events”}消息 `切换到服装橡皮擦`{：class =“block3looks”} `将笔颜色`{：class =“block3extensions”}设置为白色 \--- /提示\--- \---提示\--- 以下是您需要的所有块：

```blocks3
当我收到[橡皮擦v]

开关服装（橡皮擦v）时，将笔颜色设置为[#FFFFFF]

```

\--- /提示\--- \---提示\--- 这是代码的样子： ![铅笔](images/pencil.png)

```blocks3
当我收到[橡皮擦v]
开关服装（橡皮擦v）
套笔颜色为[#FFFFFF]
```

\--- /提示\--- \--- /提示\--- \--- /任务\---

\--- task \--- 测试你的项目，看看你是否可以清除舞台并擦除铅笔线。

![截屏](images/paint-erase-test.png) \--- /task \---

铅笔还有一个问题：你可以在舞台上的任何地方画画，包括“透明”和橡皮擦按钮附近！

![截屏](images/paint-draw-problem.png)

\--- task \--- 要解决此问题，请更改代码，以便在单击鼠标时仅向下笔 **和** 鼠标指针的 `y` 位置大于 `-120`：

![铅笔](images/pencil.png)

```blocks3
当标记点击时
擦除所有
开关服装（铅笔蓝色v）
设置笔颜色为[＃0035FF]
永远
  转到（鼠标指针v）
+如果 <<mouse down?> 和 <（鼠标y） > [-120]>> 然后 
  笔下来
  其他
  笔下来
结束
```

\--- /task \---

\--- task \--- 测试你的项目。 你现在不应该在按钮附近画画。

![截屏](images/paint-fixed.png) \--- /task \---