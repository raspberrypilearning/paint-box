## रंगीन पेंसिलें

चलिए अपने प्रोजेक्ट में विभिन्न रंगों के पेंसिल जोड़ें, और उपयोगकर्ता को उनके बीच चुनने की अनुमति दें!

+ अपने पेंसिल स्प्राइट पर क्लिक करें, 'पोशाक' पर क्लिक करें और अपनी 'पेंसिल-नीली' पोशाक की नकल(duplicate) बनाएँ।

![screenshot](images/paint-blue-duplicate.png)

+ अपनी नई पोशाक 'पेंसिल-हरी' को नया नाम दें, और पेंसिल को हरे रंग में रंग दें।

![screenshot](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ दो नई स्प्राइट बनाएँ - एक नीला वर्ग(square) और एक हरा वर्ग। आप इनका उपयोग नीली या हरी पेंसिल चुनने के लिए करेंगे।

![screenshot](images/paint-selectors.png)

+ अपने sprites का पुनः नाम रखें ताकि उन्हें 'नीला' और 'हरा' कहा जाए।

+ 'हरे' स्प्राइट में कुछ कोड जोड़ें ताकि जब इसे क्लिक किया जाए, तो यह पेंसिल स्प्राइट को संदेश "हरा" `प्रसारित` {: class = "blockevents"} करें, उसे अपनी पोशाक और पेंसिल का रंग बदलने के लिए बताएं।

![Broadcast green](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ अपने पेंसिल स्प्राइट पर जाए। कुछ कोड जोड़ें ताकि जब इस स्प्राइट को हरा(green) `प्रसारण`{: class = "blockevents"} प्राप्त हो, तो उसका पेंसिल पोशाक और कलम का रंग हरा हो जाए।

![Broadcast green](images/broadcast-green.png)

पेंसिल को हरे रंग करने पर सेट करने के लिए, `रंग सेट करें`{:class="blockpen"} ब्लॉक में रंगीन बॉक्स पर क्लिक करें, और अपने पेंसिल रंग के समान रंग का चयन करने के लिए हरे रंग के स्प्राइट पर क्लिक करें।

+ नीले पेंसिल आइकन के साथ भी ऐसा कर सकते हैं: इस कोड को नीले वर्ग(square) स्प्राइट से जोड़े:

```blocks
जब यह स्प्राइट क्लिक किया जाए
प्रसारण करें [blue v]
```

...और इस कोड को अपने पेंसिल स्प्राइट से जोड़ें:

```blocks
मुझे [blue v] प्राप्त हो
पोशाक बदल कर [pencil-blue v] करें
पेन का रंग [#0000ff] सेट करें
```

+ Finally, add this code to tell the pencil sprite which colour to start with, and make sure that the screen is clear.

![Start pencil](images/start-pencil.png)

We chose to start with blue but if you prefer, you can start with a different colour pencil.

+ Test out your project. Can you switch between blue and green pens by clicking on the blue or green square sprites?

![screenshot](images/paint-pens-test.png)