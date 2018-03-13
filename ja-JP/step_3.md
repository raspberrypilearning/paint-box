## えんぴつを作る

まず、ステージでお絵かきをするえんぴつを作ります。

+ 「お絵かきの箱」という名前のスクラッチ・プロジェクトを開きます。オンラインで開く場合はこちら[jumpto.cc/paint-go](http://jumpto.cc/paint-go){:target="_blank"} から、オフラインエディターを使う場合はこちら<http://jumpto.cc/paint-get>{:target="_blank"}からダウンロードして、プロジェクトを開きます。

えんぴつと消しゴムのスプライトが出てきます。

![screenshot](images/paint-starter.png)

+ えんぴつスプライトにコードを追加して、マウスに`ずっと`{:class="blockcontrol"}ついていって絵が描けるようにします。

```blocks
    旗がクリックされた時
　ずっと
　　マウスポインターへ行く
```

+ Click the flag and then move the mouse around the stage to test whether the code works.

Next, let's make your pencil only draw `if`{:class="blockcontrol"} the mouse has been clicked.

+ Add this code to your pencil sprite:

![screenshot](images/paint-pencil-draw-code.png)

+ Test your code again. This time, move the pencil around the stage and hold down the mouse button. Can you draw with your pencil?

![screenshot](images/paint-draw.png)

## \--- collapse \---

## title: If you're having problems...

If your pencil seems to be drawing the line from the middle of the pencil rather than the tip, you will need to change your costume center.

![Costume center](images/costume-center.png)

The crosshair for the pencil must be placed **just below** the tip of the pencil, not on the tip of the pencil.

A changes in a sprite's 'costume center' isn't registered until another tab is clicked, so click on another costume, or on the 'Scripts' tab to finalise your changes to the costume center.

\--- /collapse \---