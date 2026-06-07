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
1.9 Chuyển bàn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
1.9.1 | ☐ | Mở chức năng chuyển bàn từ bàn đang dùng | 1. Từ Trang chủ, bấm vào một bàn đang có đơn (trạng thái "Đang sử dụng") 2. Tại màn hình Order, bấm icon "Chuyển bàn" trên thanh công cụ (hoặc menu `...` → chọn Chuyển bàn) 3. Quan sát màn hình mở ra | Hiện danh sách bàn đích để chọn |
1.9.2 | ☐ | Bàn đích (bàn trống) hiển thị màu vàng | 1. Mở chức năng chuyển bàn từ bàn đang dùng 2. Quan sát màu sắc các thẻ bàn trong danh sách bàn đích 3. So sánh màu thẻ bàn trống và bàn đang dùng | Các bàn trống hiển thị màu vàng để gợi ý; bàn đang dùng hiển thị màu khác (xám hoặc tối) |
1.9.3 | ☐ | Chọn bàn trống để chuyển | 1. Mở chức năng chuyển bàn từ "Bàn A" đang có đơn 2. Trong danh sách bàn đích, bấm chọn "Bàn B" đang trống (màu vàng) 3. Xác nhận chuyển bàn 4. Quan sát trạng thái Bàn A và Bàn B ngoài Trang chủ | Toàn bộ đơn của Bàn A chuyển sang Bàn B; Bàn A trở về trạng thái "trống"; Bàn B chuyển sang "Đang sử dụng" với đúng dữ liệu đơn cũ |
1.9.4 | ☐ | Chỉ cho chọn bàn trống | 1. Mở chức năng chuyển bàn từ Bàn A 2. Trong danh sách bàn đích, thử bấm vào một bàn "đang sử dụng" 3. Quan sát phản hồi | Hệ thống không cho chọn bàn đang dùng; thẻ bàn đó bị mờ, không thể bấm hoặc hiện thông báo không hợp lệ |
1.9.5 | ☐ | Chưa mở ca / không có quyền | 1. Đảm bảo ca chưa mở hoặc dùng tài khoản không có quyền chuyển bàn 2. Vào màn hình Order của bàn đang có đơn 3. Tìm và bấm nút Chuyển bàn | Hệ thống chặn thao tác, hiển thị thông báo "Chưa mở ca" hoặc "Không có quyền" |
1.9.6 | ☐ | Dữ liệu đơn giữ nguyên sau chuyển bàn | 1. Ghi nhận danh sách món, số lượng, ghi chú và tổng tiền tại Bàn A trước khi chuyển 2. Chuyển sang Bàn B trống 3. Vào màn hình Order của Bàn B, kiểm tra lại toàn bộ thông tin | Danh sách món, số lượng, ghi chú, tổng tiền tại Bàn B khớp hoàn toàn với Bàn A trước khi chuyển |
1.9.7 | ☐ | Trạng thái thẻ bàn cập nhật ngay sau chuyển | 1. Thực hiện chuyển Bàn A sang Bàn B 2. Xác nhận xong, ngay lập tức quay về "Trang chủ" (không reload thủ công) 3. Quan sát thẻ Bàn A và Bàn B | Bàn A hiển thị "trống" ngay lập tức; Bàn B hiển thị "Đang sử dụng" với đúng tổng tiền — không cần F5 mới thấy |
1.9.8 | ☐ | Chuyển bàn khi món đã gửi bếp | 1. Tại Bàn A, thêm món và bấm "Báo bếp" (món đã gửi bếp) 2. Mở chức năng chuyển bàn, chọn Bàn B trống 3. Xác nhận chuyển 4. Vào Bàn B kiểm tra trạng thái món | Món chuyển sang Bàn B vẫn giữ trạng thái "đã gửi bếp", không bị reset về "Chưa báo bếp" |
1.9.9 | ☐ | Hủy thao tác chuyển bàn giữa chừng | 1. Mở chức năng chuyển bàn từ Bàn A 2. Danh sách bàn đích hiện ra, nhưng "không chọn bàn nào" 3. Bấm "Hủy" hoặc "Đóng" (X) 4. Quan sát dữ liệu Bàn A | Không có thay đổi nào xảy ra; đơn tại Bàn A giữ nguyên như trước |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
