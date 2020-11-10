## தவறுகளை திரும்பப் பெறவும்(undo)

சில நேரங்களில் தவறுகள் நடக்கும், எனவே ஒரு 'clear' பொத்தானையும், ஒரு அழிப்பான்(eraser) பொத்தானையும் சேர்க்கவும்.

\--- task \---

நூலகத்தின் எழுத்துக்கள்(Letters) பிரிவில் இருந்து, 'X-block' sprite-ஐச் சேர்க்கவும். Sprite-இன் costume-க்கு சிவப்பு நிறத்தில் வண்ணம் பூசி, அதை கொஞ்சம் சிறியதாக ஆக்குங்கள். இந்த sprite-தான் 'clear' பொத்தான்.

[[[generic-scratch3-sprite-from-library]]]

![திரைப்பிடிப்பு](படங்கள்/paint-x.png)

\--- / பணி \---

\--- / பணி \---

Sprite -ஐக் கிளிக் செய்யும்போது, மேடையில் உள்ள அனைத்தையும் அழிப்பதற்கான குறியீட்டை 'X-block' sprite-இல் சேர்க்கவும்.

![குறுக்கு](படங்கள்/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- / பணி \---

மேடையில் உள்ள அனைத்தையும் அழிக்க நீங்கள் `broadcast`{: class = "block3extensions"} தொகுதியை பயன்படுத்தத் தேவையில்லை, ஏனெனில் `erase all`{: class = "block3extensions"} தொகுதி அந்த வேலையைச் செய்கிறது.

பென்சில் sprite, ஒரு அழிப்பான் costume-ஐயும் உள்ளடக்கியிருப்பதைப் பார்க்கிறீர்களா?

![திரைப்பிடிப்பு](படங்கள்/paint-eraser-costume.png)

உங்கள் திட்டத்தில் ஒரு தனி அழிப்பான் sprite-உம் உள்ளது.

\--- / பணி \---

Click on this eraser sprite and then select **show**.

![திரைப்பிடிப்பு](images/show-eraser.png)

Here is how your Stage should look now:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

\--- /task \---

When the pencil sprite receives the 'eraser' message, it should switch its costume to the eraser and switch the pen colour to white, which is the same colour as the Stage!

\--- task \---

Add some code to create the eraser.

\--- hints \--- \--- hint \---

Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

\--- / குறிப்பு \--- \--- குறிப்பு \---

Here are all the blocks you need:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
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
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
  go to (mouse pointer v)
+if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \---

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---