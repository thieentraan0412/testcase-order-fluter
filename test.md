# Checklist Testcase — App F&B (NASYS POS)

> Nền tảng: Ordertable riêng. Đổi ☐ → ☑ khi pass, đánh **x** khi fail.

Link thực hiện: https://table1.klkim.com/v2/order/cashier

**Tài khoản**
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258
| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
| ☐ | Giảm giá (giảm giá trực tiếp theo %) | 1. Vào link cashier, chọn bàn, vào trang order món, thêm 5 món vào hóa đơn. 2. Click vào "Giảm giá". 3. Chọn "Giảm giá trực tiếp", click "Chọn" và chọn 1 chương trình cụ thể, nhập % rồi click "Xác nhận". 4. Click "Thanh toán" → click "Xác nhận". 5. Vào trang quản lý/lịch sử đơn hàng. 6. Kiểm tra hóa đơn sinh ra có đúng với hóa đơn lúc cashier thanh toán. | Số tiền thanh toán phải đúng. 


 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.

Sau khi hoàn thành toàn bộ testcase ở trên, hãy thay đổi kích thước trình duyệt và thực hiện lại toàn bộ testcase theo từng độ phân giải sau:

1. **Màn hình POS** — thay đổi kích thước màn hình sang 1366*768. Chạy lại toàn bộ testcase 1.1.1 → 1.1.20, 

 Sau khi hoàn tất, xuất file result_Pos_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_Pos_`tên file hiện tại`.md.