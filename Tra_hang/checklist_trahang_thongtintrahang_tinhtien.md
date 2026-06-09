# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

8. Modal "Thông tin trả hàng" — Tính tiền & trường nhập

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 8.1 Cột "Tổng giá trị đơn hàng" | 1. Quan sát cột trái | Hiển thị read-only: Tổng tiền hàng, VAT, Phụ thu, Giảm giá, Tích điểm, Tổng tiền thanh toán |
| ☐ | 8.2 Cột "Số tiền trả hàng" | 1. Quan sát cột phải | Hiển thị: Tổng tiền hàng, VAT, Phụ thu, Giảm giá, Tích điểm, Tổng tiền trả lại |
| ☐ | 8.3 Tự động tính tiền trả | 1. Thay đổi số lượng trả | Tổng tiền hàng/VAT/Tổng tiền trả lại cập nhật tự động đúng |
| ☐ | 8.4 Sửa Phụ thu (trả) | 1. Nhập giá trị "Phụ thu" cột trả | Tổng tiền trả lại tính lại đúng |
| ☐ | 8.5 Sửa Giảm giá (trả) | 1. Nhập giá trị "Giảm giá" cột trả | Tổng tiền trả lại trừ đúng giảm giá |
| ☐ | 8.6 Sửa Tích điểm (trả) | 1. Nhập giá trị "Tích điểm" cột trả | Cập nhật đúng theo logic tích điểm |
| ☐ | 8.7 Nhập giá trị âm/ký tự lạ vào các ô tiền | 1. Nhập số âm, chữ | Chặn/cảnh báo, không phá vỡ phép tính |
| ☐ | 8.8 Giảm giá vượt tổng tiền | 1. Nhập Giảm giá > tổng tiền trả | Chặn/cảnh báo, không cho âm tiền trả |
| ☐ | 8.9 Phương thức thanh toán | 1. Mở dropdown "Phương thức thanh toán" | Chọn được phương thức (Tiền mặt, …) |
| ☐ | 8.10 Tên khách hàng (bắt buộc) | 1. Để trống "Tên khách hàng*" 2. Bấm Trả hàng | Báo lỗi yêu cầu nhập tên khách hàng |
| ☐ | 8.11 Số điện thoại | 1. Nhập SĐT hợp lệ / sai định dạng | Hợp lệ thì nhận; sai định dạng thì cảnh báo (nếu có validate) |
| ☐ | 8.12 Lý do trả hàng (bắt buộc) | 1. Để trống "Lý do trả hàng*" 2. Bấm Trả hàng | Báo lỗi yêu cầu nhập lý do |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
