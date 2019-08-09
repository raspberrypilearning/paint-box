## Bút chì màu

Bây giờ bạn sẽ thêm bút chì màu khác nhau vào dự án của bạn và cho phép người dùng lựa chọn giữa chúng.

\--- task \--- Đổi tên `bút chì` sprite thành `bút chì xanh`

![đổi tên bút chì](images/rename-pencil.png) \--- /bài tập \---

\--- task \--- Nhấp chuột phải vào bút chì và sao chép trang phục 'bút chì màu xanh'.

![ảnh chụp màn hình](images/paint-blue-duplicate.png) \--- /bài tập \---

\--- nhiệm vụ \--- tên cho trang phục mới là 'bút chì màu xanh lá cây' và tô màu cho cây bút chì màu xanh lá cây.

![ảnh chụp màn hình](images/paint-pencil-green.png)

\--- /bài tập \---

\--- task \--- Vẽ hai họa tiết mới: một hình vuông màu xanh và một hình vuông màu xanh lá cây. Đây là để lựa chọn giữa bút chì màu xanh và màu xanh lá cây.

![ảnh chụp màn hình](images/paint-selectors.png) \--- /bài tập \---

\--- task \--- Đổi tên các họa tiết mới để chúng được gọi là 'blue' và 'green'

[[[generic-scratch3-rename-sprite]]]

\--- /bài tập \---

\--- Nhiệm vụ \--- Thêm một số mã để các sprite 'xanh' để khi sprite này được nhấp, nó `chương trình phát sóng`{: class = "block3events"} thông điệp "xanh".

![quảng trường xanh](images/green_square.png)

```blocks3
khi sprite này nhấp
phát (green v)
```

[[[generic-scratch3-broadcast-message]]] \--- / nhiệm vụ \---

Sprite bút chì nên lắng nghe thông điệp "xanh" và thay đổi trang phục và màu bút chì của nó để đáp ứng.

\--- task \--- Chuyển sang sprite bút chì của bạn. Thêm một số mã để khi sprite này nhận được phát sóng `green`{: class = "block3events"}, nó sẽ chuyển sang trang phục bút chì màu xanh lá cây và thay đổi màu bút thành màu xanh lá cây.

![bút chì](images/pencil.png)

```blocks3
khi tôi nhận được [xanh v]
trang phục chuyển sang (bút chì xanh v)
đặt màu bút thành [# 00CC44]
```

Để đặt bút chì thành màu xanh lục, hãy nhấp vào hình vuông màu trong khối `đặt bút màu`{: class = "block3extensions"}, sau đó nhấp vào hình vuông màu xanh lá cây. \--- /bài tập \---

Sau đó đến một điều tương tự để bạn có thể chuyển màu bút chì sang màu xanh.

\--- task \--- Nhấp vào sprite hình vuông màu xanh và thêm mã này:

![màu xanh](images/blue_square.png)

```blocks3
khi sprite này nhấp
phát (màu xanh v)
```

Sau đó bấm vào bút chì sprite và thêm mã này: ![bút chì](images/pencil.png)

```blocks3
khi tôi nhận được [blue v]
trang phục chuyển sang (bút chì màu xanh v)
đặt màu bút thành [# 0000ff]
```

\--- /bài tập \---

\--- task \--- Cuối cùng, thêm mã này để báo cho bút chì biết màu nào sẽ bắt đầu và để đảm bảo rằng màn hình rõ ràng khi chương trình của bạn bắt đầu.

![bút chì](images/pencil.png)

```blocks3
khi lá cờ nhấp
+ xóa tất cả
+ chuyển trang phục để (v bút chì màu xanh)
+ thiết bút màu để [# 0035FF]
mãi mãi
  đi tới (con trỏ chuột v)
nếu <mouse down?> sau đó
  bút xuống
  khác
  bút lên
kết thúc
```

\--- /bài tập \---

Nếu bạn thích, bạn có thể bắt đầu với một cây bút chì màu khác.

\--- nhiệm vụ \--- Kiểm tra mã của bạn. Bạn có thể chuyển đổi giữa các màu bút chì màu xanh dương và màu xanh lá cây bằng cách nhấp vào các hình vuông vuông màu xanh hoặc màu xanh lá cây?

![ảnh chụp màn hình](images/paint-pens-test.png) \--- /bài tập \---