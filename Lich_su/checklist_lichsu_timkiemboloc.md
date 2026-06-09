Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table.nasys.vn/v2/order/cashier/history

4. Lịch sử
---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

4.2 Tìm kiếm & bộ lọc

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 4.2.1 | ☐ | Tìm theo mã đơn | 1. Vào trang lịch sử 2. Tìm ô tìm kiếm trên thanh bộ lọc 3. Nhập đúng mã đơn có sẵn (VD: DH-00123) 4. Quan sát kết quả | Trả về đúng đơn có mã tương ứng |
| 4.2.2 | ☐ | Tìm theo số điện thoại | 1. Vào trang lịch sử 2. Nhập số điện thoại khách hàng vào ô tìm kiếm 3. Quan sát kết quả | Trả về các đơn của khách hàng có số điện thoại đó |
| 4.2.3 | ☐ | Tìm không khớp | 1. Vào trang lịch sử 2. Nhập chuỗi bất kỳ không tồn tại (VD: "xxxx9999") vào ô tìm kiếm 3. Quan sát danh sách | Danh sách rỗng, không hiện đơn nào |
| 4.2.4 | ☐ | Trạng thái: Đã thanh toán thành công | 1. Vào trang lịch sử 2. Tìm dropdown lọc trạng thái 3. Chọn "Đã thanh toán thành công" 4. Quan sát danh sách | Chỉ hiện các đơn đã thanh toán thành công |
| 4.2.5 | ☐ | Trạng thái: Chưa thanh toán | 1. Vào trang lịch sử 2. Bấm dropdown trạng thái 3. Chọn "Chưa thanh toán" 4. Quan sát danh sách | Chỉ hiện các đơn chưa thanh toán |
| 4.2.6 | ☐ | Trạng thái: Đã hủy | 1. Vào trang lịch sử 2. Bấm dropdown trạng thái 3. Chọn "Đã hủy" 4. Quan sát danh sách | Chỉ hiện các đơn đã bị hủy |
| 4.2.7 | ☐ | Trạng thái: Đã xử lý trả hàng | 1. Vào trang lịch sử 2. Bấm dropdown trạng thái 3. Chọn "Đã xử lý trả hàng" 4. Quan sát danh sách | Chỉ hiện các đơn đã xử lý trả hàng |
| 4.2.8 | ☐ | Trạng thái: Công nợ | 1. Vào trang lịch sử 2. Bấm dropdown trạng thái 3. Chọn "Công nợ" 4. Quan sát danh sách | Chỉ hiện các đơn đang ở trạng thái công nợ |
| 4.2.9 | ☐ | Lọc theo Tài khoản (nhân viên) | 1. Vào trang lịch sử 2. Tìm dropdown "Tài khoản" hoặc "Nhân viên" 3. Chọn một nhân viên cụ thể 4. Quan sát danh sách | Chỉ hiện các đơn do nhân viên đó tạo |
| 4.2.10 | ☐ | Khoảng ngày: Hôm nay | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian 3. Chọn "Hôm nay" 4. Quan sát danh sách | Chỉ hiện đơn được tạo trong ngày hôm nay |
| 4.2.11 | ☐ | Khoảng ngày: Hôm qua | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian 3. Chọn "Hôm qua" 4. Quan sát danh sách | Chỉ hiện đơn được tạo ngày hôm qua |
| 4.2.12 | ☐ | Khoảng ngày: Tuần này | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian 3. Chọn "Tuần này" 4. Quan sát danh sách | Chỉ hiện đơn trong tuần hiện tại |
| 4.2.13 | ☐ | Khoảng ngày: Tháng này | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian 3. Chọn "Tháng này" 4. Quan sát danh sách | Chỉ hiện đơn trong tháng hiện tại |
| 4.2.14 | ☐ | Khoảng ngày: Tùy chọn | 1. Vào trang lịch sử 2. Bấm bộ lọc thời gian, chọn "Tùy chọn" 3. Nhập ngày bắt đầu và ngày kết thúc cụ thể 4. Xác nhận và quan sát danh sách | Chỉ hiện đơn trong khoảng ngày đã nhập |
| 4.2.15 | ☐ | Kết hợp nhiều bộ lọc | 1. Vào trang lịch sử 2. Bật đồng thời: tab "Tại bàn" + Trạng thái "Đã thanh toán" + Thời gian "Hôm nay" 3. Quan sát danh sách kết quả | Chỉ hiện đơn thỏa tất cả điều kiện đã chọn |
| 4.2.16 | ☐ | Ngày bắt đầu > ngày kết thúc | 1. Vào trang lịch sử, bật lọc thời gian tùy chọn 2. Nhập ngày bắt đầu lớn hơn ngày kết thúc (VD: từ 10/06 đến 01/06) 3. Xác nhận và quan sát phản hồi | Hệ thống chặn hoặc hiển thị thông báo lỗi, không trả kết quả sai |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
