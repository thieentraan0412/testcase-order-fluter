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

1.3 Modal tùy chọn món

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.3.1 | ☐ | Mở modal khi món có tùy chọn | 1. Tại màn hình Order, bấm vào một món có cấu hình tùy chọn (thuộc tính hoặc món thêm) 2. Quan sát màn hình | Hiện modal "Chọn món kèm theo" |
| 1.3.2 | ☐ | Chọn thuộc tính (Size, độ ngọt...) | 1. Trong modal, tìm nhóm thuộc tính (VD: Size, Độ ngọt) 2. Bấm chọn một giá trị bất kỳ trong nhóm 3. Quan sát lựa chọn được ghi nhận và giá thay đổi nếu có | Ghi nhận lựa chọn, giá cập nhật nếu giá trị đó có phụ thu |
| 1.3.3 | ☐ | Chọn món thêm | 1. Trong modal, tìm nhóm "Món thêm" (VD: Nước ngọt) 2. Tích chọn một hoặc nhiều món thêm 3. Điều chỉnh số lượng từng món thêm nếu cần | Ghi nhận đúng các món thêm và số lượng đã chọn |
| 1.3.4 | ☐ | Tăng/giảm số lượng | 1. Trong modal, tìm nút +/- bên cạnh tên món chính 2. Bấm + để tăng, bấm - để giảm 3. Thử giảm về 1 rồi tiếp tục bấm - | Thay đổi đúng, không xuống dưới 1 |
| 1.3.5 | ☐ | Nhập ghi chú | 1. Trong modal, tìm ô "Ghi chú" phía cuối 2. Nhập nội dung ghi chú bất kỳ 3. Bấm "Chọn" để xác nhận 4. Quan sát dòng món trong hóa đơn | Ghi chú lưu kèm theo dòng món |
| 1.3.6 | ☐ | Bấm "Chọn" | 1. Trong modal, chọn đủ các tùy chọn mong muốn 2. Bấm nút "Chọn" 3. Quan sát hóa đơn bên phải | Món cùng toàn bộ tùy chọn được thêm vào hóa đơn |
| 1.3.7 | ☐ | Bấm "Đóng" | 1. Mở modal của bất kỳ món có tùy chọn nào 2. Không chọn gì, bấm nút "Đóng" 3. Quan sát hóa đơn | Đóng modal, không thêm món vào hóa đơn |
| 1.3.8 | ☐ | Tùy chọn hiển thị trong dòng món | 1. Sau khi bấm "Chọn", quan sát dòng món vừa thêm trong hóa đơn 2. Kiểm tra thông tin tùy chọn hiển thị bên dưới tên món | Hiển thị rõ các tùy chọn đã chọn (VD: Size S, Nước ngọt: Pepsi 5%) |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
