## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

Hãy sử dụng google chorme và thực hiện các testcase sau

6.6 Thêm khách hàng mới (modal phụ "Thêm / Chỉnh sửa")

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 6.6.1 | ☐ | Modal phụ hiển thị đủ trường | 1. Trong modal Đặt bàn, bấm "+ Thêm mới" 2. Quan sát toàn bộ các trường trong modal Thêm/Chỉnh sửa | Hiển thị đủ: Hình ảnh (upload), Mã KH (tự động), Tên KH*, Căn cước CD, Nhóm KH*, Giới tính, Điện thoại*, Ngày sinh, Email, Địa chỉ, Ghi chú, Loại (Cá nhân/Doanh nghiệp) |
| 6.6.2 | ☐ | Bỏ trống Tên khách hàng (bắt buộc) | 1. Mở modal Thêm/Chỉnh sửa 2. Điền đầy đủ các trường khác, để trống ô "Tên khách hàng" 3. Bấm "Lưu" 4. Quan sát phản hồi | Hệ thống chặn lưu, báo lỗi Tên là bắt buộc |
| 6.6.3 | ☐ | Bỏ trống Nhóm khách hàng (bắt buộc) | 1. Mở modal Thêm/Chỉnh sửa 2. Điền Tên và Điện thoại, để trống "Nhóm khách hàng" 3. Bấm "Lưu" 4. Quan sát phản hồi | Hệ thống chặn lưu, báo lỗi Nhóm là bắt buộc |
| 6.6.4 | ☐ | Bỏ trống Điện thoại (bắt buộc) | 1. Mở modal Thêm/Chỉnh sửa 2. Điền Tên và Nhóm, để trống "Điện thoại" 3. Bấm "Lưu" 4. Quan sát phản hồi | Hệ thống chặn lưu, báo lỗi Điện thoại là bắt buộc |
| 6.6.5 | ☐ | Upload ảnh đại diện | 1. Mở modal Thêm/Chỉnh sửa 2. Bấm nút "Tải lên" ảnh đại diện 3. Chọn một ảnh từ máy tính 4. Quan sát sau khi chọn | Ảnh được upload và hiển thị preview trong form |
| 6.6.6 | ☐ | Chọn loại Cá nhân / Doanh nghiệp | 1. Mở modal Thêm/Chỉnh sửa 2. Tìm phần "Loại" 3. Chọn lần lượt "Cá nhân" và "Doanh nghiệp" 4. Quan sát giá trị ghi nhận | Ghi nhận đúng loại khách hàng đã chọn |
| 6.6.7 | ☐ | Lưu khách hàng mới thành công | 1. Mở modal Thêm/Chỉnh sửa 2. Điền đầy đủ tất cả trường bắt buộc (Tên, Nhóm, Điện thoại) 3. Bấm "Lưu" 4. Quan sát modal Đặt bàn phía sau | Tạo khách hàng mới thành công; tên khách tự động điền vào trường Khách hàng của modal Đặt bàn |
| 6.6.8 | ☐ | Bấm "Đóng" modal phụ | 1. Mở modal Thêm/Chỉnh sửa 2. Nhập một vài thông tin 3. Bấm nút "Đóng" 4. Quan sát kết quả | Modal phụ đóng lại, quay về modal Đặt bàn; không tạo khách hàng mới |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
