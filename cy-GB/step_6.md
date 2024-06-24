## Newid lled y pensil

Rwyt ti nawr am ychwanegu côd i ganiatâu'r defnyddiwr i dynnu llun yn defnyddio amrywiaeth o feintiau pensiliau gwahanol.

--- task --- Yn gyntaf, ychwanega newidyn newydd o'r enw `lled`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]] --- /task ---

--- task --- Ychwanega'r llinell hon **tu fewn** dolen `am byth`{:class="block3control"} côd corlun y pensil:

```blocks3
when flag clicked
erase all
switch costume to(pencil-glas v)
set pen color to [#0035FF]
forever
go to (pwyntydd llygoden v)
+set pen size to (lled :: variables)
if <<mouse down?> and <(llygoden y) > [-120]>> then 
  pen down
  else
  pen up
end
```

--- /task ---

Mae lled dy bensil nawr yn cael ei osod i gyfanswm `lled`{:class="block3variables"} y newidyn.

--- task --- Gwna clic dde ar newidyn `lled`{:class="block3variables"} sy'n ymddangos ar y Llwyfan, yna clicia'r **llithrydd**.

![sgrinlun](images/paint-slider.png) --- /task ---

Galli di nawr lusgo’r llithrydd o dan y newidyn i newid ei werth.

![sgrinlun](images/paint-slider-change.png)

--- task --- Profa dy brosiect a gweld os wyt ti'n gallu ychwanegu côd i newid lled y pen.

![sgrinlun](images/paint-width-test.png) --- /task ---