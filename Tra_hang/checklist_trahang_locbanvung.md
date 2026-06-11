# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau

3. Lọc theo Khu vực bàn & Bàn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 3.1 Mở dropdown khu vực | 1. Bấm "Chọn khu vực bàn" | Hiển thị danh sách khu vực + ô search |
| ☐ | 3.2 Chọn 1 khu vực | 1. Chọn 1 khu vực (VD: Khu 1) | Khu vực được chọn hiển thị dạng tag có dấu (×) |
| ☐ | 3.3 Search khu vực | 1. Gõ tên khu vào ô search dropdown | Lọc đúng khu vực theo từ khóa |
| ☐ | 3.4 Bỏ chọn khu vực | 1. Bấm dấu (×) trên tag khu vực đã chọn | Khu vực bị bỏ chọn, filter reset |
| ☐ | 3.5 Mở dropdown bàn | 1. Bấm "Chọn bàn" | Hiển thị danh sách bàn + ô search |
| ☐ | 3.6 Chọn 1 bàn | 1. Chọn 1 bàn cụ thể | Bàn được chọn, danh sách lọc theo bàn |
| ☐ | 3.7 Liên kết khu vực ↔ bàn | 1. Chọn khu vực rồi mở dropdown bàn | Danh sách bàn phù hợp/cập nhật theo khu vực (nếu áp dụng) |
| ☐ | 3.8 Search bàn | 1. Gõ tên bàn vào ô search | Lọc đúng bàn theo từ khóa |
| ☐ | 3.9 Kết hợp nhiều filter | 1. Áp dụng đồng thời search + khu vực + bàn + ngày | Kết quả khớp tất cả điều kiện |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
