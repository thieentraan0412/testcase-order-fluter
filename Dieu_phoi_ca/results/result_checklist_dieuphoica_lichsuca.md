
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

5.1 Lịch sử ca — Kết quả thực thi (ngày chạy: 10-06-2026)

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi | Kết quả thực tế |
|-----|---|----------|--------------------|------------------|-----------------|
| 5.1.1 | ☑ | Hiển thị danh sách các ca | 1. Đăng nhập 2. Vào cashier history 3. Quan sát danh sách | Danh sách hiển thị đúng: nhân viên, người mở, mã ca, giờ mở, giờ đóng, tổng tiền mặt | PASS — card ca SCR00000057CN2 hiển thị đủ NV/người mở/mã ca/giờ mở/giờ đóng/tổng tiền mặt |
| 5.1.2 | ☑ | Ca đang mở hiển thị đúng trạng thái | 1. Vào trang lịch sử ca 2. Quan sát ca chưa đóng 3. Kiểm tra cột giờ đóng | Hiện "Đang mở" thay vì giờ đóng | PASS — ca SCR58 hiển thị "Giờ đóng ca: Đang mở" + badge "Đang mở" |
| 5.1.3 | ☑ | Lọc theo Thời gian (khoảng ngày) | 1. Bộ lọc thời gian 2. Chọn 01/06–05/06 3. Áp lọc 4. Quan sát | Chỉ hiện các ca trong khoảng ngày | PASS — lọc 01/06–05/06 chỉ hiện ca đóng trong khoảng |
| 5.1.4 | ☑ | Lọc theo Nhân viên | 1. Bộ lọc nhân viên 2. Chọn 1 NV 3. Quan sát | Chỉ hiện ca của NV đã chọn | PASS — chọn "manager0001" → danh sách rỗng; chọn "Admin master" → hiện ca |
| 5.1.5 | ☑ | Bấm vào 1 ca để xem chi tiết | 1. Bấm 1 dòng ca 2. Quan sát panel bên phải | Hiện chi tiết ca ở panel phải | PASS — bấm SCR57 → panel phải hiển thị chi tiết ca đó |
| 5.1.6 | ☑ | Nút "In phiếu" của ca | 1. Bấm vào ca 2. Bấm "In phiếu" 3. Quan sát | Kích hoạt lệnh in phiếu kết ca | PASS — toast "Gửi in thành công" |
| 5.1.7 | ☑ | Nút "Chi tiết ca" | 1. Bấm vào ca 2. Bấm "Chi tiết ca" 3. Quan sát | Mở modal chi tiết ca | PASS — modal "Chi tiết ca" mở đúng |
| 5.1.8 | ☑ | Nút "Mở màn hình phụ" | 1. Bấm ca đang mở 2. Bấm "Mở màn hình phụ" | Mở màn hình phụ của ca đang mở | PASS — mở tab mới /secondary-screen?shift_id=58 |

Tổng: 8/8 PASS
