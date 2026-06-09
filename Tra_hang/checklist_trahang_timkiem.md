# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

2. Ô tìm kiếm "Mã phiếu trả hàng | Khách hàng"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 2.1 Tìm theo mã phiếu | 1. Nhập mã phiếu trả hàng hợp lệ 2. Quan sát | Bảng lọc đúng phiếu theo mã |
| ☐ | 2.2 Tìm theo tên khách hàng | 1. Nhập tên khách hàng | Bảng lọc đúng phiếu theo khách hàng |
| ☐ | 2.3 Tìm không có kết quả | 1. Nhập chuỗi không tồn tại | Bảng trả về rỗng, không lỗi |
| ☐ | 2.4 Tìm chuỗi rỗng | 1. Xóa hết nội dung ô tìm kiếm | Hiển thị lại toàn bộ danh sách |
| ☐ | 2.5 Tìm ký tự đặc biệt/khoảng trắng | 1. Nhập ký tự đặc biệt, dấu cách | Không lỗi, xử lý hợp lý |
| ☐ | 2.6 Phân biệt hoa/thường | 1. Nhập tên dạng chữ hoa & chữ thường | Kết quả tìm kiếm nhất quán |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
