
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table.nasys.vn/v2/order/cashier/history

## 5. Điều phối ca
---

5.5 Đối soát ca (logic tính)

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
5.5.1 | ☐ | Tổng tiền mặt trong ca tính đúng công thức | 1. Mở chi tiết một ca đã có đủ các loại giao dịch 2. Ghi lại: tiền mặt bán hàng, tiền mặt phiếu thu, tiền mặt trả hàng, tiền mặt phiếu chi 3. Tính tay: (tiền mặt bán hàng + phiếu thu) − (trả hàng + phiếu chi) 4. So sánh với "Tổng tiền mặt trong ca" hiển thị | Tổng tiền mặt trong ca = tiền mặt bán hàng + phiếu thu − trả hàng − phiếu chi |
5.5.2 | ☐ | Tiền mặt đầu ca KHÔNG cộng vào tổng | 1. Mở chi tiết một ca 2. Ghi nhận số "Tiền mặt đầu ca" 3. Tính tổng tiền mặt trong ca theo công thức (không cộng đầu ca) 4. So sánh với con số "Tổng tiền mặt trong ca" hiển thị | Tiền mặt đầu ca không được cộng vào "Tổng tiền mặt trong ca" |
5.5.3 | ☐ | Chỉ tính giao dịch tiền mặt vào tổng | 1. Mở chi tiết ca có giao dịch bằng nhiều phương thức (tiền mặt + CK + QR) 2. Quan sát "Tổng tiền mặt trong ca" 3. Kiểm tra xem các giao dịch CK / thẻ / QR có được cộng vào không | Chỉ các giao dịch tiền mặt được tính; CK, thẻ, QR không ảnh hưởng tổng tiền mặt trong ca |
5.5.4 | ☐ | Phiếu bán hàng ghi nhận vào ca | 1. Tạo và hoàn tất một đơn bán hàng trong ca đang mở 2. Quay lại trang lịch sử ca, mở chi tiết ca đang mở 3. Kiểm tra danh sách giao dịch | Đơn bán vừa tạo xuất hiện trong danh sách giao dịch ca |
5.5.5 | ☐ | Phiếu trả hàng làm giảm tổng đúng | 1. Tạo phiếu trả hàng tiền mặt trong ca đang mở 2. Ghi lại tổng tiền mặt trong ca trước và sau khi tạo phiếu trả 3. So sánh chênh lệch với số tiền trả | Tổng tiền mặt trong ca giảm đúng bằng số tiền trả hàng |
5.5.6 | ☐ | Phiếu thu cộng vào ca đúng | 1. Tạo phiếu thu tiền mặt trong ca đang mở 2. Ghi lại tổng tiền mặt trong ca trước và sau khi tạo phiếu thu 3. So sánh chênh lệch với số tiền thu | Tổng tiền mặt trong ca tăng đúng bằng số tiền thu |
5.5.7 | ☐ | Phiếu chi trừ khỏi ca đúng | 1. Tạo phiếu chi tiền mặt trong ca đang mở 2. Ghi lại tổng tiền mặt trong ca trước và sau khi tạo phiếu chi 3. So sánh chênh lệch với số tiền chi | Tổng tiền mặt trong ca giảm đúng bằng số tiền chi |
5.5.8 | ☐ | Giao dịch đã hủy không tính vào tổng | 1. Trong danh sách giao dịch ca, lọc trạng thái "Đã hủy" để xác định giao dịch bị hủy 2. Lọc trạng thái "Hoàn thành", tính tay tổng tiền các giao dịch hoàn thành 3. So sánh với "Tổng tiền mặt trong ca" hiển thị | Tổng tiền chỉ tính giao dịch hoàn thành; giao dịch đã hủy không được cộng vào |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
