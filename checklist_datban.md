# Checklist Kiểm thử – Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

## 1. Màn hình chính – Lịch đặt bàn theo tuần

### 1.1 Điều hướng tuần & ngày

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Hiển thị 7 tab ngày trong tuần | 1. Đăng nhập vào hệ thống 2. Mở menu "Bàn đặt" → vào trang Đặt bàn 3. Quan sát dải tab ngày ở đầu trang | Hiển thị 7 tab ngày trong tuần hiện tại (Thứ Hai → Chủ Nhật), tab "Hôm nay" được highlight |
| ☐ | Bấm tab từng ngày chuyển lịch | 1. Vào trang Đặt bàn 2. Lần lượt bấm từng tab ngày (Thứ Hai, Thứ Ba, ...) 3. Quan sát vùng lịch sau mỗi lần bấm | Vùng lịch chuyển sang hiển thị các đặt bàn của ngày tương ứng |
| ☐ | Nút "Tuần trước" | 1. Vào trang Đặt bàn 2. Bấm nút "Tuần trước" 3. Quan sát dải tab ngày và dropdown Tuần | Dải tab cập nhật sang tuần trước; dropdown Tuần khớp khoảng ngày mới |
| ☐ | Nút "Tuần sau" | 1. Vào trang Đặt bàn 2. Bấm nút "Tuần sau" 3. Quan sát dải tab ngày | Dải tab cập nhật sang tuần tiếp theo |
| ☐ | Dropdown "Năm" chuyển đúng năm | 1. Vào trang Đặt bàn 2. Tìm và bấm dropdown "Năm" 3. Chọn một năm khác (VD: 2027) 4. Quan sát dropdown Tuần và dải tab | Dropdown Tuần và dải tab cập nhật theo năm đã chọn |
| ☐ | Dropdown "Tuần" nhảy đến tuần chọn | 1. Vào trang Đặt bàn 2. Bấm dropdown "Tuần" 3. Chọn một khoảng tuần cụ thể (VD: 08/06/2026 – 14/06/2026) 4. Quan sát dải tab ngày | Dải tab ngày nhảy đến đúng tuần đã chọn |

---

### 1.2 Bộ lọc lịch

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Lọc theo khoảng giờ | 1. Vào trang Đặt bàn 2. Nhập giờ vào ô "Từ" (Thời gian) 3. Nhập giờ vào ô "Đến" 4. Quan sát lịch | Lịch chỉ hiện các đặt bàn trong khoảng giờ đã nhập |
| ☐ | Lọc theo Bàn | 1. Vào trang Đặt bàn 2. Bấm dropdown "Chọn bàn" 3. Gõ tên bàn vào ô Search 4. Chọn một bàn cụ thể 5. Quan sát lịch | Lịch chỉ hiện slot của bàn đã chọn |
| ☐ | Lọc trạng thái "Chờ xác nhận" | 1. Vào trang Đặt bàn 2. Bấm dropdown "Trạng thái" 3. Chọn "Chờ xác nhận" 4. Quan sát lịch | Chỉ hiện các đặt bàn đang ở trạng thái "Chờ xác nhận" |
| ☐ | Lọc trạng thái "Đã hủy" | 1. Vào trang Đặt bàn 2. Bấm dropdown "Trạng thái" 3. Chọn "Đã hủy" 4. Quan sát lịch | Chỉ hiện các đặt bàn đã hủy |
| ☐ | Lọc theo Tên khách | 1. Vào trang Đặt bàn 2. Nhập họ và tên khách vào ô tìm kiếm tên 3. Quan sát lịch | Chỉ hiện đặt bàn của khách khớp tên |
| ☐ | Lọc theo Số điện thoại | 1. Vào trang Đặt bàn 2. Nhập số điện thoại khách vào ô tìm kiếm SĐT 3. Quan sát lịch | Chỉ hiện đặt bàn của khách khớp số điện thoại |
| ☐ | Kết hợp nhiều bộ lọc | 1. Vào trang Đặt bàn 2. Bật đồng thời: chọn Bàn + Trạng thái + nhập Tên khách 3. Quan sát lịch | Kết quả hiển thị đúng giao của tất cả điều kiện đã lọc |

---

### 1.3 Bấm "Tra cứu đặt bàn"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Nút "Tra cứu đặt bàn" chuyển trang | 1. Vào trang Đặt bàn 2. Tìm và bấm nút "Tra cứu đặt bàn" (màu vàng, góc dưới panel) 3. Quan sát màn hình mở ra | Chuyển sang trang "Tra cứu lịch đặt bàn" |

---

## 2. Tạo đặt bàn (modal "Đặt bàn")

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Mở modal "Đặt bàn" | 1. Vào trang Đặt bàn 2. Bấm nút "+ Đặt bàn" (xanh đậm, góc trên phải) 3. Quan sát màn hình | Mở modal "Đặt bàn" với 2 phần: Thông tin khách hàng & Thông tin đặt bàn |
| ☐ | Bỏ trống cả Khách hàng và Bàn | 1. Mở modal "Đặt bàn" 2. Không điền Khách hàng và không chọn Bàn 3. Bấm nút "Đặt bàn" 4. Quan sát phản hồi | Hệ thống chặn, hiển thị thông báo lỗi: "Trường Khách hàng là bắt buộc. Trường Bàn là bắt buộc." |
| ☐ | Bỏ trống chỉ Khách hàng | 1. Mở modal "Đặt bàn" 2. Chọn Bàn nhưng để trống Khách hàng 3. Bấm "Đặt bàn" 4. Quan sát phản hồi | Hệ thống chặn, báo lỗi Khách hàng là bắt buộc |
| ☐ | Bỏ trống chỉ Bàn | 1. Mở modal "Đặt bàn" 2. Chọn Khách hàng nhưng không chọn Bàn 3. Bấm "Đặt bàn" 4. Quan sát phản hồi | Hệ thống chặn, báo lỗi Bàn là bắt buộc |

---

### 2.1 Thông tin khách hàng

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Tìm và chọn khách hàng có sẵn | 1. Mở modal "Đặt bàn" 2. Bấm dropdown "Khách hàng" 3. Gõ tên hoặc SĐT khách để tìm 4. Chọn một khách từ danh sách 5. Quan sát thông tin hiện ra | Khách hàng được chọn, hiển thị tên và điểm tích lũy / hạng thành viên |
| ☐ | Bấm "+ Thêm mới" mở modal khách | 1. Mở modal "Đặt bàn" 2. Tại phần Khách hàng, bấm nút "+ Thêm mới" (xanh dương) 3. Quan sát màn hình | Mở modal "Thêm / Chỉnh sửa" khách hàng mới |
| ☐ | Chọn Nhân viên đặt bàn | 1. Mở modal "Đặt bàn" 2. Tìm dropdown "Nhân viên đặt bàn" 3. Bấm dropdown phần loại, chọn loại (VD: Thu ngân) 4. Chọn tên nhân viên từ danh sách 5. Quan sát giá trị được ghi nhận | Ghi nhận đúng loại và tên nhân viên đặt bàn |

---

### 2.2 Thêm khách hàng mới (modal phụ "Thêm / Chỉnh sửa")

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Modal phụ hiển thị đủ trường | 1. Trong modal Đặt bàn, bấm "+ Thêm mới" 2. Quan sát toàn bộ các trường trong modal Thêm/Chỉnh sửa | Hiển thị đủ: Hình ảnh (upload), Mã KH (tự động), Tên KH*, Căn cước CD, Nhóm KH*, Giới tính, Điện thoại*, Ngày sinh, Email, Địa chỉ, Ghi chú, Loại (Cá nhân/Doanh nghiệp) |
| ☐ | Bỏ trống Tên khách hàng (bắt buộc) | 1. Mở modal Thêm/Chỉnh sửa 2. Điền đầy đủ các trường khác, để trống ô "Tên khách hàng" 3. Bấm "Lưu" 4. Quan sát phản hồi | Hệ thống chặn lưu, báo lỗi Tên là bắt buộc |
| ☐ | Bỏ trống Nhóm khách hàng (bắt buộc) | 1. Mở modal Thêm/Chỉnh sửa 2. Điền Tên và Điện thoại, để trống "Nhóm khách hàng" 3. Bấm "Lưu" 4. Quan sát phản hồi | Hệ thống chặn lưu, báo lỗi Nhóm là bắt buộc |
| ☐ | Bỏ trống Điện thoại (bắt buộc) | 1. Mở modal Thêm/Chỉnh sửa 2. Điền Tên và Nhóm, để trống "Điện thoại" 3. Bấm "Lưu" 4. Quan sát phản hồi | Hệ thống chặn lưu, báo lỗi Điện thoại là bắt buộc |
| ☐ | Upload ảnh đại diện | 1. Mở modal Thêm/Chỉnh sửa 2. Bấm nút "Tải lên" ảnh đại diện 3. Chọn một ảnh từ máy tính 4. Quan sát sau khi chọn | Ảnh được upload và hiển thị preview trong form |
| ☐ | Chọn loại Cá nhân / Doanh nghiệp | 1. Mở modal Thêm/Chỉnh sửa 2. Tìm phần "Loại" 3. Chọn lần lượt "Cá nhân" và "Doanh nghiệp" 4. Quan sát giá trị ghi nhận | Ghi nhận đúng loại khách hàng đã chọn |
| ☐ | Lưu khách hàng mới thành công | 1. Mở modal Thêm/Chỉnh sửa 2. Điền đầy đủ tất cả trường bắt buộc (Tên, Nhóm, Điện thoại) 3. Bấm "Lưu" 4. Quan sát modal Đặt bàn phía sau | Tạo khách hàng mới thành công; tên khách tự động điền vào trường Khách hàng của modal Đặt bàn |
| ☐ | Bấm "Đóng" modal phụ | 1. Mở modal Thêm/Chỉnh sửa 2. Nhập một vài thông tin 3. Bấm nút "Đóng" 4. Quan sát kết quả | Modal phụ đóng lại, quay về modal Đặt bàn; không tạo khách hàng mới |

---

### 2.3 Thông tin đặt bàn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Nhập số lượng người lớn / trẻ em | 1. Mở modal "Đặt bàn" 2. Tìm ô "Số lượng người lớn", nhập một số nguyên dương (VD: 3) 3. Tìm ô "Số lượng trẻ em", nhập một số (VD: 1) 4. Quan sát giá trị ghi nhận | Ghi nhận đúng; chỉ nhận số nguyên dương |
| ☐ | Trường Thời gian mặc định và chỉnh sửa được | 1. Mở modal "Đặt bàn" 2. Quan sát giá trị mặc định trong ô Thời gian 3. Thử bấm vào ô và sửa ngày giờ sang giá trị khác | Hiển thị ngày giờ hiện tại làm mặc định; có thể chỉnh sửa sang ngày giờ khác |
| ☐ | Chọn Khu vực bàn → danh sách bàn cập nhật | 1. Mở modal "Đặt bàn" 2. Bấm dropdown "Chọn Khu vực bàn" 3. Chọn "Khu 1" → quan sát danh sách bàn 4. Đổi sang "Khu 2" → quan sát lại | Danh sách bàn chỉ hiện bàn thuộc khu đã chọn |
| ☐ | Chọn Bàn | 1. Mở modal "Đặt bàn", đã chọn Khu vực 2. Bấm dropdown chọn Bàn 3. Gõ tên bàn vào ô Search nếu cần 4. Chọn một bàn cụ thể | Bàn được ghi nhận đúng vào form |
| ☐ | Chọn món trước khi đặt bàn | 1. Mở modal "Đặt bàn" 2. Bấm nút "+ Chọn món" 3. Quan sát màn hình Danh sách món 4. Bấm chọn 1–2 món 5. Bấm "Trở lại" để quay về modal 6. Quan sát số lượng mặt hàng đã chọn | Màn hình Danh sách món mở ra; có ô "Tìm và chọn món"; số lượng mặt hàng đã chọn cập nhật đúng sau khi trở lại |
| ☐ | Toggle "Ẩn hình ảnh" trong Danh sách món | 1. Trong màn hình Danh sách món (sau khi bấm "+ Chọn món") 2. Tìm toggle "Ẩn hình ảnh" 3. Bật toggle → quan sát lưới món 4. Tắt toggle → quan sát lại | Lưới món ẩn ảnh khi toggle bật và hiện ảnh trở lại khi toggle tắt |
| ☐ | Đổi số cột trong Danh sách món | 1. Trong màn hình Danh sách món 2. Tìm dropdown số cột (VD: "6 cột") 3. Chọn số cột khác (VD: 4 cột) 4. Quan sát bố cục lưới món | Lưới món thay đổi số cột tương ứng với lựa chọn |
| ☐ | Tìm món trong Danh sách món | 1. Trong màn hình Danh sách món 2. Tìm ô "Tìm và chọn món" 3. Gõ tên món (thử cả có dấu lẫn không dấu) 4. Quan sát kết quả lọc | Lưới món lọc đúng theo từ khóa đã nhập |
| ☐ | Tiền đặt cọc và Phương thức thanh toán | 1. Mở modal "Đặt bàn" 2. Nhập số tiền vào ô "Tiền đặt cọc" 3. Bấm dropdown "Chọn phương thức" 4. Chọn "Tiền mặt" hoặc "Chuyển khoản" 5. Quan sát giá trị ghi nhận | Số tiền và phương thức được ghi nhận đúng; nếu nhập tiền cọc thì bắt buộc phải chọn phương thức |
| ☐ | Ghi chú giới hạn 200 ký tự | 1. Mở modal "Đặt bàn" 2. Tìm ô "Ghi chú" 3. Quan sát bộ đếm ký tự (x/200) 4. Nhập nội dung dần đến 200 ký tự 5. Thử nhập thêm ký tự thứ 201 | Bộ đếm tăng dần; không cho nhập vượt quá 200 ký tự |
| ☐ | Đặt bàn thành công | 1. Mở modal "Đặt bàn" 2. Điền đầy đủ Khách hàng và Bàn (tối thiểu) 3. Bấm nút "Đặt bàn" 4. Quan sát lịch tuần | Tạo đặt bàn thành công; slot hiện trên lịch đúng ngày giờ; trạng thái "Chờ xác nhận" |
| ☐ | Bấm "Đóng" không tạo đặt bàn | 1. Mở modal "Đặt bàn" 2. Nhập một vài thông tin vào form 3. Bấm nút "Đóng" (hoặc ✕) 4. Quan sát lịch | Modal đóng lại; không có đặt bàn mới nào được tạo |

---

## 3. Xem & thao tác đặt bàn trên lịch tuần

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Bấm vào slot đặt bàn | 1. Vào trang Đặt bàn, quan sát lịch tuần 2. Tìm một slot đặt bàn đã có 3. Bấm vào slot đó 4. Quan sát màn hình mở ra | Mở modal chi tiết / chỉnh sửa đặt bàn đó |
| ☐ | Xem thông tin chi tiết đặt bàn | 1. Bấm vào một slot trên lịch để mở chi tiết 2. Kiểm tra từng thông tin hiển thị trong modal | Hiển thị đúng: tên KH, SĐT, bàn, khu vực, thời gian, số khách, tiền cọc, PTTT, ghi chú, trạng thái |
| ☐ | Xác nhận đặt bàn (Chờ xác nhận → Đã xác nhận) | 1. Bấm vào slot có trạng thái "Chờ xác nhận" 2. Tìm và bấm nút xác nhận đặt bàn trong modal 3. Quan sát trạng thái trên lịch | Trạng thái cập nhật thành "Đã xác nhận"; lịch phản ánh đúng |
| ☐ | Hủy đặt bàn | 1. Bấm vào một slot đặt bàn trên lịch 2. Tìm và bấm nút "Hủy" trong modal 3. Quan sát xem có yêu cầu nhập Lý do hủy không 4. Nhập lý do và xác nhận hủy | Yêu cầu nhập Lý do hủy; sau khi xác nhận trạng thái chuyển sang "Đã hủy" |
| ☐ | Chỉnh sửa thông tin đặt bàn | 1. Bấm vào một slot trên lịch để mở chi tiết 2. Chỉnh sửa một thông tin (VD: đổi số khách hoặc ghi chú) 3. Bấm "Lưu" 4. Mở lại chi tiết đặt bàn đó | Thông tin đã chỉnh sửa cập nhật đúng trên lịch và trong chi tiết |

---

## 4. Tra cứu lịch đặt bàn (trang `/booking/table-reservation`)

### 4.1 Bộ lọc Tra cứu

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Mở trang Tra cứu đặt bàn | 1. Vào trang Đặt bàn 2. Bấm nút "Tra cứu đặt bàn" 3. Quan sát trang mở ra | Trang "Tra cứu lịch đặt bàn" mở ra với bộ lọc phía trên và bảng danh sách bên dưới |
| ☐ | Lọc theo Tên khách hàng | 1. Vào trang Tra cứu 2. Nhập tên khách vào ô "Tên khách hàng" 3. Quan sát bảng kết quả | Chỉ hiện đặt bàn của khách khớp tên; không khớp → bảng rỗng |
| ☐ | Lọc theo Số điện thoại | 1. Vào trang Tra cứu 2. Nhập SĐT vào ô "Số điện thoại" 3. Quan sát bảng kết quả | Chỉ hiện đặt bàn của khách khớp số điện thoại |
| ☐ | Lọc theo Khu vực bàn | 1. Vào trang Tra cứu 2. Bấm dropdown "Khu vực bàn" 3. Chọn "Khu 1" hoặc "Khu 2" 4. Quan sát bảng | Chỉ hiện đặt bàn thuộc khu đã chọn |
| ☐ | Lọc theo Tên bàn ăn | 1. Vào trang Tra cứu 2. Bấm dropdown "Tên bàn ăn" 3. Gõ tên bàn vào ô Search 4. Chọn một bàn 5. Quan sát bảng | Chỉ hiện đặt bàn của bàn đã chọn |
| ☐ | Lọc theo khoảng ngày | 1. Vào trang Tra cứu 2. Nhập ngày vào ô "Từ" 3. Nhập ngày vào ô "Đến" 4. Quan sát bảng kết quả | Chỉ hiện đặt bàn trong khoảng ngày đã nhập |
| ☐ | Lọc theo Trạng thái | 1. Vào trang Tra cứu 2. Bấm dropdown "Trạng thái" 3. Lần lượt chọn: Chờ xác nhận / Đã xác nhận / Hủy tạm / Đã hủy 4. Quan sát bảng sau mỗi lần chọn | Mỗi lần chọn chỉ hiện đặt bàn đúng trạng thái tương ứng |
| ☐ | Kết hợp nhiều bộ lọc | 1. Vào trang Tra cứu 2. Bật đồng thời: nhập Tên khách + chọn Trạng thái + nhập khoảng ngày 3. Quan sát bảng kết quả | Kết quả giao đúng tất cả điều kiện đã lọc |
| ☐ | Nút "Làm mới" reset bộ lọc | 1. Vào trang Tra cứu, đã áp một số bộ lọc 2. Bấm nút "Làm mới" 3. Quan sát các ô bộ lọc và bảng | Toàn bộ bộ lọc bị xóa; bảng hiển thị lại toàn bộ dữ liệu |

---

### 4.2 Bảng danh sách tra cứu

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Bảng hiển thị đủ 16 cột | 1. Vào trang Tra cứu 2. Quan sát bảng kết quả 3. Kiểm tra từng cột từ trái sang phải | Đủ cột: STT, Mã đặt bàn, Mã hóa đơn, Họ và tên, Số điện thoại, Tên bàn ăn, Thời gian đặt, Tổng số khách, Tiền đặt cọc, Phương thức TT, Trạng thái, Lý do hủy, Người hủy, Ngày hủy, Ghi chú, Hành động |
| ☐ | Bấm icon xem chi tiết | 1. Trong bảng tra cứu, tìm cột "Hành động" ở cuối dòng 2. Bấm icon xem (mắt) tại một dòng bất kỳ 3. Quan sát màn hình mở ra | Mở chi tiết đúng đặt bàn của dòng đó |
| ☐ | Cột Trạng thái hiển thị đúng | 1. Vào trang Tra cứu 2. Quan sát cột "Trạng thái" trên các dòng khác nhau 3. So sánh màu / nhãn với trạng thái thực tế của từng đặt bàn | Mỗi trạng thái hiển thị đúng nhãn và màu phân biệt: Chờ xác nhận / Đã xác nhận / Hủy tạm / Đã hủy |
| ☐ | Thông tin hủy hiển thị đúng | 1. Vào trang Tra cứu, lọc Trạng thái = "Đã hủy" 2. Tìm một dòng đặt bàn đã hủy 3. Kiểm tra các cột: Lý do hủy, Người hủy, Ngày hủy | Hiển thị đầy đủ thông tin hủy; các cột này chỉ có dữ liệu khi đặt bàn bị hủy |
| ☐ | Mã hóa đơn liên kết đúng | 1. Vào trang Tra cứu 2. Tìm dòng có dữ liệu ở cột "Mã hóa đơn" (đặt bàn đã thanh toán) 3. Bấm vào mã hóa đơn đó 4. Quan sát trang điều hướng đến | Liên kết dẫn tới đúng đơn hóa đơn tương ứng |
| ☐ | Phân trang | 1. Vào trang Tra cứu với đủ dữ liệu nhiều trang 2. Quan sát điều hướng trang (số trang, nút chuyển) 3. Bấm sang trang 2, trang 3 4. Quan sát dữ liệu từng trang | Phân trang đúng, dữ liệu mỗi trang không lặp |
| ☐ | Nút "← Trở lại" quay về lịch | 1. Vào trang Tra cứu 2. Bấm nút "← Trở lại" góc trên trái 3. Quan sát trang điều hướng đến | Quay lại đúng màn hình lịch đặt bàn theo tuần |

---

## 5. Logic nghiệp vụ

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Trùng lịch cùng bàn cùng giờ | 1. Tạo đặt bàn cho Bàn X lúc 18:00 ngày T, bấm "Đặt bàn" 2. Tạo thêm đặt bàn thứ 2 cho đúng Bàn X, cùng 18:00, cùng ngày T 3. Bấm "Đặt bàn" lần 2 4. Quan sát phản hồi | Hệ thống cảnh báo hoặc chặn tạo đặt bàn trùng lịch bàn |
| ☐ | Tạo đặt cọc → phát sinh phiếu Thu | 1. Tạo đặt bàn mới có nhập tiền đặt cọc (VD: 200,000đ, Tiền mặt) 2. Bấm "Đặt bàn" thành công 3. Vào trang Thu chi, lọc Loại nguồn 4. Tìm phiếu tương ứng | Phát sinh phiếu Thu trong Thu chi với số tiền = tiền cọc, PTTT khớp |
| ☐ | Hủy đặt bàn có cọc → phát sinh phiếu hoàn | 1. Mở chi tiết đặt bàn đã đặt cọc 2. Thực hiện hủy đặt bàn 3. Vào trang Thu chi, kiểm tra phiếu mới phát sinh | Phát sinh phiếu Chi (hoàn tiền) tương ứng nếu cần hoàn cọc |
| ☐ | Đổi trạng thái Chờ → Đã xác nhận | 1. Mở chi tiết đặt bàn đang ở "Chờ xác nhận" 2. Bấm xác nhận 3. Kiểm tra trạng thái trên lịch tuần 4. Kiểm tra trạng thái trên trang Tra cứu | Trạng thái cập nhật đúng "Đã xác nhận" ở cả hai màn hình |
| ☐ | Chọn món trước → mang sang đơn bán | 1. Tạo đặt bàn và chọn trước một số món (bấm "+ Chọn món") 2. Bấm "Đặt bàn" thành công 3. Khi khách đến, mở đơn từ đặt bàn đó 4. Quan sát danh sách món trong đơn | Danh sách món đã chọn trước được mang đầy đủ sang đơn bán hàng |
| ☐ | Mã hóa đơn liên kết sau thanh toán | 1. Tạo đặt bàn, khách đến và thanh toán xong 2. Vào trang Tra cứu, tìm đặt bàn đó 3. Kiểm tra cột "Mã hóa đơn" | Mã hóa đơn xuất hiện và liên kết đúng với đơn thanh toán tương ứng |

---

## 6. Ghi chú rà soát

- **Trạng thái** trên lịch tuần chỉ lọc được 2 giá trị: **Chờ xác nhận** và **Đã hủy**.  
  Trang Tra cứu có đầy đủ 4 giá trị: **Chờ xác nhận, Đã xác nhận, Hủy tạm, Đã hủy** → cần kiểm thử riêng ở mỗi màn hình.
- **Bắt buộc** khi Đặt bàn: **Khách hàng** và **Bàn** (theo thông báo validation thực tế).
- **Phương thức đặt cọc** chỉ có 2: **Tiền mặt** và **Chuyển khoản**.
- **Khu vực bàn** có: khu 1, khu 2.
- **Nhân viên đặt bàn** gồm 4 loại: Thu ngân / Admin / Nhân viên / Quầy bếp.
- **Ghi chú** giới hạn **200 ký tự** (bộ đếm x/200).
- Trang Tra cứu có **16 cột** trong bảng, trong đó Lý do hủy, Người hủy, Ngày hủy chỉ có dữ liệu khi đặt bàn bị hủy.
- Nút "**Làm mới**" trên Tra cứu reset toàn bộ bộ lọc.
