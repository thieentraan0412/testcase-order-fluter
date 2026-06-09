# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

9. Xác nhận & lưu phiếu trả hàng

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 9.1 Bấm "Trả hàng" trong modal | 1. Điền đủ thông tin 2. Bấm "Trả hàng" | Hiển thị hộp xác nhận "Bạn có chắc muốn trả hàng?" |
| ☐ | 9.2 Hủy xác nhận | 1. Ở hộp xác nhận bấm "Đóng" | Đóng hộp xác nhận, giữ nguyên dữ liệu, chưa lưu |
| ☐ | 9.3 Xác nhận trả hàng | 1. Bấm "Xác nhận" | Tạo phiếu trả hàng thành công, hiển thị thông báo |
| ☐ | 9.4 Phiếu xuất hiện trong danh sách | 1. Sau khi trả hàng, quan sát bảng chính | Phiếu mới hiển thị với đầy đủ thông tin (mã, bàn, thời gian, khách, đã trả) |
| ☐ | 9.5 Trả hàng khi chưa chọn món nào | 1. Để số lượng trả = 0 toàn bộ 2. Bấm Trả hàng | Chặn/cảnh báo phải chọn ít nhất 1 món |
| ☐ | 9.6 Nút "Đóng" modal trả hàng | 1. Bấm "Đóng" | Đóng modal, không lưu, không tạo phiếu |
| ☐ | 9.7 Trả hàng cho hóa đơn đã trả 1 phần | 1. Chọn hóa đơn đã trả 1 phần trước đó | Chỉ cho trả phần còn lại, số lượng đúng |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
