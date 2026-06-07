## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

6.11 Logic nghiệp vụ

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
6.11.1 | ☐ | Trùng lịch cùng bàn cùng giờ | 1. Tạo đặt bàn cho Bàn X lúc 18:00 ngày T, bấm "Đặt bàn" 2. Tạo thêm đặt bàn thứ 2 cho đúng Bàn X, cùng 18:00, cùng ngày T 3. Bấm "Đặt bàn" lần 2 4. Quan sát phản hồi | Hệ thống cảnh báo hoặc chặn tạo đặt bàn trùng lịch bàn |
6.11.2 | ☐ | Tạo đặt cọc → phát sinh phiếu Thu | 1. Tạo đặt bàn mới có nhập tiền đặt cọc (VD: 200,000đ, Tiền mặt) 2. Bấm "Đặt bàn" thành công 3. Vào trang Thu chi, lọc Loại nguồn 4. Tìm phiếu tương ứng | Phát sinh phiếu Thu trong Thu chi với số tiền = tiền cọc, PTTT khớp |
6.11.3 | ☐ | Hủy đặt bàn có cọc → phát sinh phiếu hoàn | 1. Mở chi tiết đặt bàn đã đặt cọc 2. Thực hiện hủy đặt bàn 3. Vào trang Thu chi, kiểm tra phiếu mới phát sinh | Phát sinh phiếu Chi (hoàn tiền) tương ứng nếu cần hoàn cọc |
6.11.4 | ☐ | Đổi trạng thái Chờ → Đã xác nhận | 1. Mở chi tiết đặt bàn đang ở "Chờ xác nhận" 2. Bấm xác nhận 3. Kiểm tra trạng thái trên lịch tuần 4. Kiểm tra trạng thái trên trang Tra cứu | Trạng thái cập nhật đúng "Đã xác nhận" ở cả hai màn hình |
6.11.5 | ☐ | Chọn món trước → mang sang đơn bán | 1. Tạo đặt bàn và chọn trước một số món (bấm "+ Chọn món") 2. Bấm "Đặt bàn" thành công 3. Khi khách đến, mở đơn từ đặt bàn đó 4. Quan sát danh sách món trong đơn | Danh sách món đã chọn trước được mang đầy đủ sang đơn bán hàng |
6.11.6 | ☐ | Mã hóa đơn liên kết sau thanh toán | 1. Tạo đặt bàn, khách đến và thanh toán xong 2. Vào trang Tra cứu, tìm đặt bàn đó 3. Kiểm tra cột "Mã hóa đơn" | Mã hóa đơn xuất hiện và liên kết đúng với đơn thanh toán tương ứng |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
