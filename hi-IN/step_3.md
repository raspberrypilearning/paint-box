## रंगीन पेंसिलें

अब आप कई अलग रंगो की पेन्सिलें आपने प्रोजेक्ट में जोड़ेंगे और आप अब यूजर को उन में से एक चुनने की अनुमति देंगे।

\--- task \---

'Pencil' स्प्राइट के Costumes टैब पर क्लिक करें।

`pencil-a` पोशाक का नाम बदलकर `pencil-blue` रखें

![नाम बदलें-पेंसिल](images/rename-pencil.png)

\--- /task \---

\--- task \---

pencil-blue पोशाक पर राइट क्लिक करें और **duplicate** चुनें।

![स्क्रीनशॉट](images/paint-blue-duplicate.png)

\--- /task \---

\--- task \---

नई पोशाक को 'pencil-green' नाम दें, और पेंसिल को हरा रंग दें।

![स्क्रीनशॉट](images/paint-pencil-green.png)

\--- /task \---

\--- task \---

दो नए स्प्राइट ड्रॉ करें: एक नीला चौकोर और एक हरा चौकोर। ये नीले और हरे रंग की पेंसिल के बीच चुनने के लिए हैं।

![स्क्रीनशॉट](images/paint-selectors.png)

\--- /task \---

\--- task \---

नए स्प्राइट्स का नाम बदलें ताकि उन्हें 'blue' और 'green' कहा जाए

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \---

'green' स्प्राइट में कुछ कोड जोड़ें ताकि जब इस स्प्राइट पर क्लिक किया जाए, तो यह "green" संदेश को `broadcast`{:class="block3events"} करे।

![हरा चौकोर](images/green_square.png)

```blocks3
when this sprite clicked
broadcast (green v)
```

[[[generic-scratch3-broadcast-message]]]

\--- /task \---

पेंसिल स्प्राइट को "green" संदेश को सुनना चाहिए और इसकी प्रतिक्रिया में अपनी पोशाक और पेंसिल के रंग को बदलना चाहिए।

\--- task \---

अपने पेंसिल स्प्राइट पर जाए। अपने स्प्राइट में ऐसी कोड जोड़े ताकि जब यह स्प्राइट इस `green`{:class="block3events"} संदेश को सुनता है तब यह पेंसिल के कॉस्ट्यूम और पेन के रंग को हरें में बदल दें।

![पेंसिल](images/pencil.png)

```blocks3
when I receive [green v]
switch costume to (pencil-green v)
set pen color to [#00CC44]
```

आपके पेंसिल के रंग को हरा बनाने के लिए, `set pen color`{:class="block3extensions"} ब्लॉक के अंदर रंगीन चौकोर पर क्लिक करे, और फिर हरे चौकोर स्प्राइट पर क्लिक करे।

\--- /task \---

फिर इसी तरह की बात करें ताकि आप पेंसिल के रंग को नीले रंग में बदल सकें।

\--- task \---

नीले चौकोर स्प्राइट पर क्लिक करें और इस कोड को जोड़ें:

![नीला_चौकोर](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blue v)
```

फिर पेंसिल स्प्राइट पर क्लिक करें और यह कोड जोड़ें:

![पेंसिल](images/pencil.png)

```blocks3
when I receive [blue v]
switch costume to (pencil-blue v)
set pen color to [#0000ff]
```

\--- /task \---

\--- task \---

अंत में, इस कोड को पेंसिल स्प्राइट को बताने के लिए जोड़ें कि किस रंग से शुरू करना है, और यह सुनिश्चित करने के लिए कि आपका प्रोग्राम शुरू होने पर स्क्रीन साफ़ हो।

![पेंसिल](images/pencil.png)

```blocks3
when flag clicked
+erase all
+switch costume to (pencil-blue v)
+set pen color to [#0035FF]
forever
  go to (mouse pointer v)
if <mouse down?> then
  pen down
  else
  pen up
end
```

\--- /task \---

यदि आप चाहें, तो आप एक अलग रंग की पेंसिल से शुरू कर सकते हैं।

\--- task \---

अपने कोड का परीक्षण करें। क्या आप नीले या हरे रंग के चौकोर स्प्राइट पर क्लिक करके नीले और हरे रंग के पेंसिल रंगों के बीच बदल कर सकते हैं?

![स्क्रीनशॉट](images/paint-pens-test.png)

\--- /task \---