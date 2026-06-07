
## 2. Thu chi

Link login: https://table1.klkim.com/login

Tài khoản:
- Cửa hàng: trong
- Tài khoản: admin
- Mật khẩu: 147258

Link cashier: https://table1.klkim.com/v2/order/cashier/income-expense

---

2.7 Công nợ (tab Công nợ)

| STT | ✓ | Các bước thực hiện | Kết quả mong đợi |
|-----|---|--------------------|------------------|
| 2.7.1 | ☐ | 1. Mở Thu chi → bấm tab "Công nợ". | Mở màn hình Công nợ với panel "Bộ Lọc" bên trái. |
| 2.7.2 | ☐ | 1. Quan sát mục "Đối tượng" gồm 2 checkbox. | Có checkbox "Khách hàng" và "Nhà cung cấp", mặc định cả 2 được tích. |
| 2.7.3 | ☐ | 1. Bỏ tích "Nhà cung cấp", chỉ giữ "Khách hàng". 2. Xem danh sách. | Chỉ hiển thị công nợ của Khách hàng. |
| 2.7.4 | ☐ | 1. Bỏ tích "Khách hàng", chỉ giữ "Nhà cung cấp". 2. Xem danh sách. | Chỉ hiển thị công nợ của Nhà cung cấp. |
| 2.7.5 | ☐ | 1. Bỏ tích cả 2 checkbox đối tượng. | Danh sách rỗng (không có đối tượng nào được chọn). |
| 2.7.6 | ☐ | 1. Tại ô "Tên đối tượng", gõ tên một khách/NCC có công nợ. | Chỉ hiển thị công nợ của đối tượng khớp tên; tên sai → rỗng. |
| 2.7.7 | ☐ | 1. Tại ô "Mã công nợ", gõ một mã công nợ. | Trả đúng dòng công nợ khớp mã; không khớp → rỗng. |
| 2.7.8 | ☐ | 1. Mở dropdown "Chi nhánh". 2. Chọn/bỏ chọn chi nhánh (multi-select, có nút xóa ×). | Chỉ hiện công nợ của chi nhánh đã chọn; bỏ chọn thì cập nhật lại. |
| 2.7.9 | ☐ | 1. Mở dropdown "Người tạo". 2. Chọn 1 người tạo. | Chỉ hiện công nợ do người đã chọn tạo. |
| 2.7.10 | ☐ | 1. Kết hợp nhiều bộ lọc (Đối tượng + Chi nhánh + Tên). | Kết quả giao đúng tất cả điều kiện đã chọn. |
| 2.7.11 | ☐ | 1. Khi có dữ liệu, quan sát bảng công nợ. 2. Đọc các cột. | Hiển thị thông tin công nợ: đối tượng, mã công nợ, chi nhánh, số tiền nợ, người tạo... |
| 2.7.12 | ☐ | 1. Bấm xem chi tiết một dòng công nợ (nếu có). | Mở chi tiết công nợ của đối tượng đúng. |
| 2.7.13 | ☐ | 1. Chuyển qua lại giữa tab "Quản lý thu chi" và "Công nợ". | Mỗi tab giữ đúng dữ liệu & bộ lọc của mình, không lẫn. |

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó Đổi ☐ → ☑ khi xong khi pass testcase, còn fail thì đánh x
