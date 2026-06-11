## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

Hãy sử dụng google chorme và thực hiện các testcase sau

6.7 Thông tin đặt bàn

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 6.7.1 | ☐ | Nhập số lượng người lớn / trẻ em | 1. Mở modal "Đặt bàn" 2. Tìm ô "Số lượng người lớn", nhập một số nguyên dương (VD: 3) 3. Tìm ô "Số lượng trẻ em", nhập một số (VD: 1) 4. Quan sát giá trị ghi nhận | Ghi nhận đúng; chỉ nhận số nguyên dương |
| 6.7.2 | ☐ | Trường Thời gian mặc định và chỉnh sửa được | 1. Mở modal "Đặt bàn" 2. Quan sát giá trị mặc định trong ô Thời gian 3. Thử bấm vào ô và sửa ngày giờ sang giá trị khác | Hiển thị ngày giờ hiện tại làm mặc định; có thể chỉnh sửa sang ngày giờ khác |
| 6.7.3 | ☐ | Chọn Khu vực bàn → danh sách bàn cập nhật | 1. Mở modal "Đặt bàn" 2. Bấm dropdown "Chọn Khu vực bàn" 3. Chọn "Khu 1" → quan sát danh sách bàn 4. Đổi sang "Khu 2" → quan sát lại | Danh sách bàn chỉ hiện bàn thuộc khu đã chọn |
| 6.7.4 | ☐ | Chọn Bàn | 1. Mở modal "Đặt bàn", đã chọn Khu vực 2. Bấm dropdown chọn Bàn 3. Gõ tên bàn vào ô Search nếu cần 4. Chọn một bàn cụ thể | Bàn được ghi nhận đúng vào form |
| 6.7.5 | ☐ | Chọn món trước khi đặt bàn | 1. Mở modal "Đặt bàn" 2. Bấm nút "+ Chọn món" 3. Quan sát màn hình Danh sách món 4. Bấm chọn 1–2 món 5. Bấm "Trở lại" để quay về modal 6. Quan sát số lượng mặt hàng đã chọn | Màn hình Danh sách món mở ra; có ô "Tìm và chọn món"; số lượng mặt hàng đã chọn cập nhật đúng sau khi trở lại |
| 6.7.6 | ☐ | Toggle "Ẩn hình ảnh" trong Danh sách món | 1. Trong màn hình Danh sách món (sau khi bấm "+ Chọn món") 2. Tìm toggle "Ẩn hình ảnh" 3. Bật toggle → quan sát lưới món 4. Tắt toggle → quan sát lại | Lưới món ẩn ảnh khi toggle bật và hiện ảnh trở lại khi toggle tắt |
| 6.7.7 | ☐ | Đổi số cột trong Danh sách món | 1. Trong màn hình Danh sách món 2. Tìm dropdown số cột (VD: "6 cột") 3. Chọn số cột khác (VD: 4 cột) 4. Quan sát bố cục lưới món | Lưới món thay đổi số cột tương ứng với lựa chọn |
| 6.7.8 | ☐ | Tìm món trong Danh sách món | 1. Trong màn hình Danh sách món 2. Tìm ô "Tìm và chọn món" 3. Gõ tên món (thử cả có dấu lẫn không dấu) 4. Quan sát kết quả lọc | Lưới món lọc đúng theo từ khóa đã nhập |
| 6.7.9 | ☐ | Tiền đặt cọc và Phương thức thanh toán | 1. Mở modal "Đặt bàn" 2. Nhập số tiền vào ô "Tiền đặt cọc" 3. Bấm dropdown "Chọn phương thức" 4. Chọn "Tiền mặt" hoặc "Chuyển khoản" 5. Quan sát giá trị ghi nhận | Số tiền và phương thức được ghi nhận đúng; nếu nhập tiền cọc thì bắt buộc phải chọn phương thức |
| 6.7.10 | ☐ | Ghi chú giới hạn 200 ký tự | 1. Mở modal "Đặt bàn" 2. Tìm ô "Ghi chú" 3. Quan sát bộ đếm ký tự (x/200) 4. Nhập nội dung dần đến 200 ký tự 5. Thử nhập thêm ký tự thứ 201 | Bộ đếm tăng dần; không cho nhập vượt quá 200 ký tự |
| 6.7.11 | ☐ | Đặt bàn thành công | 1. Mở modal "Đặt bàn" 2. Điền đầy đủ Khách hàng và Bàn (tối thiểu) 3. Bấm nút "Đặt bàn" 4. Quan sát lịch tuần | Tạo đặt bàn thành công; slot hiện trên lịch đúng ngày giờ; trạng thái "Chờ xác nhận" |
| 6.7.12 | ☐ | Bấm "Đóng" không tạo đặt bàn | 1. Mở modal "Đặt bàn" 2. Nhập một vài thông tin vào form 3. Bấm nút "Đóng" (hoặc ✕) 4. Quan sát lịch | Modal đóng lại; không có đặt bàn mới nào được tạo |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
