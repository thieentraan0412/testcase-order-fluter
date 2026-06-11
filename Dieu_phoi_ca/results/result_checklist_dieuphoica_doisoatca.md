
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

5.5 Đối soát ca (logic tính) — Kết quả thực thi (ngày chạy: 10-06-2026)

Dữ liệu ca SCR00000058CN2 dùng để đối soát:
- Tiền mặt đầu ca: 150,000đ
- Bán hàng tiền mặt: 2,328,476đ (QR 261,000đ — không tính vào tiền mặt)
- Phiếu thu tiền mặt (test): 10,000đ
- Phiếu chi tiền mặt: 20,000đ (5,000 thủ công + 15,000 hoàn trả hàng)
- Trả hàng: 15,000đ
- Tổng tiền mặt trong ca hiển thị: 2,318,476đ

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi | Kết quả thực tế |
|-----|---|----------|--------------------|------------------|-----------------|
| 5.5.1 | ☑ | Tổng tiền mặt tính đúng công thức | Cộng/trừ tay rồi so với hiển thị | Tổng = TM bán hàng + phiếu thu − trả hàng − phiếu chi | PASS — 2,328,476 + 10,000 − 20,000 = 2,318,476 khớp. (Khoản hoàn trả hàng được ghi nhận như Phiếu chi nên trừ 1 lần qua Phiếu chi, không trừ trùng với thẻ Trả hàng) |
| 5.5.2 | ☑ | Tiền mặt đầu ca KHÔNG cộng vào tổng | So tổng với/không có đầu ca | Đầu ca không cộng vào "Tổng tiền mặt trong ca" | PASS — 2,318,476 ≠ 2,318,476 + 150,000; đầu ca chỉ cộng ở "Tiền mặt cuối ca" lúc đóng ca |
| 5.5.3 | ☑ | Chỉ tính giao dịch tiền mặt vào tổng | Quan sát ca có nhiều phương thức | CK/thẻ/QR không ảnh hưởng tổng tiền mặt | PASS — QR 261,000đ không cộng vào tổng tiền mặt |
| 5.5.4 | ☑ | Phiếu bán hàng ghi nhận vào ca | Tạo đơn bán trong ca, kiểm tra | Đơn bán xuất hiện trong danh sách giao dịch | PASS — tạo đơn POS00002359CN2 (15,000đ TM): Bán hàng 18→19 đơn, tổng +15,000 |
| 5.5.5 | ☑ | Phiếu trả hàng làm giảm tổng đúng | Tạo phiếu trả, so chênh lệch | Tổng giảm đúng bằng số tiền trả | PASS — trả HT000038 (15,000đ): tổng 2,333,476 → 2,318,476 (giảm đúng 15,000) |
| 5.5.6 | ☑ | Phiếu thu cộng vào ca đúng | Tạo phiếu thu, so chênh lệch | Tổng tăng đúng bằng số tiền thu | PASS — tạo PT00001840 (10,000đ TM): thẻ Phiếu thu = 10,000, tổng tăng đúng 10,000 |
| 5.5.7 | ☑ | Phiếu chi trừ khỏi ca đúng | Tạo phiếu chi, so chênh lệch | Tổng giảm đúng bằng số tiền chi | PASS — tạo PC00000082 (5,000đ TM): thẻ Phiếu chi = 5,000, tổng giảm đúng 5,000 |
| 5.5.8 | ⚠ | Giao dịch đã hủy không tính vào tổng | Lọc "Đã hủy", tính tổng "Hoàn thành", so sánh | Tổng chỉ tính giao dịch hoàn thành | CHƯA KIỂM CHỨNG TRỰC TIẾP — thao tác duy nhất để vô hiệu phiếu trong module Thu chi là "Xóa" (xóa vĩnh viễn, không thực hiện theo nguyên tắc an toàn); ca sạch không có giao dịch hủy sẵn để quan sát. Bằng chứng gián tiếp: tổng tiền mặt luôn khớp đúng tổng các giao dịch hoàn thành (xác minh nhiều lần ở 5.5.1/5.5.6/5.5.7). KHUYẾN NGHỊ: cần test lại bằng cách hủy (không xóa) 1 giao dịch và đối chiếu tổng |

Tổng: 7/8 PASS, 1 chưa kiểm chứng (5.5.8)
