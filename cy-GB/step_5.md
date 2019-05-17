## Dadwneud camgymeriadau

Weithiau mae camgymeriadau'n digwydd, felly ychwanega fotwm 'clirio' a botwm dileuwr.

\--- task \--- Ychwanega'r corlun 'X-block' o adran llythrennau'r llyfrgell. Lliwia gwisg y corlun yn goch a'i wneud ychywig yn llai. Y corlun yma yw'r botwm 'clirio'.

[[[generic-scratch3-sprite-from-library]]]

![sgrinlun](images/paint-x.png) \--- /task \---

\--- task \--- Ychwanega gôd i gorlun 'X-block' i glirio'r Llwyfan pan mae'r corlun yn cael ei glicio.

![croes](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- /task \---

Does dim angen defnyddio `darlledu`{:class="block3events"} i glirio'r Llwyfan, gan fod y bloc `dileu popeth`{:class="block3extensions"} yn gwneud hynny.

Wyt ti'n gweld fod y corlun pensil yn cynnwys gwisg dileuwr?

![sgrinlun](images/paint-eraser-costume.png)

Mae dy brosiect hefyd yn cynnwys corlun dileuwr ar wahân.

\--- task \--- Gwna clic-dde ar gorlun y dileuwr a chlicia **dangos**. Dyma sut y dylai dy Lwyfan ymddangos nawr:

![sgrinlun](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Ychwanega gôd i gorlun y dileuwr i anfon `darllediad 'dileuwr'`{:class="block3events"} pan mae'r dileuwr yn cael ei glicio.

![dileuwr](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

\--- /task \---

Pan fo'r corlun pensil yn derbyn neges 'dileuwr', fe ddylai newid gwisg i'r dileuwr a newid lliw y pen i wyn, sef yr un lliw â'r Llwyfan!

\--- task \--- Ychwanega gôd i greu dileuwr.

\--- hints \--- \--- hint \--- Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white \--- /hint \--- \--- hint \--- Here are all the blocks you need:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

\--- /hint \--- \--- hint \--- Dyma sut dylai dy gôd edrych: ![pensil](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \--- Profa dy brosiect i weld os wyt ti'n gallu clirio'r Llwyfan a dileu'r llinellau pensil.

![sgrinlun](images/paint-erase-test.png) \--- /task \---

Mae un problem arall gyda'r pensil: rwyt ti'n gallu tynnu llun unrhywle ar y Llwyfan, gan gynnwys ger y botymau 'clirio' a dileuwr!

![sgrinlun](images/paint-draw-problem.png)

\--- task \--- I ddatrys hyn, mae angen i ti ddweud wrth y pensil i dynnu llun os yw’r llygoden wedi clicio **ac**os yw `y-position` y llygoden yn fwy na `-120`:

![pensil](images/pencil.png)

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

\--- task \--- Profa dy brosiect. Ni ddylet ti nawr allu tynnu llun ger y botymau.

![sgrinlun](images/paint-fixed.png) \--- /task \---