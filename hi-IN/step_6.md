## पेंसिल की चौड़ाई बदलना

Let's allow the user to draw using a range of different pencil sizes.

+ पहले, `चौड़ाई`{:class="blockvariable"} नामक नया वेरिएबल जोड़े।

[[[generic-scratch-add-variable]]]

+ इस लाइन को अपनी पेंसिल के कोड `हमेशा के लिए(forever)`{:class="blockcontrol"} लूप के*अंदर* जोड़ें:

```blocks
    पेन का अाकार (चौड़ाई) पर सेट करे
```

पेंसिल की चौड़ाई अब बार-बार 'चौड़ाई' वेरिएबल(variable) के मान पर सेट की जाएगी।

+ स्टेज पर वेरिएबल प्रदर्शक(display) पर राइट क्लिक करें और 'स्लाइडर' पर क्लिक करें।

![screenshot](images/paint-slider.png)

अब आप वेरिएबल के नीचे स्लाइडर को मान बदलने के लिए खींच सकते हैं।

![screenshot](images/paint-slider-change.png)

+ अपने प्रोजेक्ट का परीक्षण करें, और देखें कि क्या आप पेंसिल की चौड़ाई बदल सकते हैं।

![screenshot](images/paint-width-test.png)

यदि आप चाहें, तो आप 'चौड़ाई' के न्यूनतम और अधिकतम मान को सेट कर सकते हैं जिसकी अनुमति है। ऐसा करने के लिए, फिर से वेरिएबल पर राइट-क्लिक करें और 'स्लाइडर न्यूनतम और अधिकतम सेट करें' पर क्लिक करें। Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![screenshot](images/paint-slider-max.png)

Keep testing your 'width' variable until you're happy.