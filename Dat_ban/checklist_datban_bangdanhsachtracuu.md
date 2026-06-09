## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

6.10 Bảng danh sách tra cứu

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 6.10.1 | ☐ | Bảng hiển thị đủ 16 cột | 1. Vào trang Tra cứu 2. Quan sát bảng kết quả 3. Kiểm tra từng cột từ trái sang phải | Đủ cột: STT, Mã đặt bàn, Mã hóa đơn, Họ và tên, Số điện thoại, Tên bàn ăn, Thời gian đặt, Tổng số khách, Tiền đặt cọc, Phương thức TT, Trạng thái, Lý do hủy, Người hủy, Ngày hủy, Ghi chú, Hành động |
| 6.10.2 | ☐ | Bấm icon xem chi tiết | 1. Trong bảng tra cứu, tìm cột "Hành động" ở cuối dòng 2. Bấm icon xem (mắt) tại một dòng bất kỳ 3. Quan sát màn hình mở ra | Mở chi tiết đúng đặt bàn của dòng đó |
| 6.10.3 | ☐ | Cột Trạng thái hiển thị đúng | 1. Vào trang Tra cứu 2. Quan sát cột "Trạng thái" trên các dòng khác nhau 3. So sánh màu / nhãn với trạng thái thực tế của từng đặt bàn | Mỗi trạng thái hiển thị đúng nhãn và màu phân biệt: Chờ xác nhận / Đã xác nhận / Hủy tạm / Đã hủy |
| 6.10.4 | ☐ | Thông tin hủy hiển thị đúng | 1. Vào trang Tra cứu, lọc Trạng thái = "Đã hủy" 2. Tìm một dòng đặt bàn đã hủy 3. Kiểm tra các cột: Lý do hủy, Người hủy, Ngày hủy | Hiển thị đầy đủ thông tin hủy; các cột này chỉ có dữ liệu khi đặt bàn bị hủy |
| 6.10.5 | ☐ | Mã hóa đơn liên kết đúng | 1. Vào trang Tra cứu 2. Tìm dòng có dữ liệu ở cột "Mã hóa đơn" (đặt bàn đã thanh toán) 3. Bấm vào mã hóa đơn đó 4. Quan sát trang điều hướng đến | Liên kết dẫn tới đúng đơn hóa đơn tương ứng |
| 6.10.6 | ☐ | Phân trang | 1. Vào trang Tra cứu với đủ dữ liệu nhiều trang 2. Quan sát điều hướng trang (số trang, nút chuyển) 3. Bấm sang trang 2, trang 3 4. Quan sát dữ liệu từng trang | Phân trang đúng, dữ liệu mỗi trang không lặp |
| 6.10.7 | ☐ | Nút "← Trở lại" quay về lịch | 1. Vào trang Tra cứu 2. Bấm nút "← Trở lại" góc trên trái 3. Quan sát trang điều hướng đến | Quay lại đúng màn hình lịch đặt bàn theo tuần |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
