## ಬಣ್ಣದ ಸೀಸಕಡ್ಡಿ‌ಗಳು

ಈಗ ನೀವು ನಿಮ್ಮ ಯೋಜನೆಗೆ ವಿಭಿನ್ನ ಬಣ್ಣದ ಸೀಸಕಡ್ಡಿ‌ಗಳನ್ನು ಸೇರಿಸಲು ಹೊರಟಿದ್ದೀರಿ ಮತ್ತು ಅವುಗಳ ನಡುವೆ ಆಯ್ಕೆ ಮಾಡಲು ಬಳಕೆದಾರರಿಗೆ ಅವಕಾಶ ಮಾಡಿಕೊಡುತ್ತೀರಿ.

\--- task \---

'ಸೀಸಕಡ್ಡಿ' sprite ‌ನ ವೇಷಭೂಷಣಗಳ ಟ್ಯಾಬ್ ಕ್ಲಿಕ್ ಮಾಡಿ.

`pencil-a` ಉಡುಪನ್ನು `pencil-blue` ಎಂದು ಮರುಹೆಸರಿಸಿ

![rename-pencil](images/rename-pencil.png)

\--- /ಕಾರ್ಯ \---

\--- ಕಾರ್ಯ \---

ಪೆನ್ಸಿಲ್-ಬ್ಲೂ ಉಡುಪಿನ ಮೇಲೆ ಬಲ ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು **duplicate** ಆಯ್ಕೆಮಾಡಿ.

![screenshot](images/paint-blue-duplicate.png)

\--- /ಕಾರ್ಯ \---

\--- ಕಾರ್ಯ \---

ಹೊಸ ಉಡುಪಿಗೆ 'pencil-blue' ಎಂದು ಹೆಸರಿಸಿ, ಮತ್ತು ಸೀಸಕಡ್ಡಿ ಹಸಿರು ಬಣ್ಣ ಮಾಡಿ.

![screenshot](images/paint-pencil-green.png)

\--- /ಕಾರ್ಯ \---

\--- ಕಾರ್ಯ \---

ಎರಡು ಹೊಸ sprite ಗಳನ್ನು ರಚಿಸಿ: ಒಂದು ನೀಲಿ ಚೌಕ ಮತ್ತು ಒಂದು ಹಸಿರು ಚೌಕ. ನೀಲಿ ಮತ್ತು ಹಸಿರು ಸೀಸಕಡ್ಡಿ ನಡುವೆ ಆಯ್ಕೆ ಮಾಡಲು ಇವು.

![screenshot](images/paint-selectors.png)

\--- /ಕಾರ್ಯ \---

\--- ಕಾರ್ಯ \---

ಹೊಸ sprite ‌ಗಳನ್ನು ಮರುಹೆಸರಿಸಿ ಇದರಿಂದ ಅವುಗಳನ್ನು 'blue' ಮತ್ತು 'green' ಎಂದು ಕರೆಯಲಾಗುತ್ತದೆ

[[[generic-scratch3-rename-sprite]]]

\--- /ಕಾರ್ಯ \---

\--- ಕಾರ್ಯ \---

'ಹಸಿರು' sprite ಗೆ ಕೆಲವು ಕೋಡ್ ಸೇರಿಸಿ ಆದ್ದರಿಂದ ಈ sprite ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಅದು "green" ಎಂಬ ಸಂದೇಶವನ್ನು `broadcasts`{:class="block3events"} ಮಾಡುತ್ತದೆ.

![green square](images/green_square.png)

```blocks3
when this sprite clicked
broadcast (green v)
```

[[[generic-scratch3-broadcast-message]]]

\--- /ಕಾರ್ಯ \---

ಸೀಸಕಡ್ಡಿ sprite "ಹಸಿರು" ಸಂದೇಶವನ್ನು ಆಲಿಸಬೇಕು ಮತ್ತು ಪ್ರತಿಕ್ರಿಯೆಯಾಗಿ ಅದರ ವೇಷಭೂಷಣ ಮತ್ತು ಸೀಸಕಡ್ಡಿ ಬಣ್ಣವನ್ನು ಬದಲಾಯಿಸಬೇಕು.

\--- ಕಾರ್ಯ \---

ನಿಮ್ಮ ಸೀಸಕಡ್ಡಿsprite ಗೆ ಬದಲಿಸಿ. ಕೆಲವು ಕೋಡ್ ಸೇರಿಸಿ ಆದ್ದರಿಂದ ಈ ಸ್ಪ್ರೈಟ್ `green`{:class="block3events"} ಪ್ರಸಾರವನ್ನು ಪಡೆದಾಗ, ಅದು ಹಸಿರು ಪೆನ್ಸಿಲ್ ಉಡುಪಿಗೆ ಬದಲಾಗುತ್ತದೆ ಮತ್ತು ಪೆನ್ ಬಣ್ಣವನ್ನು ಹಸಿರು ಬಣ್ಣಕ್ಕೆ ಬದಲಾಯಿಸುತ್ತದೆ.

![pencil](images/pencil.png)

```blocks3
when I receive [green v]
switch costume to (pencil-green v)
set pen color to [#00CC44]
```

ಸೀಸಕಡ್ಡಿ ಬಣ್ಣವನ್ನು ಹಸಿರು ಬಣ್ಣಕ್ಕೆ ಹೊಂದಿಸಲು, `set pen color`{:class="block3extensions"} ಬ್ಲಾಕ್‌ನಲ್ಲಿ ಬಣ್ಣದ ಚೌಕವನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿ, ತದನಂತರ ಹಸಿರು ಚದರ sprite ಅನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿ.

\--- /ಕಾರ್ಯ \---

ನಂತರ ಇದೇ ರೀತಿಯ ವಿಷಯಕ್ಕೆ ನೀವು ಸೀಸಕಡ್ಡಿ ಬಣ್ಣವನ್ನು ನೀಲಿ ಬಣ್ಣಕ್ಕೆ ಬದಲಾಯಿಸಬಹುದು.

\--- ಕಾರ್ಯ \---

ನೀಲಿ ಚದರ sprite ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ಈ ಕೋಡ್ ಸೇರಿಸಿ:

![blue_square](images/blue_square.png)

```blocks3
when this sprite clicked
broadcast (blue v)
```

ನಂತರ ಸೀಸಕಡ್ಡಿ sprite ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ಈ ಕೋಡ್ ಸೇರಿಸಿ:

![pencil](images/pencil.png)

```blocks3
when I receive [blue v]
switch costume to (pencil-blue v)
set pen color to [#0000ff]
```

\--- /ಕಾರ್ಯ \---

\--- ಕಾರ್ಯ \---

ಅಂತಿಮವಾಗಿ, ಸೀಸಕಡ್ಡಿ sprite ‌ಗೆ ಯಾವ ಬಣ್ಣದಿಂದ ಪ್ರಾರಂಭಿಸಬೇಕು ಎಂದು ಹೇಳಲು ಮತ್ತು ನಿಮ್ಮ ಪ್ರೋಗ್ರಾಂ ಪ್ರಾರಂಭವಾದಾಗ ಪರದೆಯು ಸ್ಪಷ್ಟವಾಗಿದೆ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಲು ಈ ಕೋಡ್ ಸೇರಿಸಿ.

![pencil](images/pencil.png)

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

\--- /ಕಾರ್ಯ \---

ನೀವು ಬಯಸಿದರೆ, ನೀವು ಬೇರೆ ಬಣ್ಣದ ಸೀಸಕಡ್ಡಿ‌ಯೊಂದಿಗೆ ಪ್ರಾರಂಭಿಸಬಹುದು.

\--- ಕಾರ್ಯ \---

ನಿಮ್ಮ ಕೋಡ್ ಅನ್ನು ಪರೀಕ್ಷಿಸಿ. ನೀಲಿ ಅಥವಾ ಹಸಿರು ಚದರ sprite ಗಳ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡುವುದರ ಮೂಲಕ ನೀವು ನೀಲಿ ಮತ್ತು ಹಸಿರು ಸೀಸಕಡ್ಡಿ ಬಣ್ಣಗಳ ನಡುವೆ ಬದಲಾಯಿಸಬಹುದೇ?

![screenshot](images/paint-pens-test.png)

\--- /ಕಾರ್ಯ \---