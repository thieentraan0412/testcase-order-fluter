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

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

1.10 Gộp bàn

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.10.1 | ☐ | Mở chức năng gộp bàn | 1. Từ Trang chủ, bấm vào một bàn đang có đơn 2. Tại màn hình Order, bấm icon "Gộp bàn" trên thanh công cụ (hoặc menu `...` → chọn Gộp bàn) 3. Quan sát màn hình mở ra | Hiện danh sách bàn để gộp; các bàn đang sử dụng được hiển thị để chọn |
| 1.10.2 | ☐ | Gộp đơn vào 2+ bàn đang hoạt động | 1. Mở chức năng gộp bàn từ "Bàn A" đang có đơn 2. Trong danh sách, chọn thêm "Bàn B" và "Bàn C" (cũng đang có đơn) 3. Xác nhận gộp 4. Quan sát kết quả tại Bàn A | Bàn A hiển thị thông tin đơn của cả 3 bàn (A + B + C); Bàn B và Bàn C về trạng thái trống; tổng tiền Bàn A = tổng A + B + C |
| 1.10.3 | ☐ | Đơn đã thanh toán không cho gộp | 1. Mở chức năng gộp bàn 2. Trong danh sách bàn, tìm bàn đã hoàn tất thanh toán 3. Thử chọn bàn đó để gộp 4. Quan sát phản hồi | Hệ thống không cho chọn bàn đã thanh toán; thẻ bàn đó bị mờ hoặc hiện thông báo không hợp lệ |
| 1.10.4 | ☐ | Xác nhận hoàn tất gộp | 1. Mở chức năng gộp bàn từ Bàn A 2. Chọn Bàn B đang có đơn để gộp vào 3. Bấm nút "Xác nhận" / "Hoàn tất" 4. Quan sát trạng thái tất cả các bàn liên quan ngoài Trang chủ | Trạng thái các bàn cập nhật đúng: bàn được gộp vào (Bàn A) giữ trạng thái "Đang sử dụng"; các bàn bị gộp (Bàn B) về trạng thái trống |
| 1.10.5 | ☐ | Tổng tiền sau gộp tính đúng | 1. Ghi nhận tổng tiền Bàn A (= a) và Bàn B (= b) trước khi gộp 2. Gộp Bàn B vào Bàn A 3. Quan sát tổng tiền Bàn A sau gộp | Tổng tiền Bàn A sau gộp = a + b (không mất tiền, không cộng dư) |
| 1.10.6 | ☐ | Danh sách món sau gộp hiển thị đúng | 1. Bàn A có món X; Bàn B có món Y 2. Gộp Bàn B vào Bàn A 3. Vào màn hình Order của Bàn A, quan sát danh sách món | Bàn A hiển thị đầy đủ cả món X lẫn món Y; không bị mất hoặc trùng dòng |
| 1.10.7 | ☐ | Gộp bàn khi các bàn đã gửi bếp | 1. Tại Bàn A và Bàn B, thêm món và bấm "Báo bếp" tại từng bàn 2. Thực hiện gộp Bàn B vào Bàn A 3. Quan sát trạng thái từng dòng món tại Bàn A sau gộp | Các món đã gửi bếp từ Bàn B vẫn giữ trạng thái "đã gửi bếp" sau khi gộp vào Bàn A |
| 1.10.8 | ☐ | Gộp bàn giữ nguyên ghi chú và tùy chọn món | 1. Tại Bàn B có món kèm ghi chú (VD: "ít đá") và tùy chọn (VD: Size L) 2. Gộp Bàn B vào Bàn A 3. Quan sát dòng món từ Bàn B trong hóa đơn Bàn A | Ghi chú và tùy chọn của món từ Bàn B được giữ nguyên, không bị mất sau khi gộp |
| 1.10.9 | ☐ | Hủy thao tác gộp giữa chừng | 1. Mở chức năng gộp bàn từ Bàn A 2. Chọn Bàn B để gộp 3. "Không" bấm Xác nhận, thay vào đó bấm "Hủy" hoặc "Đóng" (X) 4. Quan sát dữ liệu Bàn A và Bàn B | Không có thay đổi nào xảy ra; đơn tại Bàn A và Bàn B giữ nguyên như trước |
| 1.10.10 | ☐ | Chưa mở ca / không có quyền | 1. Đảm bảo ca chưa mở hoặc dùng tài khoản không có quyền gộp bàn 2. Vào màn hình Order của bàn đang có đơn 3. Tìm và bấm nút Gộp bàn | Hệ thống chặn thao tác, hiển thị thông báo "Chưa mở ca" hoặc "Không có quyền" |
| 1.10.11 | ☐ | Trạng thái thẻ bàn cập nhật ngay sau gộp | 1. Gộp Bàn B vào Bàn A, bấm Xác nhận 2. Ngay lập tức quay về "Trang chủ" (không reload thủ công) 3. Quan sát thẻ Bàn A và Bàn B | Bàn B hiển thị "trống" ngay lập tức; Bàn A hiển thị tổng tiền mới — không cần F5 mới thấy |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
