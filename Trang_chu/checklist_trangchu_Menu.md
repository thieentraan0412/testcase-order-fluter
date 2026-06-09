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

1.2 Menu (Thực đơn) 

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.2.1 | ☐ | Hiển thị danh mục món | 1. Từ Trang chủ, bấm vào bất kỳ bàn nào để vào màn hình Order 2. Quan sát thanh tab danh mục phía trên lưới món (TẤT CẢ, BÁN CHẠY, MÓN MỚI...) | Hiện đủ các tab danh mục |
| 1.2.2 | ☐ | Lọc theo danh mục | 1. Tại màn hình Order, bấm vào một tab danh mục bất kỳ (VD: NƯỚC NGỌT) 2. Quan sát lưới món thay đổi | Chỉ hiện món thuộc danh mục đã chọn |
| 1.2.3 | ☐ | Tìm món (F1) | 1. Tại màn hình Order, bấm vào ô "Tìm và chọn món (F1)" 2. Gõ từ khóa tên món (thử cả có dấu và không dấu) 3. Quan sát kết quả lọc | Lọc đúng theo từ khóa, kể cả tiếng Việt có dấu |
| 1.2.4 | ☐ | Ẩn/hiện hình ảnh món | 1. Tại màn hình Order, tìm toggle "Ẩn hình ảnh" phía trên lưới món 2. Bật toggle → quan sát 3. Tắt toggle → quan sát lại | Lưới ẩn/hiện ảnh tương ứng |
| 1.2.5 | ☐ | Đổi số cột hiển thị món | 1. Tại màn hình Order, tìm dropdown "6 cột" phía trên lưới món 2. Bấm vào dropdown, chọn số cột khác 3. Quan sát bố cục lưới món | Bố trí lại đúng số cột đã chọn |
| 1.2.6 | ☐ | Phân trang (1/5, 2/5...) | 1. Tại màn hình Order, quan sát chỉ số trang hiện tại (VD: 1/5) 2. Bấm mũi tên sang phải để chuyển sang trang tiếp 3. Quan sát món hiển thị và chỉ số trang cập nhật | Hiện trang tiếp theo, số trang đúng |
| 1.2.7 | ☐ | Giá món | 1. Tại màn hình Order, quan sát giá hiển thị bên dưới từng món trong lưới 2. So sánh với giá thực tế đã cấu hình | Hiển thị đúng định dạng VND |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
