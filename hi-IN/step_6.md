## पेन की चौड़ाई बदलें

आगे, आप कोड जोड़ेंगे जो आपके प्रोग्राम का उपयोग करने वाले व्यक्ति को विभिन्न पेन चौड़ाई के साथ चीजों को ड्रॉ करने की अनुमति देगा।

\--- task \---

पहले, `width`{:class="blockvariable"} नामक नया वेरिएबल जोड़े।

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

इस लाइन को अपनी पेंसिल के कोड के `forever`{:class="blockcontrol"} लूप के **अंदर (inside)** जोड़ें:

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
go to (mouse pointer v)
+set pen size to (width :: variables)
if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

\--- /task \---

पेन की चौड़ाई अब बार-बार `width`{:class="block3variables"} वेरिएबल के मान पर सेट हो जाती है।

\--- task \---

स्टेज पर प्रदर्शित `width`{:class="block3variables"} वेरिएबल पर राइट-क्लिक करें, और फिर **slider** पर क्लिक करें।

![स्क्रीनशॉट](images/paint-slider.png)

\--- /task \---

अब आप वैरिएबल के मान को बदलने के लिए उसके नीचे दिखाई देने वाले स्लाइडर को खींच सकते हैं।

![स्क्रीनशॉट](images/paint-slider-change.png)

\--- task \---

अपनी प्रोजेक्ट का परीक्षण करें और देखें कि क्या आप पेन की चौड़ाई को बदलने के लिए कोड जोड़ सकते हैं।

![स्क्रीनशॉट](images/paint-width-test.png)

\--- /task \---