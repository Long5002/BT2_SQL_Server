# BT2_SQL_Server

## Phần mở đầu:

**Thông tin cá nhân**:

* Họ và tên: Nguyễn Việt Long

* MSSV: K235480106047

* Lớp: K59KMT

* Đề tài: Quản lý nhà hàng

* Tên database: QuanLyNhaHang_K235480106047

**Yêu cầu đầu bài**

Phần 1: Thiết kế và Khởi tạo Cấu trúc Dữ liệu

* Tự chọn một chủ đề quản lý

* Tạo một Database mới với tên [Tên dự án]_[MaSV] (QuanLyNhaHang_K235480106047).

* Tạo ít nhất 3 bảng có quan hệ với nhau. Yêu cầu:

* Sử dụng đa dạng các kiểu dữ liệu (Số nguyên, số thực, chuỗi ký tự Unicode, ngày tháng, tiền tệ, ...).

* Áp dụng đúng quy tắc đặt tên (BướuLạcĐà).

* Sử dụng cặp ngoặc [ ] để bọc tên bảng và tên trường trong script khởi tạo.

* Có giải thích chỗ nào là PK, chỗ nào là FK, trường nào có ràng buộc cứng CK (ví dụ điểm từ 0..10),...

Phần 2: Xây dựng Function

* Hãy cho biết trong SQL Server có những loại function build_in (hàm có sẵn) nào, nêu 1 vài system function build_in mà em tìm hiểu được (ko cần nhiều, cần đặc sắc theo góc nhìn của em), cho SQL khai thác các hàm đó.

* Hàm do người dùng tự viết trong SQL thường mang mục đích gì? Nó có những loại nào? Mỗi loại thường được dùng khi nào? Tại sao có nhiều system function rồi mà vẫn cần tự viết fn riêng?

* Viết 01 Scalar Function (Hàm trả về một giá trị): Đưa ra 1 logic cho cơ sở dữ liệu của em, mà cần dùng đến function này. (SV TỰ NGHĨ RA YÊU CẦU CỦA HÀM VÀ VIẾT HÀM GIẢI QUYẾT NÓ)

Sau khi đã có hàm, viết câu lệnh sql khai thác hàm đó.

* Viết 01 Inline Table-Valued Function: Trả về danh sách các bản ghi theo một điều kiện lọc cụ thể (SV TỰ NGHĨ RA YÊU CẦU CỦA HÀM VÀ VIẾT HÀM GIẢI QUYẾT NÓ)

Sau khi đã có hàm, viết câu lệnh sql khai thác hàm đó.

* Viết 01 Multi-statement Table-Valued Function: Thực hiện xử lý logic phức tạp bên trong (có sử dụng biến bảng) trước khi trả về kết quả. (SV TỰ NGHĨ RA YÊU CẦU CỦA HÀM VÀ VIẾT HÀM GIẢI QUYẾT NÓ)

Sau khi đã có hàm, viết câu lệnh sql khai thác hàm đó.

Phần 3: Xây dựng Store Procedure 

* Trong SQL Server có những SP có sẵn nào? nêu 1 vài system sp mà em tìm hiểu được, giải thích cách dùng chúng.

* Viết 01 Store Procedure đơn giản để thực hiện lệnh INSERT hoặc UPDATE dữ liệu, có kiểm tra điều kiện logic (SV TỰ NGHĨ RA YÊU CẦU CỦA SP VÀ VIẾT SP GIẢI QUYẾT NÓ)

* Viết 01 Store Procedure có sử dụng tham số OUTPUT để trả về một giá trị tính toán (SV TỰ NGHĨ RA YÊU CẦU CỦA SP VÀ VIẾT SP GIẢI QUYẾT NÓ, SP NÀY CÓ DÙNG THAM SỐ LOẠI OUTPUT)

* Viết 01 Store Procedure trả về một tập kết quả (Result set) từ lệnh SELECT sau khi đã join nhiều bảng. (SV TỰ NGHĨ RA YÊU CẦU CỦA SP VÀ VIẾT SP GIẢI QUYẾT NÓ)

Phần 4: Trigger và Xử lý logic nghiệp vụ

* Viết 01 Trigger để tự động làm gì đó tại 1 bảng B khi mà dữ liệu thay đổi dữ liệu ở bảng A. Logic giải quyết do sv tự nghĩ ra, sao cho thực tế và thuyết phục.

* Thử viết Trigger cho Bảng A : Khi insert thì cập nhật dữ liệu vào bảng B; sau đó viết trigger cho bảng B để khi B được cập nhật thì cập nhật sang bảng A : Quan sát các thông báo (nếu có) của hệ thống, giải thích các thông báo đó (nếu có). Đưa ra nhật xét cuối cùng về tình trạng này.

Phần 5: Cursor và Duyệt dữ liệu

* Viết một đoạn script sử dụng CURSOR để duyệt qua danh sách của 1 câu lệnh SQL dạng SELECT, duyệt qua từng bản ghi, xử lý riêng từng bản ghi (THEO LOGIC SV TỰ ĐẶT RA: SAO CHO HỢP LÝ VÀ THUYẾT PHỤC)

* Tìm cách không sử dụng CURSOR để giải quyết bài toán mà em đã dùng CURSOR mới giải quyết được ở trên. thử so sánh tốc độ giữa có dùng cursor và không dùng cursor (nếu cùng kết quả) thì thời gian xử lý cái nào nhanh hơn, cần ảnh chụp màn hình minh chứng.

* Nếu vẫn tìm được cách dùng SQL để giải quyết vấn đề mà ko cần CURSOR: thử nghĩ bài toán khác, mà chỉ CURSOR mới giải quyết được, còn SQL rất khó giải quyết đc (theo logic suy nghĩ của em)

**Giới thiệu về hệ thống quản lý nhà hàng**

Xây dựng một hệ thống quản lý nhà hàng (QuanLyNhaHang_K235480106047) từ nền tảng SQL Server, bao gồm các chức năng chủ yếu như: quản lý thực đơn, quản lý bàn và đặt bàn, quản lý bán hàng và quản lý nhân sự.

Xây dựng hệ thống quản lý nhà hàng nhằm tối ưu hóa quy trình vận hành hệ thống, thiết lập các mối liên kết chặt chẽ thông qua khóa chính và khóa ngoại, giúp đảm bảo tính đồng bộ và chính xác trong việc quản lý doanh thu cũng như phục vụ khách hàng.

## Phần 1: Khởi tạo bảng

Chủ đề quản lý: Hệ thống quản lý nhà hàng

Tạo mới database và đặt tên: QuanLyNhaHang_K235480106047

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/bbad981e-6e48-4e96-afc4-f543367037b2" />

Tạo bảng:

1. NhanVien: gồm các trường: MaNV (PK), HoTen (không để trống), ChucVu (Nvarchar dùng để viết tiếng việt có dấu), SoDienThoai, Luong

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/d7f29de4-7566-4b99-b1df-0f3d7090456e" />

2. DanhMuc: gồm các trường: MaDanhMuc (PK tự động tăng), TenDanhMuc (không để trống)

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/b47d36b7-1716-43d0-8d3d-d9e157a0fea1" />

3. MonAn: gồm các trường: MaMon (PK tự động tăng), TenMon (không để trống), MaDanhMuc (FK), GiaTien, TrangThai (đang bán, ngừng bán)

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/19b024fe-555f-4f2a-89e5-f85ada638ff8" />

4. BanAn: gồm các trường: MaBan (PK tự động tăng), SoBan (không để trống), SucChua, TrangThai (trống, có khách, đã đặt)

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/a4254581-cdb4-4c15-b16c-f9cfcf1d9081" />

5. DatBan: gồm các trường: MaDatBan (PK tự động tăng), TenKhachHang (không để trống), SoDienThoai, ThoiGianDat, MaBan (FK)

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/0ccff755-7975-4fde-9f19-47fa3826eec1" />

6. HoaDon: gồm các trường: MaHD (PK tự động tăng), NgayLap, MaBan (FK), MaNV (FK), TongTien, TrangThaiThanhToan (chưa thanh toán, đã thanh toán)

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/97665edd-0993-42f8-864a-9aa2a2e14aad" />

7. ChiTietHoaDon: gồm các trường: MaCTHD (PK tự động tăng), MaHD (FK), MaMon (FK), SoLuong, DonGia

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/45e3608b-7bd2-4fa2-b10d-028635d19891" />

Nhập thông tin vào các bảng:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/9caaf171-650b-4823-943d-34e5e8ec5cf2" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/60b831fd-8949-47a9-9d10-e81a7e64c158" />

## Phần 2: Xây dựng Function

Trong SQL Server có nhiều nhóm loại Function build_in như:

- Aggregate Functions
- Configuration Functions
- Cursor Functions
- Date and Time Functions
- Hierarchy Id Functions
- Mathematical Functions
- Metadata Functions
- Other Functions
- Rowset Functions
- Security Functions
- String Functions
- System Statistical Functions
- Text and Image Functions
- Vector Functions

Một vài system function build_in mà em tìm hiểu được:
* Date Function (Nhóm hàm Ngày tháng)
- GETDATE(): Tự động lấy thời gian hiện tại khi khách thanh toán hoặc đặt bàn.
- DATEDIFF(): Tính toán khoảng thời gian.
* Aggregate Functions (Nhóm hàm Tổng hợp)
- SUM(): Tính tổng doanh thu.
- COUNT(): Đếm số lượng.
- AVG(): Tính trung bình.
* String Functions (Nhóm hàm Xử lý Chuỗi)
- UPPER() / LOWER(): Chuyển chữ hoa/chữ thường.
- FORMAT(): Định dạng kiểu dữ liệu.

Hàm do người dùng tự viết trong SQL thường mang mục đích để tạo ra công cụ tự giải quyết công việc, ngoài ra còn nhằm có thể tái sử dụng và có tính đóng gói. Thay vì phải viết đi viết lại một công thức phức tạp hoặc một logic định dạng khác nhau, ta chỉ cần gọi lại hàm đã viết giúp code sạch hơn và dễ dàng sửa lỗi.

Có 3 loại hàm chính:
- Scalar Function: Dùng thực hiện các tính toán logic nhỏ, định dạng dữ liệu hoặc chuyển đổi giá trị.
- Inline table-valued function: Dùng lọc hoặc gom nhóm dữ liệu phức tạp nhưng có thể tái sử dụng nhiều nơi.
- Multi-statement table-valued function: Dùng khi để lấy dữ liệu ra một bảng nhưng logic quá rắc rối và phức tạp

* Viết hàm Scalar Function: Hiện tại trong bảng HoaDon ở cột TongTien vẫn phải tính tay để nhập vào. Em sẽ dùng hàm Function để tự động tính tổng nhờ cột SoLuong và DonGia ở bảng ChiTietHoaDon sau đó dùng lệnh UPDATE vào bảng HoaDon

 <img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/60e774cf-dea0-468b-89d1-bdce7193644e" />

* Viết hàm Inline table-valued function: Hàm này nhận vào @MaHD và trả về danh sách các món ăn khách đã gọi trong hóa đơn đó

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/b5397eeb-3963-4dd4-a129-37983b6f39a2" />

Kết quả:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/f7acae05-492b-4db5-a458-d4f327e3e724" />

* Viết hàm Multi-statement Table-Valued Function: Hàm này sẽ trả về danh sách nhân viên kèm theo tổng số hóa đơn họ đã lập và tổng số tiền họ mang về cho nhà hàng

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/38757648-e946-49c9-bd58-7974cce19fe7" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/1d5115b9-f89f-444d-8c31-5cc447e6de72" />

Kết quả:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/78863140-3780-4907-b591-336ff3893955" />

## Phần 3: Xây dựng Store Procedure

Trong SQL Server có rất nhiều SP có sẵn, có thể tìm thấy chúng trong phần Object Explore -> Programmability -> Stored Procedures -> System Stored Procedures

Một vài SP mà em đã tìm hiểu:
- sp_help: Xem thông tin tổng quát về đối tượng
- sp_rename: Đổi tên bảng hoặc cột
- sp_who: Kiểm tra các kết nối hiện tại vào server
- sp_databases: Liệt kê các database có trên server

Viết một Store Procedure đơn giản để thực hiện lệnh Insert hoặc Update dữ liệu: Dựa vào trường GiaTien của bảng MonAn để cập nhật giá trị mới cho các món ăn trong thực đơn. Đầu tiên, thủ tục cần thực hiện kiểm tra logic để đảm bảo mã món ăn tồn tại trong hệ thống và giá tiền mới phải là một số dương hợp lệ. Sau đó, sử dụng lệnh UPDATE để thay đổi dữ liệu trực tiếp trong bảng. Cuối cùng, thực hiện truy vấn hiển thị danh sách món ăn đã cập nhật để kiểm tra tính chính xác. Sử dụng lệnh EXEC để thực thi

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/b6a7a36a-6055-4df9-9ec9-132bf8f50622" />

Kết quả:

Trước khi dùng lệnh:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/4862effe-d398-4d4d-984d-e6aef0c60b43" />

Sau khi dùng lệnh:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/b67c5e71-efb4-4e2e-9c76-ac294ccf076e" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/4fbe866d-9b12-449a-9dba-1a63c0eb02ff" />

Viết 01 Store Procedure có sử dụng tham số OUTPUT: Dựa vào mã nhân viên (MaNV) được truyền vào, thủ tục sẽ thực hiện đếm tổng số lượng hóa đơn mà nhân viên đó đã lập trong bảng HoaDon. Đầu tiên, thủ tục kiểm tra xem mã nhân viên có tồn tại trong hệ thống hay không. Sau đó, kết quả tính toán sẽ được gán vào tham số đầu ra (OUTPUT) để có thể tái sử dụng cho các mục đích thống kê khác. Cuối cùng, thực hiện gọi thủ tục bằng lệnh EXEC kèm theo biến nhận giá trị để kiểm tra kết quả.

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/98ac99a7-a776-492a-89a1-887f4c3073f9" />

Kết quả:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/42ce25e8-26dc-4702-9144-bf2a87fc7ec6" />

Viết 01 Store Procedure trả về một tập kết quả (Result set) từ lệnh SELECT sau khi đã join nhiều bảng: Thủ tục thực hiện lệnh JOIN giữa các bảng HoaDon, ChiTietHoaDon, MonAn và NhanVien để tổng hợp thông tin chi tiết của một bàn ăn cụ thể

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/6a94f41b-166c-46e3-a8b4-38f51e18420d" />

Kết quả:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/0c68c5fd-4750-4bb0-8b29-c971b0a42121" />

## Phần 4: Trigger và Xử lý logic nghiệp vụ

Viết 1 Trigger tự động cập nhật trạng thái bàn ăn (BanAn) dựa trên sự thay đổi của hóa đơn (HoaDon)

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/62d97305-bbb8-4ddc-a629-c375af3ef5f9" />

Kết quả Trigger:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/bcc89a90-a663-498f-ae5e-7c2eec0871a8" />

Thử viết Trigger cho Bảng A : Khi insert thì cập nhật dữ liệu vào bảng B; sau đó viết trigger cho bảng B để khi B được cập nhật thì cập nhật sang bảng A

Trigger cho bảng A:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/7cb8c368-d030-4c9d-a567-2bff5328c66d" />

Trigger cho bảng B:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/1ac48caf-e058-4d3c-9c97-69f858331c54" />

Insert dữ liệu vào bảng B:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/40ac9a84-3a23-49a6-a049-8a56f2e10c58" />

Kết quả: 

Trước:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/86498375-635b-4b71-a417-8cb4250ade71" />

Sau:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/5ef56047-dea3-4ec0-9197-07c52b12b6aa" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/109cbf5c-60ff-4b6e-80e2-32fa924f7d3b" />

Nhận xét: Trigger là một công cụ mạnh mẽ giúp tự động hóa việc duy trì tính toàn vẹn và đồng bộ dữ liệu giữa các bảng giúp giảm tải logic cho phần mềm ứng dụng. Tuy nhiên, qua quá trình tìm hiểu, ta thấy đây là một "con dao hai lưỡi". Nếu thiết kế không cẩn trọng sẽ dẫn đến hiện tượng đệ quy vô hạn (vòng lặp 32 cấp) gây treo hệ thống. Vì vậy, bài học quan trọng nhất là nên ưu tiên luồng cập nhật một chiều, xác định chính xác các sự kiện kích hoạt (INSERT, UPDATE, DELETE) và hạn chế tối đa các logic cập nhật chéo phức tạp để đảm bảo hiệu năng tối ưu cho cơ sở dữ liệu.

## Phần 5: Cursor và Duyệt dữ liệu

- Viết một đoạn script sử dụng Cursor để duyệt qua danh sách bảng MonAn và dữ liệu bán trong ChiTietHoaDon. Với mỗi món ăn, Cursor sẽ tính tổng số lượng đã bán và tổng số tiền thu về. Nếu doanh thu của món ăn đạt trên 500.000 VNĐ, hệ thống sẽ in thông báo phân loại là 'Món ăn tiềm năng', ngược lại nếu chưa có lượt bán nào sẽ cảnh báo là 'Món cần xem xét cải thiện'

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/bc5c7cba-6ce9-42d0-9768-712e9f4dcad5" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/cca41287-7726-46ef-892b-88b579c6e62c" />

Kết quả:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/b70f1ea2-fa16-432d-84cb-49d43947dfa4" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/6476dada-3347-4020-995c-be31a0295d87" />

- Không dùng Cursor để giải quyết bài toán Cursor đã được giải quyết ở trên, em sẽ sử dụng lệnh SELECT kết hợp biểu thức CASE WHEN

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/ac6cdef6-37d8-40be-a468-0376da5df857" />

Kết quả:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/ef6270c9-9bca-41ce-8385-dea3770b6b20" />

Kết luận so sánh: Không sử dụng Cursor sẽ nhanh hơn vì dùng Cursor sẽ phải duyệt chạy từng dòng, còn khi dùng CASE WHEN sẽ duyệt chạy cả bảng không những thế còn tối ưu, sử dụng ít tài nguyên hơn Cursor, bảng được tạo ra còn ngắn gọn, dễ đọc hơn.

- Bài toán Cursor giải quyết tốt hơn thay vì dùng SQL: Giảm giá món ăn theo số lượng bán ra, món bán ít thì giảm nhiều, bán được nhiều thì giảm ít hoặc không giảm

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/715a3152-acd8-4247-a235-5bbe433e61d9" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/1b4c89d2-482c-4ef5-936f-af6cd14ddbf7" />

Kết quả:

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/92f37070-c71c-4988-ba53-8604cf03977c" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/6f485fb1-8273-4424-9845-8072a0caf956" />
