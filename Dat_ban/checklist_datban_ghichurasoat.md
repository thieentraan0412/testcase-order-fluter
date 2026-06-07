## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

6.12 Ghi chú rà soát

- **Trạng thái** trên lịch tuần chỉ lọc được 2 giá trị: **Chờ xác nhận** và **Đã hủy**.  
  Trang Tra cứu có đầy đủ 4 giá trị: **Chờ xác nhận, Đã xác nhận, Hủy tạm, Đã hủy** → cần kiểm thử riêng ở mỗi màn hình.
- **Bắt buộc** khi Đặt bàn: **Khách hàng** và **Bàn** (theo thông báo validation thực tế).
- **Phương thức đặt cọc** chỉ có 2: **Tiền mặt** và **Chuyển khoản**.
- **Khu vực bàn** có: khu 1, khu 2.
- **Nhân viên đặt bàn** gồm 4 loại: Thu ngân / Admin / Nhân viên / Quầy bếp.
- **Ghi chú** giới hạn **200 ký tự** (bộ đếm x/200).
- Trang Tra cứu có **16 cột** trong bảng, trong đó Lý do hủy, Người hủy, Ngày hủy chỉ có dữ liệu khi đặt bàn bị hủy.
- Nút "**Làm mới**" trên Tra cứu reset toàn bộ bộ lọc.

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
