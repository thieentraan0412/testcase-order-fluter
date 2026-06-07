
## 2. Thu chi

Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense

---

2.4 Thêm phiếu

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
2.4.1 | ☐ | Bấm "Thêm" mở modal | 1. Vào trang Thu chi 2. Tìm và bấm nút "Thêm" (góc trên phải hoặc đầu bảng) 3. Quan sát màn hình | Modal "Thêm phiếu" mở ra |
2.4.2 | ☐ | Mã phiếu tự sinh | 1. Mở modal "Thêm phiếu" 2. Quan sát ô "Mã phiếu" ngay khi modal vừa mở | Mã phiếu được điền tự động (VD: vote-00001), không cần nhập tay |
2.4.3 | ☐ | Bỏ trống "Loại thu chi" (bắt buộc) | 1. Mở modal "Thêm phiếu" 2. Điền đầy đủ các trường khác nhưng để trống "Loại thu chi" 3. Bấm nút "Lưu" 4. Quan sát phản hồi | Hệ thống chặn lưu, hiển thị thông báo lỗi yêu cầu chọn Loại thu chi |
2.4.4 | ☐ | Bỏ trống "Số tiền" (bắt buộc) | 1. Mở modal "Thêm phiếu" 2. Điền đầy đủ các trường khác nhưng để trống ô "Số tiền" 3. Bấm nút "Lưu" 4. Quan sát phản hồi | Hệ thống chặn lưu, hiển thị thông báo lỗi yêu cầu nhập Số tiền |
2.4.5 | ☐ | Chọn Loại đối tượng / Người nộp | 1. Mở modal "Thêm phiếu" 2. Tìm dropdown "Loại đối tượng", chọn một loại (VD: Khách hàng) 3. Tìm ô "Người nộp", chọn hoặc nhập tên người nộp 4. Quan sát giá trị được ghi nhận | Loại đối tượng và Người nộp được chọn và hiển thị đúng trong form |
2.4.6 | ☐ | Chọn Phân loại thu chi | 1. Mở modal "Thêm phiếu" 2. Tìm dropdown "Phân loại thu chi" 3. Bấm dropdown, chọn một phân loại 4. Quan sát giá trị sau khi chọn | Phân loại được ghi nhận, hiển thị đúng trong ô |
2.4.7 | ☐ | Chọn Phương thức thanh toán | 1. Mở modal "Thêm phiếu" 2. Quan sát giá trị mặc định của "Phương thức thanh toán" (PTTT) 3. Đổi sang một phương thức khác (VD: Chuyển khoản) 4. Quan sát giá trị sau khi chọn | PTTT mặc định là "Tiền mặt"; đổi được sang phương thức khác và ghi nhận đúng |
2.4.8 | ☐ | Nhập Số tiền | 1. Mở modal "Thêm phiếu" 2. Bấm vào ô "Số tiền" 3. Thử nhập chữ cái → quan sát 4. Xóa, nhập số hợp lệ (VD: 150000) → quan sát định dạng hiển thị | Ô chỉ nhận số, tự định dạng theo kiểu tiền (VD: 150,000) |
2.4.9 | ☐ | Đính kèm tệp | 1. Mở modal "Thêm phiếu" 2. Tìm nút đính kèm tệp 3. Bấm và chọn một file từ máy tính 4. Quan sát file sau khi tải lên | File được tải lên thành công, hiển thị tên file trong form |
2.4.10 | ☐ | Mô tả giới hạn 200 ký tự | 1. Mở modal "Thêm phiếu" 2. Tìm ô "Mô tả" 3. Quan sát bộ đếm ký tự (0/200) 4. Nhập dần đến 200 ký tự → quan sát 5. Thử nhập thêm ký tự thứ 201 | Bộ đếm tăng dần; dừng tại 200, không nhập thêm được hoặc bị cắt ngắn |
2.4.11 | ☐ | Bấm "Lưu" hợp lệ | 1. Mở modal "Thêm phiếu" 2. Điền đầy đủ tất cả trường bắt buộc (Loại thu chi, Số tiền) 3. Bấm nút "Lưu" 4. Quan sát danh sách phiếu và thẻ tổng quan | Phiếu mới xuất hiện đầu danh sách; thẻ Tổng thu hoặc Tổng chi cập nhật tương ứng |
2.4.12 | ☐ | Bấm "Đóng" không tạo phiếu | 1. Mở modal "Thêm phiếu" 2. Điền một vài thông tin vào form 3. Bấm nút "Đóng" (không bấm Lưu) 4. Quan sát danh sách phiếu | Modal đóng lại; không có phiếu mới nào được tạo; danh sách không thay đổi |
2.4.13 | ☐ | Mã phiếu tăng dần sau mỗi lần tạo | 1. Mở modal "Thêm phiếu", ghi nhận mã phiếu hiển thị (VD: vote-00005) 2. Điền đủ trường bắt buộc, bấm "Lưu" 3. Mở lại modal "Thêm phiếu" lần 2 4. Quan sát mã phiếu mới | Mã phiếu lần 2 tăng thêm 1 (VD: vote-00006), không bị lặp lại mã cũ |
2.4.14 | ☐ | Nhập Số tiền = 0 | 1. Mở modal "Thêm phiếu" 2. Điền đầy đủ Loại thu chi 3. Nhập "0" vào ô Số tiền 4. Bấm "Lưu" 5. Quan sát phản hồi | Hệ thống chặn lưu, hiển thị thông báo lỗi yêu cầu số tiền lớn hơn 0 |
2.4.15 | ☐ | Loại đối tượng thay đổi → danh sách Người nộp thay đổi | 1. Mở modal "Thêm phiếu" 2. Bấm dropdown "Loại đối tượng", chọn "Khách hàng" → bấm dropdown "Người nộp" quan sát danh sách 3. Đổi "Loại đối tượng" sang "Nhân viên" → bấm dropdown "Người nộp" quan sát lại | Danh sách Người nộp thay đổi theo Loại đối tượng: chọn Khách hàng → chỉ list khách hàng; chọn Nhân viên → chỉ list nhân viên |
2.4.16 | ☐ | Loại đối tượng chưa chọn → Người nộp | 1. Mở modal "Thêm phiếu" 2. Không chọn "Loại đối tượng" 3. Bấm vào dropdown "Người nộp" 4. Quan sát trạng thái ô | Ô "Người nộp" bị disabled hoặc danh sách rỗng khi chưa chọn Loại đối tượng |
2.4.17 | ☐ | Loại thu chi = "Chi" → label đổi sang "Người nhận" | 1. Mở modal "Thêm phiếu" 2. Bấm dropdown "Loại thu chi", chọn "Thu" → quan sát nhãn bên phải 3. Đổi sang chọn "Chi" → quan sát lại nhãn | Chọn "Thu": nhãn hiển thị "Người nộp". Chọn "Chi": nhãn đổi thành "Người nhận" |
2.4.18 | ☐ | Xóa file đính kèm sau khi đã chọn | 1. Mở modal "Thêm phiếu" 2. Bấm "Chọn tệp", chọn một file từ máy 3. Quan sát file hiển thị trong ô đính kèm 4. Tìm và bấm nút xóa (X) bên cạnh tên file 5. Quan sát lại ô đính kèm | File bị xóa khỏi form, ô đính kèm trở về trạng thái "Chưa có tệp nào được chọn" |
2.4.19 | ☐ | Lưu phiếu thu → Tồn quỹ tăng đúng | 1. Vào trang Thu chi, ghi nhận "Tồn quỹ cuối kỳ" hiện tại (VD: 8,962,000đ) 2. Mở modal "Thêm phiếu", chọn Loại = "Thu", nhập Số tiền = 200,000đ, bấm "Lưu" 3. Quan sát thẻ "Tồn quỹ cuối kỳ" sau khi lưu | Tồn quỹ cuối kỳ tăng đúng 200,000đ (VD: thành 9,162,000đ) |
2.4.20 | ☐ | Lưu phiếu chi → Tồn quỹ giảm đúng | 1. Vào trang Thu chi, ghi nhận "Tồn quỹ cuối kỳ" hiện tại 2. Mở modal "Thêm phiếu", chọn Loại = "Chi", nhập Số tiền = 100,000đ, bấm "Lưu" 3. Quan sát thẻ "Tồn quỹ cuối kỳ" sau khi lưu | Tồn quỹ cuối kỳ giảm đúng 100,000đ |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
