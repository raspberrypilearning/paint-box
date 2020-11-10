## 間違いを元に戻す

時々起きる間違いのために、「クリア」ボタンと消しゴムボタンを追加します。

\--- task \---

ライブラリの文字セクションから「Block-X」スプライトを追加します。 スプライトのコスチュームを赤で着色し、少し小さくします。 このスプライトが「クリア」ボタンです。

[[[generic-scratch3-sprite-from-library]]]

![スクリーンショット](images/paint-x.png)

\--- /task \---

\--- task \---

「Block-X」スプライトにコードを追加して、スプライトがクリックされたときにステージをクリアします。

![クロス](images/cross.png)

```blocks3
このスプライトが押されたとき
全部消す
```

\--- /task \---

ステージをクリアするのに`メッセージを送る`{:class="block3events"}を使用する必要はありません。なぜなら、`全部消す`{:class="block3extensions"}ブロックで事が済むするからです。

鉛筆のスプライトに消しゴムのコスチュームが含まれているのが分かりますか？

![スクリーンショット](images/paint-eraser-costume.png)

プロジェクトには別に消しゴムのスプライトも含まれています。

\--- task \---

Click on this eraser sprite and then select **show**.

![スクリーンショット](images/show-eraser.png)

Here is how your Stage should look now:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
このスプライトが押されたとき
(消しゴム v) を送る
```

\--- /task \---

When the pencil sprite receives the 'eraser' message, it should switch its costume to the eraser and switch the pen colour to white, which is the same colour as the Stage!

\--- task \---

Add some code to create the eraser.

\--- hints \--- \--- hint \---

Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

\--- /hint \--- \--- hint \---

Here are all the blocks you need:

```blocks3
ペンの色を [#FFFFFF] にする
[消しゴム v] を受け取ったとき

コスチュームを (消しゴム v) にする
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
[消しゴム v] を受け取ったとき
コスチュームを (消しゴム v) にする
ペンの色を [#FFFFFF] にする
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \---

Test your project to see if you can clear the Stage and erase pencil lines.

![screenshot](images/paint-erase-test.png)

\--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![screenshot](images/paint-draw-problem.png)

\--- task \---

To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![pencil](images/pencil.png)

```blocks3
⚑ が押されたとき
全部消す
コスチュームを (鉛筆-青 v) にする
ペンの色を [#0035FF] にする
ずっと 
  (マウスのポインター v) へ行く
  +もし <<mouse down?> かつ <(マウスのy座標) > [-120]>> なら 
    ペンを下ろす
  でなければ 
    ペンを上げる
  end
end
```

\--- /task \---

\--- task \---

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---