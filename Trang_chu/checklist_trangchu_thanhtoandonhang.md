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
1.15 Thanh toán đơn hàng (qua Chờ thanh toán)

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
1.15.1 | ☐ | Tab "Chờ thanh toán" hiển thị đơn chờ | 1. Tại Trang chủ, bấm chọn checkbox "Chờ thanh toán" 2. Quan sát danh sách bàn lọc ra | Hiển thị đúng các bàn/đơn đang chờ thanh toán |
1.15.2 | ☐ | Thanh toán từ tab Chờ thanh toán | 1. Tại Trang chủ, lọc tab "Chờ thanh toán" 2. Bấm vào bàn cần thanh toán 3. Thực hiện thanh toán đơn 4. Quan sát bàn sau khi xong | Thanh toán thành công, bàn về trạng thái trống |
1.15.3 | ☐ | Thanh toán bằng cách chọn bàn đang dùng | 1. Tại Trang chủ, bấm trực tiếp vào bàn đang sử dụng 2. Vào màn hình Order của bàn đó 3. Thực hiện thanh toán theo yêu cầu khách | Thanh toán thành công, bàn về trống |
1.15.4 | ☐ | Thanh toán đơn order gửi từ tablet/mobile | 1. Đảm bảo có đơn được gửi từ thiết bị tablet/mobile của khách 2. Tại màn hình cashier, xác nhận đơn vào bàn 3. Thực hiện thanh toán đơn đó | Đơn được tiếp nhận và thanh toán đúng |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
