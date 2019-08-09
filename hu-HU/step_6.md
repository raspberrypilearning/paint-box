## Módosítsd a vonal vastagságát

Ezúttal hozzáadunk egy kódot, amely lehetővé teszi, hogy a programot használó különböző vastagságú vonalakat rajzoljon.

\--- task \--- Először adj hozzá egy új, `vonalvastagság`{:class="block3variables"} nevű változót.

[[[generic-scratch3-add-variable]]] \--- /task \---

\--- task \--- Add hozzá ezt a blokkot a `mindig`{:class="block3control"} hurokon **belülre** a ceruza szereplő kódjánál:

```blocks3
⚑ -ra kattintáskor
töröld a rajzokat
jelmez legyen (ceruza-kék v)
toll színe legyen [#0035FF]
mindig 
ugorj (egérmutató v) helyére
+ toll mérete legyen (width :: variables)
ha <<egér lenyomva?> és <(egér y) >[-120]>> akkor 
  tollat tedd le
  különben 
  tollat emeld fel
end
```

\--- /task \---

A vonal vastagsága most ismételten a `vonalvastagság`{:class="block3variables"} változó értékére áll.

\--- task \--- Kattints a jobb egérgombbal a `vonalvastagság`{:class="block3variables"} változóra, amely megjelent a játéktéren, majd kattints a **csúszka** menüpontra.

![képernyőkép](images/paint-slider.png) \--- /task \---

A változó értékének módosításához most húzd el a változó alatt látható csúszkát.

![képernyőkép](images/paint-slider-change.png)

\--- task \--- Teszteld a projekted, és nézd meg, hogy működik-e a vonalvastagság állító kód.

![képernyőkép](images/paint-width-test.png) \--- /task \---