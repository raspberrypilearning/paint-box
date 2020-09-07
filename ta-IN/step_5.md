## தவறுகளை திரும்பப் பெறவும்(undo)

சில நேரங்களில் தவறுகள் நடக்கும், எனவே ஒரு 'clear' பொத்தானையும், ஒரு அழிப்பான்(eraser) பொத்தானையும் சேர்க்கவும்.

--- task ---

நூலகத்தின் எழுத்துக்கள்(Letters) பிரிவில் இருந்து, 'X-block' sprite-ஐச் சேர்க்கவும். Sprite-இன் costume-க்கு சிவப்பு நிறத்தில் வண்ணம் பூசி, அதை கொஞ்சம் சிறியதாக ஆக்குங்கள். இந்த sprite-தான் 'clear' பொத்தான்.

[[[generic-scratch3-sprite-from-library]]]

![திரைப்பிடிப்பு](images/paint-x.png)

--- /task ---

--- task ---

Sprite -ஐக் கிளிக் செய்யும்போது, மேடையில் உள்ள அனைத்தையும் அழிப்பதற்கான குறியீட்டை 'X-block' sprite-இல் சேர்க்கவும்.

![குறுக்கு](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

--- /task ---

மேடையில் உள்ள அனைத்தையும் அழிக்க நீங்கள் `broadcast`{:class="block3extensions"} தொகுதியை பயன்படுத்தத் தேவையில்லை, ஏனெனில் `erase all`{:class="block3extensions"} தொகுதி அந்த வேலையைச் செய்கிறது.

பென்சில் sprite, ஒரு அழிப்பான் costume-ஐயும் உள்ளடக்கியிருப்பதைப் பார்க்கிறீர்களா?

![திரைப்பிடிப்பு](images/paint-eraser-costume.png)

உங்கள் திட்டத்தில் ஒரு தனி அழிப்பான் sprite-உம் உள்ளது.

--- task ---

இந்த அழிப்பான் sprite-இல் வலது கிளிக் செய்து, பின்னர் **show**(காட்டு) என்பதைக் கிளிக் செய்க. உங்கள் மேடை இப்போது எப்படி இருக்க வேண்டும் என்பது இங்கே:

![திரைப்பிடிப்பு](images/paint-eraser-stage.png)

--- /task ---

--- task ---

அழிப்பான் sprite-ஐ கிளிக் செய்யும் போது, அது `'eraser' broadcast`{:class="block3events"} செய்தியை அனுப்புவதற்கான குறியீட்டை அழிப்பான் sprite -இல் சேர்க்கவும்.

![அழிப்பான்](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

--- /task ---

பென்சில் sprite, 'eraser' செய்தியைப் பெறும்போது, அது அதன் costume -ஐ, அழிப்பான் costume-ஆகவும், பேனாவின் நிறத்தை, மேடையின் நிறமான வெள்ளை நிறத்துக்கும் மாற்ற வேண்டும்!

--- task ---

அழிப்பான் உருவாக்க சில குறியீட்டைச் சேர்க்கவும்.

--- hints --- --- hint ---

பென்சில் sprite-இல் சில குறியீட்டைச் சேர்க்கவும்: `Eraser`{:class="block3events"} செய்தியை நான் பெறும்போது(`When I receive`{:class="block3events"}), அழிப்பான் costume-க்கு மாறி (`Switch to costume eraser`{:class="block3looks"}) , பின்னர், பேனா நிறத்தை வெள்ளையாக அமைக்கவும் (`Set pen color`{:class="block3extensions"} to white).

--- /hint --- --- hint ---

உங்களுக்கு தேவையான அனைத்து தொகுதிகளும் இங்கே:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

--- /hint --- --- hint ---

குறியீடு எப்படி இருக்க வேண்டும் என்பது இங்கே:

![பென்சில்](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

--- /hint --- --- /hints --- --- /task ---

--- task ---

உங்களால் மேடையில் உள்ள அனைத்தையும் துடைக்க(clear) முடிகிறதா மற்றும் பென்சிலால் வரைந்த கோடுகளையும் அழிக்க முடிகிறதா என்று தெரிந்து கொள்ள, உங்கள் திட்டத்தை சோதிக்கவும்.

![திரைப்பிடிப்பு](images/paint-erase-test.png)

--- /task ---

பென்சிலில் இன்னும் ஒரு சிக்கல் உள்ளது: மேடையில் எங்கும் நீங்கள் வரையலாம், 'clear' மற்றும் அழிப்பான் பொத்தான்களுக்கு அருகே உட்பட!

![திரைப்பிடிப்பு](images/paint-draw-problem.png)

--- task ---

இதைச் சரிசெய்ய, குறியீட்டை மாற்றவும். இதனால் சுட்டியைக் கிளிக் செய்தால் மற்றும் (**and**) சுட்டியின் சுட்டுக்குறியின் `y` நிலை `-120` -ஐ விட அதிகமாக இருந்தால் மட்டுமே பேனா கீழே இருக்கும்:

![பென்சில்](images/pencil.png)

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

--- /task ---

--- task ---

உங்கள் திட்டத்தை சோதிக்கவும். நீங்கள் இப்போது பொத்தான்களுக்கு அருகில் வரைய முடியாது.

![திரைப்பிடிப்பு](images/paint-fixed.png)

--- /task ---