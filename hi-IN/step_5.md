## पेंसिल की चौड़ाई में परिवर्तन करना

कभी-कभी गलती हो जाती है, तो चलिए अपने प्रोजेक्ट में 'साफ़ करें' बटन और रबड़ जोड़ें!

\--- task \--- लाइब्रेरी के लेटर्स में से 'एक्स-ब्लॉक' स्प्राइट कोड़े। स्प्राइट के कस्टम को लाल और थोड़ा छोटा बना दीजिये। यह स्प्राइट आपकी 'साफ़ करें' बटन है।

[[[generic-scratch3-sprite-from-library]]]

![स्क्रीनशॉट](images/paint-x.png) \--- /task \---

\--- task \--- Add code to the 'X-block' sprite to clear the Stage when the sprite clicked.

![cross](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- /task \---

You don't need to use a `broadcast`{:class="block3events"} to clear the Stage, because the `erase all`{:class="block3extensions"} block does that job.

Do you see that the pencil sprite includes an eraser costume?

![स्क्रीनशॉट](images/paint-eraser-costume.png)

आपके प्रोजेक्ट में एक अलग से रबड़ स्प्राइट भी शामिल है।

\--- task \--- Right-click on this eraser sprite and then click on **show**. Here is how your Stage should look now:

![स्क्रीनशॉट](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

\--- /task \---

When the pencil sprite receives the 'eraser' message, it should switch its costume to the eraser and switch the pen colour to white, which is the same colour as the Stage!

\--- task \--- रबड़ बनाने के लिए कुछ कोड जोड़ें

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white \--- /hint \--- \--- hint \--- Here are all the blocks you need:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

\--- /hint \--- \--- hint \--- आपका कोड कुछ ऐसा दिखना चाहिए: ![pencil](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Test your project to see if you can clear the Stage and erase pencil lines.

![स्क्रीनशॉट](images/paint-erase-test.png) \--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![स्क्रीनशॉट](images/paint-draw-problem.png)

\--- task \--- To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

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

\--- task \--- Test your project. You now should not be able to draw near the buttons.

![स्क्रीनशॉट](images/paint-fixed.png) \--- /task \---