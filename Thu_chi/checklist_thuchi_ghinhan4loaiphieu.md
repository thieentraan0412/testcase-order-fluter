
## 2. Thu chi

Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense

---

2.5 Ghi nhận 4 loại phiếu (logic chính)

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
2.5.1 | ☐ | Tạo Phiếu thu thủ công | 1. Vào trang Thu chi, ghi nhận "Tổng thu" và "Tồn quỹ cuối kỳ" hiện tại 2. Bấm "Thêm", chọn Loại = "Thu", nhập số tiền (VD: 100,000đ), bấm "Lưu" 3. Quan sát danh sách và thẻ tổng quan | Phiếu mới có Loại = Thu xuất hiện; Tổng thu và Tồn quỹ cuối kỳ tăng đúng 100,000đ |
2.5.2 | ☐ | Tạo Phiếu chi thủ công | 1. Vào trang Thu chi, ghi nhận "Tổng chi" và "Tồn quỹ cuối kỳ" hiện tại 2. Bấm "Thêm", chọn Loại = "Chi", nhập số tiền (VD: 50,000đ), bấm "Lưu" 3. Quan sát danh sách và thẻ tổng quan | Phiếu mới có Loại = Chi xuất hiện; Tổng chi tăng và Tồn quỹ cuối kỳ giảm đúng 50,000đ |
2.5.3 | ☐ | Phiếu thu hiển thị đúng thông tin | 1. Trong danh sách phiếu, tìm một phiếu thu thủ công vừa tạo 2. Kiểm tra từng cột: Loại = Thu, Số tiền đúng, tên Người nộp, PTTT đã chọn | Tất cả cột hiển thị đúng với dữ liệu đã nhập lúc tạo |
2.5.4 | ☐ | Phiếu chi hiển thị đúng thông tin | 1. Trong danh sách phiếu, tìm một phiếu chi thủ công vừa tạo 2. Kiểm tra từng cột: Loại = Chi, Số tiền đúng, tên Người nhận, PTTT đã chọn | Tất cả cột hiển thị đúng với dữ liệu đã nhập lúc tạo |
2.5.5 | ☐ | Hoàn tất đơn bán → tự sinh Phiếu bán hàng | 1. Vào cashier, chọn bàn, thêm món, thực hiện thanh toán thành công 2. Quay lại trang Thu chi, lọc "Loại nguồn = Bán hàng" 3. Tìm phiếu vừa sinh ra tương ứng với đơn bán 4. Kiểm tra thông tin phiếu | Phiếu Loại = Thu, Loại nguồn = Bán hàng, số tiền = tổng đơn bán vừa thanh toán |
2.5.6 | ☐ | Thực hiện trả hàng → tự sinh Phiếu trả hàng | 1. Thực hiện một phiếu trả hàng (hoàn tiền) từ màn hình cashier hoặc quản lý đơn 2. Quay lại trang Thu chi, lọc "Loại nguồn = Trả hàng" 3. Tìm phiếu vừa sinh ra 4. Kiểm tra thông tin phiếu | Phiếu Loại = Chi (hoàn tiền), Loại nguồn = Trả hàng, số tiền = giá trị hàng trả |
2.5.7 | ☐ | Lọc Loại nguồn = Bán hàng | 1. Vào trang Thu chi 2. Bật bộ lọc "Loại nguồn", chọn "Bán hàng" 3. Quan sát toàn bộ danh sách | Chỉ hiện các phiếu được sinh tự động từ đơn bán hàng |
2.5.8 | ☐ | Lọc Loại nguồn = Trả hàng | 1. Vào trang Thu chi 2. Bật bộ lọc "Loại nguồn", chọn "Trả hàng" 3. Quan sát toàn bộ danh sách | Chỉ hiện các phiếu được sinh tự động từ phiếu trả hàng |
2.5.9 | ☐ | Lọc Loại nguồn = Tự tạo | 1. Vào trang Thu chi 2. Bật bộ lọc "Loại nguồn", chọn "Tự tạo" 3. Quan sát toàn bộ danh sách | Chỉ hiện các phiếu thu/chi được tạo thủ công bởi nhân viên |
2.5.10 | ☐ | Số tiền phiếu bán hàng khớp đơn gốc | 1. Ghi lại tổng tiền thanh toán của một đơn bán vừa hoàn tất (VD: 250,000đ) 2. Vào trang Thu chi, lọc Loại nguồn = Bán hàng 3. Tìm phiếu tương ứng với đơn đó 4. So sánh số tiền phiếu với tổng đơn | Số tiền phiếu bán hàng = tổng tiền thanh toán đơn gốc |
2.5.11 | ☐ | Số tiền phiếu trả hàng khớp đơn gốc | 1. Ghi lại giá trị hàng trả của một phiếu trả hàng vừa thực hiện 2. Vào trang Thu chi, lọc Loại nguồn = Trả hàng 3. Tìm phiếu tương ứng 4. So sánh số tiền | Số tiền phiếu trả hàng = giá trị hàng trả của đơn gốc |
2.5.12 | ☐ | PTTT của phiếu tự sinh khớp đơn gốc | 1. Hoàn tất một đơn bán bằng phương thức "Chuyển khoản" 2. Vào trang Thu chi, tìm phiếu sinh ra từ đơn đó 3. Kiểm tra cột "PTTT" của phiếu | PTTT của phiếu = phương thức thanh toán của đơn bán/trả gốc (VD: Chuyển khoản) |
2.5.13 | ☐ | Đơn bán bị hủy → phiếu không tính vào quỹ | 1. Ghi nhận Tổng thu hiện tại 2. Tạo một đơn bán rồi hủy đơn đó (không thanh toán) 3. Vào trang Thu chi, kiểm tra Tổng thu và Tồn quỹ | Tổng thu và Tồn quỹ không thay đổi; không có phiếu mới sinh ra từ đơn bị hủy |
2.5.14 | ☐ | Số liệu Thu chi khớp với Điều phối ca | 1. Mở tab Điều phối ca, ghi lại số tiền và PTTT của một giao dịch bất kỳ trong ca 2. Vào trang Thu chi, tìm phiếu tương ứng 3. So sánh số tiền và PTTT giữa hai màn hình | Số tiền và phương thức thanh toán khớp nhau, không bị lệch |
2.5.15 | ☐ | Tổng thu = Σ tất cả nguồn thu | 1. Vào trang Thu chi, bật lọc Loại = "Thu" 2. Cộng tay tất cả số tiền phiếu thu trong danh sách (bao gồm thu thủ công + bán hàng) 3. So sánh kết quả với thẻ "Tổng thu" | Tổng thu trên thẻ = Σ số tiền tất cả phiếu thu (thủ công + bán hàng) |
2.5.16 | ☐ | Tổng chi = Σ tất cả nguồn chi | 1. Vào trang Thu chi, bật lọc Loại = "Chi" 2. Cộng tay tất cả số tiền phiếu chi trong danh sách (bao gồm chi thủ công + trả hàng) 3. So sánh kết quả với thẻ "Tổng chi" | Tổng chi trên thẻ = Σ số tiền tất cả phiếu chi (thủ công + trả hàng) |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
