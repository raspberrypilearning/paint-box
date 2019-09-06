## පැන්සලක් සෑදීම

වේදිකාව(stage එක) මත ඇඳීමට භාවිතා කළ හැකි පැන්සලක් සෑදීමෙන් ආරම්භ කරමු.

\--- task \--- Scratch හි 'තීන්ත පෙට්ටිය'('Paint box') ආරම්භක(starter) ව්‍යාපෘතිය(project එක) විවෘත කරන්න.

**අන්තර්ජාල මාර්ගගත(Online):** [rpf.io/paint-box-on](http://rpf.io/paint-box-on){:target="_blank"} හි අන්තර්ජාල මාර්ගගතව නව Scratch ව්‍යාපෘතියක් විවෘත කරන්න.

ඔබට Scratch ගිණුමක්(account එකක්) තිබේ නම් **රීමික්ස්(Remix)** ක්ලික් කිරීමෙන් පිටපතක් සාදාගත හැකිය.

**අන්තර්ජාලයට නොබැඳිව**: [ආරම්භක ව්‍යාපෘතිය(starter project)](http://rpf.io/p/en/paint-box-go){:target="_blank"} නොබැඳි සංස්කාරකයේ විවෘත කරන්න.

ඔබට Scratch නොබැඳි සංස්කාරකය(offline editor එක) බාගත(download) කර ස්ථාපනය(install) කිරීමට අවශ්‍ය නම්, ඔබට එය [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"} වෙතින් ලබාගත හැකිය.

ආරම්භක ව්‍යාපෘතියේදී, ඔබට පැන්සල් සහ මකන sprites දැකිය හැකිය:

![තිර රුව(screenshot)](images/paint-starter.png) \--- /task \---

\--- task \---

ඔබේ ව්‍යාපෘතියට පෙන්(pen) දිගුව(extension එක) එක් කරන්න.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

පැන්සල් sprite එකට කේතයක් එක් කිරීම මගින්, පැන්සල් sprite එක මූසික(mouse) දර්ශකය(pointer එක) `දිගින් දිගටම(forever)`{:class="block3control"} පසුපස යන පරිදි සකසන්න එවිට ඔබට එය භාවිතා කරමින් අඳින්න පුළුවන් වේවි:

![පැන්සල](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

\--- /task \---

\--- task \--- ඔබේ කේතය ක්‍රියාත්මක වේදැයි පරීක්ෂා කිරීම සඳහා ධජය මත ක්ලික් කර වේදිකාව වටා මූසික දර්ශකය ගෙනයන්න. \--- /task \---

ඊළඟට, ඔබේ පැන්සලේ මූසික(mouse) බොත්තම(button එක) ක්ලික් කරනු ලැබේ `නම්(if)`{:class="block3control"} පමණක් අඳින්නට සලස්වන්න.

\--- task \--- මෙම කේතය(code එක) ඔබේ පැන්සල්(pencil) sprite එකට එක් කරන්න:

![පැන්සල](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)

+ if <mouse down?> then
  pen down
  else
  pen up 
end
```

\--- /task \---

\--- task \--- ඔබේ කේතය(code එක) නැවත පරීක්ෂා කරන්න. දැන්, මූසික(mouse) බොත්තම(button එක) තද කරගෙන පැන්සල වේදිකාව(stage එක) වටා ගෙනයන්න. ඔබට පැන්සල භාවිතාකර ඇඳිය හැකිද?

![තිර රුව(screenshot)](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: ඔබේ පැන්සල ඇදීම සිදුකරන්නේ එහි තුඩෙන්(tip) නොවේද?

ඔබේ පැන්සලෙන් අඳින රේඛා පැන්සල මැදින් එන බවක් පෙනේ නම්, ඔබේ පැන්සල් sprite එකේ තුඩ එහි කේන්ද්‍රය ලෙස වෙනස් කළ යුතුය, එවිට පැන්සල් තුඩ sprite එකේ කේන්ද්‍රය වේ.

පැන්සල් sprite එක මත ක්ලික් කරන්න, ඉන්පසු **ඇදුම්(costume)** පටිත්ත(tab එක) මත ක්ලික් කරන්න.

පැන්සලෙහි තුඩ මධ්‍යස්ථානයට **මදක් ඉහළින්(just above)** පිහිටන පරිදි ඇඳුම(cpstume එක) සකසන්න.

![ඇඳුම්(costume) මධ්‍යස්ථානය(center)](images/costume-center-annotated.png)

දැන් පැන්සල වේදිකාව(stage එක) වටා ගෙන යමින් අදින්න. පැන්සල දැන් එහි කෙළවරේ ඇති තුඩෙන් රේඛාවක් අඳිනුඇත.

\--- /collapse \---