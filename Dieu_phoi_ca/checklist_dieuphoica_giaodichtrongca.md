
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

Hãy sử dụng google chorme và thực hiện các testcase sau

5.4 Giao dịch trong ca

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 5.4.1 | ☐ | Hiển thị danh sách giao dịch | 1. Mở chi tiết một ca 2. Tìm tab hoặc mục "Giao dịch" trong panel chi tiết 3. Quan sát danh sách giao dịch | Hiển thị đúng các cột: STT, mã chứng từ, loại, số tiền, phương thức, trạng thái |
| 5.4.2 | ☐ | Đếm đúng tổng số giao dịch | 1. Mở danh sách giao dịch của một ca 2. Đếm thủ công số dòng giao dịch hiển thị 3. So sánh với số tổng hiển thị trên giao diện | Số tổng giao dịch khớp với số dòng thực tế |
| 5.4.3 | ☐ | Lọc loại: Phiếu bán hàng | 1. Trong danh sách giao dịch, tìm dropdown hoặc tab lọc loại 2. Chọn "Phiếu bán hàng" 3. Quan sát kết quả lọc | Chỉ hiện các phiếu bán hàng |
| 5.4.4 | ☐ | Lọc loại: Phiếu trả hàng | 1. Trong danh sách giao dịch, bấm vào bộ lọc loại 2. Chọn "Phiếu trả hàng" 3. Quan sát kết quả lọc | Chỉ hiện các phiếu trả hàng |
| 5.4.5 | ☐ | Lọc loại: Phiếu thu | 1. Trong danh sách giao dịch, bấm vào bộ lọc loại 2. Chọn "Phiếu thu" 3. Quan sát kết quả lọc | Chỉ hiện các phiếu thu |
| 5.4.6 | ☐ | Lọc loại: Phiếu chi | 1. Trong danh sách giao dịch, bấm vào bộ lọc loại 2. Chọn "Phiếu chi" 3. Quan sát kết quả lọc | Chỉ hiện các phiếu chi |
| 5.4.7 | ☐ | Lọc loại: Tất cả | 1. Trong danh sách giao dịch, bấm vào bộ lọc loại 2. Chọn "Tất cả" 3. Quan sát kết quả lọc | Hiển thị mọi loại giao dịch |
| 5.4.8 | ☐ | Lọc trạng thái "Hoàn thành" | 1. Trong danh sách giao dịch, tìm bộ lọc trạng thái 2. Chọn "Hoàn thành" 3. Quan sát kết quả | Chỉ hiện các giao dịch đã hoàn thành |
| 5.4.9 | ☐ | Lọc trạng thái "Đã hủy" | 1. Trong danh sách giao dịch, tìm bộ lọc trạng thái 2. Chọn "Đã hủy" 3. Quan sát kết quả | Chỉ hiện các giao dịch đã hủy |
| 5.4.10 | ☐ | Tìm theo mã / chú thích | 1. Trong danh sách giao dịch, tìm ô tìm kiếm 2. Nhập mã chứng từ hoặc từ khóa trong chú thích 3. Quan sát kết quả tìm kiếm | Trả về đúng giao dịch khớp với từ khóa |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
