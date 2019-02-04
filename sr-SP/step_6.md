## Промени дебљину оловке

Сада ћеш додати код, који ће омогућити кориснику; да црта ствари са оловкама разних величина.

\--- task \--- Прво додај нову променљиву која ће се звати `дебљина`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]] \--- /task \---

\--- task \--- Додај ову наредбу **унутар** петље `понављај`{:class="block3control"} у коду оловке:

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

\--- /task \---

Ширина трага оловке сада ће стално бити постављена на вредност променљиве `дебљина`{:class="block3variables"}.

\--- task \--- Кликни десним тастером миша на променљиву `дебљина`{:class="block3variables"} приказану на Позорници, а затим кликни на **клизач**.

![снимак екрана](images/paint-slider.png) \--- /task \---

Сада можеш да помераш клизач који се налази испод променљиве да би променио њену вредност.

![снимак екрана](images/paint-slider-change.png)

\--- task \--- Испробај свој пројекат и провери да ли можеш да додаш код за подешавање дебљине оловке.

![снимак екрана](images/paint-width-test.png) \--- /task \---