
## 2. Thu chi — Kết quả kiểm thử

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense
Ngày chạy: 10-06-2026 | Chi nhánh: Chi nhánh Hồ Chí Minh

2.2 Tổng quan quỹ

| STT | ✓ | Testcase | Kết quả thực tế |
|-----|---|----------|-----------------|
| 2.2.1 | ☑ | Hiển thị Tồn quỹ đầu kỳ | Thẻ "Tồn quỹ đầu kỳ" hiển thị số dư theo kỳ đã lọc (VD lọc "Hôm nay" hiển thị ~55,065 tỷ). Ghi chú: số đầu kỳ ở chế độ tổng hiển thị làm tròn "~ ... tỷ"; giá trị chính xác đến đồng xem được khi lọc theo loại/nguồn. |
| 2.2.2 | ☑ | Hiển thị Tổng thu | Lọc "Hôm nay": 2 phiếu Thu = 15,000 + 10,000 = 25,000. Thẻ "Tổng thu" = 25,000. Khớp. |
| 2.2.3 | ☑ | Hiển thị Tổng chi | Lọc "Hôm nay": 2 phiếu Chi = 15,000 + 5,000 = 20,000. Thẻ "Tổng chi" = 20,000. Khớp. |
| 2.2.4 | ☑ | Tồn quỹ cuối kỳ tính đúng | Công thức Cuối kỳ = Đầu kỳ + Tổng thu − Tổng chi được xác minh chính xác đến đồng qua các view lọc: VD (lọc Tự tạo) Đầu −64,949,998 + Thu 10,000 − Chi 5,000 = Cuối −64,944,998 ✓; (lọc Trả hàng) −13,369,464 − 15,000 = −13,384,464 ✓. |
| 2.2.5 | ☑ | Đổi bộ lọc thời gian → thẻ cập nhật | Đổi "Hôm nay" (Thu 25,000 / Chi 20,000) sang "Hôm qua" (Thu 459,000 / Chi 0) → cả 4 thẻ cập nhật theo kỳ mới. |

Tổng: 5/5 PASS.

Ghi chú chung: Giá trị "Tồn quỹ đầu/cuối kỳ" ở chế độ tổng rất lớn (~55,065 tỷ) và hiển thị làm tròn nên thay đổi nhỏ (vài nghìn đồng) không nhìn thấy trên thẻ; tuy nhiên quan hệ Cuối = Đầu + Thu − Chi đã được kiểm chứng đúng chính xác trên các view lọc.
