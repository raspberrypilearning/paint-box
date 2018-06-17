## 改变铅笔宽度

让我们允许用户使用不同粗细的铅笔来绘图。

+ 首先，新建一个名为`宽度`{:class="blockvariable"}的变量。

[[[generic-scratch-add-variable]]]

+ 将这行代码添加到铅笔代码的`重复执行`{:class="blockcontrol"} 循环*内*：

```blocks
    笔迹宽度设为 (宽度)
```

现在铅笔的宽度会不断地被设置为变量“宽度”的值。

+ Right click on the variable display on the stage and click 'slider'.

![screenshot](images/paint-slider.png)

You can now drag the slider below the variable to change its value.

![screenshot](images/paint-slider-change.png)

+ Test your project, and see if you can modify the pencil width.

![screenshot](images/paint-width-test.png)

If you prefer, you can set the minimum and maximum value of 'width' that's allowed. To do this, right-click on the variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![screenshot](images/paint-slider-max.png)

Keep testing your 'width' variable until you're happy.