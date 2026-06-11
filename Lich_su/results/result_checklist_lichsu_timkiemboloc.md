Link login: https://table1.klkim.com/login
Link cashier: https://table1.klkim.com/v2/order/cashier/history

4. Lịch sử — 4.2 Tìm kiếm & bộ lọc
---
Ngày chạy: 10-06-2026 | Trình duyệt: Google Chrome | Tài khoản: admin
Dữ liệu test: cửa hàng có nhiều đơn (hôm nay 10-06, hôm qua 09-06, và các ngày 03→08-06), gồm đơn Đã thanh toán, Chưa thanh toán, Công nợ, Mang về → đủ để kiểm chứng các bộ lọc.
Lưu ý: 4.2.1–4.2.10 chạy trên cửa hàng "trong" (ít đơn); 4.2.11–4.2.16 chạy trên cửa hàng nhiều đơn sau khi đổi kết nối trình duyệt. Kết quả lọc đều đúng logic ở cả hai.

| STT | ✓ | Testcase | Kết quả thực tế |
|-----|---|----------|-----------------|
| 4.2.1 | ☑ | Tìm theo mã đơn | Nhập mã đơn có sẵn → trả về đúng đơn tương ứng. Đúng. |
| 4.2.2 | ☐ | Tìm theo số điện thoại | CHƯA KIỂM CHỨNG ĐẦY ĐỦ — các đơn kiểm tra đều là "Khách lẻ" không gắn SĐT nên không có dữ liệu dương để xác minh kết quả. Ô tìm kiếm dùng chung với tìm mã đơn (đã PASS). |
| 4.2.3 | ☑ | Tìm không khớp | Nhập "xxxx9999" → "Không tìm thấy dữ liệu phù hợp". Đúng. |
| 4.2.4 | ☑ | Trạng thái: Đã thanh toán thành công | Lọc → chỉ hiện đơn "Đã thanh toán". Đúng. |
| 4.2.5 | ☑ | Trạng thái: Chưa thanh toán | Lọc → chỉ hiện đơn "Chưa thanh toán". Đúng. |
| 4.2.6 | ☑ | Trạng thái: Đã hủy | Lọc áp dụng đúng (danh sách rỗng khi không có đơn hủy). Đúng. |
| 4.2.7 | ☑ | Trạng thái: Đã xử lý trả hàng | Lọc áp dụng đúng. Đúng. |
| 4.2.8 | ☑ | Trạng thái: Công nợ | Lọc áp dụng đúng; cửa hàng nhiều đơn có đơn "Công nợ" (VD POS00002300CN2, Tiền nợ 960,000đ). Đúng. |
| 4.2.9 | ☑ | Lọc theo Tài khoản (nhân viên) | Chọn "Admin master" → hiện đơn của NV đó; chọn "Nguyễn Thị A" → rỗng. Lọc đúng. |
| 4.2.10 | ☑ | Khoảng ngày: Hôm nay | Chọn "Hôm nay" → chỉ hiện đơn ngày 10-06-2026. Đúng. |
| 4.2.11 | ☑ | Khoảng ngày: Hôm qua | Chọn "Hôm qua" → tất cả đơn đều ngày 09-06-2026. Đúng. |
| 4.2.12 | ☑ | Khoảng ngày: Tuần này | Chọn "Tuần này" → đơn nằm trong 08→10-06-2026 (T2–T4 tuần hiện tại). Đúng. |
| 4.2.13 | ☑ | Khoảng ngày: Tháng này | Chọn "Tháng này" → đơn trải từ 03→10-06-2026 (trong tháng 6). Đúng. |
| 4.2.14 | ☑ | Khoảng ngày: Tùy chọn | Đặt khoảng 08-06 → 09-06-2026, Xác nhận → chỉ hiện đơn trong 2 ngày đó (không có 10-06 hay sớm hơn). Đúng. |
| 4.2.15 | ☑ | Kết hợp nhiều bộ lọc | Tại bàn + "Đã thanh toán thành công" + Hôm nay → đúng 3 đơn (POS00002391/02387/02359), loại 2 đơn chưa thanh toán hôm nay. Lọc AND đúng. |
| 4.2.16 | ☑ | Ngày bắt đầu > ngày kết thúc | Đặt bắt đầu 10-06 > kết thúc 08-06, Xác nhận → "Không tìm thấy dữ liệu phù hợp" (KHÔNG trả kết quả sai). Đạt yêu cầu cốt lõi. |

⚠ Phát hiện (4.2.16): Hệ thống KHÔNG chặn việc chọn ngày bắt đầu > ngày kết thúc và KHÔNG hiển thị thông báo lỗi rõ ràng; chỉ trả danh sách rỗng. Đề xuất bổ sung validation/thông báo để UX rõ ràng hơn.

Tổng kết: 15 PASS / 0 FAIL / 1 chưa kiểm chứng đầy đủ (4.2.2 – thiếu đơn có SĐT khách).
