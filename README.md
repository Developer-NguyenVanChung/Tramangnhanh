# Tra Mạng Nhanh (Android 9+)

Ứng dụng Android Java có bong bóng nổi, tra cứu tên **nhà mạng gốc** theo đầu số, hỗ trợ 0xxxxxxxxx và +84xxxxxxxxx. Không yêu cầu Internet.

## Biên dịch APK
1. Cài Android Studio (JDK 17), mở thư mục `TraMangNhanh`.
2. Đợi Gradle đồng bộ (cần Internet lần đầu để tải Android Gradle Plugin và SDK 35).
3. Chọn **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. APK debug tại `app/build/outputs/apk/debug/app-debug.apk`.
5. Chuyển APK sang OPPO A31, cài đặt và cấp quyền **Hiển thị trên ứng dụng khác** khi được hỏi.
6. Mở ứng dụng, chọn **BẬT BONG BÓNG NỔI**. Chạm bong bóng để mở cửa sổ nhập số, bấm **DÁN SỐ** hoặc dán trực tiếp.

## Giới hạn quan trọng
- Không xác định được **nhà mạng hiện tại** nếu số đã chuyển mạng giữ số.
- Android 9 có thể cho phép đọc clipboard khi chạy nền, nhưng ứng dụng này **chỉ đọc clipboard khi bảng tra cứu nổi đang mở** để bảo vệ riêng tư. Vì vậy việc sao chép số ở ứng dụng khác không đảm bảo tự hiện kết quả khi bong bóng đang thu nhỏ.
- Các đầu số mạng di động ảo và các thay đổi cấp phát mới cần cập nhật dữ liệu; khi chưa rõ sẽ hiện `Chưa xác định`.
- Chưa được biên dịch/kiểm thử trên thiết bị thật trong môi trường này.
