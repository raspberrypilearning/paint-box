## गलतियों को पूर्ववत करें

कभी-कभी गलती हो जाती है, तो चलिए अपने प्रोजेक्ट में 'clear' बटन और रबड़ जोड़ें!

--- task ---

लायब्रेरी के letters अनुभाग से 'X-block' स्प्राइट जोड़ें। स्प्राइट के कॉस्ट्यूम को लाल रंग जोड़े और थोड़ा छोटा बना दीजिये। यह स्प्राइट आपका 'Clear' बटन है।

[[[generic-scratch3-sprite-from-library]]]

![स्क्रीनशॉट](images/paint-x.png)

--- /task ---

--- task ---

'X-block' स्प्राइट में कोड जोड़ें ताकि जब यह क्लिक किया जाए तो स्टेज साफ हो जाए।

![cross](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

--- /task ---

आपको स्टेज को साफ़ करने के लिए `broadcast`{:class="block3events"} का उपयोग करने की आवश्यकता नहीं है, क्योंकि `erase all`{:class="block3extensions"} ब्लॉक वह काम करता है।

क्या आप देखते हैं कि पेंसिल स्प्राइट में रबड़(Eraser) कॉस्ट्यूम भी शामिल है?

![स्क्रीनशॉट](images/paint-eraser-costume.png)

आपके प्रोजेक्ट में एक अलग से रबड़ स्प्राइट भी शामिल है।

--- task ---

इस eraser स्प्राइट पर राइट-क्लिक करें और फिर **show(दिखाइये)** पर क्लिक करें। यहां बताया गया है कि आपका स्टेज अब कैसा दिखना चाहिए:

![स्क्रीनशॉट](images/paint-eraser-stage.png)

--- /task ---

--- task ---

Eraser स्प्राइट में `'eraser' broadcast`{:class="block3events"} भेजने के लिए कोड जोड़ें ताकि जब eraser स्प्राइट पर क्लिक किया जाता है तब यह कोड चले।

![रबड़](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

--- /task ---

जब पेंसिल स्प्राइट से 'eraser' संदेश प्राप्त होता है, तो उसे अपनी कॉस्ट्यूम को eraser में बदलना चाहिए और पेन के रंग को सफेद रंग में बदलना चाहिए, जो कि स्टेज का ही रंग है!

--- task ---

रबड़ बनाने के लिए कुछ कोड जोड़ें

--- hints --- --- hint ---

Pencil स्प्राइट में कुछ कोड जोड़ें: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

--- /hint --- --- hint ---

यहां वे सभी ब्लॉक हैं जिनकी आपको आवश्यकता है:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

--- /hint --- --- hint ---

आपका कोड ऐसा दिखना चाहिए:

![पेंसिल](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

--- /hint --- --- /hints --- --- /task ---

--- task ---

आपके प्रोजेक्ट का निरीक्षण करें यह देखने के लिए कि क्या आप स्टेज को खाली कर सकते हैं और पेंसिल लाइनों को मिटा सकते हैं।

![स्क्रीनशॉट](images/paint-erase-test.png)

--- /task ---

पेंसिल में एक और समस्या है – आप स्टेज पर कहीं भी चित्र बना सकते हैं, clear और eraser बटनों पर भी!

![स्क्रीनशॉट](images/paint-draw-problem.png)

--- task ---

इसे ठीक करने के लिए, कोड को बदलें ताकि पेन केवल नीचे हो अगर माउस को क्लिक किया गया है ** और(and)** `y` माउस पॉइंटर की स्थिति ` -120` से अधिक हों।

![पेंसिल](images/pencil.png)

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

--- /task ---

--- task ---

अपने प्रोजेक्ट का परीक्षण करें। अब आप बटनों के पास ड्रा नही कर पाएंगे।

![स्क्रीनशॉट](images/paint-fixed.png)

--- /task ---