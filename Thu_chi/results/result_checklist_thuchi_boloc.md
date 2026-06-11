
## 2. Thu chi — Kết quả kiểm thử

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense
Ngày chạy: 10-06-2026 | Chi nhánh: Chi nhánh Hồ Chí Minh

2.1 Bộ lọc

| STT | ✓ | Testcase | Kết quả thực tế |
|-----|---|----------|-----------------|
| 2.1.1 | ☑ | Tìm theo Mã phiếu | Nhập mã đúng (PT00001841CN2) → trả về đúng 1 phiếu. Nhập "xxxx999" → danh sách rỗng. Đúng như mong đợi. |
| 2.1.2 | ☑ | Lọc theo Chi nhánh | Chọn "Chi nhánh 3" → danh sách rỗng + tồn quỹ riêng của chi nhánh; chọn lại "Hồ Chí Minh" → hiện đúng phiếu. Bộ lọc chi nhánh hoạt động. |
| 2.1.3 | ☑ | Thời gian: Hôm nay / Hôm qua | "Hôm nay" → chỉ phiếu 10-06-2026; "Hôm qua" → chỉ phiếu 09-06-2026. Đúng. |
| 2.1.4 | ☑ | Thời gian: Tuần này / Tuần trước | "Tuần này" → khoảng 07-06 đến 10-06; "Tuần trước" → 31-05 đến 06-06. Phiếu nằm đúng khoảng. |
| 2.1.5 | ☑ | Thời gian: Tháng này / Tháng trước | "Tháng này" → 01-06 đến 10-06; "Tháng trước" → 01-05 đến 31-05. Đúng. |
| 2.1.6 | ☑ | Thời gian: tùy chọn ngày | Chọn tay Từ 01-05-2026 đến 05-06-2026 → danh sách chỉ hiện phiếu trong khoảng đã chọn. Đúng. |
| 2.1.7 | ☑ | Lọc theo Người tạo | Chọn "manager0001" → danh sách rỗng (người này không tạo phiếu nào trong kỳ). Bộ lọc người tạo hoạt động đúng. |
| 2.1.8 | ☑ | Lọc theo Loại thu chi (Thu / Chi) | "Phiếu thu" → chỉ phiếu Thu (Tổng chi = 0); "Phiếu chi" → chỉ phiếu Chi (Tổng thu = 0). Đúng. |
| 2.1.9 | ☑ | Lọc theo Phân loại thu chi | Chọn "Đơn bán hàng" → danh sách đổi đúng theo phân loại. Bộ lọc hoạt động. (Ghi chú: cột "Phân loại thu chi" hiển thị trống ở một số dòng.) |
| 2.1.10 | ☑ | Lọc theo Loại nguồn | Bán hàng → phiếu thu từ đơn bán; Tự tạo → 2 phiếu tạo tay (có nút sửa/xóa); Trả hàng → phiếu chi hoàn tiền; Mua hàng → rỗng. Mỗi nguồn ra đúng tập phiếu riêng. |
| 2.1.11 | ☑ | Kết hợp nhiều bộ lọc | Chi nhánh HCM + Loại "Thu" + "Tháng này" → danh sách chỉ phiếu thỏa cả 3 điều kiện; thẻ tổng quan (Tổng thu 5,165,936 / Tổng chi 0) cập nhật theo bộ lọc. |

Tổng: 11/11 PASS.
