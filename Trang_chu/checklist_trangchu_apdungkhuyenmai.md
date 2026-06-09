# Checklist Testcase — App F&B (NASYS POS)

> Nền tảng: Ordertable riêng. Xây dựng dần qua từng video. Đổi ☐ → ☑ khi xong.

Link login https://table1.klkim.com/login
tài khoản
    Cửa hàng : trong
    Tài khoản: admin
    Mật khẩu : 147258

Link cashier https://table1.klkim.com/v2/order/cashier
Sau khi truy cập link: Click vào bàn    

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

1.13 Áp dụng khuyến mãi

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.13.1 | ☐ | Mở chức năng khuyến mãi trên đơn | 1. Trong màn hình Order có món, tìm nút "..." hoặc mục "Khuyến mãi" 2. Bấm mở chức năng khuyến mãi 3. Quan sát danh sách | Hiện danh sách chương trình khuyến mãi còn hiệu lực |
| 1.13.2 | ☐ | Áp khuyến mãi vào đơn | 1. Mở danh sách khuyến mãi, chọn một CTKM phù hợp 2. Xác nhận áp 3. Quan sát dòng "Giảm giá" và Tổng tiền thanh toán | Giảm giá áp đúng theo CTKM, tổng tiền thanh toán giảm tương ứng |
| 1.13.3 | ☐ | CTKM hết hiệu lực | 1. Mở danh sách khuyến mãi 2. Tìm CTKM đã hết ngày hoặc hết lượt 3. Quan sát xem có hiển thị không | CTKM hết hiệu lực không xuất hiện trong danh sách hoặc không áp được |
| 1.13.4 | ☐ | Đơn không thỏa điều kiện CTKM | 1. Tạo đơn có giá trị thấp hơn điều kiện tối thiểu của CTKM 2. Thử áp CTKM đó 3. Quan sát phản hồi | Hệ thống không cho áp, hiển thị thông báo lỗi |
| 1.13.5 | ☐ | Bỏ khuyến mãi đã áp | 1. Sau khi đã áp CTKM thành công, tìm tùy chọn gỡ/bỏ khuyến mãi 2. Xác nhận gỡ 3. Quan sát lại Tổng tiền thanh toán | Giảm giá bị xóa, tổng tiền hoàn về giá gốc |
| 1.13.6 | ☐ | Chưa mở ca | 1. Đảm bảo ca chưa được mở 2. Vào màn hình Order, thử mở chức năng khuyến mãi 3. Quan sát phản hồi | Hệ thống chặn, không cho áp khuyến mãi |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
