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
1.7 Xác nhận đơn (tại bàn / QR / mang về)

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.7.1 | ☐ | Tab "Chờ xác nhận" hiển thị đơn chờ | 1. Tại Trang chủ, bấm chọn checkbox "Chờ xác nhận" 2. Quan sát danh sách bàn lọc ra 3. Kiểm tra các đơn hiển thị | Hiện đúng các đơn đang chờ thu ngân xác nhận |
| 1.7.2 | ☐ | Xác nhận đơn tại bàn (gửi từ tablet/mobile) | 1. Đảm bảo có đơn được nhân viên gửi từ thiết bị tablet/mobile 2. Tại Trang chủ, lọc "Chờ xác nhận", tìm bàn tương ứng 3. Bấm vào thẻ bàn → bấm "Xác nhận" 4. Quan sát trạng thái bàn | Đơn được tiếp nhận vào bàn, trạng thái chuyển sang "Đang sử dụng" |
| 1.7.3 | ☐ | Xác nhận đơn QR (khách quét QR tại bàn) | 1. Khách quét mã QR tại bàn và đặt món 2. Tại Trang chủ, lọc "Chờ xác nhận", tìm bàn của khách 3. Bấm vào thẻ bàn → bấm "Xác nhận" 4. Quan sát trạng thái | Đơn QR của khách được tiếp nhận vào bàn |
| 1.7.4 | ☐ | Xác nhận đơn mang về | 1. Có đơn mang về đang chờ xác nhận 2. Tại Trang chủ, lọc "Chờ xác nhận", tìm thẻ đơn mang về 3. Bấm "Xác nhận" 4. Quan sát kết quả | Đơn mang về được tiếp nhận vào hệ thống |
| 1.7.5 | ☐ | Từ chối đơn | 1. Tại Trang chủ, lọc "Chờ xác nhận", tìm bàn có đơn chờ 2. Bấm vào thẻ bàn, chọn "Từ chối" thay vì "Xác nhận" 3. Quan sát kết quả | Đơn bị từ chối, không tiếp nhận vào bàn |
| 1.7.6 | ☐ | Tìm kiếm/chọn bàn cần xác nhận | 1. Tại Trang chủ đang lọc "Chờ xác nhận", dùng dropdown khu hoặc tìm kiếm để lọc bàn cụ thể 2. Quan sát kết quả | Lọc đúng bàn/đơn cần tìm |
| 1.7.7 | ☐ | Sau xác nhận, số đếm "Chờ xác nhận" giảm | 1. Ghi nhận số đếm trên checkbox "Chờ xác nhận" (VD: Chờ xác nhận (3)) 2. Xác nhận một đơn 3. Quan sát lại số đếm trên checkbox | Số đếm giảm đúng 1 đơn sau mỗi lần xác nhận |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
