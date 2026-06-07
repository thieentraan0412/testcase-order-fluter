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
1.5 Hoa hồng nhân viên

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.5.1 | ☐ | Bấm "Hoa hồng" trên dòng món | 1. Trong hóa đơn, tìm dòng món có link "% Hoa hồng" bên dưới tên món 2. Bấm vào link đó 3. Quan sát màn hình | Mở modal "Hoa hồng nhân viên" |
| 1.5.2 | ☐ | Modal hiện các mục hoa hồng | 1. Mở modal Hoa hồng của bất kỳ món nào 2. Quan sát danh sách các mục trong modal (VD: 123 (10%), 456 (5%)) | Hiện đủ các mục kèm tên và % hoa hồng đã cấu hình |
| 1.5.3 | ☐ | Chọn nhân viên mỗi mục | 1. Trong modal, bấm vào dropdown bên cạnh một mục hoa hồng 2. Chọn một nhân viên từ danh sách xổ xuống | Nhân viên được chọn và ghi nhận vào mục đó |
| 1.5.4 | ☐ | Gán nhiều NV nhiều mục | 1. Trong modal, lần lượt chọn nhân viên khác nhau cho từng mục hoa hồng 2. Bấm "Xác nhận" | Tất cả các mục đều gán được đồng thời, không bị ghi đè |
| 1.5.5 | ☐ | Bấm "Xác nhận" | 1. Trong modal, chọn nhân viên cho ít nhất một mục 2. Bấm nút "Xác nhận" 3. Quan sát dòng món trong hóa đơn | Thông tin hoa hồng hiển thị trên dòng món |
| 1.5.6 | ☐ | Bấm "Đóng" | 1. Mở modal Hoa hồng, chọn nhân viên vào một mục 2. Bấm nút "Đóng" thay vì "Xác nhận" 3. Mở lại modal kiểm tra | Thay đổi không được lưu, dữ liệu cũ giữ nguyên |
| 1.5.7 | ☐ | Mở lại modal để sửa | 1. Sau khi đã gán hoa hồng và bấm "Xác nhận", bấm lại "% Hoa hồng" trên dòng món đó 2. Thay đổi nhân viên hoặc xóa chọn 3. Bấm "Xác nhận" | Cập nhật được nhân viên mới, dữ liệu cũ bị thay thế |
| 1.5.8 | ☐ | Hoa hồng theo món độc lập | 1. Gán hoa hồng cho Món A, bấm "Xác nhận" 2. Mở modal Hoa hồng của Món B (chưa gán) 3. Quan sát modal Món B | Modal Món B trống, không bị ảnh hưởng từ Món A |
| 1.5.9 | ☐ | Tính tiền hoa hồng | 1. Gán nhân viên cho mục có % xác định (VD: 10%) trên món có giá cụ thể (VD: 50,000đ) 2. Tính tay: 10% × 50,000đ = 5,000đ 3. Kiểm tra giá trị hoa hồng ghi nhận trong hệ thống | Hoa hồng = % × giá trị món, tính đúng |
| 1.5.10 | ☐ | Để trống nhân viên | 1. Mở modal Hoa hồng 2. Không chọn nhân viên cho bất kỳ mục nào 3. Bấm "Xác nhận" | Hệ thống cho phép xác nhận, không báo lỗi bắt buộc |
| 1.5.11 | ☐ | 1 NV gán nhiều mục | 1. Trong modal, chọn cùng một nhân viên cho cả 2 mục hoa hồng (VD: 123 (10%) và 456 (5%)) 2. Bấm "Xác nhận" 3. Kiểm tra tổng hoa hồng của nhân viên đó trong link "https://table.nasys.vn/v2/report/end-day?type=commission" vào mục "Báo cáo hoa hồng.| số tiền nhận được phải đúng với %

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
