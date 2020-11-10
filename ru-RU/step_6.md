## Измени ширину пера

Теперь попробуй добавить код, позволяющий человеку, использующему твою программу, рисовать что-либо с разной шириной пера.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
когда щёлкнут по зелёному флагу
стереть всё
изменить костюм на (карандаш-синий v)
установить цвет пера [#0035FF]
повторять всегда 
  перейти на (указатель мыши v)
  + установить размер пера (ширина :: variables)
  если <<mouse down?> и <(y мыши) > [-120]>> , то 
    опустить перо
  иначе 
    поднять перо
  end
end
```

\--- /task \---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

\--- task \---

Right-click on the `width`{:class="block3variables"} variable displayed on the Stage, and then click on **slider**.

![screenshot](images/paint-slider.png)

\--- /task \---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can change the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---