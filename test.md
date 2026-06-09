# Checklist Testcase — App F&B (NASYS POS)

> Nền tảng: Ordertable riêng. Đổi ☐ → ☑ khi pass, đánh **x** khi fail.

Link thực hiện: https://table1.klkim.com/v2/order/cashier

**Tài khoản**
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258
| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Giảm giá (giảm giá trực tiếp theo %) | 1. Vào link cashier, chọn bàn, vào trang order món, thêm 5 món vào hóa đơn. 2. Click vào "Giảm giá". 3. Chọn "Giảm giá trực tiếp", click "Chọn" và chọn 1 chương trình cụ thể, nhập % rồi click "Xác nhận". 4. Click "Thanh toán" → click "Xác nhận". 5. Vào trang quản lý/lịch sử đơn hàng. 6. Kiểm tra hóa đơn sinh ra có đúng với hóa đơn lúc cashier thanh toán. | Số tiền thanh toán phải đúng. 

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
