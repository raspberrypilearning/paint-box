## पेन रुंदी बदला

पुढे आपण आपल्या प्रोग्रामचा वापर करणार्या व्यक्तीस वेगवेगळ्या पेन रुंदीसह वस्तू काढण्यासाठी अनुमती देण्यासाठी कोड जोडाल.

--- task ---

प्रथम `width`{:class="block3variables"} अर्थात रुंदी नावाचे नवीन व्हेरिएबल जोडा.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

ही ओळ **inside** अर्थात आतल्या `forever`{:class="block3control"} अर्थात कायमच्या पेन्सिल स्प्राइटच्या लूप मघ्ये टाका:

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

--- /task ---

पेन रूंदी आता वारंवार `width`{:class="block3variables"} अर्थात रुंदीच्या मूल्यावर सेट केली जाते.

--- task ---

`width`{:class="block3variables"} अर्थात रुंदीवर उजवे क्लिक करा आणि नंतर **slider** क्लिक करा.

![स्क्रीनशॉट](images/paint-slider.png)

--- /task ---

व्हेरिएबलचे मूल्य बदलण्यासाठी आपण व्हेरिएबलच्या खाली दिसणारे स्लाइडर ड्रॅग करू शकता.

![स्क्रीनशॉट](images/paint-slider-change.png)

--- task ---

आपल्या प्रोजेक्टची चाचणी घ्या आणि आपण पेन रूंदी बदलू शकता की नाही ते पहा.

![स्क्रीनशॉट](images/paint-width-test.png)

--- /task ---