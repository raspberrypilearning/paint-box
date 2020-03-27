## ペン幅を変える

次に、コードを追加して、このプログラムを使用する人がそれぞれのペン幅で描画できるようにします。

\--- task \---

まず最初に、`幅`{:class="block3variables"}という新しい変数を追加します。

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

鉛筆スプライトコードの`ずっと`{:class="block3control"}ループの**内部に**この行を追加します。

```blocks3
⚑ が押されたとき
全部消す
コスチュームを (鉛筆-青 v) にする
ペンの色を [#0035FF] にする
ずっと 
  (マウスのポインター v) へ行く
  +ペンの太さを (幅:: variables) にする
  もし <<mouse down?> かつ <(マウスのy座標) > [-120]>> なら 
    ペンを下ろす
  でなければ 
    ペンを上げる
  end
end
```

\--- /task \---

ペンの幅は`幅`{:class="block3variables"}変数の値に繰り返し設定されます。

\--- task \---

ステージに表示された`幅`{:class="block3variables"}変数を右クリックし、**スライダー**をクリックします。

![スクリーンショット](images/paint-slider.png)

\--- /task \---

変数の下に表示されているスライダーをドラッグして変数の値を変更できます。

![スクリーンショット](images/paint-slider-change.png)

\--- task \---

プロジェクトをテストして、ペン幅を調整するコードを追加できたかどうか確認します。

![スクリーンショット](images/paint-width-test.png)

\--- /task \---