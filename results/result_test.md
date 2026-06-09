# Kết quả Test — result_test.md

- **File nguồn:** test.md
- **Ngày thực hiện:** 09-06-2026
- **Trình duyệt:** Google Chrome (Browser 1) — tài khoản đăng nhập sẵn **Admin Master**
- **Hệ thống:** NASYS POS — https://table1.klkim.com/v2/order/cashier
- **Cửa hàng thao tác:** CN1

## Tổng quan

| Chỉ số | Số lượng |
|--------|----------|
| Tổng testcase | 1 |
| Pass ☑ | 1 |
| Fail x | 0 |

## Chi tiết

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi | Kết quả thực tế |
|---|----------|--------------------|------------------|-----------------|
| ☑ | Giảm giá (giảm giá trực tiếp theo %) | 1. Vào link cashier, chọn bàn (ban8), vào trang order món, thêm 5 món. 2. Click "Giảm giá". 3. Chọn "Giảm giá trực tiếp", chọn chương trình "giám giá hằng tuần", nhập 10%, "Xác nhận". 4. Click "Thanh toán" → "Xác nhận". 5. Vào Lịch sử đơn hàng. 6. Đối chiếu hóa đơn sinh ra với hóa đơn lúc cashier thanh toán. | Số tiền thanh toán phải đúng. | **PASS** — Số tiền khớp 100% giữa cashier và lịch sử đơn hàng. |

## Dữ liệu kiểm chứng

- **Mã đơn:** POS00002356CN2 — Bàn: ban8 — Hình thức: Tiền mặt — Trạng thái: **Đã thanh toán** — Thời gian: 09-06-2026 16:54
- **5 món:** tran chau (10.000đ), cf sua new (30.000đ), Test Kho 8 (500.000đ), Test Kho 7 (500.000đ), Test Kho 5 (500.000đ)

| Khoản mục | Giá trị |
|-----------|---------|
| Tổng tiền hàng | 1.540.000đ |
| Phụ thu | 0đ |
| Giảm giá (10%) | 154.000đ |
| Tích điểm | 0 |
| VAT | 135.450đ |
| **Tổng tiền thanh toán** | **1.521.450đ** |
| Tiền mặt | 1.521.450đ |

**Công thức:** 1.540.000 − 154.000 = 1.386.000; 1.386.000 + 135.450 (VAT) = **1.521.450đ**.
Số tiền tại màn hình cashier (1.521.450đ) **trùng khớp** với hóa đơn POS00002356CN2 trong Lịch sử đơn hàng → **PASS**.

## Ghi chú kỹ thuật

- Trong "Giảm giá trực tiếp", ô nhập % bị khóa cho đến khi chọn một chương trình ở dropdown "Chọn".
- Nhóm món "Test Kho", "tran chau", "cf sua new" thêm trực tiếp; một số món khác (Trà A Hỷ, Cơm...) có hộp thoại "Chọn món kèm theo" (Size/Ngọt/Đá) cần xác nhận trước khi thêm.
