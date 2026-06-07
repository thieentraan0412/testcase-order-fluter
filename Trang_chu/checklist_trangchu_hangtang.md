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
1.12 Hàng tặng

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
1.12.1 | ☐ | Mở chức năng hàng tặng trên đơn | 1. Trong màn hình Order, tìm nút "..." hoặc menu chức năng 2. Chọn "Hàng tặng" 3. Quan sát màn hình | Hiện danh sách món có thể tặng |
1.12.2 | ☐ | Chọn món tặng áp vào đơn | 1. Trong danh sách hàng tặng, chọn một món 2. Xác nhận thêm vào đơn 3. Quan sát hóa đơn | Món tặng xuất hiện trong hóa đơn với giá 0đ |
1.12.3 | ☐ | Chọn lý do tặng | 1. Khi thêm món tặng, quan sát có bước chọn lý do tặng 2. Chọn một lý do từ danh sách 3. Xác nhận | Lý do được ghi nhận kèm theo dòng món tặng |
1.12.4 | ☐ | Món tặng hiển thị trong đơn | 1. Sau khi thêm hàng tặng thành công 2. Quan sát dòng món tặng trong hóa đơn | Dòng món tặng thể hiện rõ là hàng tặng (nhãn hoặc giá 0đ) |
1.12.5 | ☐ | Hàng tặng không cộng vào tổng tiền | 1. Ghi nhận tổng tiền thanh toán trước khi thêm hàng tặng 2. Thêm món tặng vào đơn 3. So sánh tổng tiền thanh toán trước và sau | Tổng tiền thanh toán không thay đổi sau khi thêm hàng tặng |
1.12.6 | ☐ | Đơn không thỏa điều kiện | 1. Tạo đơn với giá trị thấp hoặc không đủ điều kiện áp hàng tặng 2. Thử mở chức năng hàng tặng 3. Quan sát phản hồi | Hệ thống không cho áp, hiển thị thông báo phù hợp |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
