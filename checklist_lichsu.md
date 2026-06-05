
## Lịch sử

Link login https://table1.klkim.com/login

tài khoản
    Cửa hàng : trong
    Tài khoản: admin   
    Mật khẩu : 147258

Link cashier::https://table.nasys.vn/v2/order/cashier/history

### Bộ lọc loại đơn

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Lọc tab "Tất cả" | Hiện tất cả đơn |
| ☐ | Lọc tab "Tại bàn" | Chỉ hiện đơn tại bàn |
| ☐ | Lọc tab "Mang về" | Chỉ hiện đơn mang về |
| ☐ | Lọc tab "Đặt online" | Chỉ hiện đơn online (rỗng → trạng thái rỗng) |
| ☐ | Dropdown "Chọn bàn" | Lọc đúng đơn theo bàn đã chọn |

### Tìm kiếm & bộ lọc

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Tìm theo mã đơn | Trả đúng đơn |
| ☐ | Tìm theo số điện thoại | Trả đúng đơn |
| ☐ | Tìm không khớp | Danh sách rỗng |
| ☐ | Trạng thái: Đã thanh toán thành công | Chỉ hiện đơn đã TT thành công |
| ☐ | Trạng thái: Chưa thanh toán | Chỉ hiện đơn chưa TT |
| ☐ | Trạng thái: Đã hủy | Chỉ hiện đơn đã hủy |
| ☐ | Trạng thái: Đã xử lý trả hàng | Chỉ hiện đơn trả hàng |
| ☐ | Trạng thái: Công nợ | Chỉ hiện đơn công nợ |
| ☐ | Lọc theo Tài khoản | Chỉ hiện đơn của NV đã chọn |
| ☐ | Khoảng ngày: Hôm nay | Đơn trong hôm nay |
| ☐ | Khoảng ngày: Hôm qua | Đơn hôm qua |
| ☐ | Khoảng ngày: Tuần này | Đơn tuần này |
| ☐ | Khoảng ngày: Tháng này | Đơn tháng này |
| ☐ | Khoảng ngày: Tùy chọn | Đơn trong khoảng chọn |
| ☐ | Kết hợp nhiều bộ lọc | Kết quả giao đúng |
| ☐ | Ngày bắt đầu > kết thúc | Chặn/báo lỗi |

### Danh sách đơn

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Thẻ đơn hiển thị | Đúng tên bàn, tài khoản, ngày giờ, mã đơn, số tiền |
| ☐ | Trạng thái thanh toán | Đúng (Chưa/Đã thanh toán) |
| ☐ | Trạng thái HDDT | Đúng (Không xác định / Chờ ký) |
| ☐ | Màu theo trạng thái | Xám = chưa, xanh = đã thanh toán |
| ☐ | Số tiền trên thẻ | Khớp chi tiết đơn |

### Chi tiết đơn hàng

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Bấm vào đơn | Mở modal "Chi tiết đơn hàng" đúng mã đơn |
| ☐ | Thông tin đơn | Đúng bàn, khách hàng, nhân viên, ngày tạo |
| ☐ | Danh sách món | Đúng tên, SL, đơn giá, thành tiền |
| ☐ | Tổng tiền hàng | = Σ thành tiền các món |
| ☐ | Phụ thu / Giảm giá / Tiền điểm / VAT | Tính đúng |
| ☐ | Tổng tiền thanh toán | = Tổng hàng + Phụ thu − Giảm giá − Tiền điểm + VAT |
| ☐ | Phương thức thanh toán | Hiển thị đúng |
| ☐ | Bấm "Đóng" | Đóng modal, giữ nguyên bộ lọc |

### Xuất Excel

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Bấm "Xuất Excel" | Kích hoạt tải file |
| ☐ | File xuất | Đúng bộ lọc đang áp dụng |
