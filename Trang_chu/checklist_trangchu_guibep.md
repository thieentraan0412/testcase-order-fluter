# Checklist Testcase — App F&B (NASYS POS)

> Nền tảng: Ordertable riêng. Xây dựng dần qua từng video. Đổi ☐ → ☑ khi xong.

Link login https://table1.klkim.com/login
tài khoản
    Cửa hàng : trong
    Tài khoản: admin
    Mật khẩu : 147258

Link cashier https://table1.klkim.com/v2/order/cashier
Link manager https://table1.klkim.com/v2/dashboard

---

Hãy sử dụng google chorme và thực hiện các testcase sau và trong lúc thực hiện hãy bổ sung thêm các testcase còn thiếu vào file này theo mẫu luôn

1.8 Gửi bếp

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.8.1 | ☐ | Gửi bếp sau khi chọn món | 1. Thêm ít nhất 1 món vào hóa đơn 2. Bấm nút "Báo bếp" (màu cam) 3. Quan sát trạng thái dòng món | Trạng thái món chuyển sang "chờ chế biến", không còn nhãn "Chờ báo bếp" |
| 1.8.2 | ☐ | Món chưa gửi bếp | 1. Thêm món vào hóa đơn 2. Chưa bấm "Báo bếp" 3. Quan sát nhãn hiển thị trên dòng món và thẻ bàn ngoài Trang chủ | Hiển thị "Chờ báo bếp" trên dòng món |
| 1.8.3 | ☐ | Gửi bếp khi giỏ trống | 1. Tạo hóa đơn mới hoặc xóa hết món 2. Bấm nút "Báo bếp" 3. Quan sát phản hồi | Hệ thống chặn, không gửi bếp |
| 1.8.4 | ☐ | Gửi bếp chỉ áp món mới thêm | 1. Thêm Món A, bấm "Báo bếp" 2. Tiếp tục thêm Món B vào cùng hóa đơn 3. Bấm "Báo bếp" lần 2 4. Quan sát trạng thái từng dòng món | Chỉ Món B được gửi bếp, Món A không bị gửi lại trùng |

sau khi thực hiện xong hết tất cả testcase thì Đổi ☐ → ☑ khi pass testcase, còn fail thì đánh x
