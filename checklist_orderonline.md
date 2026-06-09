## 3. Đặt online (Order Online)
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/order-online

3.1 Màn hình danh sách đơn đặt online

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 3.1.1 | ☐ | Hiển thị màn hình Đặt online | 1. Đăng nhập thành công 2. Click menu "Đặt online" 3. Quan sát màn hình | Hiển thị màn Đặt online với thanh tìm kiếm, bộ lọc thời gian, bộ lọc trạng thái và vùng danh sách đơn |
| 3.1.2 | ☐ | Hiển thị danh sách đơn online | 1. Vào màn Đặt online 2. Quan sát vùng danh sách đơn | Hiển thị đầy đủ các đơn online đúng theo khoảng thời gian và trạng thái đang chọn |
| 3.1.3 | ☐ | Hiển thị khi không có đơn | 1. Chọn khoảng thời gian không phát sinh đơn 2. Quan sát danh sách | Danh sách trống, các tab trạng thái hiển thị số lượng (0) |
| 3.1.4 | ☐ | Tìm kiếm đơn theo mã đơn | 1. Nhập mã đơn vào ô "Tìm theo đơn, số điện thoại, tên khách" 2. Thực hiện tìm kiếm | Hiển thị đúng đơn khớp với mã đơn đã nhập |
| 3.1.5 | ☐ | Tìm kiếm đơn theo số điện thoại | 1. Nhập số điện thoại khách vào ô tìm kiếm 2. Thực hiện tìm kiếm | Hiển thị các đơn có số điện thoại khớp |
| 3.1.6 | ☐ | Tìm kiếm đơn theo tên khách | 1. Nhập tên khách vào ô tìm kiếm 2. Thực hiện tìm kiếm | Hiển thị các đơn có tên khách khớp |
| 3.1.7 | ☐ | Tìm kiếm không có kết quả | 1. Nhập từ khóa không tồn tại 2. Thực hiện tìm kiếm | Danh sách trống, không báo lỗi |
| 3.1.8 | ☐ | Lọc đơn theo "Hôm nay" | 1. Click nút "Hôm nay" 2. Quan sát danh sách | Hiển thị đơn phát sinh trong ngày hiện tại, ô ngày tự cập nhật về hôm nay |
| 3.1.9 | ☐ | Lọc đơn theo "Tuần này" | 1. Click nút "Tuần này" 2. Quan sát danh sách | Hiển thị đơn trong tuần hiện tại |
| 3.1.10 | ☐ | Lọc đơn theo "Tuần trước" | 1. Click nút "Tuần trước" 2. Quan sát danh sách | Hiển thị đơn trong tuần trước |
| 3.1.11 | ☐ | Lọc đơn theo "Tháng này" | 1. Click nút "Tháng này" 2. Quan sát danh sách | Hiển thị đơn trong tháng hiện tại |
| 3.1.12 | ☐ | Lọc đơn theo "Tháng trước" | 1. Click nút "Tháng trước" 2. Quan sát danh sách | Hiển thị đơn trong tháng trước |
| 3.1.13 | ☐ | Lọc đơn theo "Năm nay" | 1. Click nút "Năm nay" 2. Quan sát danh sách | Hiển thị đơn trong năm hiện tại |
| 3.1.14 | ☐ | Lọc đơn theo "Năm trước" | 1. Click nút "Năm trước" 2. Quan sát danh sách | Hiển thị đơn trong năm trước |
| 3.1.15 | ☐ | Lọc đơn theo khoảng ngày tùy chọn | 1. Chọn ngày bắt đầu và ngày kết thúc 2. Quan sát danh sách | Hiển thị đơn nằm trong khoảng ngày đã chọn |
| 3.1.16 | ☐ | Lọc theo trạng thái "Tất cả" | 1. Click tab "Tất cả" 2. Quan sát danh sách | Hiển thị toàn bộ đơn ở mọi trạng thái, số lượng đúng |
| 3.1.17 | ☐ | Lọc theo trạng thái "Chờ xác nhận" | 1. Click tab "Chờ xác nhận" 2. Quan sát danh sách | Chỉ hiển thị đơn ở trạng thái chờ xác nhận, số lượng đúng |
| 3.1.18 | ☐ | Lọc theo trạng thái "Đang tiến hành" | 1. Click tab "Đang tiến hành" 2. Quan sát danh sách | Chỉ hiển thị đơn đang tiến hành, số lượng đúng |
| 3.1.19 | ☐ | Lọc theo trạng thái "Đã xác nhận" | 1. Click tab "Đã xác nhận" 2. Quan sát danh sách | Chỉ hiển thị đơn đã xác nhận, số lượng đúng |
| 3.1.20 | ☐ | Lọc theo trạng thái "Chờ giao hàng" | 1. Click tab "Chờ giao hàng" 2. Quan sát danh sách | Chỉ hiển thị đơn chờ giao hàng, số lượng đúng |
| 3.1.21 | ☐ | Lọc theo trạng thái "Đã giao" | 1. Click tab "Đã giao" 2. Quan sát danh sách | Chỉ hiển thị đơn đã giao, số lượng đúng |
| 3.1.22 | ☐ | Lọc theo trạng thái "Đã hủy" | 1. Click tab "Đã hủy" 2. Quan sát danh sách | Chỉ hiển thị đơn đã hủy, số lượng đúng |
| 3.1.23 | ☐ | Kết hợp lọc thời gian và trạng thái | 1. Chọn 1 khoảng thời gian 2. Chọn 1 tab trạng thái 3. Quan sát danh sách | Danh sách hiển thị đúng đơn thỏa cả 2 điều kiện lọc |
| 3.1.24 | ☐ | Xem chi tiết đơn online | 1. Click vào 1 đơn trong danh sách 2. Quan sát | Mở chi tiết đơn: thông tin khách, danh sách món, tổng tiền, trạng thái |
| 3.1.25 | ☐ | Mở chức năng "Đặt bàn" / Tra cứu đặt bàn | 1. Click nút "Đặt bàn" 2. Quan sát | Hiển thị form tra cứu với Họ và tên, Số điện thoại, chọn Năm/Tuần và nút "Tra cứu đặt bàn" |
| 3.1.26 | ☐ | Tra cứu đặt bàn theo thông tin khách | 1. Mở form tra cứu 2. Nhập họ tên / số điện thoại, chọn tuần 3. Click "Tra cứu đặt bàn" | Hiển thị kết quả đặt bàn khớp với thông tin tra cứu |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
