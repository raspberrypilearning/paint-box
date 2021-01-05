## ಲೇಖನಿ ಅಗಲವನ್ನು ಬದಲಾಯಿಸಿ

ಮುಂದೆ ನೀವು ನಿಮ್ಮ ಪ್ರೋಗ್ರಾಂ ಅನ್ನು ಬಳಸುವ ವ್ಯಕ್ತಿಗೆ ವಿಭಿನ್ನ ಲೇಖನಿ ಅಗಲಗಳನ್ನು ಸೆಳೆಯಲು ಅನುಮತಿಸಲು ಕೋಡ್ ಅನ್ನು ಸೇರಿಸುತ್ತೀರಿ.

--- task ---

ಮೊದಲಿಗೆ, `width`{:class="block3variables"} ಎಂಬ ಹೊಸ ವೇರಿಯಬಲ್(variable) ಅನ್ನು ಸೇರಿಸಿ.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

ಪೆನ್ಸಿಲ್ ಸ್ಪ್ರೈಟ್‌ನ ಕೋಡ್‌ನ `forever`{:class="block3control"} ಲೂಪ್ **ಒಳಗೆ** ಈ ಸಾಲನ್ನು ಸೇರಿಸಿ:

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

ಲೇಖನಿ ಅಗಲವು ಈಗ ಮತ್ತೆ ಮತ್ತೆ `width`{:class="block3variables"} ವೇರಿಯೇಬಲ್ ಮೌಲ್ಯಕ್ಕೆ ಹೊಂದಿಸಲ್ಪಡುತ್ತದೆ.

--- task ---

ಹಂತದಲ್ಲಿ ಪ್ರದರ್ಶಿಸಲಾದ `width`{:class="block3variables"} ವೇರಿಯೇಬಲ್ ಮೇಲೆ ಬಲ ಕ್ಲಿಕ್ ಮಾಡಿ, ತದನಂತರ **slider** ಕ್ಲಿಕ್ ಮಾಡಿ.

![screenshot](images/paint-slider.png)

--- /task ---

ವೇರಿಯೇಬಲ್ ಮೌಲ್ಯವನ್ನು ಬದಲಾಯಿಸಲು ನೀವು ಈಗ ವೇರಿಯೇಬಲ್ ಕೆಳಗೆ ಗೋಚರಿಸುವ ಸ್ಲೈಡರ್ ಅನ್ನು ಎಳೆಯಬಹುದು.

![screenshot](images/paint-slider-change.png)

--- task ---

ನಿಮ್ಮ ಯೋಜನೆಯನ್ನು ಪರೀಕ್ಷಿಸಿ ಮತ್ತು ನೀವು ಲೇಖನಿ ಅಗಲವನ್ನು ಬದಲಾಯಿಸಬಹುದೇ ಎಂದು ನೋಡಿ.

![screenshot](images/paint-width-test.png)

--- /task ---