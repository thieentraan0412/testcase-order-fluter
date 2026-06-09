# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

1. Tải trang & bố cục chung

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 1.1 Hiển thị trang Trả hàng | 1. Đăng nhập 2. Vào menu "Trả hàng" | Trang tải thành công, tab "Trả hàng" được highlight, hiển thị thanh filter + bảng danh sách phiếu |
| ☐ | 1.2 Hiển thị thanh công cụ lọc | 1. Quan sát phía trên bảng | Hiển thị đủ: ô tìm kiếm, dropdown "Chọn khu vực bàn", dropdown "Chọn bàn", nút "Khoảng ngày", nút "Trả hàng" (đỏ), nút "Xuất Excel" |
| ☐ | 1.3 Hiển thị tiêu đề bảng | 1. Quan sát bảng danh sách | Có đủ cột: STT, Bàn, Mã phiếu trả hàng, Thời gian trả hàng, Khách hàng, Đã trả, Hành động |
| ☐ | 1.4 Danh sách rỗng | 1. Khi chưa có phiếu trả hàng phù hợp | Bảng hiển thị trống, không lỗi |
| ☐ | 1.5 Điều hướng menu khác | 1. Bấm các menu Trang chủ/Lịch sử/CRM... | Chuyển đúng trang tương ứng |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
