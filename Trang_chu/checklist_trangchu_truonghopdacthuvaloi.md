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

Hãy sử dụng google chorme và thực hiện các testcase sau
Trong khi thực hiện testcase hãy bổ sung chi tiết từng bước click trong cột "Các bước thực hiện" và trong ghi thêm những testcase mới vào file này

1.16 Trường hợp đặc thù & lỗi

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.16.1 | ☐ | Số lượng món = 0 | 1. Trong hóa đơn, giảm số lượng một món về 0 (nếu cho phép nhập tay) 2. Thử lưu hoặc thanh toán 3. Quan sát phản hồi | Hệ thống không cho lưu, xử lý đúng khi số lượng = 0 |
| 1.16.2 | ☐ | Giá rất lớn (999,999,999đ) | 1. Vào cấu hình hoặc chỉnh sửa đơn giá thủ công, nhập giá trị rất lớn (VD: 999,999,999đ) 2. Thêm vào hóa đơn 3. Quan sát hiển thị và tổng tiền | Tính và hiển thị đúng số lớn, không bị tràn giao diện |
| 1.16.3 | ☐ | Làm tròn tiền VND | 1. Tạo đơn có thuế % dẫn đến kết quả lẻ thập phân (VD: 10% của 15,000đ = 1,500đ) 2. Quan sát tổng tiền thanh toán | Tổng tiền hiển thị số nguyên, không có số lẻ thập phân |
| 1.16.4 | ☐ | Mất mạng khi thanh toán | 1. Chuẩn bị đơn hàng sẵn sàng thanh toán 2. Tắt mạng (ngắt WiFi hoặc kéo cáp) 3. Bấm "Thanh toán" 4. Bật lại mạng, kiểm tra trong Lịch sử đơn | Đơn không bị tạo trùng, dữ liệu nhất quán |
| 1.16.5 | ☐ | Hai thu ngân cùng 1 bàn | 1. Mở bàn đang có đơn trên 2 thiết bị/tab khác nhau 2. Cả 2 cùng thêm món hoặc chỉnh sửa đồng thời 3. Quan sát kết quả trên cả 2 thiết bị | Không bị ghi đè hoặc mất dữ liệu của nhau |
| 1.16.6 | ☐ | Ghi chú có dấu / ký tự đặc biệt | 1. Trong hóa đơn, tích checkbox "Ghi chú" trên một dòng món 2. Nhập nội dung có dấu tiếng Việt và ký tự đặc biệt (VD: @, #, !, ...) 3. Lưu và quan sát lại dòng món | Ghi chú lưu và hiển thị đúng, không bị lỗi ký tự |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
