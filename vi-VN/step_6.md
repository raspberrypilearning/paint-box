## Thay đổi chiều rộng bút

Tiếp theo, bạn sẽ thêm mã để cho phép người sử dụng chương trình của bạn vẽ những thứ có độ rộng bút khác nhau.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /bài tập \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
khi cờ nhấp
xóa tất cả
trang phục chuyển sang (bút chì màu xanh v)
đặt màu bút thành [# 0035FF]
mãi mãi
đi tới (con trỏ chuột v)
+ đặt kích thước bút thành (width :: biến)
nếu <<mouse down?> và <(chuột y) > [-120]>> rồi 
  bút xuống
  khác
  bút lên
kết thúc
```

\--- /bài tập \---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

\--- task \---

Right-click on the `width`{:class="block3variables"} variable displayed on the Stage, and then click on **slider**.

![screenshot](images/paint-slider.png)

\--- /task \---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can add code to adjust the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---