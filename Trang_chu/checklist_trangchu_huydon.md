# Checklist Testcase — App F&B (NASYS POS)

> Nền tảng: Ordertable riêng. Xây dựng dần qua từng video. Đổi ☐ → ☑ khi xong.

Link login https://table1.klkim.com/login
tài khoản
    Cửa hàng : trong
    Tài khoản: admin
    Mật khẩu : 147258

Link cashier https://table1.klkim.com/v2/order/cashier
Link manager https://table1.klkim.com/v2/dashboard
Sau khi truy cập link: Click vào bàn    
---
1.14 Hủy đơn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
1.14.1 | ☐ | Hủy đơn chưa thanh toán | 1. Vào bàn có đơn chưa thanh toán 2. Tìm chức năng "Hủy đơn" (thường trong menu "...") 3. Chọn lý do và xác nhận hủy 4. Quan sát bàn ngoài Trang chủ | Đơn bị hủy, bàn về trạng thái trống |
1.14.2 | ☐ | Chọn lý do hủy (bắt buộc) | 1. Mở chức năng hủy đơn 2. Bỏ qua bước chọn lý do, thử bấm xác nhận ngay 3. Quan sát phản hồi | Hệ thống bắt buộc chọn lý do, không hủy được nếu bỏ trống |
1.14.3 | ☐ | Xác nhận hủy | 1. Mở chức năng hủy đơn 2. Chọn lý do hủy 3. Bấm "Xác nhận" 4. Quan sát kết quả | Đơn hoàn tất hủy, không còn trong danh sách đơn hoạt động |
1.14.4 | ☐ | Hủy đơn đã thanh toán | 1. Vào Lịch sử, tìm một đơn đã thanh toán thành công 2. Thử thao tác hủy đơn đó 3. Quan sát phản hồi | Hệ thống chặn, không cho hủy đơn đã thanh toán |
1.14.5 | ☐ | Không có quyền / chưa mở ca | 1. Đăng nhập bằng tài khoản không có quyền hủy đơn hoặc đảm bảo ca chưa mở 2. Vào bàn có đơn 3. Thử thao tác hủy đơn | Hệ thống chặn, hiển thị thông báo không có quyền hoặc yêu cầu mở ca |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
