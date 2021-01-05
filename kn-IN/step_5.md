## ತಪ್ಪುಗಳನ್ನು ರದ್ದುಗೊಳಿಸಿ

ಕೆಲವೊಮ್ಮೆ ತಪ್ಪುಗಳು ಸಂಭವಿಸುತ್ತವೆ, ಆದ್ದರಿಂದ 'clear' ಬಟನ್ ಮತ್ತು eraser ಬಟನ್ ಸೇರಿಸಿ.

\--- task \---

ಗ್ರಂಥಾಲಯದ ಅಕ್ಷರಗಳ ವಿಭಾಗದಿಂದ 'X-block' sprite ಸೇರಿಸಿ. sprite ನ ಉಡುಪನ್ನು ಕೆಂಪು ಬಣ್ಣದಲ್ಲಿ ಬಣ್ಣ ಮಾಡಿ ಮತ್ತು ಅದನ್ನು ಸ್ವಲ್ಪ ಚಿಕ್ಕದಾಗಿಸಿ. ಈ sprite 'clear' ಬಟನ್ ಆಗಿದೆ.

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png)

\--- /task \---

\--- task \---

sprite ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಹಂತವನ್ನು ತೆರವುಗೊಳಿಸಲು 'X-block' sprite ‌ಗೆ ಕೋಡ್ ಸೇರಿಸಿ.

![cross](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- /task \---

ಹಂತವನ್ನು ತೆರವುಗೊಳಿಸಲು ನೀವು `broadcast`{:class="block3events"} ಅನ್ನು ಬಳಸಬೇಕಾಗಿಲ್ಲ, ಏಕೆಂದರೆ `erase-all`{:class="block3extensions"} ಬ್ಲಾಕ್ ಆ ಕೆಲಸವನ್ನು ಮಾಡುತ್ತದೆ.

ಸೀಸಕಡ್ಡಿ sprte ಅಳಿಸುವ ವಸ್ತು ವೇಷಭೂಷಣವನ್ನು ಒಳಗೊಂಡಿದೆ ಎಂದು ನೀವು ನೋಡುತ್ತೀರಾ?

![screenshot](images/paint-eraser-costume.png)

ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್ ಪ್ರತ್ಯೇಕ eraser spite ಅನ್ನು ಸಹ ಒಳಗೊಂಡಿದೆ.

\--- task \---

ಈ eraser sprite ಅನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ನಂತರ **show** ಆಯ್ಕೆಮಾಡಿ.

![screenshot](images/show-eraser.png)

ನಿಮ್ಮ ಹಂತವು ಈಗ ಹೇಗೆ ಕಾಣಬೇಕು ಎಂಬುದು ಇಲ್ಲಿದೆ:

![screenshot](images/paint-eraser-stage.png)

\--- /ಕಾರ್ಯ \---

\--- ಕಾರ್ಯ \---

eraser sprite ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ `eraser broadcast`{:class="block3events"} ಕಳುಹಿಸಲು eraser sprite ‌ಗೆ ಕೋಡ್ ಸೇರಿಸಿ.

![eraser](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

\--- /ಕಾರ್ಯ \---

ಸೀಸಕಡ್ಡಿ sprite 'error' ಸಂದೇಶವನ್ನು ಸ್ವೀಕರಿಸಿದಾಗ, ಅದು ತನ್ನ ವೇಷಭೂಷಣವನ್ನು ಅಳಿಸುವ ವಸ್ತುಗೆ ಬದಲಾಯಿಸಬೇಕು ಮತ್ತು ಲೇಖನಿ ಬಣ್ಣವನ್ನು ಬಿಳಿ ಬಣ್ಣಕ್ಕೆ ಬದಲಾಯಿಸಬೇಕು, ಇದು ಹಂತದಂತೆಯೇ ಇರುತ್ತದೆ!

\--- ಕಾರ್ಯ \---

eraser ರಚಿಸಲು ಕೆಲವು ಕೋಡ್ ಸೇರಿಸಿ.

\--- ಸುಳಿವುಗಳು \--- \--- ಸುಳಿವು \---

ಸೀಸಕಡ್ಡಿ ಸ್ಪ್ರೈಟ್‌ಗೆ ಕೆಲವು ಕೋಡ್ ಸೇರಿಸಿ: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

\--- /hint \--- \--- hint \---

ನಿಮಗೆ ಅಗತ್ಯವಿರುವ ಎಲ್ಲಾ ಬ್ಲಾಕ್‌ಗಳು ಇಲ್ಲಿವೆ:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

\--- /hint \--- \--- hint \---

ಕೋಡ್ ಹೇಗಿರಬೇಕು ಎಂಬುದು ಇಲ್ಲಿದೆ:

![pencil](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- ಕಾರ್ಯ \---

ನೀವು ಹಂತವನ್ನು ತೆರವುಗೊಳಿಸಬಹುದು ಮತ್ತು ಸೀಸಕಡ್ಡಿ ರೇಖೆಗಳನ್ನು ಅಳಿಸಬಹುದೇ ಎಂದು ನೋಡಲು ನಿಮ್ಮ ಯೋಜನೆಯನ್ನು ಪರೀಕ್ಷಿಸಿ.

![screenshot](images/paint-erase-test.png)

\--- /ಕಾರ್ಯ \---

ಸೀಸಕಡ್ಡಿ‌ಯೊಂದಿಗೆ ಇನ್ನೂ ಒಂದು ಸಮಸ್ಯೆ ಇದೆ: ನೀವು 'clear' ಮತ್ತು eraser ಗುಂಡಿಗಳನ್ನು ಒಳಗೊಂಡಂತೆ ವೇದಿಕೆಯಲ್ಲಿ ಎಲ್ಲಿಯಾದರೂ ಸೆಳೆಯಬಹುದು!

![screenshot](images/paint-draw-problem.png)

\--- ಕಾರ್ಯ \---

ಇದನ್ನು ಸರಿಪಡಿಸಲು, ಕೋಡ್ ಅನ್ನು ಬದಲಾಯಿಸಿ ಇದರಿಂದ ಮೌಸ್ ಕ್ಲಿಕ್ ಮಾಡಿದರೆ ಮಾತ್ರ ಪೆನ್ ಡೌನ್ ಆಗುತ್ತದೆ **ಮತ್ತು** ಮೌಸ್ ಪಾಯಿಂಟರ್‌ನ `y` ಸ್ಥಾನವು `-120` ಗಿಂತ ಹೆಚ್ಚಿದ್ದರೆ:

![pencil](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
  go to (mouse pointer v)
+if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

\--- /ಕಾರ್ಯ \---

\--- ಕಾರ್ಯ \---

ನಿಮ್ಮ ಯೋಜನೆಯನ್ನು ಪರೀಕ್ಷಿಸಿ. ನೀವು ಈಗ ಬಟನ್ ಗಳ ಬಳಿ ಸೆಳೆಯಲು ಸಾಧ್ಯವಾಗಬಾರದು.

![screenshot](images/paint-fixed.png)

\--- /ಕಾರ್ಯ \---