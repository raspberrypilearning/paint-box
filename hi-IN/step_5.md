## गलतियाँ करना

कभी-कभी गलती हो जाती है, तो चलिए अपने प्रोजेक्ट में 'साफ़ करें' बटन और रबड़ जोड़ें!

+ 'X-block' स्प्राइट जोड़ें - आप इसे अक्षर अनुभाग के लाइब्रेरी में पाएंगे। पोशाक को लाल में रंगे। यह 'साफ' बटन बन जाएगा।

![screenshot](images/paint-x.png)

+ इस स्प्राइट में कोड जोड़ें ताकि जब यह क्लिक किया जाए तो स्टेज साफ हो जाए।

![Clear stage](images/clear-stage.png)

ध्यान दें कि आपको स्टेज को साफ करने के लिए संदेश नहीं भेजना होगा, आप इस स्प्राइट से 'साफ' ब्लॉक का उपयोग कर सकते हैं।

शायद आपने ध्यान दिया होगा कि आपके पेंसिल स्प्राइट में रबड़ पोशाक शामिल है:

![screenshot](images/paint-eraser-costume.png)

+ आपके प्रोजेक्ट में एक अलग से रबड़ स्प्राइट भी शामिल है। इस स्प्राइट पर राइट क्लिक करें और 'दिखाए(show)' चुनें। यहाँ दिखाया गया है कि कैसा आपका स्टेज दिखना चाहिए:

![screenshot](images/paint-eraser-stage.png)

+ स्प्राइट क्लिक होने पर पेंसिल को रबड़ होने के लिए रबड़ स्प्राइट में कोड जोड़ें।

![Broadcast eraser](images/broadcast-eraser.png)

जब पेंसिल को "रबड़(eraser)" संदेश प्राप्त होता है, तो आप पेंसिल पोशाक को रबड़ में बदल सकते हैं, और पेंसिल रंग को सफेद बदल सकते हैं - स्टेज के समान रंग!

+ रबड़ बनाने के लिए कुछ कोड जोड़ें

\--- hints \--- \--- hint \--- पेंसिल स्प्राइट में कुछ कोड जोड़ें: **जब मुझे** **रबड़** संदेश प्राप्त हो **पोषक बदल जाए** रबड़ में **पेन बदल जाए** सफेद रंग में \--- /hint \--- \--- hint \--- यहाँ बताया गया है कि पेंसिल स्प्राइट के अंदर कोड कैसे दिखना चाहिए::

```blocks
जब मुझे [blue v] प्राप्त हो
पोशाक बदल कर [pencil-blue v] करें
पेन का रंग [#FFFFFF] सेट करें
```

\--- /hint \--- \--- /hints \---

+ Test your project, to see if you can clear and erase on the stage.

![screenshot](images/paint-erase-test.png)

There's one more problem with the pencil - you can draw anywhere on the stage, including near the selector icons!

![screenshot](images/paint-draw-problem.png)

To fix this, tell the pencil only to draw if the mouse is clicked *and* if the y-position of the mouse is greater than -120:

![screenshot](images/pencil-gt-code.png)

+ Test your project; you now shouldn't be able to draw near the selector blocks.

![screenshot](images/paint-fixed.png)