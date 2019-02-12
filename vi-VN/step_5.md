## Hoàn tác sai lầm

Đôi khi xảy ra lỗi, vì vậy hãy thêm nút 'xóa' và nút xóa.

\--- task \--- Thêm sprite 'X-block' từ phần chữ cái của thư viện. Tô màu trang phục của sprite bằng màu đỏ và làm cho nó nhỏ hơn một chút. Sprite này là nút 'xóa'.

[[[generic-scratch3-sprite-from-library]]]

![ảnh chụp màn hình](images/paint-x.png) \--- /bài tập \---

\--- task \--- Thêm mã vào sprite 'X-block' để xóa Giai đoạn khi sprite nhấp vào.

![vượt qua](images/cross.png)

```blocks3
Khi sprite này nhấp
xóa tất cả
```

\--- /bài tập \---

Bạn không cần sử dụng `phát`{: class = "block3events"} để xóa Giai đoạn, vì khối `xóa cả`{: class = "block3extensions"} thực hiện công việc đó.

Bạn có thấy rằng bút chì sprite bao gồm một trang phục tẩy?

![ảnh chụp màn hình](images/paint-eraser-costume.png)

Dự án của bạn cũng bao gồm một sprite eraser riêng.

\--- task \--- Nhấp chuột phải vào sprite eraser này và sau đó nhấp vào **show**. Đây là cách Giai đoạn của bạn sẽ nhìn bây giờ:

![ảnh chụp màn hình](images/paint-eraser-stage.png) \--- /bài tập \---

\--- task \--- Thêm mã vào sprite eraser để gửi `'eraser' Broadcast`{: class = "block3events"} khi nhấp vào sprite eraser.

![cục gôm](images/eraser.png)

```blocks3
khi sprite này nhấp
phát (eraser v)
```

\--- /bài tập \---

Khi bút chì nhận được thông báo 'cục tẩy', nó sẽ chuyển trang phục của nó sang cục tẩy và chuyển màu bút sang màu trắng, cùng màu với Sân khấu!

\--- task \--- Thêm một số mã để tạo cục tẩy.

\--- gợi ý \--- \--- gợi ý \--- Thêm một số mã vào bút chì sprite: `Khi tôi nhận được`{: class = "block3events"} `cụ xóa`{: class = "block3events"} message `Chuyển sang công cụ xóa trang phục`{: class = "block3looks"} `Đặt màu bút`{: class = "block3extensions"} thành màu trắng \--- / gợi ý \--- \--- gợi ý \--- Dưới đây là tất cả các khối bạn cần:

```blocks3
đặt màu bút thành [#FFFFFF]
khi tôi nhận được [eraser v]

trang phục chuyển sang (tẩy v
```

\--- / gợi ý \--- \--- gợi ý \--- Đây là đoạn mã sẽ như thế nào: ![bút chì](images/pencil.png)

```blocks3
khi tôi nhận được [eraser v]
trang phục chuyển sang (eraser v)
đặt màu bút thành [#FFFFFF]
```

\--- / gợi ý \--- \--- / gợi ý \--- \--- / nhiệm vụ \---

\--- task \--- Kiểm tra dự án của bạn để xem bạn có thể xóa Giai đoạn và xóa các đường bút chì không.

![ảnh chụp màn hình](images/paint-erase-test.png) \--- /bài tập \---

Có thêm một vấn đề với bút chì: bạn có thể vẽ bất cứ nơi nào trên Sân khấu, bao gồm gần các nút 'xóa' và xóa!

![ảnh chụp màn hình](images/paint-draw-problem.png)

\--- task \--- Để sửa lỗi này, hãy thay đổi mã để bút chỉ xuống nếu chuột được nhấp **và** vị trí `y` của con trỏ chuột lớn hơn `-120`:

![bút chì](images/pencil.png)

```blocks3
khi cờ nhấp
xóa tất cả
trang phục chuyển sang (bút chì màu xanh v)
đặt màu bút thành [# 0035FF]
mãi mãi
  đi tới (con trỏ chuột v)
+ nếu <<mouse down?> và <(chuột y) > [-120]>> sau đó 
  bút xuống
  khác
  bút lên
đầu
```

\--- /bài tập \---

\--- nhiệm vụ \--- Kiểm tra dự án của bạn. Bây giờ bạn không thể vẽ gần các nút.

![ảnh chụp màn hình](images/paint-fixed.png) \--- /bài tập \---