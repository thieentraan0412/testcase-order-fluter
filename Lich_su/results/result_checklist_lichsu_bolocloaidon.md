Link login: https://table1.klkim.com/login
Link cashier: https://table1.klkim.com/v2/order/cashier/history

4. Lịch sử — 4.1 Bộ lọc loại đơn
---
Ngày chạy: 10-06-2026 | Trình duyệt: Google Chrome | Tài khoản: admin (cửa hàng "trong")
Ghi chú dữ liệu: Tại thời điểm test chỉ có 1 đơn trong ngày — Bàn 1 / POS00000405CN2 / 684,000đ / Chưa thanh toán (đơn Tại bàn).

| STT | ✓ | Testcase | Kết quả mong đợi | Kết quả thực tế |
|-----|---|----------|------------------|-----------------|
| 4.1.1 | ☑ | Lọc tab "Tất cả" | Hiển thị tất cả đơn không phân biệt loại | Tab "Tất cả" hiển thị đơn Bàn 1 (đơn duy nhất trong ngày). Đúng. |
| 4.1.2 | ☑ | Lọc tab "Tại bàn" | Chỉ hiện các đơn loại tại bàn | Hiển thị đúng đơn Bàn 1 (loại tại bàn). Đúng. |
| 4.1.3 | ☑ | Lọc tab "Mang về" | Chỉ hiện các đơn mang về | Hiển thị "Không tìm thấy dữ liệu phù hợp" — không có đơn mang về trong ngày. Đúng. |
| 4.1.4 | ☑ | Lọc tab "Đặt online" | Chỉ hiện đơn đặt online; nếu không có thì rỗng | Danh sách rỗng ("Không tìm thấy dữ liệu phù hợp"). Đúng. |
| 4.1.5 | ☑ | Dropdown "Chọn bàn" | Chỉ hiện các đơn thuộc bàn đã chọn | Dropdown hiển thị Tất cả/Bàn 1..6. Chọn "Bàn 1" → chỉ hiện đơn của Bàn 1. Đúng. |

Tổng kết: 5/5 PASS.
