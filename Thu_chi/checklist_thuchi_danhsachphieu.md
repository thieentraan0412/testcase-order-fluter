
## 2. Thu chi

Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense

---

Hãy sử dụng google chorme và thực hiện các testcase sau

2.3 Danh sách phiếu

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 2.3.1 | ☐ | Hiển thị bảng phiếu đủ cột | 1. Vào trang Thu chi 2. Quan sát bảng danh sách phiếu 3. Kiểm tra từng cột hiển thị: mã phiếu, loại, số tiền, chi nhánh, người nộp/nhận, người tạo, phân loại, PTTT, đính kèm, thời gian, mô tả | Bảng hiển thị đầy đủ tất cả các cột, dữ liệu điền đúng theo từng phiếu |
| 2.3.2 | ☐ | Phân trang | 1. Vào trang Thu chi với đủ số phiếu để có nhiều trang 2. Quan sát điều hướng trang (số trang, nút chuyển trang) 3. Bấm sang trang 2, trang 3 4. Quan sát dữ liệu từng trang | Chuyển trang đúng, dữ liệu mỗi trang không bị trùng hoặc thiếu |
| 2.3.3 | ☐ | Bấm icon xem để mở chi tiết | 1. Trong danh sách phiếu, tìm cột "Hành động" ở cuối mỗi dòng 2. Bấm icon xem (mắt/con mắt) tại một phiếu bất kỳ 3. Quan sát màn hình mở ra | Mở đúng trang hoặc modal chi tiết của phiếu đó |
| 2.3.4 | ☐ | Phiếu có đính kèm | 1. Trong danh sách phiếu, tìm một phiếu có file đính kèm (cột đính kèm hiển thị icon/link) 2. Bấm vào đính kèm đó 3. Quan sát kết quả | File đính kèm hiển thị hoặc tải xuống được, không báo lỗi |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
