## Làm bút chì

Bắt đầu bằng cách làm một cây bút chì mà bạn có thể sử dụng để vẽ trên Sân khấu.

\--- task \--- Mở dự án Khởi động 'Hộp sơn' Scratch.

**Trực tuyến**: mở dự án khởi động tại [rpf.io/paint-box-on](http://rpf.io/paint-box-on){: target = "_ blank"}

**Ngoại tuyến**: mở dự án [starter](http://rpf.io/p/en/paint-box-go){: target = "_ blank"} trong trình chỉnh sửa ngoại tuyến.

Nếu bạn cần tải xuống và cài đặt trình soạn thảo ngoại tuyến Scratch, bạn có thể tìm thấy nó tại [rpf.io/scratchoff](http://rpf.io/scratchoff){: target = "_ blank"}

Trong dự án khởi động, bạn sẽ thấy các họa tiết bút chì và tẩy:

![ảnh chụp màn hình](images/paint-starter.png) \--- /bài tập \---

\--- bài tập \---

Thêm phần mở rộng Pen cho dự án của bạn.

[[[generic-scratch3-add-pen-extension]]]

\--- /bài tập \---

\--- bài tập \---

Thêm một số mã vào sprite bút chì để làm cho sprite theo con trỏ chuột `mãi mãi`{: class = "block3control"} để bạn có thể vẽ:

![bút chì](images/pencil.png)

```blocks3
khi cờ nhấp
mãi mãi
  đi đến (con trỏ chuột v)
kết thúc
```

\--- /bài tập \---

\--- task \--- Nhấp vào cờ và sau đó di chuyển con trỏ chuột quanh Giai đoạn để kiểm tra xem mã của bạn có hoạt động không. \--- /bài tập \---

Tiếp theo, làm cho bút chì của bạn chỉ vẽ `nếu`{: class = "block3control"} nút chuột đang được nhấp.

\--- task \--- Thêm mã này vào bút chì của bạn:

![bút chì](images/pencil.png)

```blocks3
khi cờ nhấp
mãi mãi
  đi tới (con trỏ chuột v)

+ nếu <mouse down?> thì
  bút xuống
  khác
  bút lên
kết thúc
```

\--- /bài tập \---

\--- task \--- Kiểm tra lại mã của bạn. Lần này, di chuyển bút chì xung quanh Sân khấu và giữ nút chuột. Bạn có thể vẽ bằng bút chì của bạn?

![ảnh chụp màn hình](images/paint-draw.png) \--- /bài tập \---

## \--- sự sụp đổ \---

## tiêu đề: Bút chì của bạn không rút ra từ đầu của nó?

Nếu đường kẻ mà bút chì của bạn vẽ có vẻ như đến từ giữa bút chì, bạn cần thay đổi bút chì của mình để đầu bút là trung tâm của bút chì.

Nhấp vào bút chì, và sau đó nhấp vào tab **Trang phục**.

Di chuyển trang phục sao cho đầu bút chì bằng **ngay trên** trung tâm.

![Trung tâm trang phục](images/costume-center-annotated.png)

Bây giờ di chuyển bút chì xung quanh trên sân khấu và vẽ. Bút chì bây giờ sẽ vẽ một đường từ đầu của nó.

\--- /sự sụp đổ \---