
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

Hãy sử dụng google chorme và thực hiện các testcase sau

5.6 Chi tiết ca (modal)

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 5.6.1 | ☐ | Mở modal Chi tiết ca | 1. Mở chi tiết một ca ở panel bên phải 2. Bấm nút "Chi tiết ca" 3. Quan sát modal hiện ra | Modal mở ra, hiển thị đúng mã ca, ngày giờ, tên nhân viên |
| 5.6.2 | ☐ | Bảng Thu/Chi theo phương thức trong modal | 1. Mở modal Chi tiết ca 2. Quan sát bảng Thu/Chi được phân theo từng phương thức thanh toán 3. So sánh số liệu với các thẻ tổng hợp ở panel chính | Số liệu trong modal khớp với số liệu trên các thẻ tổng hợp |
| 5.6.3 | ☐ | Tổng tiền mặt trong ca (modal) khớp panel chính | 1. Ghi nhận số "Tổng tiền mặt trong ca" hiển thị tại panel chi tiết chính 2. Mở modal Chi tiết ca 3. Tìm và ghi nhận số "Tổng tiền mặt trong ca" trong modal 4. So sánh hai con số | Giá trị tổng tiền mặt trong modal khớp với panel chính |
| 5.6.4 | ☐ | Bấm "Đóng" để thoát modal | 1. Mở modal Chi tiết ca 2. Bấm nút "Đóng" 3. Quan sát màn hình | Modal đóng lại, quay về panel chi tiết ca bên phải |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
