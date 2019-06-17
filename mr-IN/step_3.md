## रंगीत पेन्सिल

आता आपण आपल्या प्रोजेक्टमध्ये भिन्न रंगीत पेन्सिल जोडणार आहात आणि वापरकर्त्यास त्या दरम्यान निवडण्याची परवानगी देऊ शकता.

\--- task \--- Rename the `pencil` sprite to `pencil-blue`

![rename-pencil](images/rename-pencil.png) \--- / कार्य \---

\--- task \--- Right click on the pencil sprite, and duplicate the 'pencil-blue' costume.

![screenshot](images/paint-blue-duplicate.png) \--- /task \---

\--- task \--- Name the new costume 'pencil-green', and colour the pencil green.

![screenshot](images/paint-pencil-green.png)

\--- / कार्य \---

\--- task \--- Draw two new sprites: one blue square and one green square. These are for choosing between the blue and green pencil.

![screenshot](images/paint-selectors.png) \--- /task \---

\--- task \--- Rename the new sprites so that they are called 'blue' and 'green'

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- Add some code to the 'green' sprite so that when this sprite is clicked, it `broadcasts`{:class="block3events"} the message "green".

![green square](images/green_square.png)

```blocks3
जेव्हा या स्प्राइटने
प्रसारण (हिरव्या v) क्लिक केले
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

The pencil sprite should listen for the "green" message and change its costume and pencil colour in response.

\--- task \--- Switch to your pencil sprite. Add some code so that when this sprite receives the `green`{:class="block3events"} broadcast, it switchs to the green pencil costume and changes the pen colour to green.

![pencil](images/pencil.png)

```blocks3
जेव्हा मी [हिरवे व्ही]
स्विच कॉस्च्यूम (पेन्सिल-ग्रीन व्ही)
सेट पेन रंग [# 00CC44] प्राप्त करतो
```

To set the pencil to colour to green, click the coloured square in the `set pen color`{:class="block3extensions"} block, and then click on the green square sprite. \--- /task \---

Then to a similar thing so that you can switch the pencil colour to blue.

\--- task \--- Click on the blue square sprite and add this code:

![blue_square](images/blue_square.png)

```blocks3
जेव्हा या स्प्राइटने
प्रसारण (निळा वी) क्लिक केले
```

Then click on the pencil sprite and add this code: ![pencil](images/pencil.png)

```blocks3
जेव्हा मी [निळा व्ही]
स्विच कॉस्च्युम (पेन्सिल-ब्लू व्ही)
सेट पेन रंग [# 0000ff] वर प्राप्त करते
```

\--- /task \---

\--- task \--- Finally, add this code to tell the pencil sprite which colour to start with, and to make sure that the screen is clear when your program starts.

![pencil](images/pencil.png)

```blocks3
जेव्हा ध्वज
क्लिक केले तेव्हा सर्व
+ स्विच कॉस्च्यूम (पेन्सिल-ब्लू व्ही)
+ सेट पेन कलर [# 0035FF]
कायमचे काढावे
  (माउस पॉइंटर विरुद्ध)
 <mouse down?> असल्यास
  पेन डाउन

  पेन अप
अंत
```

\--- /task \---

If you prefer, you can start with a different colour pencil.

\--- task \--- Test your code. Can you switch between the blue and green pencil colours by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png) \--- /task \---