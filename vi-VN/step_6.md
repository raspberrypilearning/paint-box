## Thay đổi chiều rộng bút

Tiếp theo, bạn sẽ thêm mã để cho phép người sử dụng chương trình của bạn vẽ những thứ có độ rộng bút khác nhau.

\--- task \--- Đầu tiên, thêm một biến mới có tên `width`{: class = "block3variables"}.

[[[generic-scratch3-add-variable]]] \--- / nhiệm vụ \---

\--- task \--- Thêm dòng **vào bên trong** vòng `mãi mãi`{: class = "block3control"} của mã bút chì sprite:

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

Độ rộng bút bây giờ liên tục được đặt thành giá trị của biến `width`{: class = "block3variables"}.

\--- task \--- Nhấp chuột phải vào biến `chiều rộng`{: class = "block3variables"} được hiển thị trên Giai đoạn, sau đó nhấp vào **thanh trượt**.

![ảnh chụp màn hình](images/paint-slider.png) \--- /bài tập \---

Bây giờ bạn có thể kéo thanh trượt hiển thị bên dưới biến để thay đổi giá trị của biến.

![ảnh chụp màn hình](images/paint-slider-change.png)

\--- task \--- Kiểm tra dự án của bạn và xem bạn có thể thêm mã để điều chỉnh độ rộng bút không.

![ảnh chụp màn hình](images/paint-width-test.png) \--- /bài tập \---