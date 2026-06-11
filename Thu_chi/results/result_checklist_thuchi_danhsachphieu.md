
## 2. Thu chi — Kết quả kiểm thử

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense
Ngày chạy: 10-06-2026 | Chi nhánh: Chi nhánh Hồ Chí Minh

2.3 Danh sách phiếu

| STT | ✓ | Testcase | Kết quả thực tế |
|-----|---|----------|-----------------|
| 2.3.1 | ☑ | Hiển thị bảng phiếu đủ cột | Bảng có đủ các cột: STT, Mã phiếu, Loại thu chi, Số tiền, Tên chi nhánh, Người nộp/Người nhận, Người tạo, Phân loại thu chi, Phương thức thanh toán, Đính kèm, Thời gian ghi nhận, Mô tả, Hành động. Dữ liệu điền đúng theo từng phiếu. |
| 2.3.2 | ☑ | Phân trang | Trang 1 hiển thị STT 1–10, trang 2 hiển thị STT 11–20 (PT1833…PT1824), tuần tự, không trùng/thiếu. Chuyển trang hoạt động. |
| 2.3.3 | ☑ | Bấm icon xem để mở chi tiết | Bấm icon mắt ở cột Hành động → mở modal "Xem chi tiết" đúng phiếu (PT00001833CN2: Thu, 22,000đ, Tiền mặt, 09-06-2026, Mã hóa đơn POS00002355CN2). |
| 2.3.4 | x | Phiếu có đính kèm | KHÔNG kiểm chứng được: trong toàn bộ dữ liệu hiện có, cột "Đính kèm" của mọi phiếu đều trống — không tìm thấy phiếu nào có tệp đính kèm để mở/tải. Cần dữ liệu phiếu có đính kèm để test (không kết luận lỗi). |

Tổng: 3/4 PASS, 1 không kiểm chứng được (thiếu dữ liệu phiếu đính kèm).
