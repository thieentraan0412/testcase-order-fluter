
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table.nasys.vn/v2/order/cashier/history

## 5. Điều phối ca
---

5.1 Lịch sử ca

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 5.1.1 | ☐ | Hiển thị danh sách các ca | 1. Đăng nhập vào hệ thống 2. Truy cập link cashier history 3. Quan sát danh sách các ca hiển thị trên màn hình | Danh sách hiển thị đúng: nhân viên, người mở, mã ca, giờ mở, giờ đóng, tổng tiền mặt |
| 5.1.2 | ☐ | Ca đang mở hiển thị đúng trạng thái | 1. Đăng nhập và vào trang lịch sử ca 2. Quan sát ca đang hoạt động (chưa đóng) trong danh sách 3. Kiểm tra cột giờ đóng của ca đó | Hiện trạng thái "Đang mở" thay vì giờ đóng |
| 5.1.3 | ☐ | Lọc theo Thời gian (khoảng ngày) | 1. Vào trang lịch sử ca 2. Bấm vào bộ lọc thời gian 3. Chọn khoảng ngày cụ thể (VD: từ 01/06 đến 05/06) 4. Bấm xác nhận/áp lọc 5. Quan sát danh sách kết quả | Chỉ hiện các ca nằm trong khoảng ngày đã chọn |
| 5.1.4 | ☐ | Lọc theo Nhân viên | 1. Vào trang lịch sử ca 2. Bấm vào bộ lọc nhân viên 3. Chọn một nhân viên cụ thể từ dropdown 4. Quan sát danh sách kết quả | Chỉ hiện các ca của nhân viên đã chọn |
| 5.1.5 | ☐ | Bấm vào 1 ca để xem chi tiết | 1. Vào trang lịch sử ca 2. Bấm vào một dòng ca bất kỳ trong danh sách 3. Quan sát panel bên phải màn hình | Hiện chi tiết của ca vừa chọn ở panel bên phải |
| 5.1.6 | ☐ | Nút "In phiếu" của ca | 1. Vào trang lịch sử ca, bấm vào một ca để hiện chi tiết 2. Tìm nút "In phiếu" ở panel chi tiết bên phải 3. Bấm nút "In phiếu" 4. Quan sát kết quả | Kích hoạt lệnh in phiếu kết ca |
| 5.1.7 | ☐ | Nút "Chi tiết ca" | 1. Vào trang lịch sử ca, bấm vào một ca để hiện chi tiết 2. Tìm và bấm nút "Chi tiết ca" ở panel bên phải 3. Quan sát màn hình | Mở modal chi tiết ca |
| 5.1.8 | ☐ | Nút "Mở màn hình phụ" | 1. Vào trang lịch sử ca, bấm vào ca đang mở để hiện chi tiết 2. Tìm và bấm nút "Mở màn hình phụ" ở panel bên phải 3. Quan sát kết quả | Mở màn hình phụ của ca đang mở |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
