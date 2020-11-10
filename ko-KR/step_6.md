## 펜의 두께 변경하기

이번엔 펜의 두께를 바꾸어 선을 그려 보도록 해 봅시다.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
깃발이 클릭되었을 때
모두 삭제
모양을 (pencil-blue v) 로 바꾸기
무한 반복
 (mouse pointer v) 로 이동하기
+ 펜 사이즈를 (width :: variables) 로 설정하기
만약 <<mouse down?> 과 <(mouse y) > [-120]>> 이라면
  선그리기
  아니면
  선그리지 않기
끝
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