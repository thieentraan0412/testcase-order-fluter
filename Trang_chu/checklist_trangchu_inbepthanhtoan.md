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

1.6 In bếp / Thanh toán

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.6.1 | ☐ | In phiếu Bếp/Bar (báo bếp) | 1. Thêm ít nhất 1 món vào hóa đơn (trạng thái "Chờ báo bếp") 2. Bấm nút "Báo bếp" (màu cam) ở dưới cùng 3. Quan sát trạng thái từng dòng món trong hóa đơn | Trạng thái món chuyển từ "Chờ báo bếp" sang đã gửi bếp |
| 1.6.2 | ☐ | Tạm tính | 1. Trong hóa đơn có ít nhất 1 món, bấm nút "Tạm tính" (màu xanh lá) 2. Quan sát phiếu tạm tính hiển thị hoặc in ra | Phiếu tạm tính hiển thị đúng tổng tiền hiện tại |
| 1.6.3 | ☐ | Thanh toán tiền mặt | 1. Trong hóa đơn có món, bấm nút "Thanh toán" 2. Chọn phương thức "Tiền mặt" 3. Nhập số tiền khách đưa, xác nhận thanh toán 4. Quay lại Trang chủ quan sát bàn | Đơn hoàn tất, bàn về trạng thái trống |
| 1.6.4 | ☐ | Thanh toán chuyển khoản | 1. Trong hóa đơn có món, bấm nút "Thanh toán" 2. Chọn phương thức "Chuyển khoản" 3. Xác nhận thanh toán 4. Quan sát kết quả | Đơn hoàn tất, luồng chuyển khoản hoạt động đúng |
| 1.6.5 | ☐ | Thanh toán quẹt thẻ | 1. Trong hóa đơn có món, bấm nút "Thanh toán" 2. Chọn phương thức "Quẹt Thẻ" 3. Xác nhận thanh toán 4. Quan sát kết quả | Đơn hoàn tất, luồng quẹt thẻ hoạt động đúng |
| 1.6.6 | ☐ | Thanh toán QR tự động | 1. Trong hóa đơn có món, bấm nút "Thanh toán" 2. Chọn phương thức "QR Tự động" 3. Quan sát mã QR sinh ra 4. Giả lập hoặc thực hiện thanh toán qua QR | Mã QR được sinh, sau khi thanh toán đơn hoàn tất |
| 1.6.7 | ☐ | Tiền thừa | 1. Trong hóa đơn, xem Tổng tiền thanh toán (VD: 115,000đ) 2. Bấm "Thanh toán" → chọn Tiền mặt 3. Nhập số tiền lớn hơn tổng (VD: 150,000đ) 4. Quan sát số tiền thừa hiển thị | Tiền thừa = tiền nhận − tổng thanh toán, tính đúng |
| 1.6.8 | ☐ | Chặn hóa đơn trống | 1. Tạo hóa đơn mới, không thêm bất kỳ món nào 2. Bấm nút "Thanh toán" 3. Quan sát phản hồi | Hệ thống chặn, hiển thị thông báo lỗi, không cho thanh toán |
| 1.6.9 | ☐ | Hóa đơn điện tử | 1. Hoàn tất thanh toán một đơn hàng 2. Tại màn hình xác nhận hoặc lịch sử, tìm chức năng "Hóa đơn điện tử" 3. Bấm phát hành và quan sát kết quả | Hóa đơn điện tử được phát hành đúng |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
