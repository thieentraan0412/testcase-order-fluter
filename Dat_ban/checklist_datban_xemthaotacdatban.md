## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

Hãy sử dụng google chorme và thực hiện các testcase sau

6.8 Xem & thao tác đặt bàn trên lịch tuần

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 6.8.1 | ☐ | Bấm vào slot đặt bàn | 1. Vào trang Đặt bàn, quan sát lịch tuần 2. Tìm một slot đặt bàn đã có 3. Bấm vào slot đó 4. Quan sát màn hình mở ra | Mở modal chi tiết / chỉnh sửa đặt bàn đó |
| 6.8.2 | ☐ | Xem thông tin chi tiết đặt bàn | 1. Bấm vào một slot trên lịch để mở chi tiết 2. Kiểm tra từng thông tin hiển thị trong modal | Hiển thị đúng: tên KH, SĐT, bàn, khu vực, thời gian, số khách, tiền cọc, PTTT, ghi chú, trạng thái |
| 6.8.3 | ☐ | Xác nhận đặt bàn (Chờ xác nhận → Đã xác nhận) | 1. Bấm vào slot có trạng thái "Chờ xác nhận" 2. Tìm và bấm nút xác nhận đặt bàn trong modal 3. Quan sát trạng thái trên lịch | Trạng thái cập nhật thành "Đã xác nhận"; lịch phản ánh đúng |
| 6.8.4 | ☐ | Hủy đặt bàn | 1. Bấm vào một slot đặt bàn trên lịch 2. Tìm và bấm nút "Hủy" trong modal 3. Quan sát xem có yêu cầu nhập Lý do hủy không 4. Nhập lý do và xác nhận hủy | Yêu cầu nhập Lý do hủy; sau khi xác nhận trạng thái chuyển sang "Đã hủy" |
| 6.8.5 | ☐ | Chỉnh sửa thông tin đặt bàn | 1. Bấm vào một slot trên lịch để mở chi tiết 2. Chỉnh sửa một thông tin (VD: đổi số khách hoặc ghi chú) 3. Bấm "Lưu" 4. Mở lại chi tiết đặt bàn đó | Thông tin đã chỉnh sửa cập nhật đúng trên lịch và trong chi tiết |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
