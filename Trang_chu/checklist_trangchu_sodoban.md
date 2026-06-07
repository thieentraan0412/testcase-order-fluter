# Checklist Testcase — App F&B (NASYS POS)

> Nền tảng: Ordertable riêng. Xây dựng dần qua từng video. Đổi ☐ → ☑ khi xong.

Link login https://table1.klkim.com/login
tài khoản
    Cửa hàng : trong
    Tài khoản: admin
    Mật khẩu : 147258

Link cashier https://table1.klkim.com/v2/order/cashier
Link manager https://table1.klkim.com/v2/dashboard
Sau khi truy cập link: Click vào bàn    
---
1.1 Sơ đồ bàn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
1.1.1 | ☐ | Hiển thị danh sách bàn theo khu | 1. Mở app, đăng nhập thành công 2. Vào "Trang chủ" 3. Quan sát khu vực sơ đồ bàn | Hiện đủ các bàn, đúng số lượng theo khu |
1.1.2 | ☐ | Lọc tab "Bàn trống" | 1. Tại Trang chủ, nhìn vào thanh filter phía trên sơ đồ bàn 2. Bấm chọn checkbox "Bàn trống" 3. Quan sát danh sách bàn và số đếm trong ngoặc | Chỉ hiện bàn trống, số đếm khớp |
1.1.3 | ☐ | Lọc tab "Đang sử dụng" | 1. Tại Trang chủ, bỏ các filter đang chọn 2. Bấm chọn checkbox "Đang sử dụng" 3. Quan sát danh sách bàn và số đếm | Chỉ hiện bàn đang dùng, số đếm khớp |
1.1.4 | ☐ | Lọc tab "Chờ xác nhận" | 1. Tại Trang chủ, bỏ các filter đang chọn 2. Bấm chọn checkbox "Chờ xác nhận" 3. Quan sát danh sách bàn | Chỉ hiện đơn chờ xác nhận |
1.1.5 | ☐ | Lọc tab "Chờ thanh toán" | 1. Tại Trang chủ, bỏ các filter đang chọn 2. Bấm chọn checkbox "Chờ thanh toán" 3. Quan sát danh sách bàn | Chỉ hiện đơn chờ thanh toán |
1.1.6 | ☐ | Lọc theo khu (khu 1 / khu 2) | 1. Tại Trang chủ, tìm dropdown "Tất cả (39)" ở góc phải thanh công cụ 2. Bấm vào dropdown, chọn một khu cụ thể (VD: Khu 1) 3. Quan sát danh sách bàn hiển thị | Chỉ hiện bàn thuộc khu đã chọn |
1.1.7 | ☐ | Đổi số cột hiển thị (6 cột) | 1. Tại Trang chủ, tìm dropdown "6 cột" trên thanh công cụ 2. Bấm vào dropdown, chọn số cột khác (VD: 4 cột hoặc 8 cột) 3. Quan sát lưới bàn thay đổi bố cục | Lưới bàn bố trí lại đúng số cột đã chọn |
1.1.8 | ☐ | Đổi giao diện (1 / 2 / 3) | 1. Tại Trang chủ, tìm nút "Giao diện 3" trên thanh công cụ 2. Bấm nút để chuyển lần lượt: Giao diện 1 → 2 → 3 3. Quan sát kiểu hiển thị thẻ bàn sau mỗi lần đổi | Kiểu hiển thị thẻ bàn thay đổi tương ứng |
1.1.9 | ☐ | Thẻ bàn hiển thị thông tin | 1. Tại Trang chủ, lọc tab "Đang sử dụng" 2. Quan sát một thẻ bàn đang hoạt động (thẻ màu vàng/cam) 3. Kiểm tra từng thông tin: tên bàn, timer, icon hóa đơn, icon số khách, tổng tiền, nhãn trạng thái | Đúng tên, timer, số hóa đơn, số khách, tổng tiền, trạng thái |
1.1.10 | ☐ | Tổng tiền trên thẻ bàn | 1. Bấm vào bàn đang sử dụng để vào màn hình Order 2. Ghi nhận tổng tiền thanh toán hiển thị (đã tính thuế) 3. Bấm "Back" về Trang chủ 4. So sánh tổng tiền trên thẻ bàn với con số vừa ghi nhận | Khớp tổng đơn của bàn (đã gồm thuế) |
1.1.11 | ☐ | Trạng thái "Chưa báo bếp" | 1. Bấm vào bàn đang sử dụng, thêm ít nhất 1 món mới vào đơn 2. "Không" bấm nút "Gửi bếp / Báo bếp" 3. Back về Trang chủ 4. Quan sát thẻ bàn đó | Hiển thị nhãn "Chưa báo bếp" trên thẻ bàn |
1.1.12 | ☐ | Nút "Xác nhận" trên thẻ | 1. Tại Trang chủ, lọc tab "Chờ xác nhận" 2. Tìm thẻ bàn có nút "Xác nhận" 3. Bấm nút "Xác nhận" trực tiếp trên thẻ bàn 4. Quan sát trạng thái thẻ bàn sau thao tác | Đơn được xác nhận, trạng thái cập nhật sang "Đang sử dụng" |
1.1.13 | ☐ | Bấm vào bàn | 1. Tại Trang chủ, chọn bất kỳ thẻ bàn nào 2. Bấm vào vùng thân thẻ bàn 3. Quan sát màn hình mở ra | Mở màn hình Order của bàn đó |
1.1.14 | ☐ | Thêm đơn mang về | 1. Tại Trang chủ, tìm thẻ "Bàn mang về" (thẻ có icon Takeaway, vị trí đầu danh sách) 2. Bấm vào thẻ đó 3. Quan sát màn hình mở ra | Mở màn hình Order ở chế độ Mang đi |
1.1.15 | ☐ | Số liệu các tab nhất quán | 1. Tại Trang chủ, ghi lại số đếm từng tab: "Bàn trống (n1)", "Đang sử dụng (n2)", "Chờ xác nhận (n3)", "Chờ thanh toán (n4)" 2. Tính tổng: n1 + n2 + n3 + n4 3. So sánh với số hiển thị tại tab "Tất cả" | Tổng các tab = tổng tất cả |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
