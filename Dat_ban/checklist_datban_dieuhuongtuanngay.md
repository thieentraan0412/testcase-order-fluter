## 6. Đặt bàn (Order Booking)

> Trang: `/v2/order/cashier/order-booking` — Module **Đặt bàn**
> Gồm 2 màn hình: (1) **Lịch đặt bàn theo tuần** và (2) **Tra cứu lịch đặt bàn** (`/booking/table-reservation`)
> Hệ thống NASYS Order.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

6.1 Điều hướng tuần & ngày

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 6.1.1 | ☐ | Hiển thị 7 tab ngày trong tuần | 1. Đăng nhập vào hệ thống 2. Mở menu "Bàn đặt" → vào trang Đặt bàn 3. Quan sát dải tab ngày ở đầu trang | Hiển thị 7 tab ngày trong tuần hiện tại (Thứ Hai → Chủ Nhật), tab "Hôm nay" được highlight |
| 6.1.2 | ☐ | Bấm tab từng ngày chuyển lịch | 1. Vào trang Đặt bàn 2. Lần lượt bấm từng tab ngày (Thứ Hai, Thứ Ba, ...) 3. Quan sát vùng lịch sau mỗi lần bấm | Vùng lịch chuyển sang hiển thị các đặt bàn của ngày tương ứng |
| 6.1.3 | ☐ | Nút "Tuần trước" | 1. Vào trang Đặt bàn 2. Bấm nút "Tuần trước" 3. Quan sát dải tab ngày và dropdown Tuần | Dải tab cập nhật sang tuần trước; dropdown Tuần khớp khoảng ngày mới |
| 6.1.4 | ☐ | Nút "Tuần sau" | 1. Vào trang Đặt bàn 2. Bấm nút "Tuần sau" 3. Quan sát dải tab ngày | Dải tab cập nhật sang tuần tiếp theo |
| 6.1.5 | ☐ | Dropdown "Năm" chuyển đúng năm | 1. Vào trang Đặt bàn 2. Tìm và bấm dropdown "Năm" 3. Chọn một năm khác (VD: 2027) 4. Quan sát dropdown Tuần và dải tab | Dropdown Tuần và dải tab cập nhật theo năm đã chọn |
| 6.1.6 | ☐ | Dropdown "Tuần" nhảy đến tuần chọn | 1. Vào trang Đặt bàn 2. Bấm dropdown "Tuần" 3. Chọn một khoảng tuần cụ thể (VD: 08/06/2026 – 14/06/2026) 4. Quan sát dải tab ngày | Dải tab ngày nhảy đến đúng tuần đã chọn |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
