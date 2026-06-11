
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

Hãy sử dụng google chorme và thực hiện các testcase sau

5.2 Thông tin ca & đóng ca

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 5.2.1 | ☐ | Hiển thị header ca đúng thông tin | 1. Vào trang lịch sử ca 2. Bấm vào một ca để mở chi tiết ở panel bên phải 3. Quan sát phần header (tiêu đề) của panel chi tiết | Hiển thị đúng ngày giờ, tên nhân viên, trạng thái ca |
| 5.2.2 | ☐ | Hiển thị Tiền mặt đầu ca | 1. Mở chi tiết một ca bất kỳ 2. Tìm mục "Tiền mặt đầu ca" trong panel chi tiết 3. So sánh với số tiền nhân viên đã khai báo lúc mở ca | Hiển thị đúng số tiền mặt đã khai báo khi mở ca |
| 5.2.3 | ☐ | Nút "Đóng ca" | 1. Mở chi tiết của ca đang ở trạng thái "Đang mở" 2. Tìm và bấm nút "Đóng ca" 3. Xác nhận thao tác nếu có hộp thoại xác nhận 4. Quan sát trạng thái ca sau khi đóng | Ca chuyển sang trạng thái đóng, giờ đóng được ghi nhận chính xác |
| 5.2.4 | ☐ | Nút "Đóng và in phiếu" | 1. Mở chi tiết của ca đang ở trạng thái "Đang mở" 2. Tìm và bấm nút "Đóng và in phiếu" 3. Xác nhận nếu có hộp thoại 4. Quan sát kết quả | Ca bị đóng đồng thời in phiếu kết ca |
| 5.2.5 | ☐ | Ca đã đóng không cho thao tác lại | 1. Bấm vào một ca đã có giờ đóng (trạng thái đã đóng) 2. Quan sát panel chi tiết bên phải 3. Kiểm tra xem nút "Đóng ca" / "Đóng và in phiếu" có hiển thị hay không | Không hiển thị nút đóng ca; không thể thực hiện thao tác đóng lại ca đã đóng |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
