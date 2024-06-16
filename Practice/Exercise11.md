# Bài tập thực hành số 11 (Tiết 1 & 2)

## Câu 1. Cho thông tin như sau:

```
Phòng { Mã phòng, tên phòng }
Nhân viên { Mã nhân viên, Tên nhân viên }
Thiết bị { Mã thiết bị, Tên thiết bị }
Kiểm tra { Mã nhân viên, Mã thiết bị, Ngày kiểm tra, Tình trạng }
```

Xây dựng lược đồ quan hệ (câu lệnh SQL) thỏa mãn yêu cầu [logic business] doanh nghiệp như sau:

+  Thông tin kiểm tra: sẽ gồm thông tin của nhân viên kiểm tra thiết bị tương ứng, ngày được kiểm tra và tình trạng cụ thể.
+  Tình trạng chỉ có hai giá trị "Pass" và "Not Pass".
+  Một thiết bị có thể được kiểm tra nhiều lần bới một hoặc nhiều nhân viên trong một hoặc nhiều thời điểm cho đến khi đạt trạng thái "Pass".
+  Mõi nhân viên sẽ thuộc về một phòng ban cụ thể.
  

<I> Yêu cầu team leader: </I>


Developer <I> [Sinh viên] </I> cần xác định thuộc tính Khóa, xác định constraint của các thuộc tính [nếu có].

Thực hiện liên kết các quan hệ đảm bảo ràng buộc toàn vẹn giữa các quan hệ.

Thêm quan hệ (bảng) nếu cần. 

## Câu 2 
Thêm 05 bản ghi vào mỗi quan hệ (Bảng) sau khi các bảng đã có các ràng buộc toàn vẹn.
   
```
   Ví dụ: mathietbi: "tb01"
          manv:"nv02"
          maphong: "mp02"
          tinhtrang: "Not Pass"
 ```
## Câu 3 
1. Tạo một Trigger cho phép xuất kho (new tuple) những thiết bị có tình trạng là "Pass".

2. Hiển thị những dòng dữ liệu này. Kết quả ?
## Câu 4 
1. Tạo một Trigger trước khi xóa hoạt động kiểm tra xem thiết bị đã có trạng thái "Pass" chưa. Nếu chưa [có trạng thái "Not Pass"] thì đưa ra thông báo "Thiet bị chua dat kiem tra" và không cho phép xóa.

2. Thực hiện xóa tất cả thông tin kiểm tra thuộc về mp02. Kết quả ?
## Câu 5 
Xây dựng stored Procedure để xuất ra [temp_table] tất cả các thiết bị có liên quan đến phòng có mã phòng mp02 và có tình trạng "Not Pass" và nhân viên cụ thể kiểm tra thiết bị, cũng như ngày giờ liên quan.
## Câu 6:
Chạy stored Procedure.
Đưa ra tất cả dữ liệu trong temp_table
   
# Team [Sinh viên] trình bày giải pháp (Tiết 3)

Product Owner nhận xét, ghi nhận, và thêm yêu cầu (nếu có).

PO thỏa mãn, bàn giao sản phẩm.

Team kết thúc phát triển sản phẩm. 

HAPPY ENDING !

