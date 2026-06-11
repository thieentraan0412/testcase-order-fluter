
## 2. Thu chi — Kết quả kiểm thử

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense
Ngày chạy: 10-06-2026 | Chi nhánh: Chi nhánh Hồ Chí Minh

2.5 Ghi nhận 4 loại phiếu (logic chính)

| STT | ✓ | Testcase | Kết quả thực tế |
|-----|---|----------|-----------------|
| 2.5.1 | ☑ | Tạo Phiếu thu thủ công | Tạo phiếu Thu 200,000 (PT00001843CN2) → Tổng thu tăng 5,165,936 → 5,365,936; Tồn quỹ cuối kỳ tăng tương ứng. |
| 2.5.2 | ☑ | Tạo Phiếu chi thủ công | Tạo phiếu Chi 100,000 (PC00000084CN2) → Tổng chi tăng 20,000 → 120,000; Tồn quỹ cuối kỳ giảm tương ứng. |
| 2.5.3 | ☑ | Phiếu thu hiển thị đúng thông tin | Phiếu thu thủ công hiển thị đúng: Loại = Thu, Số tiền đúng, PTTT đúng (VD PT00001843CN2: Thu, 200,000, Tiền mặt). |
| 2.5.4 | ☑ | Phiếu chi hiển thị đúng thông tin | Phiếu chi thủ công hiển thị đúng: Loại = Chi, Số tiền 100,000, Người nhận "Nhà cung cấp 10", PTTT Chuyển khoản, Mô tả lưu đúng (PC00000084CN2). |
| 2.5.5 | ☑ | Hoàn tất đơn bán → tự sinh Phiếu bán hàng | Tạo & thanh toán đơn POS00002360CN2 (15,000, Chuyển khoản) tại Ban 3 → tự sinh phiếu PT00001844CN2: Loại = Thu, Loại nguồn = Bán hàng, chi tiết liên kết "Mã hóa đơn: POS00002360CN2". |
| 2.5.6 | ☑ | Thực hiện trả hàng → tự sinh Phiếu trả hàng | Xác minh qua phiếu sinh tự động sẵn có: PC00000083CN2 — Loại = Chi, Loại nguồn = Trả hàng, chi tiết liên kết "Mã hóa đơn: HT000038" (chứng từ hoàn trả). |
| 2.5.7 | ☑ | Lọc Loại nguồn = Bán hàng | Lọc "Bán hàng" → chỉ hiện phiếu sinh từ đơn bán (toàn bộ Loại = Thu, gồm PT00001844 vừa sinh). |
| 2.5.8 | ☑ | Lọc Loại nguồn = Trả hàng | Lọc "Trả hàng" → chỉ hiện phiếu sinh từ trả hàng (PC00000083CN2, Loại = Chi). |
| 2.5.9 | ☑ | Lọc Loại nguồn = Tự tạo | Lọc "Tự tạo" → chỉ hiện phiếu thu/chi tạo thủ công (có nút sửa/xóa, không có mã hóa đơn POS). |
| 2.5.10 | ☑ | Số tiền phiếu bán hàng khớp đơn gốc | Phiếu PT00001844CN2 = 15,000đ = tổng tiền đơn POS00002360CN2. Khớp. |
| 2.5.11 | ☑ | Số tiền phiếu trả hàng khớp đơn gốc | Phiếu PC00000083CN2 = 15,000đ, liên kết chứng từ trả hàng HT000038. Số tiền khớp giá trị trả. |
| 2.5.12 | ☑ | PTTT của phiếu tự sinh khớp đơn gốc | Thanh toán đơn POS00002360CN2 bằng "Chuyển khoản" → phiếu PT00001844CN2 có PTTT = "Chuyển khoản". Khớp. |
| 2.5.13 | – | Đơn bán bị hủy → phiếu không tính vào quỹ | KHÔNG thực hiện trong lần chạy này để tránh thao tác hủy/void đơn (mang tính phá hủy dữ liệu). Bằng chứng gián tiếp: trong Điều phối ca chỉ các giao dịch "Đã thanh toán" mới sinh phiếu; phiếu thu/chi chỉ được tạo khi thanh toán thành công (đã quan sát ở 2.5.5), nên đơn chưa/không thanh toán sẽ không sinh phiếu. Cần test thủ công riêng để xác nhận trực tiếp. |
| 2.5.14 | ☑ | Số liệu Thu chi khớp với Điều phối ca | Màn Điều phối ca (ca SCR00000060CN2) liệt kê đúng: PT00001844 (15,000/Chuyển khoản), POS00002360 (15,000/Chuyển khoản), PT00001843 (200,000/Tiền mặt), PC00000084 (100,000/Chuyển khoản) — Số tiền & PTTT khớp với phiếu Thu chi. |
| 2.5.15 | ☑ | Tổng thu = Σ tất cả nguồn thu | Lọc Hôm nay + Thu: 15,000+200,000+0+15,000+10,000 = 240,000 (gồm thủ công + bán hàng PT00001844). Thẻ "Tổng thu" = 240,000. Khớp. |
| 2.5.16 | ☑ | Tổng chi = Σ tất cả nguồn chi | Lọc Hôm nay + Chi: 100,000+15,000+5,000 = 120,000 (gồm thủ công + trả hàng PC00000083). Thẻ "Tổng chi" = 120,000. Khớp. |

Tổng: 15/16 PASS, 1 chưa kiểm chứng (2.5.13 — không thực hiện hủy đơn).

Lưu ý: Lần chạy này có tạo 1 đơn bán thật POS00002360CN2 (Ban 3, món VAT 0% = 15,000, Chuyển khoản) → sinh phiếu thu PT00001844CN2.
