# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

6. Nút "Trả hàng" → Modal "Danh sách hóa đơn"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 6.1 Mở modal danh sách hóa đơn | 1. Bấm nút "Trả hàng" (đỏ) | Mở modal "Danh sách hóa đơn" với bộ lọc và bảng hóa đơn |
| ☐ | 6.2 Hiển thị cột bảng hóa đơn | 1. Quan sát modal | Có cột: STT, Mã hóa đơn, Ngày tạo, Khách hàng, Bàn, Nhân viên, Tổng tiền + nút "Chọn" |
| ☐ | 6.3 Lọc theo "Đơn hàng" | 1. Nhập mã đơn vào ô "Đơn hàng" | Bảng lọc đúng hóa đơn |
| ☐ | 6.4 Lọc theo Từ ngày/Đến ngày | 1. Đổi Từ ngày, Đến ngày | Danh sách hóa đơn cập nhật theo khoảng ngày |
| ☐ | 6.5 Mặc định khoảng ngày | 1. Quan sát giá trị mặc định | Hiển thị khoảng ngày mặc định hợp lý (VD: tuần hiện tại) |
| ☐ | 6.6 Đóng modal bằng (×) | 1. Bấm dấu (×) góc phải | Modal đóng, về trang chính |
| ☐ | 6.7 Đóng modal bằng "Đóng" | 1. Bấm nút "Đóng" | Modal đóng |
| ☐ | 6.8 Bấm "Chọn" hóa đơn | 1. Bấm "Chọn" ở 1 hóa đơn | Mở modal "Thông tin trả hàng" của hóa đơn đó |
| ☐ | 6.9 Danh sách hóa đơn rỗng | 1. Lọc khoảng ngày không có hóa đơn | Bảng trống, không lỗi |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
