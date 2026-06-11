# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau

5. Nút "Xuất Excel"

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 5.1 Xuất Excel danh sách | 1. Bấm "Xuất Excel" | Tải về file Excel chứa danh sách phiếu trả hàng |
| ☐ | 5.2 Xuất Excel có filter | 1. Áp dụng filter 2. Bấm "Xuất Excel" | File Excel chỉ chứa dữ liệu khớp filter |
| ☐ | 5.3 Xuất Excel danh sách rỗng | 1. Lọc ra danh sách rỗng 2. Bấm "Xuất Excel" | Xử lý hợp lý (file rỗng hoặc thông báo) |
| ☐ | 5.4 Nội dung file đúng | 1. Mở file đã tải | Cột & dữ liệu khớp với bảng trên màn hình |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
