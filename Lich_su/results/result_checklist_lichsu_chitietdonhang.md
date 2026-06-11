Link login: https://table1.klkim.com/login
Link cashier: https://table1.klkim.com/v2/order/cashier/history

4. Lịch sử — 4.4 Chi tiết đơn hàng
---
Ngày chạy: 10-06-2026 | Trình duyệt: Google Chrome | Tài khoản: admin
Đơn dùng để kiểm tra: POS00002387CN2 (ban 1, cashier, Đã thanh toán, Tiền mặt).
Nội dung modal: Khách hàng "Khách lẻ"; Ngày tạo 10-06-2026 11:38 AM; Người tạo cashier; Hình thức Tiền mặt; Bàn "ban 1"; SL khách 1.
Món: "comboo hoa hồng" (kèm Test Kho 5 +25,000đ, test5, topping 2, test may in 2) — SL 1, đơn giá 999,999đ, Món thêm 25,000đ, Thành tiền 1,024,999đ.
Tổng tiền hàng 1,024,999đ | Phụ thu 0đ | Giảm giá 0đ | Tích điểm 0 | VAT 82,000đ | Tổng thanh toán 1,106,999đ | Tiền mặt 1,106,999đ.

| STT | ✓ | Testcase | Kết quả thực tế |
|-----|---|----------|-----------------|
| 4.4.1 | ☑ | Bấm vào đơn mở modal chi tiết | Menu "..." → "Chi tiết" → modal "Chi tiết đơn hàng" mở ra, tiêu đề "Mã đơn: POS00002387CN2" đúng. Đúng. |
| 4.4.2 | ☑ | Thông tin đơn hiển thị đúng | Bàn "ban 1", khách "Khách lẻ", NV "cashier", ngày "10-06-2026 11:38 AM" — khớp dữ liệu thẻ đơn. Đúng. |
| 4.4.3 | ☑ | Danh sách món hiển thị đúng | Dòng món hiển thị tên, SL (1), đơn giá (999,999đ), món thêm (25,000đ), thành tiền (1,024,999đ). Đúng. |
| 4.4.4 | ☑ | Tổng tiền hàng tính đúng | Σ thành tiền các món = 1,024,999đ = "Tổng tiền hàng" 1,024,999đ. Đúng. |
| 4.4.5 | ☑ | Phụ thu / Giảm giá / Tiền điểm / VAT | Phụ thu 0đ, Giảm giá 0đ, Tích điểm 0, VAT 82,000đ (≈8% của 1,024,999) hiển thị đầy đủ. Đúng. |
| 4.4.6 | ☑ | Tổng tiền thanh toán đúng công thức | 1,024,999 + 0 − 0 − 0 + 82,000 = 1,106,999đ = "Tổng tiền thanh toán" hiển thị. Đúng. |
| 4.4.7 | ☑ | Phương thức thanh toán hiển thị đúng | "Hình thức: Tiền mặt" và dòng "Tiền mặt 1,106,999đ" — đúng với đơn thanh toán tiền mặt. Đúng. |
| 4.4.8 | ☑ | Bấm "Đóng" thoát modal | Bấm "Đóng" → modal đóng, quay về danh sách; bộ lọc (Tất cả) và trang hiện tại giữ nguyên. Đúng. |

Tổng kết: 8/8 PASS.
