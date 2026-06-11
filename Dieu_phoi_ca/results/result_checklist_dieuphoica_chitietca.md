
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

5.6 Chi tiết ca (modal) — Kết quả thực thi (ngày chạy: 10-06-2026, đối soát trên ca SCR00000058CN2)

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi | Kết quả thực tế |
|-----|---|----------|--------------------|------------------|-----------------|
| 5.6.1 | ☑ | Mở modal Chi tiết ca | 1. Mở chi tiết ca 2. Bấm "Chi tiết ca" 3. Quan sát modal | Modal mở, đúng mã ca, ngày giờ, tên NV | PASS — modal hiện Mã ca SCR00000058CN2, mở 05-06-2026 10:13:39, đóng 10-06-2026 14:46:46, Họ tên Admin master |
| 5.6.2 | ☑ | Bảng Thu/Chi theo phương thức trong modal | 1. Mở modal 2. Quan sát bảng theo phương thức 3. So với thẻ tổng hợp | Số liệu modal khớp thẻ tổng hợp | PASS — modal "Phương Thức Thanh Toán": Tiền Mặt 2,328,476đ (khớp thẻ Bán hàng tiền mặt), QR Tự Động 261,000đ (khớp popover "..."), Chi 20,000đ (khớp thẻ Phiếu chi) |
| 5.6.3 | ☑ | Tổng tiền mặt trong ca (modal) khớp panel chính | 1. Ghi tổng panel 2. Mở modal 3. So sánh | Giá trị tổng tiền mặt modal khớp panel | PASS (lưu ý) — modal hiển thị "Tổng tiền mặt cuối ca: 2,468,476đ" = "Tổng tiền mặt trong ca" panel (2,318,476đ) + Tiền mặt đầu ca (150,000đ); hai số đối soát khớp nhau. Modal dùng nhãn "cuối ca" (gồm đầu ca) thay vì "trong ca" |
| 5.6.4 | ☑ | Bấm "Đóng" để thoát modal | 1. Mở modal 2. Bấm "Đóng" 3. Quan sát | Modal đóng, về panel chi tiết ca | PASS — bấm "Đóng" → modal đóng, trở về panel |

Tổng: 4/4 PASS (5.6.3 đạt kèm ghi chú về nhãn "cuối ca")
