Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table.nasys.vn/v2/order/cashier/history

4. Lịch sử
---

4.4 Chi tiết đơn hàng

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 4.4.1 | ☐ | Bấm vào đơn mở modal chi tiết | 1. Vào trang lịch sử 2. Bấm vào bất kỳ thẻ đơn nào trong danh sách 3. Quan sát màn hình | Modal "Chi tiết đơn hàng" mở ra, tiêu đề hiển thị đúng mã đơn |
| 4.4.2 | ☐ | Thông tin đơn hiển thị đúng | 1. Mở modal chi tiết một đơn bất kỳ 2. Kiểm tra lần lượt: tên bàn, tên khách hàng, tên nhân viên, ngày giờ tạo đơn | Tất cả thông tin khớp với dữ liệu thực tế của đơn |
| 4.4.3 | ☐ | Danh sách món hiển thị đúng | 1. Mở modal chi tiết đơn 2. Quan sát bảng danh sách món bên trong modal 3. Kiểm tra từng dòng: tên món, số lượng, đơn giá, thành tiền | Tên, SL, đơn giá, thành tiền của từng dòng món hiển thị đúng |
| 4.4.4 | ☐ | Tổng tiền hàng tính đúng | 1. Mở modal chi tiết đơn 2. Cộng tay thành tiền của tất cả dòng món (Σ thành tiền) 3. So sánh với dòng "Tổng tiền hàng" trong modal | Tổng tiền hàng = Σ thành tiền các món |
| 4.4.5 | ☐ | Phụ thu / Giảm giá / Tiền điểm / VAT tính đúng | 1. Mở modal chi tiết đơn có áp phụ thu, giảm giá hoặc điểm thưởng 2. Quan sát từng dòng: Phụ thu, Giảm giá, Tiền điểm, VAT 3. Kiểm tra từng giá trị có đúng với lúc tạo đơn không | Mỗi dòng phụ thu / giảm giá / điểm / VAT hiển thị đúng giá trị đã áp |
| 4.4.6 | ☐ | Tổng tiền thanh toán tính đúng công thức | 1. Mở modal chi tiết đơn 2. Ghi nhận: Tổng tiền hàng, Phụ thu, Giảm giá, Tiền điểm, VAT 3. Tính tay: Tổng hàng + Phụ thu − Giảm giá − Tiền điểm + VAT 4. So sánh với "Tổng tiền thanh toán" hiển thị | Tổng tiền thanh toán = Tổng hàng + Phụ thu − Giảm giá − Tiền điểm + VAT |
| 4.4.7 | ☐ | Phương thức thanh toán hiển thị đúng | 1. Mở modal chi tiết đơn đã thanh toán 2. Tìm mục "Phương thức thanh toán" trong modal 3. So sánh với phương thức đã chọn lúc thanh toán (Tiền mặt / CK / Thẻ / QR) | Phương thức hiển thị đúng với lúc thanh toán thực tế |
| 4.4.8 | ☐ | Bấm "Đóng" thoát modal | 1. Mở modal chi tiết đơn 2. Bấm nút "Đóng" 3. Quan sát màn hình và bộ lọc đang áp | Modal đóng lại, quay về danh sách; bộ lọc và trang hiện tại giữ nguyên |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
