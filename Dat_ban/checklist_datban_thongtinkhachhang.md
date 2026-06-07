## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

6.5 Thông tin khách hàng

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 6.5.1 | ☐ | Tìm và chọn khách hàng có sẵn | 1. Mở modal "Đặt bàn" 2. Bấm dropdown "Khách hàng" 3. Gõ tên hoặc SĐT khách để tìm 4. Chọn một khách từ danh sách 5. Quan sát thông tin hiện ra | Khách hàng được chọn, hiển thị tên và điểm tích lũy / hạng thành viên |
| 6.5.2 | ☐ | Bấm "+ Thêm mới" mở modal khách | 1. Mở modal "Đặt bàn" 2. Tại phần Khách hàng, bấm nút "+ Thêm mới" (xanh dương) 3. Quan sát màn hình | Mở modal "Thêm / Chỉnh sửa" khách hàng mới |
| 6.5.3 | ☐ | Chọn Nhân viên đặt bàn | 1. Mở modal "Đặt bàn" 2. Tìm dropdown "Nhân viên đặt bàn" 3. Bấm dropdown phần loại, chọn loại (VD: Thu ngân) 4. Chọn tên nhân viên từ danh sách 5. Quan sát giá trị được ghi nhận | Ghi nhận đúng loại và tên nhân viên đặt bàn |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
