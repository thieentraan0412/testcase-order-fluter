## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

6.2 Bộ lọc lịch

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
6.2.1 | ☐ | Lọc theo khoảng giờ | 1. Vào trang Đặt bàn 2. Nhập giờ vào ô "Từ" (Thời gian) 3. Nhập giờ vào ô "Đến" 4. Quan sát lịch | Lịch chỉ hiện các đặt bàn trong khoảng giờ đã nhập |
6.2.2 | ☐ | Lọc theo Bàn | 1. Vào trang Đặt bàn 2. Bấm dropdown "Chọn bàn" 3. Gõ tên bàn vào ô Search 4. Chọn một bàn cụ thể 5. Quan sát lịch | Lịch chỉ hiện slot của bàn đã chọn |
6.2.3 | ☐ | Lọc trạng thái "Chờ xác nhận" | 1. Vào trang Đặt bàn 2. Bấm dropdown "Trạng thái" 3. Chọn "Chờ xác nhận" 4. Quan sát lịch | Chỉ hiện các đặt bàn đang ở trạng thái "Chờ xác nhận" |
6.2.4 | ☐ | Lọc trạng thái "Đã hủy" | 1. Vào trang Đặt bàn 2. Bấm dropdown "Trạng thái" 3. Chọn "Đã hủy" 4. Quan sát lịch | Chỉ hiện các đặt bàn đã hủy |
6.2.5 | ☐ | Lọc theo Tên khách | 1. Vào trang Đặt bàn 2. Nhập họ và tên khách vào ô tìm kiếm tên 3. Quan sát lịch | Chỉ hiện đặt bàn của khách khớp tên |
6.2.6 | ☐ | Lọc theo Số điện thoại | 1. Vào trang Đặt bàn 2. Nhập số điện thoại khách vào ô tìm kiếm SĐT 3. Quan sát lịch | Chỉ hiện đặt bàn của khách khớp số điện thoại |
6.2.7 | ☐ | Kết hợp nhiều bộ lọc | 1. Vào trang Đặt bàn 2. Bật đồng thời: chọn Bàn + Trạng thái + nhập Tên khách 3. Quan sát lịch | Kết quả hiển thị đúng giao của tất cả điều kiện đã lọc |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
