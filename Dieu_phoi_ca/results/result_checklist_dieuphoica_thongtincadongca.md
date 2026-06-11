
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

5.2 Thông tin ca & đóng ca — Kết quả thực thi (ngày chạy: 10-06-2026)

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi | Kết quả thực tế |
|-----|---|----------|--------------------|------------------|-----------------|
| 5.2.1 | ☑ | Hiển thị header ca đúng thông tin | 1. Mở chi tiết ca 2. Quan sát header | Đúng ngày giờ, tên NV, trạng thái ca | PASS — header "05-06-2026 10:13:39 • Admin master • Đang mở" |
| 5.2.2 | ☑ | Hiển thị Tiền mặt đầu ca | 1. Mở chi tiết ca 2. Tìm "Tiền mặt đầu ca" | Đúng số tiền khai báo khi mở ca | PASS — "Tiền mặt đầu ca: 150,000đ" |
| 5.2.3 | ☑ | Nút "Đóng ca" | 1. Mở ca đang mở 2. Bấm "Đóng ca" 3. Xác nhận 4. Quan sát | Ca chuyển trạng thái đóng, giờ đóng ghi nhận đúng | PASS — đóng ca SCR58, giờ đóng 10-06-2026 14:46:46 được ghi nhận |
| 5.2.4 | ☑ | Nút "Đóng và in phiếu" | 1. Mở ca đang mở 2. Bấm "Đóng và in phiếu" 3. Xác nhận | Ca bị đóng đồng thời in phiếu kết ca | PASS — đóng ca SCR59 (giờ đóng 14:49:46) + gửi lệnh in |
| 5.2.5 | ☑ | Ca đã đóng không cho thao tác lại | 1. Bấm ca đã đóng 2. Quan sát panel 3. Kiểm tra nút đóng ca | Không hiển thị nút đóng ca | PASS — panel ca đã đóng (SCR57/SCR58) không có nút "Đóng ca"/"Đóng và in phiếu" |

Tổng: 5/5 PASS
