## रंगीन पेंसिलें

अब आप कई अलग रंगो के पेंसिल आपने प्रोजेक्ट में जोड़ेंगे और आप अब यूजर को उन में से एक चुननेका अनुमति देंगे।

\--- task \--- `पेंसिल` स्प्राइट का नाम `पेंसिल-नीली` में बदलें

![rename-pencil](images/rename-pencil.png) \--- /task \---

\--- task \--- अपने पेंसिल स्प्राइट पर राइट क्लिक कीजिये, और फिर 'पेंसिल-ब्लू' कस्टम का एक और कॉपी बनाइये।

![स्क्रीनशॉट](images/paint-blue-duplicate.png) \--- /task \---

\--- task \--- अपने नए कस्टम को 'पेंसिल-हरी' का नाम दे दीजिये, और फिर उसका रंग हरा कर दीजिये।

![स्क्रीनशॉट](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- दो नए स्प्राइट बनाये: एक नीला वर्ग और एक हरी वर्ग। ये नीले और हरे रंग की पेंसिल के बीच चुनने के लिए हैं।

![स्क्रीनशॉट](images/paint-selectors.png) \--- /task \---

\--- task \--- नए स्प्राइट का नाम बदलें ताकि उन्हें 'नीला' और 'हरा' कहा जाए

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- 'ग्रीन' स्प्राइट में कुछ कोड जोड़ें ताकि जब इस स्प्राइट पर क्लिक किया जाए, तो यह संदेश" ग्रीन "` प्रसारित करे` {"class =" block3events "}।

![हरा वर्ग](images/green_square.png)

```blocks3
when this sprite clicked
broadcast (green v)
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

पेंसिल स्प्राइट को "हरे" संदेश के लिए सुनना चाहिए और इसकी पोशाक और पेंसिल का रंग बदलना चाहिए।

\--- task \--- अपने पेंसिल स्प्राइट को बदले। अपने स्प्राइट में ऐसी कोड जोड़े ताकि जब यह स्प्राइट इस `हरी`{:class="block3events"} मैसेज सुने तब यह हरी पेंसिल में बदल जाये।

![पेंसिल](images/pencil.png)

```blocks3
when I receive [green v]
switch costume to (pencil-green v)
set pen color to [#00CC44]
```

आपके पेंसिल के रंग को हरा बनाने के लिए, `सेट पेन कलर`{:class="block3extensions"} ब्लॉक के अंदर रंगीन वर्ग पर क्लिक करे, और फिर हरी वर्ग स्प्राइट पर क्लिक करे। \--- /task \---

फिर आप पेंसिल को नीले रंग में भी बदल सकते है।

\--- task \--- नीले वर्ग स्प्राइट पर क्लिक करे और यह कोड जोड़े:

![blue_square](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blue v)
```

फिर पेंसिल स्प्राइट पर क्लिक करे और यह कोड जोड़े: ![पेंसिल](images/pencil.png)

```blocks3
when I receive [blue v]
switch costume to (pencil-blue v)
set pen color to [#0000ff]
```

\--- /task \---

\--- task \--- अंत में, पेंसिल स्प्राइट को किस रंग के साथ चालू होना है, बताने के लिए इस कोड को जोड़े और सुनिश्चित करें कि स्क्रीन साफ़ हो।

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

यदि आप चाहे, तोह आप अलग रंग से भी चालू कर सकते है।

\--- task \--- अपने कोड का परीक्षण करें। क्या आप नीले या हरे रंग के वर्ग पर क्लिक करके नीले और हरे रंग के पेन बदल सकते हैं?

![स्क्रीनशॉट](images/paint-pens-test.png) \--- /task \---