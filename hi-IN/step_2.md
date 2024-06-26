## पेंसिल बनाना

चलिए ऐसी पेंसिल बनाने से आंरभ करें, जिसे स्टेज पर चित्र बनाने के लिए उपयोग किया जा सकता है।

--- task ---

'पेंट बॉक्स' Scratch स्टार्टर प्रोजेक्ट खोलें।

**ऑनलाइन**: [rpf.io/paint-box-on](https://rpf.io/paint-box-on){:target="_blank"} पे से स्टार्टर प्रोजेक्ट खोलिये

यदि आपके पास एक Scratch खाता है, तो आप **Remix** पर क्लिक करके प्रतिलिपि बना सकते हैं।

**ऑफलाइन**: [स्टार्टर प्रोजेक्ट](https://rpf.io/p/hi-IN/paint-box-go){:target="_blank"} को ऑफलाइन एडिटर में खोलिये।

अगर आपके पास Scratch ऑफलाइन एडिटर नहीं है, तो आप यहाँ से उसे डाउनलोड कर सकते है [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}

स्टार्टर प्रोजेक्ट में, आपको पेंसिल और रबड़ स्प्राइट दिखाई देना चाहिए:

![स्क्रीनशॉट](images/paint-starter.png)

--- /task ---

--- task ---

अपने प्रोजेक्ट में Pen एक्सटेंशन जोड़ें।

[[[generic-scratch3-add-pen-extension]]]

--- /task ---

--- task ---

आपके पेंसिल स्प्राइट पर कोड जोड़े ताकि आप माउस पॉइंटर के पीछे पीछे `हमेशा (forever)`{:class="block3control"} स्प्राइट को ले जा सके ताकि आप यह बना सके:

![पेंसिल](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

--- /task ---

--- task ---

झंडे पर क्लिक करें और फिर माउस को स्टेज के चारों ओर ले जाएं यह जांचने के लिए की कोड काम करता है या नहीं।

--- /task ---

अभी, यह निश्चित कीजिये की आपका पेंसिल तभी लिख सकता है `जब (if)`{:class="block3control"} माउस क्लिक किया गया हो।

--- task ---

इस कोड को अपने पेंसिल स्प्राइट में जोड़ें:

![पेंसिल](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)

+ if <mouse down?> then
  pen down
  else
  pen up
end
```

--- /task ---

--- task ---

अपने कोड का फिर से परीक्षण करें। इस बार, स्टेज के चारों ओर पेंसिल को ले जाएं और माउस बटन दबाए रखें। क्या आप अपने पेंसिल से चित्र बना सकते हैं?

![स्क्रीनशॉट](images/paint-draw.png)

--- /task ---

--- collapse ---
---
title: क्या आपकी पेंसिल इसकी नोक से रेखा नहीं निकलती है?
---
अगर आपका पेंसिल बिच में से चित्र बना रहा है, तोह आपको अपनी पेंसिल स्प्राइट को बदलना पड़ेगा ताकि पेंसिल का नोक इस नए स्प्राइट के तीख बीच में है।

अब पेंसिल स्प्राइट पर क्लिक हरे, और फिर **Costumes** टैब पर क्लिक करे।

कॉस्ट्यूम को हटाइये ताकि आपकी पेंसिल की नोक पेंसिल के बीच से **सिर्फ तोड़ा ऊपर** रहे।

![पोशाक केंद्र](images/costume-center-annotated.png)

अब स्टेज पर पेंसिल को घुमाएँ और ड्रा करें। पेंसिल को अब अपने सिरे से एक रेखा खींचनी चाहिए।

--- /collapse ---
