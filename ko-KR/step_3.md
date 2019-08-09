## 색연필

다른 색의 연필들을 추가해서 사용자가 색을 고를 수 있도록 해 봐요.

\--- task \--- `pencil` 스프라이트를 `pencil-blue` 스프라이트로 변경합니다.

![연필 이름 바꾸기](images/rename-pencil.png) \--- /task \---

\--- 작업 \--- pencil 스프라이트를 오른쪽 클릭하고 'pencil-blue' 코스튬을 복제하십시오.

![스크린샷](images/paint-blue-duplicate.png) \--- /task \---

\--- task \--- 새 코스튬의 이름을 ’pencil-green’으로 바꾸고, 녹색으로 칠해주세요.

![스크린샷](images/paint-pencil-green.png)

\--- /task \---

\--- task \--- 새로운 사각형 스프라이트 두 개를 그려주세요. 파란색 하나, 녹색 하나. 이것은 파란색과 녹색 연필을 선택하기위한 것입니다.

![스크린샷](images/paint-selectors.png) \--- /task \---

\--- task \--- 새 스프라이트의 이름을 'blue'과 'green'으로 바꿔 주세요.

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \--- 'green' 스프라이트를 클릭하면 "green" 메시지를 `브로드캐스트`{:class="block3events"} 하도록 코드를 추가합니다.

![녹색 사각형](images/green_square.png)

```blocks3
이 스프라이트가 클릭될 때
(green v) 방송하기
```

[[[generic-scratch3-broadcast-message]]] \--- /task \---

연필 스프라이트는 "녹색" 메시지를 받고 이에 대한 응답으로 코스튬과 연필 색상을 변경해야합니다.

\--- task \--- 연필 스프라이트로 돌아가세요. 이 스프라이트가 `초록`{:class="blockevents"} 이벤트를 받으면, 녹색 연필 모양으로 바뀌고 연필 색깔을 녹색으로 바꾸는 코드를 추가 하세요.

![연필](images/pencil.png)

```blocks3
[green v] 을\(를\) 받았을 때
모양을 [pencil-green v] \(으\)로 바꾸기
펜 색깔을 [#00CC44] \(으\)로 정하기
```

펜 색상을 녹색으로 설정하려면, `펜 컬러 설정하기`{:class="block3extensions"} 블록을 클릭하고, 초록색 사각형 스프라이트를 클릭하세요. \--- /task \---

그런 다음 연필 색상이 파란색으로 전환 할 수 있도록 비슷한 작업을 수행합니다.

\--- task \--- 파란색 사각형 스프라이트를 클릭하고 다음 코드를 추가합니다:

![파란색 사각형](images/blue_square.png)

```blocks3
이 스프라이트가 클릭될 때
(파랑 v) 방송하기
```

그런 다음 연필 스프라이트를 클릭하고 다음 코드를 추가하십시오. ![연필](images/pencil.png)

```blocks3
[파랑 v] 을\(를\) 받았을 때
모양을 (파란색 연필 v) \(으\)로 바꾸기
펜 색깔을 [#0000ff] \(으\)로 정하기
```

\--- /task \---

\--- task \--- 마지막으로, 연필 스프라이트가 어떤 색으로 시작하게 될지 알려주고 시작할 때 화면이 비어있는지 확인할 수 있도록 이 코드를 추가 하세요.

![연필](images/pencil.png)

```blocks3
플래그를 클릭했을 때
+전부 삭제
+모양을 (pencil-blue v) \(으\)로 바꾸기
+펜 색깔을 [#0035FF] \(으\)로 정하기
무한 반복
  (mouse pointer v) \(으\)로 이동
만약 <mouse down?> \(이\)라면
  펜 내리기
  아니면
  펜 올리기
끝
```

\--- /task \---

원하는 경우 다른 색상의 연필로 시작할 수 있습니다.

\--- task \--- 코드를 다시 테스트 해 보세요. 파란색 사각형과 녹색 사각형을 클릭해서 연필의 색을 바꿀 수 있나요?

![스크린샷](images/paint-pens-test.png) \--- /task \---