
## 2. Thu chi — Kết quả kiểm thử

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense
Ngày chạy: 10-06-2026 | Chi nhánh: Chi nhánh Hồ Chí Minh

2.4 Thêm phiếu

| STT | ✓ | Testcase | Kết quả thực tế |
|-----|---|----------|-----------------|
| 2.4.1 | ☑ | Bấm "Thêm" mở modal | Bấm "Thêm" → mở modal "Thêm phiếu" đầy đủ các trường. |
| 2.4.2 | ☑ | Mã phiếu tự sinh | Ô Mã phiếu ở chế độ tự động (disabled, placeholder "Mã tự động"). Mã được hệ thống tự sinh khi lưu (Thu: PTxxxxxxxxCN2, Chi: PCxxxxxxxxCN2). Ghi chú: ví dụ "vote-00001" trên placeholder không khớp định dạng thật; mã không hiển thị trước trong form. |
| 2.4.3 | ☑ | Bỏ trống "Loại thu chi" (bắt buộc) | Để trống Loại thu chi, bấm Lưu → bị chặn, hiện toast "Trường Loại thu chi là bắt buộc." |
| 2.4.4 | x | Bỏ trống "Số tiền" (bắt buộc) | LỖI: để trống Số tiền (tự về 0) rồi Lưu → KHÔNG bị chặn, hệ thống tạo phiếu PT00001842CN2 với Số tiền = 0. Lẽ ra phải chặn và báo lỗi yêu cầu nhập Số tiền. |
| 2.4.5 | ☑ | Chọn Loại đối tượng / Người nộp | Chọn Loại đối tượng "Nhà cung cấp" + Người nộp "Nhà cung cấp 10" → hiển thị đúng trong form. |
| 2.4.6 | ☑ | Chọn Phân loại thu chi | Chọn "Dịch vụ" → ghi nhận trong ô. (Ghi chú: cột "Phân loại thu chi" ở danh sách hiển thị trống.) |
| 2.4.7 | ☑ | Chọn Phương thức thanh toán | PTTT mặc định "Tiền mặt"; đổi sang "Chuyển khoản" → ghi nhận đúng (phiếu PC84 lưu với PTTT Chuyển khoản). |
| 2.4.8 | ☑ | Nhập Số tiền | Nhập chữ "abc" → ô về "0" (không nhận chữ); nhập 150000 → tự định dạng "150,000". |
| 2.4.9 | ☑ | Đính kèm tệp | Chọn tệp test_attachment.png → tên file hiển thị trong ô đính kèm. |
| 2.4.10 | ☑ | Mô tả giới hạn 200 ký tự | Nhập 220 ký tự → bộ đếm dừng ở "200/200", phần dư bị cắt. |
| 2.4.11 | ☑ | Bấm "Lưu" hợp lệ | Điền đủ trường bắt buộc + Lưu → phiếu mới (PC00000084CN2) xuất hiện đầu danh sách; thẻ Tổng chi cập nhật 20,000 → 120,000. |
| 2.4.12 | ☑ | Bấm "Đóng" không tạo phiếu | Điền số tiền rồi bấm "Đóng" → modal đóng, không có phiếu mới, danh sách & thẻ không đổi. |
| 2.4.13 | ☑ | Mã phiếu tăng dần sau mỗi lần tạo | Tạo liên tiếp: PT00001842 → PT00001843 (Thu) và PC00000083 → PC00000084 (Chi) — mã tăng đúng +1, không lặp. Ghi chú: modal không hiển thị mã trước khi lưu nên không quan sát được trong form. |
| 2.4.14 | x | Nhập Số tiền = 0 | LỖI: Số tiền = 0 (qua trường hợp trống tự về 0) → hệ thống vẫn lưu thành công (phiếu PT00001842CN2 = 0đ). Lẽ ra phải chặn và yêu cầu số tiền > 0. |
| 2.4.15 | ☑ | Loại đối tượng đổi → Người nộp đổi | "Thu ngân" → list (Tịnh Tâm, tranvanc, Nguyễn C, manager0001); đổi "Nhà cung cấp" → list (Vissan, Coca, Pepsi, NCC 4–10). Danh sách Người nộp đổi đúng theo Loại đối tượng. |
| 2.4.16 | ☑ | Loại đối tượng chưa chọn → Người nộp | Khi chưa chọn Loại đối tượng, dropdown Người nộp chỉ có "Chọn" (danh sách rỗng). |
| 2.4.17 | x | Loại thu chi = "Chi" → label "Người nhận" | LỖI: Chọn "Thu" → nhãn "Người nộp" (đúng); nhưng chọn "Chi" → nhãn VẪN là "Người nộp", không đổi thành "Người nhận". |
| 2.4.18 | x | Xóa file đính kèm sau khi đã chọn | LỖI: Sau khi chọn tệp, KHÔNG có nút xóa (X) bên cạnh tên file; không thể gỡ tệp để ô trở về "Chưa có tệp nào được chọn" (chỉ có thể chọn đè tệp khác). |
| 2.4.19 | ☑ | Lưu phiếu thu → Tồn quỹ tăng đúng | Tạo phiếu Thu 200,000 (PT00001843CN2) → Tổng thu 5,165,936 → 5,365,936 (+200,000); Tồn quỹ cuối kỳ tăng tương ứng. |
| 2.4.20 | ☑ | Lưu phiếu chi → Tồn quỹ giảm đúng | Tạo phiếu Chi 100,000 (PC00000084CN2) → Tổng chi 20,000 → 120,000 (+100,000); Tồn quỹ cuối kỳ giảm tương ứng. |

Tổng: 16/20 PASS, 4 FAIL (2.4.4, 2.4.14, 2.4.17, 2.4.18).

Lưu ý: Quá trình test có tạo các phiếu thật trên hệ thống: PT00001842 (Thu 0đ), PC00000084 (Chi 100,000), PT00001843 (Thu 200,000).
