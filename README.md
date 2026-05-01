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


