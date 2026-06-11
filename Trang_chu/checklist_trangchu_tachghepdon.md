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

1.11 Tách / ghép đơn

| STT | ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|-----|---|----------|--------------------|------------------|
| 1.11.1 | ☐ | Mở chức năng tách/ghép từ bàn đang sử dụng | 1. Từ Trang chủ, bấm vào một bàn đang có đơn (trạng thái "Đang sử dụng") 2. Tại màn hình Order, bấm icon "Tách/Ghép bàn" trên thanh công cụ (hoặc menu `...`) 3. Quan sát màn hình mở ra | Giao diện tách/ghép hiển thị; panel trái liệt kê các món của bàn hiện tại; panel phải hiển thị danh sách bàn hoặc hóa đơn đích để chọn |
| 1.11.2 | ☐ | Mở từ bàn trống (không có đơn) | 1. Từ Trang chủ, bấm vào một bàn trống 2. Tại màn hình Order, tìm và bấm icon Tách/Ghép bàn 3. Quan sát phản hồi | Hệ thống không cho mở (chặn hoặc ẩn nút), vì không có món/đơn nào để tách/ghép |
| 1.11.3 | ☐ | Giao diện hiển thị đúng thông tin bàn nguồn | 1. Mở chức năng tách/ghép từ "Bàn A" đang có 3 món 2. Quan sát panel trái | Panel trái hiển thị đúng tên bàn, danh sách món và số lượng đúng với đơn thực tế của Bàn A |
| 1.11.4 | ☐ | Chọn bàn đích để ghép | 1. Mở giao diện tách/ghép từ Bàn A 2. Tại panel phải, bấm dropdown hoặc danh sách để chọn "Bàn B" (đang trống hoặc đang có đơn) 3. Quan sát panel phải cập nhật | Panel phải hiển thị thông tin của Bàn B (danh sách món nếu đang có đơn, hoặc trống nếu bàn chưa dùng) |
| 1.11.5 | ☐ | Ghép toàn bộ đơn vào bàn đích đang trống | 1. Mở giao diện tách/ghép từ "Bàn A" (có 3 món) 2. Chọn "Bàn B" đang trống làm đích 3. Tích chọn tất cả món ở panel trái 4. Bấm nút "Ghép" / "Chuyển sang" 5. Xác nhận thao tác 6. Quan sát trạng thái Bàn A và Bàn B ngoài Trang chủ | Tất cả món của Bàn A chuyển sang Bàn B; Bàn A trở về trạng thái "trống"; Bàn B chuyển sang "Đang sử dụng" với đúng 3 món |
| 1.11.6 | ☐ | Ghép toàn bộ đơn vào bàn đích đang có đơn | 1. Mở giao diện tách/ghép từ "Bàn A" (có món X, Y) 2. Chọn "Bàn B" đang có món Z làm đích 3. Tích chọn tất cả món ở panel trái 4. Bấm "Ghép" và xác nhận 5. Quan sát hóa đơn Bàn B | Bàn B có đủ 3 món (X, Y, Z); Bàn A về trống; tổng tiền Bàn B = tổng X + Y + Z |
| 1.11.7 | ☐ | Ghép một phần món sang bàn đích | 1. Mở giao diện tách/ghép từ "Bàn A" (có món X, Y, Z) 2. Chỉ tích chọn món "X" và "Y" ở panel trái (bỏ qua Z) 3. Chọn "Bàn B" làm đích 4. Bấm "Ghép" và xác nhận 5. Quan sát cả hai bàn | Bàn B nhận được món X và Y; Bàn A "vẫn còn" món Z và tiếp tục trạng thái "Đang sử dụng" |
| 1.11.8 | ☐ | Tổng tiền sau ghép tính đúng | 1. Ghi nhận tổng tiền Bàn A (= a) và Bàn B (= b) trước khi ghép 2. Ghép toàn bộ đơn Bàn A sang Bàn B 3. Quan sát tổng tiền Bàn B sau ghép | Tổng tiền Bàn B sau ghép = a + b (cộng đúng, không mất tiền) |
| 1.11.9 | ☐ | Ghép nhiều hóa đơn trong 1 bàn vào nhau | 1. Tại Bàn A đang có 2 tab hóa đơn (HĐ1 và HĐ2) 2. Mở giao diện tách/ghép 3. Chọn ghép HĐ2 vào HĐ1 4. Xác nhận | HĐ1 chứa tất cả món của HĐ1 + HĐ2; HĐ2 bị xóa; tổng tiền HĐ1 = tổng cả hai |
| 1.11.10 | ☐ | Không cho ghép sang chính bàn nguồn | 1. Mở giao diện tách/ghép từ Bàn A 2. Thử chọn chính Bàn A làm bàn đích 3. Quan sát phản hồi | Hệ thống chặn hoặc không hiển thị Bàn A trong danh sách bàn đích |
| 1.11.11 | ☐ | Ghép khi bàn đích đang chờ thanh toán | 1. Đảm bảo Bàn B đang ở trạng thái "Chờ thanh toán" 2. Mở tách/ghép từ Bàn A, chọn Bàn B làm đích 3. Thử xác nhận ghép | Hệ thống chặn, hiển thị thông báo không thể ghép vào bàn đang chờ thanh toán |
| 1.11.12 | ☐ | Tách một phần món sang hóa đơn mới trong cùng bàn | 1. Mở giao diện tách/ghép từ "Bàn A" (có món X, Y, Z) 2. Chọn mode "Tách" 3. Tích chọn món "X" muốn tách ra 4. Chọn đích là "Hóa đơn mới" trong cùng Bàn A 5. Bấm xác nhận 6. Quan sát tab hóa đơn của Bàn A | Bàn A có "2 tab hóa đơn": HĐ1 còn Y, Z — HĐ2 chứa X; tổng tiền từng tab tính đúng theo món |
| 1.11.13 | ☐ | Tách một phần món sang bàn mới (bàn trống) | 1. Mở giao diện tách/ghép từ "Bàn A" (có món X, Y, Z) 2. Chọn mode "Tách" 3. Tích chọn món "Y" và "Z" 4. Chọn đích là "Bàn B" đang trống 5. Xác nhận 6. Quan sát cả hai bàn | Bàn A chỉ còn món X; Bàn B mới bắt đầu với món Y và Z; cả hai bàn ở trạng thái "Đang sử dụng" |
| 1.11.14 | ☐ | Tách và điều chỉnh số lượng | 1. Mở giao diện tách/ghép từ Bàn A — trong đó có "2 phần Cà phê" 2. Tách "1 phần Cà phê" sang hóa đơn mới (chỉ tách một nửa số lượng) 3. Xác nhận 4. Quan sát cả hai hóa đơn | Hóa đơn nguồn còn "1 Cà phê"; hóa đơn đích có "1 Cà phê"; tổng hai hóa đơn = đúng số lượng ban đầu |
| 1.11.15 | ☐ | Tổng tiền sau tách không thay đổi tổng gộp | 1. Ghi nhận tổng tiền Bàn A trước khi tách (= T) 2. Tách một phần món sang hóa đơn mới / Bàn B 3. Tính: tổng Bàn A sau tách + tổng hóa đơn/Bàn B | Tổng A còn lại + Tổng B mới = T (không mất tiền, không cộng dư) |
| 1.11.16 | ☐ | Không cho tách khi chỉ có 1 món, số lượng = 1 | 1. Tạo đơn tại Bàn A chỉ có "1 món", số lượng = 1 2. Mở giao diện tách/ghép 3. Thử tách món đó ra | Hệ thống chặn hoặc cảnh báo: không thể tách vì không còn món nào ở đơn gốc |
| 1.11.17 | ☐ | Tách toàn bộ món (bàn nguồn sẽ trống) | 1. Mở giao diện tách/ghép từ Bàn A có 2 món 2. Tích chọn "tất cả" món 3. Chọn đích là Bàn B trống 4. Xác nhận | Bàn A về trạng thái "trống"; Bàn B có toàn bộ 2 món; Bàn A không giữ trạng thái "Đang sử dụng" khi không còn món |
| 1.11.18 | ☐ | Bấm "Xác nhận" hoàn tất ghép/tách | 1. Thực hiện thao tác ghép hoặc tách hợp lệ (đã chọn món, chọn bàn đích) 2. Bấm nút "Xác nhận" / "Hoàn tất" 3. Quan sát kết quả | Thao tác thực hiện thành công; dữ liệu các bàn cập nhật đúng; màn hình đóng giao diện tách/ghép, trở về màn hình Order |
| 1.11.19 | ☐ | Bấm "Hủy" / "Đóng" giữa chừng | 1. Mở giao diện tách/ghép, thực hiện chọn món và chọn bàn đích 2. "Không" bấm Xác nhận, thay vào đó bấm "Hủy" hoặc "Đóng" (X) 3. Quan sát dữ liệu hai bàn | Không có thay đổi nào xảy ra; đơn tại Bàn A và Bàn B giữ nguyên như trước |
| 1.11.20 | ☐ | Xác nhận khi chưa chọn món nào | 1. Mở giao diện tách/ghép 2. Không tích chọn bất kỳ món nào 3. Bấm "Xác nhận" 4. Quan sát phản hồi | Hệ thống chặn, hiển thị thông báo yêu cầu chọn ít nhất 1 món |
| 1.11.21 | ☐ | Xác nhận khi chưa chọn bàn/hóa đơn đích | 1. Mở giao diện tách/ghép 2. Tích chọn 1 hoặc nhiều món 3. Không chọn bàn đích 4. Bấm "Xác nhận" | Hệ thống chặn, hiển thị thông báo yêu cầu chọn bàn hoặc hóa đơn đích |
| 1.11.22 | ☐ | Món đã gửi bếp vẫn tách/ghép được | 1. Tại Bàn A, thêm món X và bấm "Báo bếp" 2. Mở giao diện tách/ghép 3. Tích chọn món X (đã gửi bếp) và thực hiện ghép/tách sang Bàn B 4. Quan sát kết quả | Món đã gửi bếp vẫn được tách/ghép thành công; trạng thái "đã gửi bếp" giữ nguyên theo món sau khi chuyển sang bàn đích |
| 1.11.23 | ☐ | Tách/ghép món có ghi chú | 1. Trong đơn Bàn A, có món với "ghi chú" kèm theo (VD: "ít đường") 2. Tách/ghép món đó sang Bàn B 3. Quan sát dòng món tại Bàn B | Ghi chú theo món được giữ nguyên sau khi tách/ghép, không bị mất |
| 1.11.24 | ☐ | Tách/ghép món có tùy chọn (size, topping) | 1. Trong đơn Bàn A, có món "Trà sữa Size L + Trân châu" 2. Tách/ghép món đó sang Bàn B 3. Quan sát dòng món tại Bàn B | Tùy chọn (Size L, Trân châu) được giữ đầy đủ; giá tính đúng theo tùy chọn |
| 1.11.25 | ☐ | Tách/ghép khi đơn có giảm giá | 1. Áp giảm giá cho đơn Bàn A 2. Thực hiện tách một phần món sang Bàn B 3. Quan sát xử lý giảm giá ở cả hai đơn | Hệ thống xử lý giảm giá hợp lý (áp theo đơn gốc hoặc yêu cầu nhập lại); không bị âm tiền hoặc giảm giá trùng |
| 1.11.26 | ☐ | Tách/ghép khi đơn có hàng tặng | 1. Áp hàng tặng vào đơn Bàn A 2. Thực hiện tách/ghép toàn bộ sang Bàn B 3. Quan sát hàng tặng tại Bàn B | Hàng tặng được chuyển theo hoặc hệ thống thông báo xử lý rõ ràng; tổng tiền Bàn B không bị cộng sai |
| 1.11.27 | ☐ | Trạng thái thẻ bàn cập nhật ngay sau tách/ghép | 1. Thực hiện ghép toàn bộ Bàn A sang Bàn B 2. Bấm "Xác nhận" 3. Ngay lập tức quay về "Trang chủ" (không reload thủ công) 4. Quan sát thẻ Bàn A và Bàn B | Bàn A hiển thị "trống" (màu trắng/xám); Bàn B hiển thị "Đang sử dụng" với tổng tiền mới — không cần F5 mới thấy |
| 1.11.28 | ☐ | Tổng tiền trên thẻ bàn khớp sau ghép | 1. Ghép Bàn A (tổng a) vào Bàn B (tổng b) 2. Quay về Trang chủ, quan sát thẻ Bàn B | Tổng tiền hiển thị trên thẻ Bàn B = a + b |
| 1.11.29 | ☐ | Chưa mở ca / không có quyền | 1. Đảm bảo ca chưa mở hoặc dùng tài khoản không có quyền tách/ghép bàn 2. Vào màn hình Order của bàn đang có đơn 3. Tìm và bấm nút Tách/Ghép bàn | Hệ thống chặn thao tác, hiển thị thông báo "Chưa mở ca" hoặc "Không có quyền" |
| 1.11.30 | ☐ | Tách/ghép khi có 2 người dùng cùng bàn | 1. Mở Bàn A trên 2 tab/thiết bị khác nhau 2. Trên tab 1: mở giao diện tách/ghép, bắt đầu thao tác 3. Trên tab 2: thêm một món mới vào Bàn A cùng lúc 4. Quay lại tab 1: bấm Xác nhận | Hệ thống không bị mất dữ liệu; món thêm ở tab 2 không bị mất hoặc có cảnh báo xung đột rõ ràng |

 Sau khi hoàn tất, xuất file result_`tên file hiện tại`.md vào folder `results`. đổi ☐ thành ☑ nếu pass, đánh **x** nếu fail trong file result_`tên file hiện tại`.md.
