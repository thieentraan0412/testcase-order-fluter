
## 2. Thu chi

Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense

---

2.1 Bộ lọc

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
2.1.1 | ☐ | Tìm theo Mã phiếu | 1. Đăng nhập, vào trang Thu chi 2. Tìm ô tìm kiếm "Mã phiếu" trên thanh bộ lọc 3. Nhập đúng mã phiếu có sẵn (VD: vote-00001) → quan sát kết quả 4. Xóa ô tìm kiếm, nhập chuỗi không tồn tại (VD: "xxxx999") → quan sát lại | Nhập mã đúng: trả về đúng phiếu. Nhập không khớp: danh sách rỗng |
2.1.2 | ☐ | Lọc theo Chi nhánh | 1. Vào trang Thu chi 2. Tìm dropdown "Chi nhánh" trên thanh bộ lọc 3. Bấm dropdown, chọn một chi nhánh cụ thể (VD: CN1) 4. Quan sát danh sách phiếu sau khi lọc | Chỉ hiện phiếu thuộc chi nhánh đã chọn |
2.1.3 | ☐ | Thời gian: Hôm nay / Hôm qua | 1. Vào trang Thu chi 2. Tìm bộ lọc thời gian 3. Chọn lần lượt "Hôm nay" → quan sát danh sách 4. Chọn "Hôm qua" → quan sát lại | Chỉ hiện phiếu trong ngày hôm nay / hôm qua tương ứng |
2.1.4 | ☐ | Thời gian: Tuần này / Tuần trước | 1. Vào trang Thu chi 2. Bấm bộ lọc thời gian 3. Chọn "Tuần này" → quan sát danh sách 4. Chọn "Tuần trước" → quan sát lại | Chỉ hiện phiếu trong khoảng tuần tương ứng |
2.1.5 | ☐ | Thời gian: Tháng này / Tháng trước | 1. Vào trang Thu chi 2. Bấm bộ lọc thời gian 3. Chọn "Tháng này" → quan sát danh sách 4. Chọn "Tháng trước" → quan sát lại | Chỉ hiện phiếu trong khoảng tháng tương ứng |
2.1.6 | ☐ | Thời gian: tùy chọn ngày | 1. Vào trang Thu chi 2. Bấm bộ lọc thời gian, chọn "Tùy chọn" hoặc "Khoảng ngày" 3. Nhập ngày bắt đầu và ngày kết thúc cụ thể 4. Xác nhận và quan sát danh sách | Chỉ hiện phiếu trong khoảng ngày đã nhập |
2.1.7 | ☐ | Lọc theo Người tạo | 1. Vào trang Thu chi 2. Tìm dropdown "Người tạo" trên thanh bộ lọc 3. Bấm dropdown, chọn một người dùng cụ thể 4. Quan sát danh sách phiếu | Chỉ hiện phiếu do người đã chọn tạo ra |
2.1.8 | ☐ | Lọc theo Loại thu chi (Thu / Chi) | 1. Vào trang Thu chi 2. Tìm dropdown "Loại thu chi" 3. Chọn "Thu" → quan sát danh sách 4. Đổi sang chọn "Chi" → quan sát lại | Chọn "Thu": chỉ hiện phiếu thu. Chọn "Chi": chỉ hiện phiếu chi |
2.1.9 | ☐ | Lọc theo Phân loại thu chi | 1. Vào trang Thu chi 2. Tìm dropdown "Phân loại thu chi" 3. Bấm dropdown, chọn một phân loại cụ thể 4. Quan sát danh sách phiếu | Chỉ hiện phiếu thuộc đúng phân loại đã chọn |
2.1.10 | ☐ | Lọc theo Loại nguồn | 1. Vào trang Thu chi 2. Tìm dropdown "Loại nguồn" 3. Lần lượt chọn từng giá trị: Bán hàng / Mua hàng / Tự tạo / Trả hàng 4. Quan sát danh sách sau mỗi lần chọn | Mỗi lần chọn chỉ hiện phiếu đúng nguồn tương ứng |
2.1.11 | ☐ | Kết hợp nhiều bộ lọc | 1. Vào trang Thu chi 2. Bật đồng thời nhiều bộ lọc: chọn Chi nhánh + Loại thu chi "Thu" + Thời gian "Tháng này" 3. Quan sát danh sách và các thẻ tổng quan bên trên | Danh sách chỉ hiện phiếu thỏa tất cả điều kiện; thẻ tổng quan cập nhật theo bộ lọc |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
