# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

11. Kiểm thử khác (UI/UX, phân quyền, hiệu năng)

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 11.1 Hiển thị responsive | 1. Thu nhỏ/phóng to cửa sổ trình duyệt | Layout không vỡ, các nút vẫn dùng được |
| ☐ | 11.2 Đa ngôn ngữ | 1. Đổi cờ ngôn ngữ (nếu có) | Nội dung trang đổi ngôn ngữ tương ứng |
| ☐ | 11.3 Tải lại trang giữ filter | 1. Áp dụng filter 2. F5 | Kiểm tra hành vi giữ/đặt lại filter hợp lý |
| ☐ | 11.4 Phân quyền tài khoản | 1. Đăng nhập tài khoản quyền thấp | Hiển thị/ẩn nút Trả hàng, Xuất Excel theo phân quyền |
| ☐ | 11.5 Mất kết nối khi trả hàng | 1. Ngắt mạng 2. Bấm Xác nhận trả hàng | Báo lỗi rõ ràng, không lưu sai dữ liệu |
| ☐ | 11.6 Bấm Trả hàng nhiều lần nhanh | 1. Bấm "Xác nhận" liên tục | Không tạo trùng nhiều phiếu (chống double submit) |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
