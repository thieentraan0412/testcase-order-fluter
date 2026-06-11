
Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/shift

## 5. Điều phối ca
---

5.4 Giao dịch trong ca — Kết quả thực thi (ngày chạy: 10-06-2026)

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi | Kết quả thực tế |
|-----|---|----------|--------------------|------------------|-----------------|
| 5.4.1 | ☑ | Hiển thị danh sách giao dịch | 1. Mở chi tiết ca 2. Mục "Giao dịch" 3. Quan sát | Đúng các cột: STT, mã chứng từ, loại, số tiền, phương thức, trạng thái | PASS — đủ 6 cột |
| 5.4.2 | ☑ | Đếm đúng tổng số giao dịch | 1. Mở danh sách 2. Đếm dòng 3. So sánh số tổng | Số tổng khớp số dòng thực tế | PASS — "Tổng giao dịch: 36" khớp; sau test tăng lên 42 đúng số phiếu phát sinh |
| 5.4.3 | ☑ | Lọc loại: Phiếu bán hàng | 1. Dropdown loại 2. Chọn "Phiếu bán hàng" | Chỉ hiện phiếu bán hàng | PASS |
| 5.4.4 | ☑ | Lọc loại: Phiếu trả hàng | 1. Dropdown loại 2. Chọn "Phiếu trả hàng" | Chỉ hiện phiếu trả hàng | PASS — rỗng khi chưa có trả hàng; hiện HT000038 sau khi tạo |
| 5.4.5 | ☑ | Lọc loại: Phiếu thu | 1. Dropdown loại 2. Chọn "Phiếu thu" | Chỉ hiện phiếu thu | PASS |
| 5.4.6 | ☑ | Lọc loại: Phiếu chi | 1. Dropdown loại 2. Chọn "Phiếu chi" | Chỉ hiện phiếu chi | PASS |
| 5.4.7 | ☑ | Lọc loại: Tất cả | 1. Dropdown loại 2. Chọn "Tất cả" | Hiển thị mọi loại giao dịch | PASS |
| 5.4.8 | ☑ | Lọc trạng thái "Hoàn thành" | 1. Bộ lọc trạng thái 2. Chọn "Hoàn thành" | Chỉ hiện giao dịch hoàn thành | PASS — 36 giao dịch đều "Đã thanh toán" |
| 5.4.9 | ☑ | Lọc trạng thái "Đã hủy" | 1. Bộ lọc trạng thái 2. Chọn "Đã hủy" | Chỉ hiện giao dịch đã hủy | PASS — ca sạch không có giao dịch hủy (rỗng); ca SCR57 lọc "Đã hủy" hiện đúng 288 giao dịch hủy |
| 5.4.10 | ☑ | Tìm theo mã / chú thích | 1. Ô tìm kiếm 2. Nhập mã/từ khóa 3. Quan sát | Trả về đúng giao dịch khớp | PASS — tìm "PT00001835" → đúng 1 dòng |

Tổng: 10/10 PASS
