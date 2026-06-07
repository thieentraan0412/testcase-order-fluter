# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

 1. Tải trang & bố cục chung

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 1.1 Hiển thị trang Trả hàng | 1. Đăng nhập 2. Vào menu "Trả hàng" | Trang tải thành công, tab "Trả hàng" được highlight, hiển thị thanh filter + bảng danh sách phiếu |
| ☐ | 1.2 Hiển thị thanh công cụ lọc | 1. Quan sát phía trên bảng | Hiển thị đủ: ô tìm kiếm, dropdown "Chọn khu vực bàn", dropdown "Chọn bàn", nút "Khoảng ngày", nút "Trả hàng" (đỏ), nút "Xuất Excel" |
| ☐ | 1.3 Hiển thị tiêu đề bảng | 1. Quan sát bảng danh sách | Có đủ cột: STT, Bàn, Mã phiếu trả hàng, Thời gian trả hàng, Khách hàng, Đã trả, Hành động |
| ☐ | 1.4 Danh sách rỗng | 1. Khi chưa có phiếu trả hàng phù hợp | Bảng hiển thị trống, không lỗi |
| ☐ | 1.5 Điều hướng menu khác | 1. Bấm các menu Trang chủ/Lịch sử/CRM... | Chuyển đúng trang tương ứng |

 2. Ô tìm kiếm "Mã phiếu trả hàng | Khách hàng"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 2.1 Tìm theo mã phiếu | 1. Nhập mã phiếu trả hàng hợp lệ 2. Quan sát | Bảng lọc đúng phiếu theo mã |
| ☐ | 2.2 Tìm theo tên khách hàng | 1. Nhập tên khách hàng | Bảng lọc đúng phiếu theo khách hàng |
| ☐ | 2.3 Tìm không có kết quả | 1. Nhập chuỗi không tồn tại | Bảng trả về rỗng, không lỗi |
| ☐ | 2.4 Tìm chuỗi rỗng | 1. Xóa hết nội dung ô tìm kiếm | Hiển thị lại toàn bộ danh sách |
| ☐ | 2.5 Tìm ký tự đặc biệt/khoảng trắng | 1. Nhập ký tự đặc biệt, dấu cách | Không lỗi, xử lý hợp lý |
| ☐ | 2.6 Phân biệt hoa/thường | 1. Nhập tên dạng chữ hoa & chữ thường | Kết quả tìm kiếm nhất quán |

 3. Lọc theo Khu vực bàn & Bàn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 3.1 Mở dropdown khu vực | 1. Bấm "Chọn khu vực bàn" | Hiển thị danh sách khu vực + ô search |
| ☐ | 3.2 Chọn 1 khu vực | 1. Chọn 1 khu vực (VD: Khu 1) | Khu vực được chọn hiển thị dạng tag có dấu (×) |
| ☐ | 3.3 Search khu vực | 1. Gõ tên khu vào ô search dropdown | Lọc đúng khu vực theo từ khóa |
| ☐ | 3.4 Bỏ chọn khu vực | 1. Bấm dấu (×) trên tag khu vực đã chọn | Khu vực bị bỏ chọn, filter reset |
| ☐ | 3.5 Mở dropdown bàn | 1. Bấm "Chọn bàn" | Hiển thị danh sách bàn + ô search |
| ☐ | 3.6 Chọn 1 bàn | 1. Chọn 1 bàn cụ thể | Bàn được chọn, danh sách lọc theo bàn |
| ☐ | 3.7 Liên kết khu vực ↔ bàn | 1. Chọn khu vực rồi mở dropdown bàn | Danh sách bàn phù hợp/cập nhật theo khu vực (nếu áp dụng) |
| ☐ | 3.8 Search bàn | 1. Gõ tên bàn vào ô search | Lọc đúng bàn theo từ khóa |
| ☐ | 3.9 Kết hợp nhiều filter | 1. Áp dụng đồng thời search + khu vực + bàn + ngày | Kết quả khớp tất cả điều kiện |

 4. Bộ lọc "Khoảng ngày"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 4.1 Mở popup khoảng ngày | 1. Bấm "Khoảng ngày" | Hiển thị: Hôm nay, Hôm qua, Tùy chọn, Từ ngày, Đến ngày, nút Đóng & Xác nhận |
| ☐ | 4.2 Chọn "Hôm nay" | 1. Chọn "Hôm nay" 2. Xác nhận | Lọc phiếu trả hàng trong ngày hôm nay |
| ☐ | 4.3 Chọn "Hôm qua" | 1. Chọn "Hôm qua" 2. Xác nhận | Lọc phiếu trả hàng của ngày hôm qua |
| ☐ | 4.4 Tùy chọn khoảng ngày | 1. Chọn "Tùy chọn" 2. Nhập Từ ngày, Đến ngày 3. Xác nhận | Lọc đúng phiếu trong khoảng đã chọn |
| ☐ | 4.5 Từ ngày > Đến ngày | 1. Nhập Từ ngày lớn hơn Đến ngày | Hiển thị cảnh báo / không cho áp dụng |
| ☐ | 4.6 Nút Đóng | 1. Mở popup 2. Bấm "Đóng" | Đóng popup, không thay đổi filter |
| ☐ | 4.7 Nút Xác nhận | 1. Chọn khoảng ngày 2. Bấm "Xác nhận" | Áp dụng filter, đóng popup |

 5. Nút "Xuất Excel"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 5.1 Xuất Excel danh sách | 1. Bấm "Xuất Excel" | Tải về file Excel chứa danh sách phiếu trả hàng |
| ☐ | 5.2 Xuất Excel có filter | 1. Áp dụng filter 2. Bấm "Xuất Excel" | File Excel chỉ chứa dữ liệu khớp filter |
| ☐ | 5.3 Xuất Excel danh sách rỗng | 1. Lọc ra danh sách rỗng 2. Bấm "Xuất Excel" | Xử lý hợp lý (file rỗng hoặc thông báo) |
| ☐ | 5.4 Nội dung file đúng | 1. Mở file đã tải | Cột & dữ liệu khớp với bảng trên màn hình |

 6. Nút "Trả hàng" → Modal "Danh sách hóa đơn"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 6.1 Mở modal danh sách hóa đơn | 1. Bấm nút "Trả hàng" (đỏ) | Mở modal "Danh sách hóa đơn" với bộ lọc và bảng hóa đơn |
| ☐ | 6.2 Hiển thị cột bảng hóa đơn | 1. Quan sát modal | Có cột: STT, Mã hóa đơn, Ngày tạo, Khách hàng, Bàn, Nhân viên, Tổng tiền + nút "Chọn" |
| ☐ | 6.3 Lọc theo "Đơn hàng" | 1. Nhập mã đơn vào ô "Đơn hàng" | Bảng lọc đúng hóa đơn |
| ☐ | 6.4 Lọc theo Từ ngày/Đến ngày | 1. Đổi Từ ngày, Đến ngày | Danh sách hóa đơn cập nhật theo khoảng ngày |
| ☐ | 6.5 Mặc định khoảng ngày | 1. Quan sát giá trị mặc định | Hiển thị khoảng ngày mặc định hợp lý (VD: tuần hiện tại) |
| ☐ | 6.6 Đóng modal bằng (×) | 1. Bấm dấu (×) góc phải | Modal đóng, về trang chính |
| ☐ | 6.7 Đóng modal bằng "Đóng" | 1. Bấm nút "Đóng" | Modal đóng |
| ☐ | 6.8 Bấm "Chọn" hóa đơn | 1. Bấm "Chọn" ở 1 hóa đơn | Mở modal "Thông tin trả hàng" của hóa đơn đó |
| ☐ | 6.9 Danh sách hóa đơn rỗng | 1. Lọc khoảng ngày không có hóa đơn | Bảng trống, không lỗi |

 7. Modal "Thông tin trả hàng" — Thông tin & danh sách món

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 7.1 Hiển thị thông tin đầu phiếu | 1. Mở modal trả hàng | Hiển thị: Khách hàng, Mã hóa đơn, Thời gian thanh toán, Phòng/bàn, Số lượng, Phương thức thanh toán |
| ☐ | 7.2 Hiển thị bảng món | 1. Quan sát bảng món | Cột: Tên món, Số lượng, Trả lại (− số +), Đơn giá, Thành tiền |
| ☐ | 7.3 Hiển thị topping/món thêm | 1. Quan sát món có topping/size | Hiển thị chi tiết món thêm, size và giá kèm theo |
| ☐ | 7.4 Tăng số lượng trả | 1. Bấm nút (+) ở cột Trả lại | Số lượng trả tăng, tiền trả lại cập nhật |
| ☐ | 7.5 Giảm số lượng trả | 1. Bấm nút (−) ở cột Trả lại | Số lượng trả giảm, tiền trả lại cập nhật |
| ☐ | 7.6 Nhập số lượng trả trực tiếp | 1. Nhập số vào ô số lượng trả | Cập nhật đúng, tính lại tiền |
| ☐ | 7.7 Trả vượt số đã mua | 1. Nhập số trả > số lượng đã mua | Chặn / cảnh báo, không cho vượt |
| ☐ | 7.8 Trả số âm hoặc 0 | 1. Nhập số âm hoặc 0 | Không cho nhập số âm; xử lý hợp lý với 0 |
| ☐ | 7.9 Nhập ký tự không phải số | 1. Nhập chữ/ký tự vào ô số lượng | Không nhận, giữ giá trị hợp lệ |
| ☐ | 7.10 Nút "Danh sách mặc định" | 1. Thay đổi số lượng 2. Bấm "Danh sách mặc định" | Reset danh sách món về trạng thái ban đầu |
| ☐ | 7.11 Cuộn danh sách món | 1. Mở hóa đơn nhiều món 2. Cuộn trong bảng | Cuộn mượt, hiển thị đủ món |

 8. Modal "Thông tin trả hàng" — Tính tiền & trường nhập

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 8.1 Cột "Tổng giá trị đơn hàng" | 1. Quan sát cột trái | Hiển thị read-only: Tổng tiền hàng, VAT, Phụ thu, Giảm giá, Tích điểm, Tổng tiền thanh toán |
| ☐ | 8.2 Cột "Số tiền trả hàng" | 1. Quan sát cột phải | Hiển thị: Tổng tiền hàng, VAT, Phụ thu, Giảm giá, Tích điểm, Tổng tiền trả lại |
| ☐ | 8.3 Tự động tính tiền trả | 1. Thay đổi số lượng trả | Tổng tiền hàng/VAT/Tổng tiền trả lại cập nhật tự động đúng |
| ☐ | 8.4 Sửa Phụ thu (trả) | 1. Nhập giá trị "Phụ thu" cột trả | Tổng tiền trả lại tính lại đúng |
| ☐ | 8.5 Sửa Giảm giá (trả) | 1. Nhập giá trị "Giảm giá" cột trả | Tổng tiền trả lại trừ đúng giảm giá |
| ☐ | 8.6 Sửa Tích điểm (trả) | 1. Nhập giá trị "Tích điểm" cột trả | Cập nhật đúng theo logic tích điểm |
| ☐ | 8.7 Nhập giá trị âm/ký tự lạ vào các ô tiền | 1. Nhập số âm, chữ | Chặn/cảnh báo, không phá vỡ phép tính |
| ☐ | 8.8 Giảm giá vượt tổng tiền | 1. Nhập Giảm giá > tổng tiền trả | Chặn/cảnh báo, không cho âm tiền trả |
| ☐ | 8.9 Phương thức thanh toán | 1. Mở dropdown "Phương thức thanh toán" | Chọn được phương thức (Tiền mặt, …) |
| ☐ | 8.10 Tên khách hàng (bắt buộc) | 1. Để trống "Tên khách hàng*" 2. Bấm Trả hàng | Báo lỗi yêu cầu nhập tên khách hàng |
| ☐ | 8.11 Số điện thoại | 1. Nhập SĐT hợp lệ / sai định dạng | Hợp lệ thì nhận; sai định dạng thì cảnh báo (nếu có validate) |
| ☐ | 8.12 Lý do trả hàng (bắt buộc) | 1. Để trống "Lý do trả hàng*" 2. Bấm Trả hàng | Báo lỗi yêu cầu nhập lý do |

 9. Xác nhận & lưu phiếu trả hàng

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 9.1 Bấm "Trả hàng" trong modal | 1. Điền đủ thông tin 2. Bấm "Trả hàng" | Hiển thị hộp xác nhận "Bạn có chắc muốn trả hàng?" |
| ☐ | 9.2 Hủy xác nhận | 1. Ở hộp xác nhận bấm "Đóng" | Đóng hộp xác nhận, giữ nguyên dữ liệu, chưa lưu |
| ☐ | 9.3 Xác nhận trả hàng | 1. Bấm "Xác nhận" | Tạo phiếu trả hàng thành công, hiển thị thông báo |
| ☐ | 9.4 Phiếu xuất hiện trong danh sách | 1. Sau khi trả hàng, quan sát bảng chính | Phiếu mới hiển thị với đầy đủ thông tin (mã, bàn, thời gian, khách, đã trả) |
| ☐ | 9.5 Trả hàng khi chưa chọn món nào | 1. Để số lượng trả = 0 toàn bộ 2. Bấm Trả hàng | Chặn/cảnh báo phải chọn ít nhất 1 món |
| ☐ | 9.6 Nút "Đóng" modal trả hàng | 1. Bấm "Đóng" | Đóng modal, không lưu, không tạo phiếu |
| ☐ | 9.7 Trả hàng cho hóa đơn đã trả 1 phần | 1. Chọn hóa đơn đã trả 1 phần trước đó | Chỉ cho trả phần còn lại, số lượng đúng |

 10. Bảng danh sách phiếu trả hàng & cột "Hành động"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 10.1 Hiển thị dữ liệu phiếu | 1. Quan sát các dòng phiếu | Mỗi dòng hiển thị đúng STT, Bàn, Mã phiếu, Thời gian, Khách hàng, Đã trả |
| ☐ | 10.2 Nút trong cột "Hành động" | 1. Bấm nút ở cột Hành động (xem/in...) | Thực hiện đúng chức năng (xem chi tiết / in phiếu) |
| ☐ | 10.3 Sắp xếp/cuộn danh sách dài | 1. Tạo nhiều phiếu 2. Cuộn bảng | Hiển thị mượt, không lỗi layout |
| ☐ | 10.4 Định dạng số tiền cột "Đã trả" | 1. Quan sát cột Đã trả | Định dạng tiền tệ đúng (dấu phân cách, đơn vị đ) |

 11. Kiểm thử khác (UI/UX, phân quyền, hiệu năng)

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 11.1 Hiển thị responsive | 1. Thu nhỏ/phóng to cửa sổ trình duyệt | Layout không vỡ, các nút vẫn dùng được |
| ☐ | 11.2 Đa ngôn ngữ | 1. Đổi cờ ngôn ngữ (nếu có) | Nội dung trang đổi ngôn ngữ tương ứng |
| ☐ | 11.3 Tải lại trang giữ filter | 1. Áp dụng filter 2. F5 | Kiểm tra hành vi giữ/đặt lại filter hợp lý |
| ☐ | 11.4 Phân quyền tài khoản | 1. Đăng nhập tài khoản quyền thấp | Hiển thị/ẩn nút Trả hàng, Xuất Excel theo phân quyền |
| ☐ | 11.5 Mất kết nối khi trả hàng | 1. Ngắt mạng 2. Bấm Xác nhận trả hàng | Báo lỗi rõ ràng, không lưu sai dữ liệu |
| ☐ | 11.6 Bấm Trả hàng nhiều lần nhanh | 1. Bấm "Xác nhận" liên tục | Không tạo trùng nhiều phiếu (chống double submit) |
