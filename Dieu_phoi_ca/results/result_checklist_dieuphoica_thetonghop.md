
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

5.3 Thẻ tổng hợp (Bán hàng / Trả hàng / Phiếu thu / Phiếu chi) — Kết quả thực thi (ngày chạy: 10-06-2026)

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi | Kết quả thực tế |
|-----|---|----------|--------------------|------------------|-----------------|
| 5.3.1 | ☑ | Thẻ Bán hàng hiển thị đúng | 1. Mở chi tiết ca 2. Tìm thẻ "Bán hàng" 3. Quan sát | Đúng số đơn hàng và tổng tiền mặt bán hàng | PASS — Đơn hàng 19, Tiền mặt 2,328,476đ |
| 5.3.2 | ☑ | Thẻ Trả hàng hiển thị đúng | 1. Mở ca có trả hàng 2. Tìm thẻ "Trả hàng" 3. Kiểm tra số tiền | Đúng tổng tiền trả hàng | PASS — sau khi tạo phiếu trả test: Trả hàng 15,000đ |
| 5.3.3 | ☑ | Thẻ Phiếu thu hiển thị đúng | 1. Mở ca có phiếu thu 2. Tìm thẻ "Phiếu thu" | Đúng tổng tiền thu | PASS — sau khi tạo phiếu thu test: Phiếu thu 10,000đ |
| 5.3.4 | ☑ | Thẻ Phiếu chi hiển thị đúng | 1. Mở ca có phiếu chi 2. Tìm thẻ "Phiếu chi" | Đúng tổng tiền chi | PASS — sau khi tạo phiếu chi test: Phiếu chi 20,000đ (5,000 + 15,000 hoàn trả hàng) |
| 5.3.5 | ☑ | Bấm "..." để xem chi tiết phương thức | 1. Mở chi tiết ca 2. Bấm "..." trên thẻ 3. Quan sát | Hiện chi tiết theo từng phương thức (TM/CK/thẻ/QR/khác) | PASS — popover "Thanh toán khác": Chuyển khoản 0đ, Quẹt Thẻ 0đ, QR Tự động 261,000đ |
| 5.3.6 | ☑ | Tổng các phương thức khớp với tổng thẻ | 1. Mở chi tiết thẻ 2. Cộng tay các phương thức 3. So sánh tổng | Tổng các phương thức = tổng hiển thị | PASS (lưu ý) — mặt thẻ hiển thị Tiền mặt làm số chính, các phương thức khác ở popover "..."; số liệu nhất quán (TM 2,328,476 + QR 261,000 khớp với modal Chi tiết ca). UI không có 1 ô "tổng gộp" tất cả phương thức trên mặt thẻ |

Tổng: 6/6 PASS (5.3.6 đạt kèm ghi chú về cách hiển thị)
