## 鉛筆を作る

あなたがステージ上に描画するために使用できる鉛筆を作ることから始めます。

\--- task \--- 'Paint box' Scratchスタータープロジェクトを開きます。

**オンライン**： [スタータープロジェクトを開くrpf.io/paint-box-on](http://rpf.io/paint-box-on){：target = "_ blank"}

**オフライン**：オフラインエディタで [スタータープロジェクト](http://rpf.io/p/en/paint-box-go){：target = "_ blank"}を開きます。

Scratchオフラインエディタをダウンロードしてインストールする必要がある場合は、 [検索できます。rpf.io/scratchoff](http://rpf.io/scratchoff){：target = "_ blank"}

スタータープロジェクトでは、鉛筆と消しゴムのスプライトが表示されます。

![スクリーンショット](images/paint-starter.png) \--- /task \---

\--- task \---

プロジェクトにペン拡張機能を追加します。

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

描画できるように、コードを鉛筆のスプライトに追加して、スプライトがマウスポインタ `永遠に`追従するようにします` {：class = "block3control"}</p>

<p><img src="images/pencil.png" alt="鉛筆" /></p>

<pre><code class="blocks3">フラグが永遠に
クリックしたとき
  （マウスポインタv）
端に移動
`</pre> 

\--- /task \---

\--- task \--- フラグをクリックし、ステージ上でマウスポインタを動かしてコードが機能するかどうかをテストします。 \--- /task \---

次に、</code>{：class = "block3control"}マウスボタンがクリックされている場合にのみ鉛筆に `描画させます。</p>

<p>--- task ---
このコードを鉛筆のスプライトに追加してください：</p>

<p><img src="images/pencil.png" alt="鉛筆" /></p>

<pre><code class="blocks3">フラグがいつまでも
クリックしたとき
  （マウスポインタv）

+ <mouse down?>
  下の
  それ以外
  上、

`</pre> 

\--- /task \---

\--- task \--- もう一度コードをテストしてください。 今度は、ステージ上で鉛筆を動かし、マウスボタンを押したままにします。 うまく絵がかけましたか？

![スクリーンショット](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title：鉛筆は先端から引いていませんか

鉛筆で描いた線が鉛筆の中央から来ているように見える場合は、ペン先のスプライトを変更して、先端がスプライトの中心になるようにする必要があります。

鉛筆のスプライトをクリックしてから、 **Costumes** タブをクリックします。

鉛筆の先が中心の</strong> の真上の **になるように衣装を動かします。</p> 

![コスチュームセンター](images/costume-center-annotated.png)

次にステージ上で鉛筆を動かして描画します。 鉛筆はその先端から線を引くはずです。

\--- /collapse \---