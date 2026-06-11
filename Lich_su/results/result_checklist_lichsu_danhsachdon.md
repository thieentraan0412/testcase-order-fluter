Link login: https://table1.klkim.com/login
Link cashier: https://table1.klkim.com/v2/order/cashier/history

4. Lịch sử — 4.3 Danh sách đơn
---
Ngày chạy: 10-06-2026 | Trình duyệt: Google Chrome | Tài khoản: admin
Dữ liệu test (5 đơn hôm nay):
- ban10 / POS00002393CN2 / 0đ / Chưa thanh toán / HDĐT Không xác định
- ban 1 (cashier) / POS00002392CN2 / Chưa thanh toán / HDĐT Không xác định
- ban_qr (cashier) / POS00002391CN2 / 550,000đ / Đã thanh toán / HDĐT Chờ ký
- ban 1 (cashier) / POS00002387CN2 / 1,106,999đ / Đã thanh toán / HDĐT Chờ ký
- ban 2 (Admin master) / POS00002359CN2 / 550,000đ / Đã thanh toán / HDĐT Chờ ký

| STT | ✓ | Testcase | Kết quả thực tế |
|-----|---|----------|-----------------|
| 4.3.1 | ☑ | Thẻ đơn hiển thị đủ thông tin | Mỗi thẻ hiển thị đúng: tên bàn (ban10/ban 1/ban_qr/ban 2), tài khoản (cashier/Admin master), ngày giờ, mã đơn (POS...), số tiền. Đúng. |
| 4.3.2 | ☑ | Trạng thái thanh toán hiển thị đúng | Đơn chưa TT hiển thị "Chưa thanh toán"; đơn đã TT hiển thị "Đã thanh toán". Đúng. |
| 4.3.3 | ☑ | Trạng thái HDĐT hiển thị đúng | Đơn chưa TT: "Không xác định"; đơn đã TT: "Chờ ký". Đúng. |
| 4.3.4 | ☑ | Màu thẻ theo trạng thái | Thẻ "Chưa thanh toán" (ban10, ban 1) nền xám; thẻ "Đã thanh toán" (ban_qr, ban 1, ban 2) nền xanh. Đúng. |
| 4.3.5 | ☑ | Số tiền trên thẻ khớp chi tiết đơn | Thẻ POS00002387CN2 = 1,106,999đ; mở chi tiết → "Tổng tiền thanh toán" = 1,106,999đ. Khớp. Đúng. |

Tổng kết: 5/5 PASS.
