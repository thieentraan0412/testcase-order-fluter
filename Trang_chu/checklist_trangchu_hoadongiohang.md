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
1.4 Hóa đơn / Giỏ hàng

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
1.4.1 | ☐ | Thêm món vào hóa đơn | 1. Tại màn hình Order, bấm vào bất kỳ món nào trong lưới thực đơn 2. Quan sát panel hóa đơn bên phải | Dòng món xuất hiện trong hóa đơn, số đếm "Tổng tiền (n)" tăng |
1.4.2 | ☐ | Tăng số lượng (+) | 1. Trong hóa đơn, tìm dòng món bất kỳ 2. Bấm nút + bên cạnh số lượng 3. Quan sát số lượng và cột Thành tiền | Thành tiền = đơn giá × số lượng mới |
1.4.3 | ☐ | Giảm số lượng (−) | 1. Trong hóa đơn, tìm dòng món có số lượng ≥ 2 2. Bấm nút − liên tục 3. Thử giảm khi số lượng đang là 1 | Số lượng giảm đúng; khi về 0 hệ thống xử lý đúng (xóa món hoặc chặn) |
1.4.4 | ☐ | Xóa món (nút X) | 1. Trong hóa đơn, tìm dòng món bất kỳ 2. Bấm nút X đỏ ở cuối dòng 3. Quan sát hóa đơn và tổng tiền | Dòng món bị xóa, tổng tiền cập nhật |
1.4.5 | ☐ | Sửa đơn giá thủ công | 1. Trong hóa đơn, bấm vào icon bút (chỉnh sửa) tại cột Đơn giá của một món 2. Nhập giá mới 3. Xác nhận và quan sát Thành tiền, Tổng tiền | Tổng cập nhật đúng theo giá mới |
1.4.6 | ☐ | Ghi chú từng món | 1. Trong hóa đơn, tích vào checkbox "Ghi chú" bên dưới tên món 2. Nhập nội dung ghi chú 3. Quan sát dòng món sau khi lưu | Ghi chú lưu và hiển thị theo đúng dòng món đó |
1.4.7 | ☐ | Tổng tiền (tạm tính) | 1. Thêm nhiều món vào hóa đơn 2. Tính tay: Σ (đơn giá × số lượng) của từng dòng 3. So sánh với "Tổng tiền" hiển thị (chưa cộng thuế, phụ thu) | Tổng tiền = Σ (đơn giá × SL) |
1.4.8 | ☐ | Thuế theo từng món | 1. Thêm món có cấu hình thuế riêng (VD: món VAT 0%, TOPPING 10%) 2. Quan sát dòng "Thuế sản phẩm" ở phần tổng hóa đơn | Thuế tính đúng theo % đã cấu hình từng món |
1.4.9 | ☐ | Thuế theo cả bill | 1. Thêm món vào hóa đơn 2. Kiểm tra cấu hình thuế áp theo toàn bill 3. Quan sát dòng thuế trong phần tổng | Thuế tính đúng theo setting cả bill |
1.4.10 | ☐ | Kết hợp thuế món + bill | 1. Thêm món vừa có thuế riêng, vừa có thuế bill 2. Quan sát tổng thuế hiển thị | Không tính trùng hoặc sai, thuế chỉ tính một lần đúng quy tắc |
1.4.11 | ☐ | Tổng tiền thanh toán | 1. Thêm món, nhập phụ thu và giảm giá 2. Tính tay: Tổng tiền + Phụ thu − Giảm giá + Thuế 3. So sánh với "Tổng tiền thanh toán" hiển thị (màu đỏ) | Tổng tiền thanh toán = Tổng tiền + Phụ thu − Giảm giá + Thuế |
1.4.12 | ☐ | Phụ thu | 1. Trong hóa đơn, bấm icon bút tại dòng "Phụ thu" 2. Nhập giá trị phụ thu 3. Quan sát Tổng tiền thanh toán | Phụ thu cộng đúng vào tổng |
1.4.13 | ☐ | Giảm giá | 1. vào link cashier Chọn bàn,   trang order món,  chọn thêm 5 món vào hóa đơn. 2. Click vào "giảm giá" 3. chọn vào giảm giá trực tiếp, click vào "Chọn" chọn 1 thông tin cụ thể ,  sau đó % tiền vào --> click vào "xác nhận". 4. Click vào "Thanh toán" -> click vào "Xác nhận"  5. vào trang admin -->  vào trang "quản lí đơn hàng" 6. kiểm tra hóa đơn sinh ra có đúng với hóa đơn lúc cashier thanh toán | số tiền thanh toán phải đúng 
1.4.14 | ☐ | Gợi ý nhanh tiền mặt | 1. Tại hóa đơn có tổng tiền thanh toán xác định 2. Quan sát các nút gợi ý số tiền (VD: 120,000đ, 150,000đ, 200,000đ) phía trên ô Tiền mặt | Các giá trị gợi ý đều ≥ tổng thanh toán và là mệnh giá hợp lý |
1.4.15 | ☐ | Combo / Set menu | 1. Trong lưới thực đơn, tìm và bấm vào một món Combo hoặc Set menu 2. Quan sát dòng món trong hóa đơn | Hiển thị đúng tên combo, thành phần kèm theo và giá |
1.4.16 | ☐ | Chọn khách hàng | 1. Trong hóa đơn, bấm vào dropdown "Khách lẻ" góc trên phải panel 2. Tìm và chọn một khách hàng có sẵn 3. Quan sát thông tin khách trên hóa đơn | Thông tin khách hàng gắn vào hóa đơn |
1.4.17 | ☐ | Nhiều hóa đơn / 1 bàn | 1. Tại màn hình Order của một bàn, bấm nút + bên cạnh tab hóa đơn hiện tại 2. Thêm món khác nhau vào từng tab 3. Chuyển qua lại giữa 2 tab | Mỗi tab là hóa đơn độc lập, tổng tiền không ảnh hưởng nhau |
1.4.18 | ☐ | Đơn các bàn độc lập | 1. Thêm món vào Bàn A, quay về Trang chủ 2. Vào Bàn B, thêm món khác 3. Quay lại Bàn A kiểm tra | Hóa đơn Bàn A không bị lẫn món của Bàn B |
1.4.19 | ☐ | Hóa đơn trống | 1. Tại màn hình Order, tạo hóa đơn mới (bấm +) hoặc vào bàn chưa có món 2. Quan sát panel hóa đơn | Hiển thị thông báo "Bạn chưa thêm sản phẩm nào", tổng tiền = 0 |
1.4.20 | ☐ | Nhân viên phụ trách | 1. Tại màn hình Order, quan sát tên nhân viên hiển thị trong hóa đơn (VD: "Nhân viên: Admin Master") 2. So sánh với tài khoản đang đăng nhập | Hiển thị đúng tên nhân viên đang thao tác |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
