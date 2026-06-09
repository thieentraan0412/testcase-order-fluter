
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table.nasys.vn/v2/order/cashier/history

## 5. Điều phối ca
---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

5.3 Thẻ tổng hợp (Bán hàng / Trả hàng / Phiếu thu / Phiếu chi)

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 5.3.1 | ☐ | Thẻ Bán hàng hiển thị đúng | 1. Mở chi tiết một ca bất kỳ 2. Tìm thẻ "Bán hàng" trong phần tổng hợp 3. Quan sát số đơn hàng và tổng tiền mặt bán hàng | Hiển thị đúng số đơn hàng và tổng tiền mặt bán hàng |
| 5.3.2 | ☐ | Thẻ Trả hàng hiển thị đúng | 1. Mở chi tiết một ca có phát sinh trả hàng 2. Tìm thẻ "Trả hàng" trong phần tổng hợp 3. Kiểm tra số tiền hiển thị | Hiển thị đúng tổng tiền trả hàng trong ca |
| 5.3.3 | ☐ | Thẻ Phiếu thu hiển thị đúng | 1. Mở chi tiết một ca có phát sinh phiếu thu 2. Tìm thẻ "Phiếu thu" trong phần tổng hợp 3. Kiểm tra số tiền hiển thị | Hiển thị đúng tổng tiền thu trong ca |
| 5.3.4 | ☐ | Thẻ Phiếu chi hiển thị đúng | 1. Mở chi tiết một ca có phát sinh phiếu chi 2. Tìm thẻ "Phiếu chi" trong phần tổng hợp 3. Kiểm tra số tiền hiển thị | Hiển thị đúng tổng tiền chi trong ca |
| 5.3.5 | ☐ | Bấm "..." trên thẻ để xem chi tiết phương thức | 1. Mở chi tiết một ca 2. Trên bất kỳ thẻ tổng hợp nào (VD: Bán hàng), bấm nút "..." 3. Quan sát thông tin hiện ra | Hiện chi tiết phân theo từng phương thức: tiền mặt / chuyển khoản / quẹt thẻ / QR / khác |
| 5.3.6 | ☐ | Tổng các phương thức khớp với tổng thẻ | 1. Mở chi tiết thẻ bằng cách bấm "..." 2. Cộng tay các giá trị từng phương thức (tiền mặt + CK + thẻ + QR + khác) 3. So sánh với số tổng hiển thị trên thẻ | Tổng các phương thức = tổng hiển thị trên thẻ |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
