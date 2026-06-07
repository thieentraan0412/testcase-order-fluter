## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

6.9 Bộ lọc Tra cứu

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
6.9.1 | ☐ | Mở trang Tra cứu đặt bàn | 1. Vào trang Đặt bàn 2. Bấm nút "Tra cứu đặt bàn" 3. Quan sát trang mở ra | Trang "Tra cứu lịch đặt bàn" mở ra với bộ lọc phía trên và bảng danh sách bên dưới |
6.9.2 | ☐ | Lọc theo Tên khách hàng | 1. Vào trang Tra cứu 2. Nhập tên khách vào ô "Tên khách hàng" 3. Quan sát bảng kết quả | Chỉ hiện đặt bàn của khách khớp tên; không khớp → bảng rỗng |
6.9.3 | ☐ | Lọc theo Số điện thoại | 1. Vào trang Tra cứu 2. Nhập SĐT vào ô "Số điện thoại" 3. Quan sát bảng kết quả | Chỉ hiện đặt bàn của khách khớp số điện thoại |
6.9.4 | ☐ | Lọc theo Khu vực bàn | 1. Vào trang Tra cứu 2. Bấm dropdown "Khu vực bàn" 3. Chọn "Khu 1" hoặc "Khu 2" 4. Quan sát bảng | Chỉ hiện đặt bàn thuộc khu đã chọn |
6.9.5 | ☐ | Lọc theo Tên bàn ăn | 1. Vào trang Tra cứu 2. Bấm dropdown "Tên bàn ăn" 3. Gõ tên bàn vào ô Search 4. Chọn một bàn 5. Quan sát bảng | Chỉ hiện đặt bàn của bàn đã chọn |
6.9.6 | ☐ | Lọc theo khoảng ngày | 1. Vào trang Tra cứu 2. Nhập ngày vào ô "Từ" 3. Nhập ngày vào ô "Đến" 4. Quan sát bảng kết quả | Chỉ hiện đặt bàn trong khoảng ngày đã nhập |
6.9.7 | ☐ | Lọc theo Trạng thái | 1. Vào trang Tra cứu 2. Bấm dropdown "Trạng thái" 3. Lần lượt chọn: Chờ xác nhận / Đã xác nhận / Hủy tạm / Đã hủy 4. Quan sát bảng sau mỗi lần chọn | Mỗi lần chọn chỉ hiện đặt bàn đúng trạng thái tương ứng |
6.9.8 | ☐ | Kết hợp nhiều bộ lọc | 1. Vào trang Tra cứu 2. Bật đồng thời: nhập Tên khách + chọn Trạng thái + nhập khoảng ngày 3. Quan sát bảng kết quả | Kết quả giao đúng tất cả điều kiện đã lọc |
6.9.9 | ☐ | Nút "Làm mới" reset bộ lọc | 1. Vào trang Tra cứu, đã áp một số bộ lọc 2. Bấm nút "Làm mới" 3. Quan sát các ô bộ lọc và bảng | Toàn bộ bộ lọc bị xóa; bảng hiển thị lại toàn bộ dữ liệu |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
