## ስህተቶችን ቀልብስ

አንዳንድ ጊዜ ስህተቶች ይከሰታሉ, ስለዚህ 'ግልጽ' አዝራር እና የፍርሽ አዝራር ያክሉ.

\--- task \---

Add the 'X-block' sprite from the library's letters section. Colour the sprite's costume in red and make it a little smaller. This sprite is the 'clear' button.

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png)

\--- /task \---

\--- task \---

Add code to the 'X-block' sprite to clear the Stage when the sprite clicked.

![cross](images/cross.png)

```blocks3
ይህ sprite ጠቅ ጊዜ
ደምስስ ሁሉ
```

\--- /task \---

You don't need to use a `broadcast`{:class="block3events"} to clear the Stage, because the `erase all`{:class="block3extensions"} block does that job.

Do you see that the pencil sprite includes an eraser costume?

![screenshot](images/paint-eraser-costume.png)

Your project also includes a separate eraser sprite.

\--- task \---

Right-click on this eraser sprite and then click on **show**. Here is how your Stage should look now:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
ይህ ስፒድ
ስርጭትን (ጠቅላላውን)
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
[eraser v]

መቀየሪያ ሽፋን ወደ [#FFFFFF]
ሲጽፍ (pen er v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
[eraser v]
ተቀባይን ለመቀበል (ስቴክ ገራዘር v)
ለ [#FFFFFF] የቅዳሜ ቀለም ያዘጋጁ.
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
ባንዲራ ጠቅ ጊዜ
ደምስስ ሁሉንም
(እርሳስ-ሰማያዊ v) ይቀይሩ የሚኖሩት
[# 0035FF] ወደ ስብስብ ብዕር ቀለም
ለዘላለም
  እየተጓዙ (የመዳፊት ጠቋሚ v) ወደ
+ ከሆነ <<mouse down?> እና <(የመዳፊት y) > [-120]>> ከዚያም 
  ይፃረራሉ, ሌላ
  አስገባ
  መቋጫ
መጨረሻ
```

\--- /task \---

\--- task \---

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---