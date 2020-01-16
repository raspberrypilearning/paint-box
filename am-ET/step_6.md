## የግራ ጠርዝ ቀይር

በመቀጠሌ, ፕሮግራሞች በተሇያዩ የስሌዝ ስፋቶች ስሊሳዎችን እንዱስለጥፉ ሇማዴረግ የሚፇሌጉትን ኮዶችን ያካትታለ.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- / task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
ባንዲራ ጠቅ ጊዜ
ደምስስ ሁሉንም
(እርሳስ-ሰማያዊ v) ይቀይሩ የሚኖሩት
[# 0035FF] ወደ ስብስብ ብዕር ቀለም
ለዘላለም
እየተጓዙ (የመዳፊት ጠቋሚ v) ወደ
+ ማዘጋጀት ብዕር መጠን (ስፋት :: ተለዋዋጮች) ወደ
ከሆነ <<mouse down?> እና <(መዳፊት y) > [-120]>> እና 
  ወደ ታች
  ይጣሉ
  መሀል ወደ

```

\--- / task \---

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