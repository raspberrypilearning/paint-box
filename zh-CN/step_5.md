## 孰能无过

有时我们会画错，所以让我们加入“清除”按钮和橡皮。

+ 添加‘X-block'角色 -- 你可以在角色库的字母分类中找到它。 将造型改为红色。 这样就变为了“清除”按钮。

![screenshot](images/paint-x.png)

+ 向清除按钮中添加代码，让它被点击时清空舞台上的内容。

![Clear stage](images/clear-stage.png)

注意你不需要通过发送消息来清空舞台，你可以直接在角色中使用清空代码块。

你可能已经发现铅笔角色包含来一个橡皮造型：

![screenshot](images/paint-eraser-costume.png)

+ 项目中还包含一个单独的橡皮角色。 Right click on this sprite and choose 'show'. Here is how your stage should look:

![screenshot](images/paint-eraser-stage.png)

+ Add code to the eraser sprite, to tell the pencil to switch to an eraser when the sprite is clicked.

![Broadcast eraser](images/broadcast-eraser.png)

When the pencil receives the "eraser" message, you can switch the pencil costume to the eraser, and switch the pencil colour to white - the same colour as the stage!

+ Add some code to create the eraser

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: **When I receive** the **eraser** message **Switch to costume** eraser **Set pen color** to white \--- /hint \--- \--- hint \--- Here is how the code inside the pencil sprite should look:

```blocks
when I receive [eraser v]
switch costume to [eraser v]
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Test your project, to see if you can clear and erase on the stage.

![screenshot](images/paint-erase-test.png)

There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

![screenshot](images/paint-draw-problem.png)

To fix this, tell the pencil only to draw if the mouse is clicked *and* if the y-position of the mouse is greater than -120:

![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

![screenshot](images/paint-fixed.png)