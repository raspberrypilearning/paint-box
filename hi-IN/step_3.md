## पेंसिल बनाना

आइए एक पेंसिल बनाकर शुरू करें जिसका उपयोग स्टेज पर खींच कर बनाने(draw) के लिए किया जा सकता है।

+ 'पेंटबॉक्स' स्क्रैच प्रोजेक्ट को ऑनलाइन इससे [jumpto.cc/paint-go](http://jumpto.cc/paint-go){:target="_blank"} खोलें या इससे डाउनलोड करें <http://jumpto.cc/paint-get>{:target="_blank"} और फिर यदि आप ऑफ़लाइन संपादक का उपयोग कर रहे हैं तो इसे खोलें।

आप पेंसिल और रबड़ स्प्राइट्स देखेंगे:

![screenshot](images/paint-starter.png)

+ `हमेशा के लिए(forever)` {: class = "blockcontrol"} पालन करने के लिए पेंसिल स्प्राइट में कुछ कोड जोड़ें ताकि आप खींच कर बना(draw) सकें:

```blocks
    जब झंडा क्लिक किया जाए
    forever
      go to [mouse pointer v]
    end
```

+ झंडे पर क्लिक करें और, फिर माउस को स्टेज के चारों ओर ले जाएं यह जांचने के लिए की कोड काम करता है या नहीं।

इसके बाद, चलो पेंसिल को ऐसा बनाए कि `जब` {: class = "blockcontrol"} माउस को क्लिक किया जाए तभी खींचने पर बनाए।

+ इस कोड को अपने पेंसिल स्प्राइट में जोड़ें:

![screenshot](images/paint-pencil-draw-code.png)

+ अपने कोड का फिर से परीक्षण करें। इस बार, स्टेज के चारों ओर पेंसिल को ले जाएं और माउस बटन दबाए रखें। क्या आप अपने पेंसिल से खींच कर बना सकते हैं?

![screenshot](images/paint-draw.png)

## \--- collapse \---

## title: अगर आपको समस्या आ रही हैं...

यदि आपकी पेंसिल नोक के बजाए पेंसिल के बीच से रेखा खींच रही है, तो आपको अपना पोशाक केंद्र बदलना होगा।

![Costume center](images/costume-center.png)

The crosshair for the pencil must be placed **just below** the tip of the pencil, not on the tip of the pencil.

A changes in a sprite's 'costume center' isn't registered until another tab is clicked, so click on another costume, or on the 'Scripts' tab to finalise your changes to the costume center.

\--- /collapse \---