# Calculator App

Ứng dụng máy tính đơn giản viết bằng ngôn ngữ Flutter.

## Hướng dẫn cài đặt và chạy ứng dụng

### Yêu cầu hệ thống
- Đảm bảo bạn đã cài đặt Flutter và Dart trên máy tính của bạn. Nếu chưa, bạn có thể tham khảo cách cài đặt tại [flutter.dev](https://flutter.dev/docs/get-started/install).

### Bước 1: Sao chép dự án
Sao chép dự án từ GitHub về máy tính của bạn bằng cách sử dụng lệnh sau:
Bạn vào theo đường link github tôi đã để và copy đường dẫn 
git clone https://github.com/jkay-kmm/calculator_flutter_app.git
### Bước 2: Di chuyển thư mục vào dữ án 
- cd calculator-app
### Bước 3:  Cài đặt các dependencies
Chạy lệnh sau để cài đặt tất cả các dependencies cần thiết:
- flutter pub get
### Bước 4 Chạy ứng dụng 
- flutter run 
### Sơ lược về app
- Widget đầu vào
tất cả các tiện ích đầu vào đều mở rộng StatefulWidget vì chúng cần phản hồi cử chỉ onTap.

Nút số. Hiển thị nút số (như 1,2,3...) và xử lý cử chỉ onTap.

Nút toán tử. Hiển thị nút toán tử (như +,-,*...) và xử lý cử chỉ onTap.

Nút kết quả. Hiển thị nút lệnh (như rõ ràng, bằng nhau...) và xử lý cử chỉ onTap.

- Widget đầu ra
tất cả các tiện ích đầu ra đều được mở rộng StatelessWidget vì chúng chỉ đang hiển thị.

Hiển thị kết quả. Hiển thị kết quả hiện tại và thay đổi hiển thị khi người dùng nhấn vào nút số.

HistoryBlock. Hiển thị lịch sử tính toán và thay đổi hiển thị mỗi khi người dùng nhấn vào nút hợp lệ.

- Máy tínhTrang
Máy tínhPage được mở rộng StatefulWidget và giữ Danh sách kết quả.

Máy tínhPage nhận mọi sự kiện onTap của tiện ích đầu vào, thực hiện phép tính logic cho những đầu vào này và quyết định nội dung sẽ hiển thị cho tiện ích đầu ra.
###
| Calculator Screen | History Screen |
| --- | --- |
| ![image](images/calculator.png) | ![history](images/history.png) |
