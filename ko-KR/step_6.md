## 연필 두께 변경하기

다음으로 프로그램을 사용하는 사람이 다른 펜 너비로 그림을 그릴 수 있도록 코드를 추가합니다.

먼저, `두께`{:class="block3variables"}라는 이름의 새 변수를 추가 해 보세요.

[[[generic-scratch3-add-variable]]] \--- /task \---

\--- task \--- 이 코드를 연필코드의 `무한반복`{:class="block3control"} 루프 **안쪽**에 넣어주세요:

```blocks3
flag가 클릭되었을 때
모두 삭제
모양을 (pencil-blue v) 로 바꾸기
무한 반복
 (mouse pointer v)로 이동하기
+ 펜 사이즈를 (width :: variables) 로 설정하기
만약 <<mouse down?> 과 <(mouse y) > [-120]>> 이라면
  펜 내리기
  아니면
  펜 올리기
끝
```

\--- /task \---

이제 펜 너비가 ` width ` {: class = "block3variables"} 값으로 설정됩니다. 

\--- task \--- `width`{:class="block3variables"} 를 오른쪽 클릭하여 변수를 스테이지에 표시하고, **슬라이더**를 클릭하세요.

![스크린샷](images/paint-slider.png) \--- /task \---

변수 아래의 슬라이더를 드래그 해서 변수의 값을 바꿀 수 있습니다.

![<0>#outside-pic</0> CSS 코드에서 <0>width</0>(너비) 와 <0>height</0>(높이) 값을 수정하여, 바깥 쪽에 있는 이미지를 <0>200px</0>로 수정해보세요. (<0>px</0>는 픽셀을 의미합니다.)](images/paint-slider-change.png)

\--- task \--- 프로젝트를 테스트하고 코드를 추가하여 펜 너비를 조정할 수 있는지 확인하십시오.

![스크린샷](images/paint-width-test.png) \--- /task \---