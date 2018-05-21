## Mắc lỗi

Đôi khi những sai lầm xảy ra, vì vậy, hãy thêm nút 'xóa' và công cụ xóa.

+ Thêm 'X-block' sprite - bạn sẽ tìm thấy nó trong thư viện, trong phần chữ cái. Màu trang phục màu đỏ. Điều này sẽ trở thành nút 'rõ ràng'.

![ảnh chụp màn hình](images/paint-x.png)

+ Thêm mã vào sprite này để xóa sân khấu khi nó được nhấp.

![Xóa sân khấu](images/clear-stage.png)

Lưu ý rằng bạn không cần phải gửi một tin nhắn để xóa các giai đoạn, bạn chỉ có thể sử dụng khối rõ ràng từ sprite này.

Bạn có thể nhận thấy rằng bút chì của bạn bao gồm một trang phục tẩy:

![ảnh chụp màn hình](images/paint-eraser-costume.png)

+ Dự án của bạn cũng bao gồm một eraser eraser riêng biệt. Nhấp chuột phải vào sprite này và chọn 'show'. Đây là cách mà sân khấu của bạn sẽ trông như thế nào:

![ảnh chụp màn hình](images/paint-eraser-stage.png)

+ Thêm mã vào eraser sprite, để báo cho bút chì chuyển sang một cục tẩy khi nhấn sprite.

![Phát sóng tẩy](images/broadcast-eraser.png)

Khi bút chì nhận được thông báo "tẩy", bạn có thể chuyển trang phục bút chì thành công cụ xóa và chuyển màu bút chì thành màu trắng - cùng màu với vùng hiển thị!

+ Thêm một số mã để tạo công cụ xóa

\--- gợi ý \--- \--- gợi ý \--- Thêm một số mã vào bút chì sprite: **Khi tôi nhận được** **tẩy** tin nhắn **Chuyển sang trang phục** tẩy **Đặt bút màu** đến trắng \--- / gợi ý \--- \--- hint \--- Đây là cách mã bên trong bút chì sprite nên:

```blocks
khi tôi nhận được [eraser v] chuyển trang phục sang [eraser v] đặt bút màu thành [#FFFFFF]
```

\--- / gợi ý \--- \--- / gợi ý \---

+ Kiểm tra dự án của bạn, để xem bạn có thể xóa và xóa trên sân khấu hay không.

![ảnh chụp màn hình](images/paint-erase-test.png)

Có một vấn đề nữa với bút chì - bạn có thể vẽ bất kỳ nơi nào trên sân khấu, bao gồm gần các biểu tượng chọn!

![ảnh chụp màn hình](images/paint-draw-problem.png)

Để khắc phục điều này, chỉ cho bút chì vẽ nếu chuột được nhấp *và* nếu vị trí y của chuột lớn hơn -120:

![ảnh chụp màn hình](images/pencil-gt-code.png)

+ Kiểm tra dự án của bạn; bây giờ bạn không thể vẽ gần khối chọn.

![ảnh chụp màn hình](images/paint-fixed.png)