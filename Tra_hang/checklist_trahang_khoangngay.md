# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

4. Bộ lọc "Khoảng ngày"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 4.1 Mở popup khoảng ngày | 1. Bấm "Khoảng ngày" | Hiển thị: Hôm nay, Hôm qua, Tùy chọn, Từ ngày, Đến ngày, nút Đóng & Xác nhận |
| ☐ | 4.2 Chọn "Hôm nay" | 1. Chọn "Hôm nay" 2. Xác nhận | Lọc phiếu trả hàng trong ngày hôm nay |
| ☐ | 4.3 Chọn "Hôm qua" | 1. Chọn "Hôm qua" 2. Xác nhận | Lọc phiếu trả hàng của ngày hôm qua |
| ☐ | 4.4 Tùy chọn khoảng ngày | 1. Chọn "Tùy chọn" 2. Nhập Từ ngày, Đến ngày 3. Xác nhận | Lọc đúng phiếu trong khoảng đã chọn |
| ☐ | 4.5 Từ ngày > Đến ngày | 1. Nhập Từ ngày lớn hơn Đến ngày | Hiển thị cảnh báo / không cho áp dụng |
| ☐ | 4.6 Nút Đóng | 1. Mở popup 2. Bấm "Đóng" | Đóng popup, không thay đổi filter |
| ☐ | 4.7 Nút Xác nhận | 1. Chọn khoảng ngày 2. Bấm "Xác nhận" | Áp dụng filter, đóng popup |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
