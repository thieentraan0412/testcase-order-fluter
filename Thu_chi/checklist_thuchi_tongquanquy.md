
## 2. Thu chi

Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense

---

2.2 Tổng quan quỹ

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 2.2.1 | ☐ | Hiển thị Tồn quỹ đầu kỳ | 1. Vào trang Thu chi 2. Chọn khoảng thời gian cụ thể (VD: Tháng này) 3. Quan sát thẻ "Tồn quỹ đầu kỳ" | Hiển thị đúng số dư tồn quỹ tại thời điểm đầu kỳ đã lọc |
| 2.2.2 | ☐ | Hiển thị Tổng thu | 1. Vào trang Thu chi, chọn bộ lọc thời gian 2. Lọc danh sách chỉ hiện phiếu "Thu" (bằng cách bật lọc Loại = Thu) 3. Cộng tay số tiền tất cả phiếu thu trong danh sách 4. So sánh với thẻ "Tổng thu" | Tổng thu = Σ số tiền tất cả phiếu Thu trong bộ lọc |
| 2.2.3 | ☐ | Hiển thị Tổng chi | 1. Vào trang Thu chi, chọn bộ lọc thời gian 2. Lọc danh sách chỉ hiện phiếu "Chi" 3. Cộng tay số tiền tất cả phiếu chi trong danh sách 4. So sánh với thẻ "Tổng chi" | Tổng chi = Σ số tiền tất cả phiếu Chi trong bộ lọc |
| 2.2.4 | ☐ | Tồn quỹ cuối kỳ tính đúng | 1. Vào trang Thu chi 2. Ghi nhận 3 giá trị: Tồn đầu kỳ, Tổng thu, Tổng chi 3. Tính tay: Tồn đầu kỳ + Tổng thu − Tổng chi 4. So sánh kết quả với thẻ "Tồn quỹ cuối kỳ" | Tồn quỹ cuối kỳ = Tồn đầu kỳ + Tổng thu − Tổng chi |
| 2.2.5 | ☐ | Đổi bộ lọc thời gian → thẻ cập nhật | 1. Vào trang Thu chi, ghi nhận 4 giá trị thẻ tổng quan đang hiển thị 2. Thay đổi bộ lọc thời gian (VD: từ "Tháng này" sang "Hôm nay") 3. Quan sát 4 thẻ sau khi đổi lọc | Cả 4 thẻ (Tồn đầu kỳ, Tổng thu, Tổng chi, Tồn cuối kỳ) cập nhật theo kỳ mới |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
