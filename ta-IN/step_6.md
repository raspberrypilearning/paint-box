## பேனா அகலத்தை மாற்றவும்

அடுத்து உங்கள் நிரலைப் பயன்படுத்தும் நபர், வெவ்வேறு பேனா அகலங்களைக் கொண்டு வரையுமாறு அனுமதிக்க, குறியீட்டைச் சேர்ப்பீர்கள்.

--- task ---

முதலில், `width`{:class="block3variables"} (அகலம்) எனப்படும் புதிய மாறியைச்(variable) சேர்க்கவும்.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

பென்சில் sprite குறியீட்டின் `forever`{:class="block3control"}மடக்கின் **உள்ளே** இந்த வரியை சேர்க்கவும் :

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

பேனா அகலம் இப்போது மீண்டும் மீண்டும் `width`{:class="block3variables"} என்னும் மாறியின் மதிப்பில் அமைக்கப்படுகிறது.

--- task ---

மேடையில் காட்டப்பட்டுள்ள `width`{:class="block3variables"} மாறியின் மேல், வலது கிளிக் செய்து, பின்னர், **slider**-ஐக்(ஸ்லைடர்) கிளிக் செய்யவும்.

![திரைப்பிடிப்பு](images/paint-slider.png)

--- /task ---

மாறியின் மதிப்பை மாற்ற, நீங்கள் இப்போது மாறிக்கு கீழே தெரியும் ஸ்லைடரை இழுக்கலாம்.

![திரைப்பிடிப்பு](images/paint-slider-change.png)

--- task ---

உங்கள் திட்டத்தை சோதித்து, பேனா அகலத்தை சரிசெய்ய குறியீட்டைச் சேர்க்க முடியுமா என்று பாருங்கள்.

![திரைப்பிடிப்பு](images/paint-width-test.png)

--- /task ---