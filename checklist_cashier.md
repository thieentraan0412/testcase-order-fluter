# Checklist Testcase — App F&B (NASYS POS)

> Nền tảng: Ordertable riêng. Xây dựng dần qua từng video. Đổi ☐ → ☑ khi xong.

Link thực hiện https://table1.klkim.com/v2/order/cashier
tài khoản
    Cửa hàng : trong
    Tài khoản: admin   
    Mật khẩu : 147258

Hãy sử dụng google chorme và thực hiện các testcase sau, và sau đó xuất ra một file.md mới kết quả vào ô tick
Nếu testcase nào không thành công -> note thêm: lỗi mà conselog or image lỗi vào dưới testcase đó

---

## Trang chủ

### Sơ đồ bàn


| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Hiển thị danh sách bàn theo khu | 1. Mở app, đăng nhập thành công 2. Vào **Trang chủ** 3. Quan sát khu vực sơ đồ bàn | Hiện đủ các bàn, đúng số lượng theo khu |
| ☐ | Lọc tab "Bàn trống" | 1. Tại Trang chủ, nhìn vào thanh filter phía trên sơ đồ bàn 2. Bấm chọn checkbox **"Bàn trống"** 3. Quan sát danh sách bàn và số đếm trong ngoặc | Chỉ hiện bàn trống, số đếm khớp |
| ☐ | Lọc tab "Đang sử dụng" | 1. Tại Trang chủ, bỏ các filter đang chọn 2. Bấm chọn checkbox **"Đang sử dụng"** 3. Quan sát danh sách bàn và số đếm | Chỉ hiện bàn đang dùng, số đếm khớp |
| ☐ | Lọc tab "Chờ xác nhận" | 1. Tại Trang chủ, bỏ các filter đang chọn 2. Bấm chọn checkbox **"Chờ xác nhận"** 3. Quan sát danh sách bàn | Chỉ hiện đơn chờ xác nhận |
| ☐ | Lọc tab "Chờ thanh toán" | 1. Tại Trang chủ, bỏ các filter đang chọn 2. Bấm chọn checkbox **"Chờ thanh toán"** 3. Quan sát danh sách bàn | Chỉ hiện đơn chờ thanh toán |
| ☐ | Lọc theo khu (khu 1 / khu 2) | 1. Tại Trang chủ, tìm dropdown **"Tất cả (39)"** ở góc phải thanh công cụ 2. Bấm vào dropdown, chọn một khu cụ thể (VD: Khu 1) 3. Quan sát danh sách bàn hiển thị | Chỉ hiện bàn thuộc khu đã chọn |
| ☐ | Đổi số cột hiển thị (6 cột) | 1. Tại Trang chủ, tìm dropdown **"6 cột"** trên thanh công cụ 2. Bấm vào dropdown, chọn số cột khác (VD: 4 cột hoặc 8 cột) 3. Quan sát lưới bàn thay đổi bố cục | Lưới bàn bố trí lại đúng số cột đã chọn |
| ☐ | Đổi giao diện (1 / 2 / 3) | 1. Tại Trang chủ, tìm nút **"Giao diện 3"** trên thanh công cụ 2. Bấm nút để chuyển lần lượt: Giao diện 1 → 2 → 3 3. Quan sát kiểu hiển thị thẻ bàn sau mỗi lần đổi | Kiểu hiển thị thẻ bàn thay đổi tương ứng |
| ☐ | Thẻ bàn hiển thị thông tin | 1. Tại Trang chủ, lọc tab **"Đang sử dụng"** 2. Quan sát một thẻ bàn đang hoạt động (thẻ màu vàng/cam) 3. Kiểm tra từng thông tin: tên bàn, timer, icon hóa đơn, icon số khách, tổng tiền, nhãn trạng thái | Đúng tên, timer, số hóa đơn, số khách, tổng tiền, trạng thái |
| ☐ | Tổng tiền trên thẻ bàn | 1. Bấm vào bàn đang sử dụng để vào màn hình Order 2. Ghi nhận tổng tiền thanh toán hiển thị (đã tính thuế) 3. Bấm **Back** về Trang chủ 4. So sánh tổng tiền trên thẻ bàn với con số vừa ghi nhận | Khớp tổng đơn của bàn (đã gồm thuế) |
| ☐ | Trạng thái "Chưa báo bếp" | 1. Bấm vào bàn đang sử dụng, thêm ít nhất 1 món mới vào đơn 2. **Không** bấm nút "Gửi bếp / Báo bếp" 3. Back về Trang chủ 4. Quan sát thẻ bàn đó | Hiển thị nhãn "Chưa báo bếp" trên thẻ bàn |
| ☐ | Nút "Xác nhận" trên thẻ | 1. Tại Trang chủ, lọc tab **"Chờ xác nhận"** 2. Tìm thẻ bàn có nút **"Xác nhận"** 3. Bấm nút **"Xác nhận"** trực tiếp trên thẻ bàn 4. Quan sát trạng thái thẻ bàn sau thao tác | Đơn được xác nhận, trạng thái cập nhật sang "Đang sử dụng" |
| ☐ | Bấm vào bàn | 1. Tại Trang chủ, chọn bất kỳ thẻ bàn nào 2. Bấm vào vùng thân thẻ bàn 3. Quan sát màn hình mở ra | Mở màn hình Order của bàn đó |
| ☐ | Thêm đơn mang về | 1. Tại Trang chủ, tìm thẻ **"Bàn mang về"** (thẻ có icon Takeaway, vị trí đầu danh sách) 2. Bấm vào thẻ đó 3. Quan sát màn hình mở ra | Mở màn hình Order ở chế độ Mang đi |
| ☐ | Số liệu các tab nhất quán | 1. Tại Trang chủ, ghi lại số đếm từng tab: **Bàn trống (n1)**, **Đang sử dụng (n2)**, **Chờ xác nhận (n3)**, **Chờ thanh toán (n4)** 2. Tính tổng: n1 + n2 + n3 + n4 3. So sánh với số hiển thị tại tab **"Tất cả"** | Tổng các tab = tổng tất cả |

### Menu (Thực đơn)

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Hiển thị danh mục món | 1. Từ Trang chủ, bấm vào bất kỳ bàn nào để vào màn hình Order 2. Quan sát thanh tab danh mục phía trên lưới món (TẤT CẢ, BÁN CHẠY, MÓN MỚI...) | Hiện đủ các tab danh mục |
| ☐ | Lọc theo danh mục | 1. Tại màn hình Order, bấm vào một tab danh mục bất kỳ (VD: NƯỚC NGỌT) 2. Quan sát lưới món thay đổi | Chỉ hiện món thuộc danh mục đã chọn |
| ☐ | Tìm món (F1) | 1. Tại màn hình Order, bấm vào ô "Tìm và chọn món (F1)" 2. Gõ từ khóa tên món (thử cả có dấu và không dấu) 3. Quan sát kết quả lọc | Lọc đúng theo từ khóa, kể cả tiếng Việt có dấu |
| ☐ | Ẩn/hiện hình ảnh món | 1. Tại màn hình Order, tìm toggle "Ẩn hình ảnh" phía trên lưới món 2. Bật toggle → quan sát 3. Tắt toggle → quan sát lại | Lưới ẩn/hiện ảnh tương ứng |
| ☐ | Đổi số cột hiển thị món | 1. Tại màn hình Order, tìm dropdown "6 cột" phía trên lưới món 2. Bấm vào dropdown, chọn số cột khác 3. Quan sát bố cục lưới món | Bố trí lại đúng số cột đã chọn |
| ☐ | Phân trang (1/5, 2/5...) | 1. Tại màn hình Order, quan sát chỉ số trang hiện tại (VD: 1/5) 2. Bấm mũi tên sang phải để chuyển sang trang tiếp 3. Quan sát món hiển thị và chỉ số trang cập nhật | Hiện trang tiếp theo, số trang đúng |
| ☐ | Giá món | 1. Tại màn hình Order, quan sát giá hiển thị bên dưới từng món trong lưới 2. So sánh với giá thực tế đã cấu hình | Hiển thị đúng định dạng VND |

### Modal tùy chọn món

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Mở modal khi món có tùy chọn | 1. Tại màn hình Order, bấm vào một món có cấu hình tùy chọn (thuộc tính hoặc món thêm) 2. Quan sát màn hình | Hiện modal "Chọn món kèm theo" |
| ☐ | Chọn thuộc tính (Size, độ ngọt...) | 1. Trong modal, tìm nhóm thuộc tính (VD: Size, Độ ngọt) 2. Bấm chọn một giá trị bất kỳ trong nhóm 3. Quan sát lựa chọn được ghi nhận và giá thay đổi nếu có | Ghi nhận lựa chọn, giá cập nhật nếu giá trị đó có phụ thu |
| ☐ | Chọn món thêm | 1. Trong modal, tìm nhóm "Món thêm" (VD: Nước ngọt) 2. Tích chọn một hoặc nhiều món thêm 3. Điều chỉnh số lượng từng món thêm nếu cần | Ghi nhận đúng các món thêm và số lượng đã chọn |
| ☐ | Tăng/giảm số lượng | 1. Trong modal, tìm nút +/- bên cạnh tên món chính 2. Bấm + để tăng, bấm - để giảm 3. Thử giảm về 1 rồi tiếp tục bấm - | Thay đổi đúng, không xuống dưới 1 |
| ☐ | Nhập ghi chú | 1. Trong modal, tìm ô "Ghi chú" phía cuối 2. Nhập nội dung ghi chú bất kỳ 3. Bấm "Chọn" để xác nhận 4. Quan sát dòng món trong hóa đơn | Ghi chú lưu kèm theo dòng món |
| ☐ | Bấm "Chọn" | 1. Trong modal, chọn đủ các tùy chọn mong muốn 2. Bấm nút "Chọn" 3. Quan sát hóa đơn bên phải | Món cùng toàn bộ tùy chọn được thêm vào hóa đơn |
| ☐ | Bấm "Đóng" | 1. Mở modal của bất kỳ món có tùy chọn nào 2. Không chọn gì, bấm nút "Đóng" 3. Quan sát hóa đơn | Đóng modal, không thêm món vào hóa đơn |
| ☐ | Tùy chọn hiển thị trong dòng món | 1. Sau khi bấm "Chọn", quan sát dòng món vừa thêm trong hóa đơn 2. Kiểm tra thông tin tùy chọn hiển thị bên dưới tên món | Hiển thị rõ các tùy chọn đã chọn (VD: Size S, Nước ngọt: Pepsi 5%) |

### Hóa đơn / Giỏ hàng

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Thêm món vào hóa đơn | 1. Tại màn hình Order, bấm vào bất kỳ món nào trong lưới thực đơn 2. Quan sát panel hóa đơn bên phải | Dòng món xuất hiện trong hóa đơn, số đếm "Tổng tiền (n)" tăng |
| ☐ | Tăng số lượng (+) | 1. Trong hóa đơn, tìm dòng món bất kỳ 2. Bấm nút + bên cạnh số lượng 3. Quan sát số lượng và cột Thành tiền | Thành tiền = đơn giá × số lượng mới |
| ☐ | Giảm số lượng (−) | 1. Trong hóa đơn, tìm dòng món có số lượng ≥ 2 2. Bấm nút − liên tục 3. Thử giảm khi số lượng đang là 1 | Số lượng giảm đúng; khi về 0 hệ thống xử lý đúng (xóa món hoặc chặn) |
| ☐ | Xóa món (nút X) | 1. Trong hóa đơn, tìm dòng món bất kỳ 2. Bấm nút X đỏ ở cuối dòng 3. Quan sát hóa đơn và tổng tiền | Dòng món bị xóa, tổng tiền cập nhật |
| ☐ | Sửa đơn giá thủ công | 1. Trong hóa đơn, bấm vào icon bút (chỉnh sửa) tại cột Đơn giá của một món 2. Nhập giá mới 3. Xác nhận và quan sát Thành tiền, Tổng tiền | Tổng cập nhật đúng theo giá mới |
| ☐ | Ghi chú từng món | 1. Trong hóa đơn, tích vào checkbox "Ghi chú" bên dưới tên món 2. Nhập nội dung ghi chú 3. Quan sát dòng món sau khi lưu | Ghi chú lưu và hiển thị theo đúng dòng món đó |
| ☐ | Tổng tiền (tạm tính) | 1. Thêm nhiều món vào hóa đơn 2. Tính tay: Σ (đơn giá × số lượng) của từng dòng 3. So sánh với "Tổng tiền" hiển thị (chưa cộng thuế, phụ thu) | Tổng tiền = Σ (đơn giá × SL) |
| ☐ | Thuế theo từng món | 1. Thêm món có cấu hình thuế riêng (VD: món VAT 0%, TOPPING 10%) 2. Quan sát dòng "Thuế sản phẩm" ở phần tổng hóa đơn | Thuế tính đúng theo % đã cấu hình từng món |
| ☐ | Thuế theo cả bill | 1. Thêm món vào hóa đơn 2. Kiểm tra cấu hình thuế áp theo toàn bill 3. Quan sát dòng thuế trong phần tổng | Thuế tính đúng theo setting cả bill |
| ☐ | Kết hợp thuế món + bill | 1. Thêm món vừa có thuế riêng, vừa có thuế bill 2. Quan sát tổng thuế hiển thị | Không tính trùng hoặc sai, thuế chỉ tính một lần đúng quy tắc |
| ☐ | Tổng tiền thanh toán | 1. Thêm món, nhập phụ thu và giảm giá 2. Tính tay: Tổng tiền + Phụ thu − Giảm giá + Thuế 3. So sánh với "Tổng tiền thanh toán" hiển thị (màu đỏ) | Tổng tiền thanh toán = Tổng tiền + Phụ thu − Giảm giá + Thuế |
| ☐ | Phụ thu | 1. Trong hóa đơn, bấm icon bút tại dòng "Phụ thu" 2. Nhập giá trị phụ thu 3. Quan sát Tổng tiền thanh toán | Phụ thu cộng đúng vào tổng |
| ☐ | Giảm giá | 1. Trong hóa đơn, bấm icon bút tại dòng "Giảm giá" 2. Nhập giá trị hoặc % giảm 3. Quan sát Tổng tiền thanh toán | Giảm giá trừ đúng vào tổng |
| ☐ | Gợi ý nhanh tiền mặt | 1. Tại hóa đơn có tổng tiền thanh toán xác định 2. Quan sát các nút gợi ý số tiền (VD: 120,000đ, 150,000đ, 200,000đ) phía trên ô Tiền mặt | Các giá trị gợi ý đều ≥ tổng thanh toán và là mệnh giá hợp lý |
| ☐ | Combo / Set menu | 1. Trong lưới thực đơn, tìm và bấm vào một món Combo hoặc Set menu 2. Quan sát dòng món trong hóa đơn | Hiển thị đúng tên combo, thành phần kèm theo và giá |
| ☐ | Chọn khách hàng | 1. Trong hóa đơn, bấm vào dropdown "Khách lẻ" góc trên phải panel 2. Tìm và chọn một khách hàng có sẵn 3. Quan sát thông tin khách trên hóa đơn | Thông tin khách hàng gắn vào hóa đơn |
| ☐ | Nhiều hóa đơn / 1 bàn | 1. Tại màn hình Order của một bàn, bấm nút + bên cạnh tab hóa đơn hiện tại 2. Thêm món khác nhau vào từng tab 3. Chuyển qua lại giữa 2 tab | Mỗi tab là hóa đơn độc lập, tổng tiền không ảnh hưởng nhau |
| ☐ | Đơn các bàn độc lập | 1. Thêm món vào Bàn A, quay về Trang chủ 2. Vào Bàn B, thêm món khác 3. Quay lại Bàn A kiểm tra | Hóa đơn Bàn A không bị lẫn món của Bàn B |
| ☐ | Hóa đơn trống | 1. Tại màn hình Order, tạo hóa đơn mới (bấm +) hoặc vào bàn chưa có món 2. Quan sát panel hóa đơn | Hiển thị thông báo "Bạn chưa thêm sản phẩm nào", tổng tiền = 0 |
| ☐ | Nhân viên phụ trách | 1. Tại màn hình Order, quan sát tên nhân viên hiển thị trong hóa đơn (VD: "Nhân viên: Admin Master") 2. So sánh với tài khoản đang đăng nhập | Hiển thị đúng tên nhân viên đang thao tác |

### Hoa hồng nhân viên

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Bấm "Hoa hồng" trên dòng món | 1. Trong hóa đơn, tìm dòng món có link "% Hoa hồng" bên dưới tên món 2. Bấm vào link đó 3. Quan sát màn hình | Mở modal "Hoa hồng nhân viên" |
| ☐ | Modal hiện các mục hoa hồng | 1. Mở modal Hoa hồng của bất kỳ món nào 2. Quan sát danh sách các mục trong modal (VD: 123 (10%), 456 (5%)) | Hiện đủ các mục kèm tên và % hoa hồng đã cấu hình |
| ☐ | Chọn nhân viên mỗi mục | 1. Trong modal, bấm vào dropdown bên cạnh một mục hoa hồng 2. Chọn một nhân viên từ danh sách xổ xuống | Nhân viên được chọn và ghi nhận vào mục đó |
| ☐ | Gán nhiều NV nhiều mục | 1. Trong modal, lần lượt chọn nhân viên khác nhau cho từng mục hoa hồng 2. Bấm "Xác nhận" | Tất cả các mục đều gán được đồng thời, không bị ghi đè |
| ☐ | Bấm "Xác nhận" | 1. Trong modal, chọn nhân viên cho ít nhất một mục 2. Bấm nút "Xác nhận" 3. Quan sát dòng món trong hóa đơn | Thông tin hoa hồng hiển thị trên dòng món |
| ☐ | Bấm "Đóng" | 1. Mở modal Hoa hồng, chọn nhân viên vào một mục 2. Bấm nút "Đóng" thay vì "Xác nhận" 3. Mở lại modal kiểm tra | Thay đổi không được lưu, dữ liệu cũ giữ nguyên |
| ☐ | Mở lại modal để sửa | 1. Sau khi đã gán hoa hồng và bấm "Xác nhận", bấm lại "% Hoa hồng" trên dòng món đó 2. Thay đổi nhân viên hoặc xóa chọn 3. Bấm "Xác nhận" | Cập nhật được nhân viên mới, dữ liệu cũ bị thay thế |
| ☐ | Hoa hồng theo món độc lập | 1. Gán hoa hồng cho Món A, bấm "Xác nhận" 2. Mở modal Hoa hồng của Món B (chưa gán) 3. Quan sát modal Món B | Modal Món B trống, không bị ảnh hưởng từ Món A |
| ☐ | Tính tiền hoa hồng | 1. Gán nhân viên cho mục có % xác định (VD: 10%) trên món có giá cụ thể (VD: 50,000đ) 2. Tính tay: 10% × 50,000đ = 5,000đ 3. Kiểm tra giá trị hoa hồng ghi nhận trong hệ thống | Hoa hồng = % × giá trị món, tính đúng |
| ☐ | Để trống nhân viên | 1. Mở modal Hoa hồng 2. Không chọn nhân viên cho bất kỳ mục nào 3. Bấm "Xác nhận" | Hệ thống cho phép xác nhận, không báo lỗi bắt buộc |
| ☐ | 1 NV gán nhiều mục | 1. Trong modal, chọn cùng một nhân viên cho cả 2 mục hoa hồng (VD: 123 (10%) và 456 (5%)) 2. Bấm "Xác nhận" 3. Kiểm tra tổng hoa hồng của nhân viên đó trong link "https://table.nasys.vn/v2/report/end-day?type=commission" vào mục "Báo cáo hoa hồng.| số tiền nhận được phải đúng với %

### In bếp / Thanh toán

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | In phiếu Bếp/Bar (báo bếp) | 1. Thêm ít nhất 1 món vào hóa đơn (trạng thái "Chờ báo bếp") 2. Bấm nút "Báo bếp" (màu cam) ở dưới cùng 3. Quan sát trạng thái từng dòng món trong hóa đơn | Trạng thái món chuyển từ "Chờ báo bếp" sang đã gửi bếp |
| ☐ | Tạm tính | 1. Trong hóa đơn có ít nhất 1 món, bấm nút "Tạm tính" (màu xanh lá) 2. Quan sát phiếu tạm tính hiển thị hoặc in ra | Phiếu tạm tính hiển thị đúng tổng tiền hiện tại |
| ☐ | Thanh toán tiền mặt | 1. Trong hóa đơn có món, bấm nút "Thanh toán" 2. Chọn phương thức "Tiền mặt" 3. Nhập số tiền khách đưa, xác nhận thanh toán 4. Quay lại Trang chủ quan sát bàn | Đơn hoàn tất, bàn về trạng thái trống |
| ☐ | Thanh toán chuyển khoản | 1. Trong hóa đơn có món, bấm nút "Thanh toán" 2. Chọn phương thức "Chuyển khoản" 3. Xác nhận thanh toán 4. Quan sát kết quả | Đơn hoàn tất, luồng chuyển khoản hoạt động đúng |
| ☐ | Thanh toán quẹt thẻ | 1. Trong hóa đơn có món, bấm nút "Thanh toán" 2. Chọn phương thức "Quẹt Thẻ" 3. Xác nhận thanh toán 4. Quan sát kết quả | Đơn hoàn tất, luồng quẹt thẻ hoạt động đúng |
| ☐ | Thanh toán QR tự động | 1. Trong hóa đơn có món, bấm nút "Thanh toán" 2. Chọn phương thức "QR Tự động" 3. Quan sát mã QR sinh ra 4. Giả lập hoặc thực hiện thanh toán qua QR | Mã QR được sinh, sau khi thanh toán đơn hoàn tất |
| ☐ | Tiền thừa | 1. Trong hóa đơn, xem Tổng tiền thanh toán (VD: 115,000đ) 2. Bấm "Thanh toán" → chọn Tiền mặt 3. Nhập số tiền lớn hơn tổng (VD: 150,000đ) 4. Quan sát số tiền thừa hiển thị | Tiền thừa = tiền nhận − tổng thanh toán, tính đúng |
| ☐ | Chặn hóa đơn trống | 1. Tạo hóa đơn mới, không thêm bất kỳ món nào 2. Bấm nút "Thanh toán" 3. Quan sát phản hồi | Hệ thống chặn, hiển thị thông báo lỗi, không cho thanh toán |
| ☐ | Hóa đơn điện tử | 1. Hoàn tất thanh toán một đơn hàng 2. Tại màn hình xác nhận hoặc lịch sử, tìm chức năng "Hóa đơn điện tử" 3. Bấm phát hành và quan sát kết quả | Hóa đơn điện tử được phát hành đúng |

### Xác nhận đơn (tại bàn / QR / mang về)

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Tab "Chờ xác nhận" hiển thị đơn chờ | 1. Tại Trang chủ, bấm chọn checkbox "Chờ xác nhận" 2. Quan sát danh sách bàn lọc ra 3. Kiểm tra các đơn hiển thị | Hiện đúng các đơn đang chờ thu ngân xác nhận |
| ☐ | Xác nhận đơn tại bàn (gửi từ tablet/mobile) | 1. Đảm bảo có đơn được nhân viên gửi từ thiết bị tablet/mobile 2. Tại Trang chủ, lọc "Chờ xác nhận", tìm bàn tương ứng 3. Bấm vào thẻ bàn → bấm "Xác nhận" 4. Quan sát trạng thái bàn | Đơn được tiếp nhận vào bàn, trạng thái chuyển sang "Đang sử dụng" |
| ☐ | Xác nhận đơn QR (khách quét QR tại bàn) | 1. Khách quét mã QR tại bàn và đặt món 2. Tại Trang chủ, lọc "Chờ xác nhận", tìm bàn của khách 3. Bấm vào thẻ bàn → bấm "Xác nhận" 4. Quan sát trạng thái | Đơn QR của khách được tiếp nhận vào bàn |
| ☐ | Xác nhận đơn mang về | 1. Có đơn mang về đang chờ xác nhận 2. Tại Trang chủ, lọc "Chờ xác nhận", tìm thẻ đơn mang về 3. Bấm "Xác nhận" 4. Quan sát kết quả | Đơn mang về được tiếp nhận vào hệ thống |
| ☐ | Từ chối đơn | 1. Tại Trang chủ, lọc "Chờ xác nhận", tìm bàn có đơn chờ 2. Bấm vào thẻ bàn, chọn "Từ chối" thay vì "Xác nhận" 3. Quan sát kết quả | Đơn bị từ chối, không tiếp nhận vào bàn |
| ☐ | Tìm kiếm/chọn bàn cần xác nhận | 1. Tại Trang chủ đang lọc "Chờ xác nhận", dùng dropdown khu hoặc tìm kiếm để lọc bàn cụ thể 2. Quan sát kết quả | Lọc đúng bàn/đơn cần tìm |
| ☐ | Sau xác nhận, số đếm "Chờ xác nhận" giảm | 1. Ghi nhận số đếm trên checkbox "Chờ xác nhận" (VD: Chờ xác nhận (3)) 2. Xác nhận một đơn 3. Quan sát lại số đếm trên checkbox | Số đếm giảm đúng 1 đơn sau mỗi lần xác nhận |

### Gửi bếp

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Gửi bếp sau khi chọn món | 1. Thêm ít nhất 1 món vào hóa đơn 2. Bấm nút "Báo bếp" (màu cam) 3. Quan sát trạng thái dòng món | Trạng thái món chuyển sang "chờ chế biến", không còn nhãn "Chờ báo bếp" |
| ☐ | Món chưa gửi bếp | 1. Thêm món vào hóa đơn 2. Chưa bấm "Báo bếp" 3. Quan sát nhãn hiển thị trên dòng món và thẻ bàn ngoài Trang chủ | Hiển thị "Chờ báo bếp" trên dòng món |
| ☐ | Gửi bếp khi giỏ trống | 1. Tạo hóa đơn mới hoặc xóa hết món 2. Bấm nút "Báo bếp" 3. Quan sát phản hồi | Hệ thống chặn, không gửi bếp |
| ☐ | Gửi bếp chỉ áp món mới thêm | 1. Thêm Món A, bấm "Báo bếp" 2. Tiếp tục thêm Món B vào cùng hóa đơn 3. Bấm "Báo bếp" lần 2 4. Quan sát trạng thái từng dòng món | Chỉ Món B được gửi bếp, Món A không bị gửi lại trùng |

### Chuyển bàn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Mở chức năng chuyển bàn từ bàn đang dùng | 1. Từ Trang chủ, bấm vào một bàn đang có đơn (trạng thái "Đang sử dụng") 2. Tại màn hình Order, bấm icon **"Chuyển bàn"** trên thanh công cụ (hoặc menu `...` → chọn Chuyển bàn) 3. Quan sát màn hình mở ra | Hiện danh sách bàn đích để chọn |
| ☐ | Bàn đích (bàn trống) hiển thị màu vàng | 1. Mở chức năng chuyển bàn từ bàn đang dùng 2. Quan sát màu sắc các thẻ bàn trong danh sách bàn đích 3. So sánh màu thẻ bàn trống và bàn đang dùng | Các bàn trống hiển thị màu vàng để gợi ý; bàn đang dùng hiển thị màu khác (xám hoặc tối) |
| ☐ | Chọn bàn trống để chuyển | 1. Mở chức năng chuyển bàn từ **Bàn A** đang có đơn 2. Trong danh sách bàn đích, bấm chọn **Bàn B** đang trống (màu vàng) 3. Xác nhận chuyển bàn 4. Quan sát trạng thái Bàn A và Bàn B ngoài Trang chủ | Toàn bộ đơn của Bàn A chuyển sang Bàn B; Bàn A trở về trạng thái **trống**; Bàn B chuyển sang **"Đang sử dụng"** với đúng dữ liệu đơn cũ |
| ☐ | Chỉ cho chọn bàn trống | 1. Mở chức năng chuyển bàn từ Bàn A 2. Trong danh sách bàn đích, thử bấm vào một bàn **đang sử dụng** 3. Quan sát phản hồi | Hệ thống không cho chọn bàn đang dùng; thẻ bàn đó bị mờ, không thể bấm hoặc hiện thông báo không hợp lệ |
| ☐ | Chưa mở ca / không có quyền | 1. Đảm bảo ca chưa mở hoặc dùng tài khoản không có quyền chuyển bàn 2. Vào màn hình Order của bàn đang có đơn 3. Tìm và bấm nút Chuyển bàn | Hệ thống chặn thao tác, hiển thị thông báo "Chưa mở ca" hoặc "Không có quyền" |
| ☐ | Dữ liệu đơn giữ nguyên sau chuyển bàn | 1. Ghi nhận danh sách món, số lượng, ghi chú và tổng tiền tại Bàn A trước khi chuyển 2. Chuyển sang Bàn B trống 3. Vào màn hình Order của Bàn B, kiểm tra lại toàn bộ thông tin | Danh sách món, số lượng, ghi chú, tổng tiền tại Bàn B khớp hoàn toàn với Bàn A trước khi chuyển |
| ☐ | Trạng thái thẻ bàn cập nhật ngay sau chuyển | 1. Thực hiện chuyển Bàn A sang Bàn B 2. Xác nhận xong, ngay lập tức quay về **Trang chủ** (không reload thủ công) 3. Quan sát thẻ Bàn A và Bàn B | Bàn A hiển thị **trống** ngay lập tức; Bàn B hiển thị **"Đang sử dụng"** với đúng tổng tiền — không cần F5 mới thấy |
| ☐ | Chuyển bàn khi món đã gửi bếp | 1. Tại Bàn A, thêm món và bấm **"Báo bếp"** (món đã gửi bếp) 2. Mở chức năng chuyển bàn, chọn Bàn B trống 3. Xác nhận chuyển 4. Vào Bàn B kiểm tra trạng thái món | Món chuyển sang Bàn B vẫn giữ trạng thái "đã gửi bếp", không bị reset về "Chưa báo bếp" |
| ☐ | Hủy thao tác chuyển bàn giữa chừng | 1. Mở chức năng chuyển bàn từ Bàn A 2. Danh sách bàn đích hiện ra, nhưng **không chọn bàn nào** 3. Bấm **"Hủy"** hoặc **"Đóng"** (X) 4. Quan sát dữ liệu Bàn A | Không có thay đổi nào xảy ra; đơn tại Bàn A giữ nguyên như trước |

### Gộp bàn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Mở chức năng gộp bàn | 1. Từ Trang chủ, bấm vào một bàn đang có đơn 2. Tại màn hình Order, bấm icon **"Gộp bàn"** trên thanh công cụ (hoặc menu `...` → chọn Gộp bàn) 3. Quan sát màn hình mở ra | Hiện danh sách bàn để gộp; các bàn đang sử dụng được hiển thị để chọn |
| ☐ | Gộp đơn vào 2+ bàn đang hoạt động | 1. Mở chức năng gộp bàn từ **Bàn A** đang có đơn 2. Trong danh sách, chọn thêm **Bàn B** và **Bàn C** (cũng đang có đơn) 3. Xác nhận gộp 4. Quan sát kết quả tại Bàn A | Bàn A hiển thị thông tin đơn của cả 3 bàn (A + B + C); Bàn B và Bàn C về trạng thái trống; tổng tiền Bàn A = tổng A + B + C |
| ☐ | Đơn đã thanh toán không cho gộp | 1. Mở chức năng gộp bàn 2. Trong danh sách bàn, tìm bàn đã hoàn tất thanh toán 3. Thử chọn bàn đó để gộp 4. Quan sát phản hồi | Hệ thống không cho chọn bàn đã thanh toán; thẻ bàn đó bị mờ hoặc hiện thông báo không hợp lệ |
| ☐ | Xác nhận hoàn tất gộp | 1. Mở chức năng gộp bàn từ Bàn A 2. Chọn Bàn B đang có đơn để gộp vào 3. Bấm nút **"Xác nhận"** / **"Hoàn tất"** 4. Quan sát trạng thái tất cả các bàn liên quan ngoài Trang chủ | Trạng thái các bàn cập nhật đúng: bàn được gộp vào (Bàn A) giữ trạng thái "Đang sử dụng"; các bàn bị gộp (Bàn B) về trạng thái trống |
| ☐ | Tổng tiền sau gộp tính đúng | 1. Ghi nhận tổng tiền Bàn A (= a) và Bàn B (= b) trước khi gộp 2. Gộp Bàn B vào Bàn A 3. Quan sát tổng tiền Bàn A sau gộp | Tổng tiền Bàn A sau gộp = a + b (không mất tiền, không cộng dư) |
| ☐ | Danh sách món sau gộp hiển thị đúng | 1. Bàn A có món X; Bàn B có món Y 2. Gộp Bàn B vào Bàn A 3. Vào màn hình Order của Bàn A, quan sát danh sách món | Bàn A hiển thị đầy đủ cả món X lẫn món Y; không bị mất hoặc trùng dòng |
| ☐ | Gộp bàn khi các bàn đã gửi bếp | 1. Tại Bàn A và Bàn B, thêm món và bấm **"Báo bếp"** tại từng bàn 2. Thực hiện gộp Bàn B vào Bàn A 3. Quan sát trạng thái từng dòng món tại Bàn A sau gộp | Các món đã gửi bếp từ Bàn B vẫn giữ trạng thái "đã gửi bếp" sau khi gộp vào Bàn A |
| ☐ | Gộp bàn giữ nguyên ghi chú và tùy chọn món | 1. Tại Bàn B có món kèm ghi chú (VD: "ít đá") và tùy chọn (VD: Size L) 2. Gộp Bàn B vào Bàn A 3. Quan sát dòng món từ Bàn B trong hóa đơn Bàn A | Ghi chú và tùy chọn của món từ Bàn B được giữ nguyên, không bị mất sau khi gộp |
| ☐ | Hủy thao tác gộp giữa chừng | 1. Mở chức năng gộp bàn từ Bàn A 2. Chọn Bàn B để gộp 3. **Không** bấm Xác nhận, thay vào đó bấm **"Hủy"** hoặc **"Đóng"** (X) 4. Quan sát dữ liệu Bàn A và Bàn B | Không có thay đổi nào xảy ra; đơn tại Bàn A và Bàn B giữ nguyên như trước |
| ☐ | Chưa mở ca / không có quyền | 1. Đảm bảo ca chưa mở hoặc dùng tài khoản không có quyền gộp bàn 2. Vào màn hình Order của bàn đang có đơn 3. Tìm và bấm nút Gộp bàn | Hệ thống chặn thao tác, hiển thị thông báo "Chưa mở ca" hoặc "Không có quyền" |
| ☐ | Trạng thái thẻ bàn cập nhật ngay sau gộp | 1. Gộp Bàn B vào Bàn A, bấm Xác nhận 2. Ngay lập tức quay về **Trang chủ** (không reload thủ công) 3. Quan sát thẻ Bàn A và Bàn B | Bàn B hiển thị **trống** ngay lập tức; Bàn A hiển thị tổng tiền mới — không cần F5 mới thấy |


### Tách / ghép đơn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Mở chức năng tách/ghép từ bàn đang sử dụng | 1. Từ Trang chủ, bấm vào một bàn đang có đơn (trạng thái "Đang sử dụng") 2. Tại màn hình Order, bấm icon **Tách/Ghép bàn** trên thanh công cụ (hoặc menu `...`) 3. Quan sát màn hình mở ra | Giao diện tách/ghép hiển thị; panel trái liệt kê các món của bàn hiện tại; panel phải hiển thị danh sách bàn hoặc hóa đơn đích để chọn |
| ☐ | Mở từ bàn trống (không có đơn) | 1. Từ Trang chủ, bấm vào một bàn trống 2. Tại màn hình Order, tìm và bấm icon Tách/Ghép bàn 3. Quan sát phản hồi | Hệ thống không cho mở (chặn hoặc ẩn nút), vì không có món/đơn nào để tách/ghép |
| ☐ | Giao diện hiển thị đúng thông tin bàn nguồn | 1. Mở chức năng tách/ghép từ **Bàn A** đang có 3 món 2. Quan sát panel trái | Panel trái hiển thị đúng tên bàn, danh sách món và số lượng đúng với đơn thực tế của Bàn A |
| ☐ | Chọn bàn đích để ghép | 1. Mở giao diện tách/ghép từ Bàn A 2. Tại panel phải, bấm dropdown hoặc danh sách để chọn **Bàn B** (đang trống hoặc đang có đơn) 3. Quan sát panel phải cập nhật | Panel phải hiển thị thông tin của Bàn B (danh sách món nếu đang có đơn, hoặc trống nếu bàn chưa dùng) |
| ☐ | Ghép toàn bộ đơn vào bàn đích đang trống | 1. Mở giao diện tách/ghép từ **Bàn A** (có 3 món) 2. Chọn **Bàn B** đang trống làm đích 3. Tích chọn tất cả món ở panel trái 4. Bấm nút **"Ghép"** / **"Chuyển sang"** 5. Xác nhận thao tác 6. Quan sát trạng thái Bàn A và Bàn B ngoài Trang chủ | Tất cả món của Bàn A chuyển sang Bàn B; Bàn A trở về trạng thái **trống**; Bàn B chuyển sang **"Đang sử dụng"** với đúng 3 món |
| ☐ | Ghép toàn bộ đơn vào bàn đích đang có đơn | 1. Mở giao diện tách/ghép từ **Bàn A** (có món X, Y) 2. Chọn **Bàn B** đang có món Z làm đích 3. Tích chọn tất cả món ở panel trái 4. Bấm **"Ghép"** và xác nhận 5. Quan sát hóa đơn Bàn B | Bàn B có đủ 3 món (X, Y, Z); Bàn A về trống; tổng tiền Bàn B = tổng X + Y + Z |
| ☐ | Ghép một phần món sang bàn đích | 1. Mở giao diện tách/ghép từ **Bàn A** (có món X, Y, Z) 2. Chỉ tích chọn món **X** và **Y** ở panel trái (bỏ qua Z) 3. Chọn **Bàn B** làm đích 4. Bấm **"Ghép"** và xác nhận 5. Quan sát cả hai bàn | Bàn B nhận được món X và Y; Bàn A **vẫn còn** món Z và tiếp tục trạng thái "Đang sử dụng" |
| ☐ | Tổng tiền sau ghép tính đúng | 1. Ghi nhận tổng tiền Bàn A (= a) và Bàn B (= b) trước khi ghép 2. Ghép toàn bộ đơn Bàn A sang Bàn B 3. Quan sát tổng tiền Bàn B sau ghép | Tổng tiền Bàn B sau ghép = a + b (cộng đúng, không mất tiền) |
| ☐ | Ghép nhiều hóa đơn trong 1 bàn vào nhau | 1. Tại Bàn A đang có 2 tab hóa đơn (HĐ1 và HĐ2) 2. Mở giao diện tách/ghép 3. Chọn ghép HĐ2 vào HĐ1 4. Xác nhận | HĐ1 chứa tất cả món của HĐ1 + HĐ2; HĐ2 bị xóa; tổng tiền HĐ1 = tổng cả hai |
| ☐ | Không cho ghép sang chính bàn nguồn | 1. Mở giao diện tách/ghép từ Bàn A 2. Thử chọn chính Bàn A làm bàn đích 3. Quan sát phản hồi | Hệ thống chặn hoặc không hiển thị Bàn A trong danh sách bàn đích |
| ☐ | Ghép khi bàn đích đang chờ thanh toán | 1. Đảm bảo Bàn B đang ở trạng thái "Chờ thanh toán" 2. Mở tách/ghép từ Bàn A, chọn Bàn B làm đích 3. Thử xác nhận ghép | Hệ thống chặn, hiển thị thông báo không thể ghép vào bàn đang chờ thanh toán |
| ☐ | Tách một phần món sang hóa đơn mới trong cùng bàn | 1. Mở giao diện tách/ghép từ **Bàn A** (có món X, Y, Z) 2. Chọn mode **"Tách"** 3. Tích chọn món **X** muốn tách ra 4. Chọn đích là **"Hóa đơn mới"** trong cùng Bàn A 5. Bấm xác nhận 6. Quan sát tab hóa đơn của Bàn A | Bàn A có **2 tab hóa đơn**: HĐ1 còn Y, Z — HĐ2 chứa X; tổng tiền từng tab tính đúng theo món |
| ☐ | Tách một phần món sang bàn mới (bàn trống) | 1. Mở giao diện tách/ghép từ **Bàn A** (có món X, Y, Z) 2. Chọn mode **"Tách"** 3. Tích chọn món **Y** và **Z** 4. Chọn đích là **Bàn B** đang trống 5. Xác nhận 6. Quan sát cả hai bàn | Bàn A chỉ còn món X; Bàn B mới bắt đầu với món Y và Z; cả hai bàn ở trạng thái "Đang sử dụng" |
| ☐ | Tách và điều chỉnh số lượng | 1. Mở giao diện tách/ghép từ Bàn A — trong đó có **2 phần Cà phê** 2. Tách **1 phần Cà phê** sang hóa đơn mới (chỉ tách một nửa số lượng) 3. Xác nhận 4. Quan sát cả hai hóa đơn | Hóa đơn nguồn còn **1 Cà phê**; hóa đơn đích có **1 Cà phê**; tổng hai hóa đơn = đúng số lượng ban đầu |
| ☐ | Tổng tiền sau tách không thay đổi tổng gộp | 1. Ghi nhận tổng tiền Bàn A trước khi tách (= T) 2. Tách một phần món sang hóa đơn mới / Bàn B 3. Tính: tổng Bàn A sau tách + tổng hóa đơn/Bàn B | Tổng A còn lại + Tổng B mới = T (không mất tiền, không cộng dư) |
| ☐ | Không cho tách khi chỉ có 1 món, số lượng = 1 | 1. Tạo đơn tại Bàn A chỉ có **1 món**, số lượng = 1 2. Mở giao diện tách/ghép 3. Thử tách món đó ra | Hệ thống chặn hoặc cảnh báo: không thể tách vì không còn món nào ở đơn gốc |
| ☐ | Tách toàn bộ món (bàn nguồn sẽ trống) | 1. Mở giao diện tách/ghép từ Bàn A có 2 món 2. Tích chọn **tất cả** món 3. Chọn đích là Bàn B trống 4. Xác nhận | Bàn A về trạng thái **trống**; Bàn B có toàn bộ 2 món; Bàn A không giữ trạng thái "Đang sử dụng" khi không còn món |
| ☐ | Bấm "Xác nhận" hoàn tất ghép/tách | 1. Thực hiện thao tác ghép hoặc tách hợp lệ (đã chọn món, chọn bàn đích) 2. Bấm nút **"Xác nhận"** / **"Hoàn tất"** 3. Quan sát kết quả | Thao tác thực hiện thành công; dữ liệu các bàn cập nhật đúng; màn hình đóng giao diện tách/ghép, trở về màn hình Order |
| ☐ | Bấm "Hủy" / "Đóng" giữa chừng | 1. Mở giao diện tách/ghép, thực hiện chọn món và chọn bàn đích 2. **Không** bấm Xác nhận, thay vào đó bấm **"Hủy"** hoặc **"Đóng"** (X) 3. Quan sát dữ liệu hai bàn | Không có thay đổi nào xảy ra; đơn tại Bàn A và Bàn B giữ nguyên như trước |
| ☐ | Xác nhận khi chưa chọn món nào | 1. Mở giao diện tách/ghép 2. Không tích chọn bất kỳ món nào 3. Bấm **"Xác nhận"** 4. Quan sát phản hồi | Hệ thống chặn, hiển thị thông báo yêu cầu chọn ít nhất 1 món |
| ☐ | Xác nhận khi chưa chọn bàn/hóa đơn đích | 1. Mở giao diện tách/ghép 2. Tích chọn 1 hoặc nhiều món 3. Không chọn bàn đích 4. Bấm **"Xác nhận"** | Hệ thống chặn, hiển thị thông báo yêu cầu chọn bàn hoặc hóa đơn đích |
| ☐ | Món đã gửi bếp vẫn tách/ghép được | 1. Tại Bàn A, thêm món X và bấm **"Báo bếp"** 2. Mở giao diện tách/ghép 3. Tích chọn món X (đã gửi bếp) và thực hiện ghép/tách sang Bàn B 4. Quan sát kết quả | Món đã gửi bếp vẫn được tách/ghép thành công; trạng thái "đã gửi bếp" giữ nguyên theo món sau khi chuyển sang bàn đích |
| ☐ | Tách/ghép món có ghi chú | 1. Trong đơn Bàn A, có món với **ghi chú** kèm theo (VD: "ít đường") 2. Tách/ghép món đó sang Bàn B 3. Quan sát dòng món tại Bàn B | Ghi chú theo món được giữ nguyên sau khi tách/ghép, không bị mất |
| ☐ | Tách/ghép món có tùy chọn (size, topping) | 1. Trong đơn Bàn A, có món **Trà sữa Size L + Trân châu** 2. Tách/ghép món đó sang Bàn B 3. Quan sát dòng món tại Bàn B | Tùy chọn (Size L, Trân châu) được giữ đầy đủ; giá tính đúng theo tùy chọn |
| ☐ | Tách/ghép khi đơn có giảm giá | 1. Áp giảm giá cho đơn Bàn A 2. Thực hiện tách một phần món sang Bàn B 3. Quan sát xử lý giảm giá ở cả hai đơn | Hệ thống xử lý giảm giá hợp lý (áp theo đơn gốc hoặc yêu cầu nhập lại); không bị âm tiền hoặc giảm giá trùng |
| ☐ | Tách/ghép khi đơn có hàng tặng | 1. Áp hàng tặng vào đơn Bàn A 2. Thực hiện tách/ghép toàn bộ sang Bàn B 3. Quan sát hàng tặng tại Bàn B | Hàng tặng được chuyển theo hoặc hệ thống thông báo xử lý rõ ràng; tổng tiền Bàn B không bị cộng sai |
| ☐ | Trạng thái thẻ bàn cập nhật ngay sau tách/ghép | 1. Thực hiện ghép toàn bộ Bàn A sang Bàn B 2. Bấm **"Xác nhận"** 3. Ngay lập tức quay về **Trang chủ** (không reload thủ công) 4. Quan sát thẻ Bàn A và Bàn B | Bàn A hiển thị **trống** (màu trắng/xám); Bàn B hiển thị **"Đang sử dụng"** với tổng tiền mới — không cần F5 mới thấy |
| ☐ | Tổng tiền trên thẻ bàn khớp sau ghép | 1. Ghép Bàn A (tổng a) vào Bàn B (tổng b) 2. Quay về Trang chủ, quan sát thẻ Bàn B | Tổng tiền hiển thị trên thẻ Bàn B = a + b |
| ☐ | Chưa mở ca / không có quyền | 1. Đảm bảo ca chưa mở hoặc dùng tài khoản không có quyền tách/ghép bàn 2. Vào màn hình Order của bàn đang có đơn 3. Tìm và bấm nút Tách/Ghép bàn | Hệ thống chặn thao tác, hiển thị thông báo "Chưa mở ca" hoặc "Không có quyền" |
| ☐ | Tách/ghép khi có 2 người dùng cùng bàn | 1. Mở Bàn A trên 2 tab/thiết bị khác nhau 2. Trên tab 1: mở giao diện tách/ghép, bắt đầu thao tác 3. Trên tab 2: thêm một món mới vào Bàn A cùng lúc 4. Quay lại tab 1: bấm Xác nhận | Hệ thống không bị mất dữ liệu; món thêm ở tab 2 không bị mất hoặc có cảnh báo xung đột rõ ràng |


### Hàng tặng

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Mở chức năng hàng tặng trên đơn | 1. Trong màn hình Order, tìm nút "..." hoặc menu chức năng 2. Chọn "Hàng tặng" 3. Quan sát màn hình | Hiện danh sách món có thể tặng |
| ☐ | Chọn món tặng áp vào đơn | 1. Trong danh sách hàng tặng, chọn một món 2. Xác nhận thêm vào đơn 3. Quan sát hóa đơn | Món tặng xuất hiện trong hóa đơn với giá 0đ |
| ☐ | Chọn lý do tặng | 1. Khi thêm món tặng, quan sát có bước chọn lý do tặng 2. Chọn một lý do từ danh sách 3. Xác nhận | Lý do được ghi nhận kèm theo dòng món tặng |
| ☐ | Món tặng hiển thị trong đơn | 1. Sau khi thêm hàng tặng thành công 2. Quan sát dòng món tặng trong hóa đơn | Dòng món tặng thể hiện rõ là hàng tặng (nhãn hoặc giá 0đ) |
| ☐ | Hàng tặng không cộng vào tổng tiền | 1. Ghi nhận tổng tiền thanh toán trước khi thêm hàng tặng 2. Thêm món tặng vào đơn 3. So sánh tổng tiền thanh toán trước và sau | Tổng tiền thanh toán không thay đổi sau khi thêm hàng tặng |
| ☐ | Đơn không thỏa điều kiện | 1. Tạo đơn với giá trị thấp hoặc không đủ điều kiện áp hàng tặng 2. Thử mở chức năng hàng tặng 3. Quan sát phản hồi | Hệ thống không cho áp, hiển thị thông báo phù hợp |

### Áp dụng khuyến mãi

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Mở chức năng khuyến mãi trên đơn | 1. Trong màn hình Order có món, tìm nút "..." hoặc mục "Khuyến mãi" 2. Bấm mở chức năng khuyến mãi 3. Quan sát danh sách | Hiện danh sách chương trình khuyến mãi còn hiệu lực |
| ☐ | Áp khuyến mãi vào đơn | 1. Mở danh sách khuyến mãi, chọn một CTKM phù hợp 2. Xác nhận áp 3. Quan sát dòng "Giảm giá" và Tổng tiền thanh toán | Giảm giá áp đúng theo CTKM, tổng tiền thanh toán giảm tương ứng |
| ☐ | CTKM hết hiệu lực | 1. Mở danh sách khuyến mãi 2. Tìm CTKM đã hết ngày hoặc hết lượt 3. Quan sát xem có hiển thị không | CTKM hết hiệu lực không xuất hiện trong danh sách hoặc không áp được |
| ☐ | Đơn không thỏa điều kiện CTKM | 1. Tạo đơn có giá trị thấp hơn điều kiện tối thiểu của CTKM 2. Thử áp CTKM đó 3. Quan sát phản hồi | Hệ thống không cho áp, hiển thị thông báo lỗi |
| ☐ | Bỏ khuyến mãi đã áp | 1. Sau khi đã áp CTKM thành công, tìm tùy chọn gỡ/bỏ khuyến mãi 2. Xác nhận gỡ 3. Quan sát lại Tổng tiền thanh toán | Giảm giá bị xóa, tổng tiền hoàn về giá gốc |
| ☐ | Chưa mở ca | 1. Đảm bảo ca chưa được mở 2. Vào màn hình Order, thử mở chức năng khuyến mãi 3. Quan sát phản hồi | Hệ thống chặn, không cho áp khuyến mãi |

### Hủy đơn

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Hủy đơn chưa thanh toán | 1. Vào bàn có đơn chưa thanh toán 2. Tìm chức năng "Hủy đơn" (thường trong menu "...") 3. Chọn lý do và xác nhận hủy 4. Quan sát bàn ngoài Trang chủ | Đơn bị hủy, bàn về trạng thái trống |
| ☐ | Chọn lý do hủy (bắt buộc) | 1. Mở chức năng hủy đơn 2. Bỏ qua bước chọn lý do, thử bấm xác nhận ngay 3. Quan sát phản hồi | Hệ thống bắt buộc chọn lý do, không hủy được nếu bỏ trống |
| ☐ | Xác nhận hủy | 1. Mở chức năng hủy đơn 2. Chọn lý do hủy 3. Bấm "Xác nhận" 4. Quan sát kết quả | Đơn hoàn tất hủy, không còn trong danh sách đơn hoạt động |
| ☐ | Hủy đơn đã thanh toán | 1. Vào Lịch sử, tìm một đơn đã thanh toán thành công 2. Thử thao tác hủy đơn đó 3. Quan sát phản hồi | Hệ thống chặn, không cho hủy đơn đã thanh toán |
| ☐ | Không có quyền / chưa mở ca | 1. Đăng nhập bằng tài khoản không có quyền hủy đơn hoặc đảm bảo ca chưa mở 2. Vào bàn có đơn 3. Thử thao tác hủy đơn | Hệ thống chặn, hiển thị thông báo không có quyền hoặc yêu cầu mở ca |

### Thanh toán đơn hàng (qua Chờ thanh toán)

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Tab "Chờ thanh toán" hiển thị đơn chờ | 1. Tại Trang chủ, bấm chọn checkbox "Chờ thanh toán" 2. Quan sát danh sách bàn lọc ra | Hiển thị đúng các bàn/đơn đang chờ thanh toán |
| ☐ | Thanh toán từ tab Chờ thanh toán | 1. Tại Trang chủ, lọc tab "Chờ thanh toán" 2. Bấm vào bàn cần thanh toán 3. Thực hiện thanh toán đơn 4. Quan sát bàn sau khi xong | Thanh toán thành công, bàn về trạng thái trống |
| ☐ | Thanh toán bằng cách chọn bàn đang dùng | 1. Tại Trang chủ, bấm trực tiếp vào bàn đang sử dụng 2. Vào màn hình Order của bàn đó 3. Thực hiện thanh toán theo yêu cầu khách | Thanh toán thành công, bàn về trống |
| ☐ | Thanh toán đơn order gửi từ tablet/mobile | 1. Đảm bảo có đơn được gửi từ thiết bị tablet/mobile của khách 2. Tại màn hình cashier, xác nhận đơn vào bàn 3. Thực hiện thanh toán đơn đó | Đơn được tiếp nhận và thanh toán đúng |

### Trường hợp đặc thù & lỗi

| ✓ | Testcase | Các bước thực hiện | Kết quả mong đợi |
|---|----------|--------------------|------------------|
| ☐ | Số lượng món = 0 | 1. Trong hóa đơn, giảm số lượng một món về 0 (nếu cho phép nhập tay) 2. Thử lưu hoặc thanh toán 3. Quan sát phản hồi | Hệ thống không cho lưu, xử lý đúng khi số lượng = 0 |
| ☐ | Giá rất lớn (999,999,999đ) | 1. Vào cấu hình hoặc chỉnh sửa đơn giá thủ công, nhập giá trị rất lớn (VD: 999,999,999đ) 2. Thêm vào hóa đơn 3. Quan sát hiển thị và tổng tiền | Tính và hiển thị đúng số lớn, không bị tràn giao diện |
| ☐ | Làm tròn tiền VND | 1. Tạo đơn có thuế % dẫn đến kết quả lẻ thập phân (VD: 10% của 15,000đ = 1,500đ) 2. Quan sát tổng tiền thanh toán | Tổng tiền hiển thị số nguyên, không có số lẻ thập phân |
| ☐ | Mất mạng khi thanh toán | 1. Chuẩn bị đơn hàng sẵn sàng thanh toán 2. Tắt mạng (ngắt WiFi hoặc kéo cáp) 3. Bấm "Thanh toán" 4. Bật lại mạng, kiểm tra trong Lịch sử đơn | Đơn không bị tạo trùng, dữ liệu nhất quán |
| ☐ | Hai thu ngân cùng 1 bàn | 1. Mở bàn đang có đơn trên 2 thiết bị/tab khác nhau 2. Cả 2 cùng thêm món hoặc chỉnh sửa đồng thời 3. Quan sát kết quả trên cả 2 thiết bị | Không bị ghi đè hoặc mất dữ liệu của nhau |
| ☐ | Ghi chú có dấu / ký tự đặc biệt | 1. Trong hóa đơn, tích checkbox "Ghi chú" trên một dòng món 2. Nhập nội dung có dấu tiếng Việt và ký tự đặc biệt (VD: @, #, !, ...) 3. Lưu và quan sát lại dòng món | Ghi chú lưu và hiển thị đúng, không bị lỗi ký tự |

---

## Lịch sử

### Bộ lọc loại đơn

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Lọc tab "Tất cả" | Hiện tất cả đơn |
| ☐ | Lọc tab "Tại bàn" | Chỉ hiện đơn tại bàn |
| ☐ | Lọc tab "Mang về" | Chỉ hiện đơn mang về |
| ☐ | Lọc tab "Đặt online" | Chỉ hiện đơn online (rỗng → trạng thái rỗng) |
| ☐ | Dropdown "Chọn bàn" | Lọc đúng đơn theo bàn đã chọn |

### Tìm kiếm & bộ lọc

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Tìm theo mã đơn | Trả đúng đơn |
| ☐ | Tìm theo số điện thoại | Trả đúng đơn |
| ☐ | Tìm không khớp | Danh sách rỗng |
| ☐ | Trạng thái: Đã thanh toán thành công | Chỉ hiện đơn đã TT thành công |
| ☐ | Trạng thái: Chưa thanh toán | Chỉ hiện đơn chưa TT |
| ☐ | Trạng thái: Đã hủy | Chỉ hiện đơn đã hủy |
| ☐ | Trạng thái: Đã xử lý trả hàng | Chỉ hiện đơn trả hàng |
| ☐ | Trạng thái: Công nợ | Chỉ hiện đơn công nợ |
| ☐ | Lọc theo Tài khoản | Chỉ hiện đơn của NV đã chọn |
| ☐ | Khoảng ngày: Hôm nay | Đơn trong hôm nay |
| ☐ | Khoảng ngày: Hôm qua | Đơn hôm qua |
| ☐ | Khoảng ngày: Tuần này | Đơn tuần này |
| ☐ | Khoảng ngày: Tháng này | Đơn tháng này |
| ☐ | Khoảng ngày: Tùy chọn | Đơn trong khoảng chọn |
| ☐ | Kết hợp nhiều bộ lọc | Kết quả giao đúng |
| ☐ | Ngày bắt đầu > kết thúc | Chặn/báo lỗi |

### Danh sách đơn

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Thẻ đơn hiển thị | Đúng tên bàn, tài khoản, ngày giờ, mã đơn, số tiền |
| ☐ | Trạng thái thanh toán | Đúng (Chưa/Đã thanh toán) |
| ☐ | Trạng thái HDDT | Đúng (Không xác định / Chờ ký) |
| ☐ | Màu theo trạng thái | Xám = chưa, xanh = đã thanh toán |
| ☐ | Số tiền trên thẻ | Khớp chi tiết đơn |

### Chi tiết đơn hàng

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Bấm vào đơn | Mở modal "Chi tiết đơn hàng" đúng mã đơn |
| ☐ | Thông tin đơn | Đúng bàn, khách hàng, nhân viên, ngày tạo |
| ☐ | Danh sách món | Đúng tên, SL, đơn giá, thành tiền |
| ☐ | Tổng tiền hàng | = Σ thành tiền các món |
| ☐ | Phụ thu / Giảm giá / Tiền điểm / VAT | Tính đúng |
| ☐ | Tổng tiền thanh toán | = Tổng hàng + Phụ thu − Giảm giá − Tiền điểm + VAT |
| ☐ | Phương thức thanh toán | Hiển thị đúng |
| ☐ | Bấm "Đóng" | Đóng modal, giữ nguyên bộ lọc |

### Xuất Excel

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Bấm "Xuất Excel" | Kích hoạt tải file |
| ☐ | File xuất | Đúng bộ lọc đang áp dụng |

---

## Điều phối ca

### Lịch sử ca

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Hiển thị danh sách các ca | Đúng: nhân viên, người mở, mã ca, giờ mở, giờ đóng, tổng tiền mặt |
| ☐ | Ca đang mở | Hiện trạng thái "Đang mở" thay cho giờ đóng |
| ☐ | Lọc theo Thời gian (khoảng ngày) | Chỉ hiện ca trong khoảng đã chọn |
| ☐ | Lọc theo Nhân viên | Chỉ hiện ca của nhân viên đã chọn |
| ☐ | Bấm vào 1 ca | Hiện chi tiết ca đó ở panel bên phải |
| ☐ | Nút "In phiếu" của ca | Kích hoạt in phiếu kết ca |
| ☐ | Nút "Chi tiết ca" | Mở modal chi tiết ca |
| ☐ | Nút "Mở màn hình phụ" | Mở màn hình phụ của ca đang mở |

### Thông tin ca & đóng ca

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Hiển thị header ca | Đúng ngày giờ, nhân viên, trạng thái |
| ☐ | Hiển thị Tiền mặt đầu ca | Đúng số tiền khai báo đầu ca |
| ☐ | Nút "Đóng ca" | Đóng ca, ghi nhận giờ đóng |
| ☐ | Nút "Đóng và in phiếu" | Đóng ca + in phiếu kết ca |
| ☐ | Ca đã đóng | Không cho thao tác đóng lại |

### Thẻ tổng hợp (Bán hàng / Trả hàng / Phiếu thu / Phiếu chi)

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Thẻ Bán hàng | Đúng số đơn hàng & tiền mặt bán hàng |
| ☐ | Thẻ Trả hàng | Đúng tiền trả hàng |
| ☐ | Thẻ Phiếu thu | Đúng tiền thu |
| ☐ | Thẻ Phiếu chi | Đúng tiền chi |
| ☐ | Bấm "..." trên thẻ | Hiện chi tiết theo phương thức (tiền mặt / chuyển khoản / quẹt thẻ / QR / khác) |
| ☐ | Tổng các phương thức | = tổng hiển thị trên thẻ |

### Giao dịch trong ca

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Hiển thị danh sách giao dịch | Đúng: STT, mã chứng từ, loại, số tiền, phương thức, trạng thái |
| ☐ | Tổng giao dịch | Đếm đúng số giao dịch |
| ☐ | Lọc loại: Phiếu bán hàng | Chỉ hiện phiếu bán hàng |
| ☐ | Lọc loại: Phiếu trả hàng | Chỉ hiện phiếu trả hàng |
| ☐ | Lọc loại: Phiếu thu | Chỉ hiện phiếu thu |
| ☐ | Lọc loại: Phiếu chi | Chỉ hiện phiếu chi |
| ☐ | Lọc loại: Tất cả | Hiện mọi loại giao dịch |
| ☐ | Lọc "Hoàn thành" | Chỉ hiện giao dịch hoàn thành |
| ☐ | Lọc "Đã hủy" | Chỉ hiện giao dịch đã hủy |
| ☐ | Tìm theo mã / chú thích | Trả đúng giao dịch |

### Đối soát ca (logic tính)

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Tổng tiền mặt trong ca | = tiền mặt(phiếu thu bán hàng) + phiếu thu − phiếu trả hàng − phiếu chi |
| ☐ | KHÔNG cộng Tiền mặt đầu ca vào tổng | Tiền mặt đầu ca không được tính vào "Tổng tiền mặt trong ca" |
| ☐ | Chỉ tính giao dịch tiền mặt | Các phương thức khác (CK/thẻ/QR) không vào tổng tiền mặt trong ca |
| ☐ | Mỗi phiếu bán hàng → ghi nhận vào ca | Đơn bán xong xuất hiện trong giao dịch ca |
| ☐ | Phiếu trả hàng → ghi nhận đúng (giảm) | Trả hàng làm giảm tổng tương ứng |
| ☐ | Phiếu thu → cộng vào ca | Phiếu thu xuất hiện & cộng đúng |
| ☐ | Phiếu chi → trừ khỏi ca | Phiếu chi xuất hiện & trừ đúng |
| ☐ | Giao dịch đã hủy không tính vào tổng | Tổng tiền không gồm giao dịch đã hủy |

### Chi tiết ca (modal)

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Mở modal Chi tiết ca | Đúng mã ca, ngày giờ, nhân viên |
| ☐ | Bảng Thu/Chi theo phương thức | Số liệu khớp với thẻ tổng hợp |
| ☐ | Tổng tiền mặt trong ca (modal) | Khớp với panel chính |
| ☐ | Bấm "Đóng" | Đóng modal |

---

## Thu chi

### Bộ lọc

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Tìm theo Mã phiếu | Trả đúng phiếu; không khớp → danh sách rỗng |
| ☐ | Lọc theo Chi nhánh (CN1...) | Chỉ hiện phiếu của chi nhánh đã chọn |
| ☐ | Thời gian: Hôm nay / Hôm qua | Chỉ hiện phiếu trong khoảng |
| ☐ | Thời gian: Tuần này / Tuần trước | Chỉ hiện phiếu trong khoảng |
| ☐ | Thời gian: Tháng này / Tháng trước | Chỉ hiện phiếu trong khoảng |
| ☐ | Thời gian: tùy chọn ngày | Chỉ hiện phiếu trong khoảng chọn |
| ☐ | Lọc theo Người tạo | Chỉ hiện phiếu của người đã chọn |
| ☐ | Lọc theo Loại thu chi (Thu/Chi) | Chỉ hiện đúng loại |
| ☐ | Lọc theo Phân loại thu chi | Chỉ hiện đúng phân loại |
| ☐ | Lọc theo Loại nguồn (Bán hàng/Mua hàng/Tự tạo/Trả hàng) | Chỉ hiện phiếu đúng nguồn |
| ☐ | Kết hợp nhiều bộ lọc | Kết quả giao đúng, thẻ tổng quan cập nhật theo |

### Tổng quan quỹ

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Hiển thị Tồn quỹ đầu kỳ | Đúng số dư đầu kỳ theo bộ lọc |
| ☐ | Hiển thị Tổng thu | = Σ phiếu Thu trong bộ lọc |
| ☐ | Hiển thị Tổng chi | = Σ phiếu Chi trong bộ lọc |
| ☐ | Tồn quỹ cuối kỳ | = Tồn đầu kỳ + Tổng thu − Tổng chi |
| ☐ | Đổi bộ lọc thời gian | Cả 4 thẻ cập nhật theo kỳ mới |

### Danh sách phiếu

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Hiển thị bảng phiếu | Đúng: mã phiếu, loại, số tiền, chi nhánh, người nộp/nhận, người tạo, phân loại, PTTT, đính kèm, thời gian, mô tả |
| ☐ | Phân trang | Chuyển trang đúng, dữ liệu khớp |
| ☐ | Bấm icon xem (Hành động) | Mở chi tiết phiếu đúng |
| ☐ | Phiếu có đính kèm | Hiển thị/đọc được tệp đính kèm |

### Thêm phiếu

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Bấm "Thêm" | Mở modal "Thêm phiếu" |
| ☐ | Mã phiếu tự sinh | Hiện mã tự động (ex: vote-00001) |
| ☐ | Bỏ trống "Loại thu chi" (bắt buộc) | Chặn lưu, báo lỗi |
| ☐ | Bỏ trống "Số tiền" (bắt buộc) | Chặn lưu, báo lỗi |
| ☐ | Chọn Loại đối tượng / Người nộp | Ghi nhận đúng |
| ☐ | Chọn Phân loại thu chi | Ghi nhận đúng |
| ☐ | Chọn Phương thức thanh toán | Ghi nhận đúng (mặc định Tiền mặt) |
| ☐ | Nhập Số tiền | Chỉ nhận số, định dạng tiền đúng |
| ☐ | Đính kèm tệp | Tải lên & gắn vào phiếu |
| ☐ | Mô tả giới hạn 200 ký tự | Đếm 0/200, không vượt quá |
| ☐ | Bấm "Lưu" hợp lệ | Tạo phiếu mới, xuất hiện trong danh sách, cập nhật quỹ |
| ☐ | Bấm "Đóng" | Đóng modal, không tạo phiếu |

### Ghi nhận 4 loại phiếu (logic chính)

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Tạo Phiếu thu thủ công | Phiếu Loại = Thu; cộng vào Tổng thu & tăng tồn quỹ |
| ☐ | Tạo Phiếu chi thủ công | Phiếu Loại = Chi; cộng vào Tổng chi & giảm tồn quỹ |
| ☐ | Phiếu thu hiển thị trong danh sách | Đúng loại, số tiền, người nộp, PTTT |
| ☐ | Phiếu chi hiển thị trong danh sách | Đúng loại, số tiền, người nhận, PTTT |
| ☐ | Hoàn tất 1 đơn bán → tự sinh Phiếu bán hàng | Ghi nhận là Thu, Loại nguồn = Bán hàng, số tiền = tổng đơn |
| ☐ | Thực hiện trả hàng → tự sinh Phiếu trả hàng | Ghi nhận là Chi (hoàn tiền), Loại nguồn = Trả hàng, số tiền = tiền hoàn |
| ☐ | Lọc Loại nguồn = Bán hàng | Chỉ hiện phiếu sinh từ bán hàng |
| ☐ | Lọc Loại nguồn = Trả hàng | Chỉ hiện phiếu sinh từ trả hàng |
| ☐ | Lọc Loại nguồn = Tự tạo | Chỉ hiện phiếu thu/chi tạo thủ công |
| ☐ | Số tiền phiếu bán hàng | Khớp tổng tiền thanh toán của đơn gốc |
| ☐ | Số tiền phiếu trả hàng | Khớp giá trị hàng trả của đơn gốc |
| ☐ | PTTT của phiếu tự sinh | Khớp phương thức thanh toán của đơn bán/đơn trả |
| ☐ | Đơn bán bị hủy | Phiếu bán hàng tương ứng không tính vào tồn quỹ |
| ☐ | Phiếu khớp giữa Thu chi ↔ Điều phối ca | Cùng số tiền, cùng phương thức, không lệch |
| ☐ | Tổng thu = Σ(phiếu thu thủ công + phiếu bán hàng) | Cộng đúng tất cả nguồn thu |
| ☐ | Tổng chi = Σ(phiếu chi thủ công + phiếu trả hàng) | Cộng đúng tất cả nguồn chi |

### Xuất Excel

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Bấm "Xuất Excel" | Kích hoạt tải file |
| ☐ | File xuất | Đúng dữ liệu theo bộ lọc đang áp dụng |

### Công nợ (tab)

| ✓ | Testcase | Kết quả mong đợi |
|---|----------|------------------|
| ☐ | Mở tab "Công nợ" | Hiển thị danh sách công nợ (chi tiết chờ video) |

---

## Câu hỏi còn lại

| ✓ | Câu hỏi |
|---|---------|
| ☐ | "Tạm tính" khác "Thanh toán" thế nào? |
| ☐ | Modal chi tiết đơn (Lịch sử): công thức Tổng thanh toán có đúng (− Tiền điểm, + VAT) không? |
| ☐ | **Điều phối ca** — Một đơn bán hiện 2 dòng (Phiếu bán hàng + Phiếu thu) cùng số tiền: quan hệ là gì, có tính 2 lần không? |
| ☐ | **Điều phối ca** — "Mở màn hình phụ" dùng để làm gì? |
| ☐ | **Thu chi** — Phiếu trả hàng ghi nhận là Chi (tiền ra) hay ghi âm vào Thu? Phiếu bán/trả tự sinh có cho sửa/xóa không? |
| ☐ | **Thu chi** — Tab "Công nợ" gồm những chức năng gì? |
| ☐ | Các tab Bàn đặt / Đặt online / CRM — có trong video sau? |
