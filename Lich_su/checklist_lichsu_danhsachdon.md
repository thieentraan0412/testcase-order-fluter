Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table.nasys.vn/v2/order/cashier/history

4. Lịch sử
---

4.3 Danh sách đơn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
4.3.1 | ☐ | Thẻ đơn hiển thị đủ thông tin | 1. Vào trang lịch sử 2. Quan sát một thẻ đơn bất kỳ trong danh sách 3. Kiểm tra từng thông tin: tên bàn, tài khoản nhân viên, ngày giờ, mã đơn, số tiền | Thẻ hiển thị đúng tên bàn, tài khoản, ngày giờ, mã đơn, số tiền |
4.3.2 | ☐ | Trạng thái thanh toán hiển thị đúng | 1. Vào trang lịch sử 2. Tìm một đơn đã thanh toán và một đơn chưa thanh toán 3. Quan sát nhãn trạng thái trên mỗi thẻ đơn | Đơn đã thanh toán hiển thị "Đã thanh toán"; đơn chưa thanh toán hiển thị "Chưa thanh toán" |
4.3.3 | ☐ | Trạng thái HĐĐT hiển thị đúng | 1. Vào trang lịch sử 2. Tìm đơn có cột/nhãn trạng thái hóa đơn điện tử (HĐĐT) 3. Quan sát giá trị hiển thị | Hiển thị đúng trạng thái: "Không xác định" hoặc "Chờ ký" tùy theo đơn |
4.3.4 | ☐ | Màu thẻ theo trạng thái | 1. Vào trang lịch sử 2. Quan sát màu nền hoặc màu viền các thẻ đơn 3. So sánh màu giữa đơn chưa thanh toán và đơn đã thanh toán | Đơn chưa thanh toán màu xám; đơn đã thanh toán màu xanh |
4.3.5 | ☐ | Số tiền trên thẻ khớp chi tiết đơn | 1. Quan sát số tiền hiển thị trên thẻ đơn, ghi nhận lại 2. Bấm vào thẻ đơn đó để mở chi tiết 3. So sánh số tiền trong modal chi tiết với số tiền trên thẻ | Số tiền trên thẻ = tổng tiền thanh toán trong chi tiết đơn |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
