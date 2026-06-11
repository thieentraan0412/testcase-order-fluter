# Checklist Testcase — Trang Trả hàng (Return Order)

> Link: https://table1.klkim.com/v2/order/cashier/return-order
> Nền tảng: Google Chrome. Đổi ☐ → ☑ khi test xong.

---

Hãy sử dụng google chorme và thực hiện các testcase sau

7. Modal "Thông tin trả hàng" — Thông tin & danh sách món

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | 7.1 Hiển thị thông tin đầu phiếu | 1. Mở modal trả hàng | Hiển thị: Khách hàng, Mã hóa đơn, Thời gian thanh toán, Phòng/bàn, Số lượng, Phương thức thanh toán |
| ☐ | 7.2 Hiển thị bảng món | 1. Quan sát bảng món | Cột: Tên món, Số lượng, Trả lại (− số +), Đơn giá, Thành tiền |
| ☐ | 7.3 Hiển thị topping/món thêm | 1. Quan sát món có topping/size | Hiển thị chi tiết món thêm, size và giá kèm theo |
| ☐ | 7.4 Tăng số lượng trả | 1. Bấm nút (+) ở cột Trả lại | Số lượng trả tăng, tiền trả lại cập nhật |
| ☐ | 7.5 Giảm số lượng trả | 1. Bấm nút (−) ở cột Trả lại | Số lượng trả giảm, tiền trả lại cập nhật |
| ☐ | 7.6 Nhập số lượng trả trực tiếp | 1. Nhập số vào ô số lượng trả | Cập nhật đúng, tính lại tiền |
| ☐ | 7.7 Trả vượt số đã mua | 1. Nhập số trả > số lượng đã mua | Chặn / cảnh báo, không cho vượt |
| ☐ | 7.8 Trả số âm hoặc 0 | 1. Nhập số âm hoặc 0 | Không cho nhập số âm; xử lý hợp lý với 0 |
| ☐ | 7.9 Nhập ký tự không phải số | 1. Nhập chữ/ký tự vào ô số lượng | Không nhận, giữ giá trị hợp lệ |
| ☐ | 7.10 Nút "Danh sách mặc định" | 1. Thay đổi số lượng 2. Bấm "Danh sách mặc định" | Reset danh sách món về trạng thái ban đầu |
| ☐ | 7.11 Cuộn danh sách món | 1. Mở hóa đơn nhiều món 2. Cuộn trong bảng | Cuộn mượt, hiển thị đủ món |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
