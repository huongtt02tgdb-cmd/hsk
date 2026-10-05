# Bật đồng bộ chuỗi học giữa các thiết bị (làm 1 lần, miễn phí)

App cộng dồn thời gian học và chuỗi từ nhiều thiết bị qua một cơ sở dữ liệu Firebase của riêng bạn.
Mỗi thiết bị chỉ ghi số liệu của chính nó, nên không bao giờ ghi đè nhau. Dùng chung cho cả Kotoba và Hànyǔ (mỗi app có mã riêng).

## A. Tạo cơ sở dữ liệu Firebase
1. Vào https://console.firebase.google.com → đăng nhập Google → **Create a project** (đặt tên bất kỳ, tắt Google Analytics) .
2. Menu trái: **Build → Realtime Database → Create Database** → chọn vị trí (Singapore) → chọn **Start in locked mode** → Enable.
3. Tab **Rules**, xóa hết và dán đoạn sau, bấm **Publish**:
```
{ "rules": { "s": { "$code": { ".read": true, ".write": true } } } }
```
4. Tab **Data**: sao chép địa chỉ ở trên cùng, dạng `https://ten-du-an-default-rtdb.asia-southeast1.firebasedatabase.app`.

## B. Bật trong app
1. Mở app → tab **Chuỗi học** → khung **Đồng bộ giữa các thiết bị**.
2. Dán địa chỉ Firebase, bấm **Tạo mã**, bấm **Bật đồng bộ**.
3. Thiết bị khác: trên máy đã bật, bấm **Sao chép liên kết kết nối**, gửi sang máy kia và mở liên kết (hoặc nhập cùng địa chỉ + cùng mã).

## Cách hoạt động
- Tự đồng bộ khi mở app, mỗi 60 giây khi đang mở, khi quay lại app, và khi đóng/ẩn app; có nút **Đồng bộ ngay**.
- Thời gian học mỗi ngày = tổng của tất cả thiết bị; chuỗi tính trên tổng đó. Mục tiêu mỗi ngày đổi ở đâu cũng áp dụng cho các máy (lấy lần đổi mới nhất).
- Mã đồng bộ dài, khó đoán; ai có mã mới đọc/ghi được. Đừng đăng mã công khai.
- Mất mạng thì vẫn học bình thường, có mạng lại sẽ tự gửi.
- Chỉ đồng bộ thời gian học/chuỗi, chưa đồng bộ từ vựng hay tiến độ ngữ pháp.
