# FarmTool releases

Kho phát hành public chỉ chứa README và bản ứng dụng. Không chứa mã nguồn dự án, dữ liệu tài khoản hay khóa ký.

## Tải ứng dụng

Vào [Release mới nhất](https://github.com/logg1s/farmtool-releases/releases/latest) để xem changelog và tải:

- Windows x64: `FarmTool-PC-Windows-x64.exe`, một EXE duy nhất; không cần giải nén hoặc Python. Cần Microsoft Edge WebView2.
- Android: APK arm64 cho thiết bị ARM64, APK x64 cho giả lập/thiết bị x64. Cài đè cùng chứng thư để giữ dữ liệu; không gỡ app.

## Cập nhật trong app

Từ 1.1.3, Windows tải và kiểm SHA256, chờ lượt cày kết thúc, tự đóng, thay EXE tại chỗ và mở bản mới. Chỉ khôi phục các nick vừa chạy; không bật nick đã dừng hay tính năng nhóm. Thư mục EXE cần có quyền ghi. Nếu bản mới không mở được, phục hồi EXE cũ.

Android tải APK đúng kiến trúc, kiểm SHA256 rồi mở trình cài. Khi cần cấp quyền cài từ FarmTool, cho phép rồi quay lại; trình cài tự mở, kể cả nếu Android vừa tạo lại app. Bạn vẫn phải xác nhận Cập nhật trên trình cài Android.

Changelog do người phát hành soạn trên GitHub Release và hiển thị trực tiếp trong app. ZIP/CHANGELOG assets giữ để tương thích bản cũ; file Windows chính là EXE.

Bản 1.1.2 trở về trước cần tải/mở 1.1.3 một lần để có luồng mới. Dữ liệu Windows ở `%LOCALAPPDATA%\FarmTool`, không gửi thư mục này cho người khác. Không chạy cùng nick trên nhiều runtime.
