
## Lịch sử

Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table.nasys.vn/v2/order/cashier/history

---

### Bộ lọc loại đơn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Lọc tab "Tất cả" | 1. Đăng nhập, truy cập link cashier history 2. Quan sát các tab lọc loại đơn phía trên danh sách 3. Bấm tab "Tất cả" 4. Quan sát danh sách đơn | Hiển thị tất cả đơn không phân biệt loại |
| ☐ | Lọc tab "Tại bàn" | 1. Vào trang lịch sử 2. Bấm tab "Tại bàn" 3. Quan sát từng đơn trong danh sách | Chỉ hiện các đơn loại tại bàn |
| ☐ | Lọc tab "Mang về" | 1. Vào trang lịch sử 2. Bấm tab "Mang về" 3. Quan sát danh sách | Chỉ hiện các đơn mang về |
| ☐ | Lọc tab "Đặt online" | 1. Vào trang lịch sử 2. Bấm tab "Đặt online" 3. Quan sát danh sách | Chỉ hiện đơn đặt online; nếu không có đơn nào thì danh sách rỗng |
| ☐ | Dropdown "Chọn bàn" | 1. Vào trang lịch sử 2. Tìm dropdown "Chọn bàn" trên thanh bộ lọc 3. Bấm dropdown, chọn một bàn cụ thể (VD: Bàn 1) 4. Quan sát danh sách đơn | Chỉ hiện các đơn thuộc bàn đã chọn |

---

### Tìm kiếm & bộ lọc

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Tìm theo mã đơn | 1. Vào trang lịch sử 2. Tìm ô tìm kiếm trên thanh bộ lọc 3. Nhập đúng mã đơn có sẵn (VD: DH-00123) 4. Quan sát kết quả | Trả về đúng đơn có mã tương ứng |
| ☐ | Tìm theo số điện thoại | 1. Vào trang lịch sử 2. Nhập số điện thoại khách hàng vào ô tìm kiếm 3. Quan sát kết quả | Trả về các đơn của khách hàng có số điện thoại đó |
| ☐ | Tìm không khớp | 1. Vào trang lịch sử 2. Nhập chuỗi bất kỳ không tồn tại (VD: "xxxx9999") vào ô tìm kiếm 3. Quan sát danh sách | Danh sách rỗng, không hiện đơn nào |
| ☐ | Trạng thái: Đã thanh toán thành công | 1. Vào trang lịch sử 2. Tìm dropdown lọc trạng thái 3. Chọn "Đã thanh toán thành công" 4. Quan sát danh sách | Chỉ hiện các đơn đã thanh toán thành công |
| ☐ | Trạng thái: Chưa thanh toán | 1. Vào trang lịch sử 2. Bấm dropdown trạng thái 3. Chọn "Chưa thanh toán" 4. Quan sát danh sách | Chỉ hiện các đơn chưa thanh toán |
| ☐ | Trạng thái: Đã hủy | 1. Vào trang lịch sử 2. Bấm dropdown trạng thái 3. Chọn "Đã hủy" 4. Quan sát danh sách | Chỉ hiện các đơn đã bị hủy |
| ☐ | Trạng thái: Đã xử lý trả hàng | 1. Vào trang lịch sử 2. Bấm dropdown trạng thái 3. Chọn "Đã xử lý trả hàng" 4. Quan sát danh sách | Chỉ hiện các đơn đã xử lý trả hàng |
| ☐ | Trạng thái: Công nợ | 1. Vào trang lịch sử 2. Bấm dropdown trạng thái 3. Chọn "Công nợ" 4. Quan sát danh sách | Chỉ hiện các đơn đang ở trạng thái công nợ |
| ☐ | Lọc theo Tài khoản (nhân viên) | 1. Vào trang lịch sử 2. Tìm dropdown "Tài khoản" hoặc "Nhân viên" 3. Chọn một nhân viên cụ thể 4. Quan sát danh sách | Chỉ hiện các đơn do nhân viên đó tạo |
| ☐ | Khoảng ngày: Hôm nay | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian 3. Chọn "Hôm nay" 4. Quan sát danh sách | Chỉ hiện đơn được tạo trong ngày hôm nay |
| ☐ | Khoảng ngày: Hôm qua | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian 3. Chọn "Hôm qua" 4. Quan sát danh sách | Chỉ hiện đơn được tạo ngày hôm qua |
| ☐ | Khoảng ngày: Tuần này | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian 3. Chọn "Tuần này" 4. Quan sát danh sách | Chỉ hiện đơn trong tuần hiện tại |
| ☐ | Khoảng ngày: Tháng này | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian 3. Chọn "Tháng này" 4. Quan sát danh sách | Chỉ hiện đơn trong tháng hiện tại |
| ☐ | Khoảng ngày: Tùy chọn | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian, chọn "Tùy chọn" 3. Nhập ngày bắt đầu và ngày kết thúc cụ thể 4. Xác nhận và quan sát danh sách | Chỉ hiện đơn trong khoảng ngày đã nhập |
| ☐ | Kết hợp nhiều bộ lọc | 1. Vào trang lịch sử 2. Bật đồng thời: tab "Tại bàn" + Trạng thái "Đã thanh toán" + Thời gian "Hôm nay" 3. Quan sát danh sách kết quả | Chỉ hiện đơn thỏa tất cả điều kiện đã chọn |
| ☐ | Ngày bắt đầu > ngày kết thúc | 1. Vào trang lịch sử, bật lọc thời gian tùy chọn 2. Nhập ngày bắt đầu lớn hơn ngày kết thúc (VD: từ 10/06 đến 01/06) 3. Xác nhận và quan sát phản hồi | Hệ thống chặn hoặc hiển thị thông báo lỗi, không trả kết quả sai |

---

### Danh sách đơn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Thẻ đơn hiển thị đủ thông tin | 1. Vào trang lịch sử 2. Quan sát một thẻ đơn bất kỳ trong danh sách 3. Kiểm tra từng thông tin: tên bàn, tài khoản nhân viên, ngày giờ, mã đơn, số tiền | Thẻ hiển thị đúng tên bàn, tài khoản, ngày giờ, mã đơn, số tiền |
| ☐ | Trạng thái thanh toán hiển thị đúng | 1. Vào trang lịch sử 2. Tìm một đơn đã thanh toán và một đơn chưa thanh toán 3. Quan sát nhãn trạng thái trên mỗi thẻ đơn | Đơn đã thanh toán hiển thị "Đã thanh toán"; đơn chưa thanh toán hiển thị "Chưa thanh toán" |
| ☐ | Trạng thái HĐĐT hiển thị đúng | 1. Vào trang lịch sử 2. Tìm đơn có cột/nhãn trạng thái hóa đơn điện tử (HĐĐT) 3. Quan sát giá trị hiển thị | Hiển thị đúng trạng thái: "Không xác định" hoặc "Chờ ký" tùy theo đơn |
| ☐ | Màu thẻ theo trạng thái | 1. Vào trang lịch sử 2. Quan sát màu nền hoặc màu viền các thẻ đơn 3. So sánh màu giữa đơn chưa thanh toán và đơn đã thanh toán | Đơn chưa thanh toán màu xám; đơn đã thanh toán màu xanh |
| ☐ | Số tiền trên thẻ khớp chi tiết đơn | 1. Quan sát số tiền hiển thị trên thẻ đơn, ghi nhận lại 2. Bấm vào thẻ đơn đó để mở chi tiết 3. So sánh số tiền trong modal chi tiết với số tiền trên thẻ | Số tiền trên thẻ = tổng tiền thanh toán trong chi tiết đơn |

---

### Chi tiết đơn hàng

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Bấm vào đơn mở modal chi tiết | 1. Vào trang lịch sử 2. Bấm vào bất kỳ thẻ đơn nào trong danh sách 3. Quan sát màn hình | Modal "Chi tiết đơn hàng" mở ra, tiêu đề hiển thị đúng mã đơn |
| ☐ | Thông tin đơn hiển thị đúng | 1. Mở modal chi tiết một đơn bất kỳ 2. Kiểm tra lần lượt: tên bàn, tên khách hàng, tên nhân viên, ngày giờ tạo đơn | Tất cả thông tin khớp với dữ liệu thực tế của đơn |
| ☐ | Danh sách món hiển thị đúng | 1. Mở modal chi tiết đơn 2. Quan sát bảng danh sách món bên trong modal 3. Kiểm tra từng dòng: tên món, số lượng, đơn giá, thành tiền | Tên, SL, đơn giá, thành tiền của từng dòng món hiển thị đúng |
| ☐ | Tổng tiền hàng tính đúng | 1. Mở modal chi tiết đơn 2. Cộng tay thành tiền của tất cả dòng món (Σ thành tiền) 3. So sánh với dòng "Tổng tiền hàng" trong modal | Tổng tiền hàng = Σ thành tiền các món |
| ☐ | Phụ thu / Giảm giá / Tiền điểm / VAT tính đúng | 1. Mở modal chi tiết đơn có áp phụ thu, giảm giá hoặc điểm thưởng 2. Quan sát từng dòng: Phụ thu, Giảm giá, Tiền điểm, VAT 3. Kiểm tra từng giá trị có đúng với lúc tạo đơn không | Mỗi dòng phụ thu / giảm giá / điểm / VAT hiển thị đúng giá trị đã áp |
| ☐ | Tổng tiền thanh toán tính đúng công thức | 1. Mở modal chi tiết đơn 2. Ghi nhận: Tổng tiền hàng, Phụ thu, Giảm giá, Tiền điểm, VAT 3. Tính tay: Tổng hàng + Phụ thu − Giảm giá − Tiền điểm + VAT 4. So sánh với "Tổng tiền thanh toán" hiển thị | Tổng tiền thanh toán = Tổng hàng + Phụ thu − Giảm giá − Tiền điểm + VAT |
| ☐ | Phương thức thanh toán hiển thị đúng | 1. Mở modal chi tiết đơn đã thanh toán 2. Tìm mục "Phương thức thanh toán" trong modal 3. So sánh với phương thức đã chọn lúc thanh toán (Tiền mặt / CK / Thẻ / QR) | Phương thức hiển thị đúng với lúc thanh toán thực tế |
| ☐ | Bấm "Đóng" thoát modal | 1. Mở modal chi tiết đơn 2. Bấm nút "Đóng" 3. Quan sát màn hình và bộ lọc đang áp | Modal đóng lại, quay về danh sách; bộ lọc và trang hiện tại giữ nguyên |

---

### Xuất Excel

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Bấm "Xuất Excel" | 1. Vào trang lịch sử 2. Áp một bộ lọc bất kỳ (VD: Trạng thái "Đã thanh toán", Hôm nay) 3. Tìm và bấm nút "Xuất Excel" 4. Quan sát phản hồi trình duyệt | Trình duyệt kích hoạt tải file, file Excel được tải xuống thành công |
| ☐ | File xuất đúng dữ liệu theo bộ lọc | 1. Áp bộ lọc cụ thể, ghi nhận số đơn và thông tin hiển thị trên màn hình 2. Bấm "Xuất Excel", mở file vừa tải 3. So sánh nội dung file với dữ liệu trên màn hình | File Excel chứa đúng các đơn khớp với bộ lọc đang áp dụng |
