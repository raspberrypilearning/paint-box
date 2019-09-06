## වැරදි(mistakes) නිවැරදි(undo) කිරීම

සමහර විට වැරදීම් සිදු වේ, එබැවින් 'අස්කරන්න'('clear') බොත්තමක්(button එකක්) සහ මකන්න(eraser) බොත්තමක් එක් කරන්න.

\--- කාර්යය \--- පුස්තකාලයේ(library එකේ) අකුරු(letters) අංශයෙන්(section එකෙන්) 'X-block' sprite එක එක් කරන්න. sprite එකේ ඇඳුම(costume එක) රතු පැහැයෙන් වර්ණවත් කර එය මදක් කුඩා කරන්න. මෙම sprite එක 'අස්කරන්න'('clear') බොත්තම(button එක) වනු ඇත.

[[[generic-scratch3-sprite-from-library]]]

![තිර රුව(screenshot)](images/paint-x.png) \--- /task \---

\--- task \--- 'X-block' sprite එක ක්ලික් කළ විට වේදිකාව(stage එක) අස්කිරීම සඳහා එයට කේතය(code එකක්) එක් කරන්න.

![කතිරය](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- /task \---

වේදිකාව(stage එක) අස්කිරීම සඳහා ඔබට `විකාශනයක්(broadcast)`{:class="block3events"} භාවිතා කිරීමට අවශ්‍ය නැත, මන්ද `සියල්ල මකන්න(erase all)`{:class="block3extensions"} කට්ටිය(block එක) එම කාර්යය කරන බැවිනි. 

පැන්සල් sprite එකට මකන(eraser) ඇඳුමක්(costume එකක්) ඇතුළත් බව ඔබට පෙනේද?

![තිර රුව(screenshot)](images/paint-eraser-costume.png)

ඔබේ ව්‍යාපෘතියට(project එකට) වෙනම මකන(eraser) sprite එකක් ද ඇතුළත් වේ.

\--- task \--- මෙම මකන(eraser) sprite එක මත දකුණු-ක්ලික්(right-click) කර **පෙන්වන්න(show)** ක්ලික් කරන්න. ඔබගේ වේදිකාව(stage එක) දැන් දිස්වියයුතුආකාරය මෙහි දැක්වේ:

![තිර රුව(screenshot)](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- මකන(eraser) sprite එක ක්ලික් කළ විට ` 'මකන්න'('eraser') විකාශනයක්(broadcast එකක්)`{:class="block3events"} යවන පරිදි මකන sprite එකට කේතයක්(code එකක්) එක් කරන්න.

![මකනය](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

\--- /task \---

පැන්සල් sprite එකට 'මකනය'('eraser') පණිවිඩය(message එක) ලැබුණු විට, එය ඇඳුම(costume එක) මකනයට(eraser) මාරු කළ යුතු අතර, පෑනේ(pen) වර්ණය(colour එක) සුදු පැහැයට මාරු විය යුතුය.

\--- task \--- මකනය(eraser) නිර්මාණය(create) කිරීම සඳහා කේතයක්(code එකක්) එක් කරන්න.

\--- hints \--- \--- hint \--- පැන්සල් sprite එකට කේතය(code) එක් කරන්න: `මකන්න(eraser)`{:class="block3events"} පණිවිඩය(message එක) `මට ලැබුණු විට(when I recieve)`{:class="block3events"} `මකන(eraser) ඇඳුමට(costume එකට) මාරු(switch) වන්න`{:class="block3looks"} `පෑනනේ වර්ණය සුදු පැහයට සැකසීම(set pen color)`{:class="block3extensions"} \--- /hint \--- \--- hint \--- ඔබට අවශ්‍ය සියලුම කට්ටි(blocks) මෙහි දැක්වේ:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

\--- /hint \--- \--- hint \---- ඔබේ කේතය(code එක) මෙබඳු එකක් විය යුතුයි: ![පැන්සල](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- ඔබට ඔබේ ව්‍යාපෘතියේ(project එකේ) වේදිකාව අස්කර(clear කර) පැන්සල් රේඛා මකා දැමිය හැකිදැයි පරීක්ෂා(test) කරන්න.

![තිර රුව(screenshot)](images/paint-erase-test.png) \--- /task \---

පැන්සල සමඟ තවත් එක් ගැටළුවක් තිබේ: ඔබට 'අස්කරන්න'('clear') සහ මකන්න(eraser) බොත්තම් අසල සහ වේදිකාවේ ඕනෑම තැනක ඇඳිය හැකිය!

![තිර රුව(screenshot)](images/paint-draw-problem.png)

\--- task \--- මෙය නිවැරදි කිරීම සඳහා, පෑනෙන් ඇඳිය හැක්කේ මූසිකය ක්ලික් කළවිට පමණක් **සහ(and)** මූසික(mouse) දර්ශකයේ(pointer එකේ) `y` පිහිටීම(position එක) `-120` ට වඩා වැඩි විට පමණක් වන පරිදි කේතය(code එක) වෙනස් කරන්න:

![පැන්සල](images/pencil.png)

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

\--- /task \---

\--- task \--- ඔබේ කේතය(code එක) පරීක්ෂා(test) කරන්න. ඔබට දැන් බොත්තම්(buttons) අසල ඇඳීමට නොහැකි විය යුතුය.

![තිර රුව(screenshot)](images/paint-fixed.png) \--- /task \---