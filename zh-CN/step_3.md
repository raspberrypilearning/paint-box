## 创建铅笔

让我们从创建一支能在舞台上绘画的铅笔开始。

+ 在线打开“颜色盒”工程[jumpto.cc/paint-go](http://jumpto.cc/paint-go){:target="_blank"} 或者从 <http://jumpto.cc/paint-get>{:target="_blank"}下载离线项目用离线编辑器打开。

你将会看到铅笔和橡皮：

![screenshot](images/paint-starter.png)

+ 向铅笔中添加代码让它`永远`{:class="blockcontrol"} 跟随鼠标移动，这样你就可以画画了：

```blocks
    点击绿旗时
    重复无限次 
      定位到 [mouse pointer v] 位置
    end
```

+ 点击绿旗然后在舞台上移动鼠标测试代码是否正常工作。

接下来，我们让铅笔仅在`如果`{:class="blockcontrol"}鼠标点击的情况下绘画。

+ 将下面的代码添加到铅笔角色中：

![screenshot](images/paint-pencil-draw-code.png)

+ 再次测试代码。 这次，在舞台上按住鼠标左键并移动鼠标。 你能用铅笔画画吗？

![screenshot](images/paint-draw.png)

## \--- collapse \---

## title: 如果你遇到了困难...

如果你的铅笔看上去像是用铅笔中断在划线而不是铅笔尖划线，你需要修改造型的中心。

![Costume center](images/costume-center.png)

铅笔的中心十字线必须放置在笔尖的**正下方**，不要放置在笔尖上。

A changes in a sprite's 'costume center' isn't registered until another tab is clicked, so click on another costume, or on the 'Scripts' tab to finalise your changes to the costume center.

\--- /collapse \---