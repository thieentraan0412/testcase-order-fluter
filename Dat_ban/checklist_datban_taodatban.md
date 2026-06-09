## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

6.4 Tạo đặt bàn (modal "Đặt bàn")

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 6.4.1 | ☐ | Mở modal "Đặt bàn" | 1. Vào trang Đặt bàn 2. Bấm nút "+ Đặt bàn" (xanh đậm, góc trên phải) 3. Quan sát màn hình | Mở modal "Đặt bàn" với 2 phần: Thông tin khách hàng & Thông tin đặt bàn |
| 6.4.2 | ☐ | Bỏ trống cả Khách hàng và Bàn | 1. Mở modal "Đặt bàn" 2. Không điền Khách hàng và không chọn Bàn 3. Bấm nút "Đặt bàn" 4. Quan sát phản hồi | Hệ thống chặn, hiển thị thông báo lỗi: "Trường Khách hàng là bắt buộc. Trường Bàn là bắt buộc." |
| 6.4.3 | ☐ | Bỏ trống chỉ Khách hàng | 1. Mở modal "Đặt bàn" 2. Chọn Bàn nhưng để trống Khách hàng 3. Bấm "Đặt bàn" 4. Quan sát phản hồi | Hệ thống chặn, báo lỗi Khách hàng là bắt buộc |
| 6.4.4 | ☐ | Bỏ trống chỉ Bàn | 1. Mở modal "Đặt bàn" 2. Chọn Khách hàng nhưng không chọn Bàn 3. Bấm "Đặt bàn" 4. Quan sát phản hồi | Hệ thống chặn, báo lỗi Bàn là bắt buộc |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
