## कलम रूंदी बदला

पुढे आपण आपल्या प्रोग्रामचा वापर करणार्या व्यक्तीस वेगवेगळ्या पेन रुंदीसह वस्तू काढण्यासाठी अनुमती देण्यासाठी कोड जोडू शकता.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- / कार्य \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
जेव्हा ध्वज क्लिक केले
सर्व
स्विच कॉस्च्यूम (पेन्सिल-ब्लू व्ही)
सेट कलम रंग [# 0035FF]
कायमचे मिटवा,
(माउस पॉइंटर विरुद्ध)
+ सेट पेन आकार (रुंदी :: व्हेरिएबल्स) वर
असल्यास <<mouse down?> आणि <(माऊस वाई) > [-120]>> नंतर 
  पेन डाउन

  पेन अप
डा
```

\--- / कार्य \---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

\--- task \---

Right-click on the `width`{:class="block3variables"} variable displayed on the Stage, and then click on **slider**.

![screenshot](images/paint-slider.png)

\--- /task \---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can add code to adjust the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---