Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table.nasys.vn/v2/order/cashier/history

4. Lịch sử
---

4.1 Bộ lọc loại đơn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
4.1.1 | ☐ | Lọc tab "Tất cả" | 1. Đăng nhập, truy cập link cashier history 2. Quan sát các tab lọc loại đơn phía trên danh sách 3. Bấm tab "Tất cả" 4. Quan sát danh sách đơn | Hiển thị tất cả đơn không phân biệt loại |
4.1.2 | ☐ | Lọc tab "Tại bàn" | 1. Vào trang lịch sử 2. Bấm tab "Tại bàn" 3. Quan sát từng đơn trong danh sách | Chỉ hiện các đơn loại tại bàn |
4.1.3 | ☐ | Lọc tab "Mang về" | 1. Vào trang lịch sử 2. Bấm tab "Mang về" 3. Quan sát danh sách | Chỉ hiện các đơn mang về |
4.1.4 | ☐ | Lọc tab "Đặt online" | 1. Vào trang lịch sử 2. Bấm tab "Đặt online" 3. Quan sát danh sách | Chỉ hiện đơn đặt online; nếu không có đơn nào thì danh sách rỗng |
4.1.5 | ☐ | Dropdown "Chọn bàn" | 1. Vào trang lịch sử 2. Tìm dropdown "Chọn bàn" trên thanh bộ lọc 3. Bấm dropdown, chọn một bàn cụ thể (VD: Bàn 1) 4. Quan sát danh sách đơn | Chỉ hiện các đơn thuộc bàn đã chọn |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
