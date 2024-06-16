# Bài tập thực hành số 11 (Tiết 1 & 2)

## Câu 1. Cho thông tin như sau:

```
Phòng { Mã phòng, tên phòng}
Nhân viên { Mã nhân viên, Tên nhân viên}
Thiết bị {Mã thiết bị, Tên thiết bị}
Kiểm tra (Mã nhân viên, Mã thiết bị, Ngày kiểm tra, Tình trạng)
```

Xây dựng lược đồ quan hệ (câu lệnh SQL) thỏa mãn yêu cầu:

+  Thông tin kiểm tra: sẽ gồm thông tin của nhân viên kiểm tra thiết bị tương ứng, ngày được kiểm tra và tình trạng cụ thể.
+  Tình trạng chỉ có hai giá trị "Pass" và "Not Pass".
+  Mõi nhân viên sẽ thuộc về một phòng ban cụ thể.
  

Sinh viên cần xác định thuộc tính Khóa, xác định constraint của các thuộc tính [nếu có].

Thực hiện liên kết các quan hệ đảm bảo ràng buộc toàn vẹn giữa các quan hệ.

Thêm quan hệ (bảng) nếu cần. 

## Câu 2 
Thêm 05 bản ghi vào mỗi quan hệ (Bảng) sau khi các bảng đã có các ràng buộc toàn vẹn.
   
```
   Ví dụ: mathietbi: tb01
          manv:nv02
          maphong: mp02
 ```
## Câu 3 
Tạo một Trigger cho phép xuất kho (new tuple) những thiết bị có tình trạng là "Pass".
## Câu 4 
Tạo một Trigger trước khi xóa hoạt động kiểm tra xem thiết bị đã có trạng thái "Pass" chưa. Nếu chưa [có trạng thái "Not Pass"] thì đưa ra thông báo "Thiet bị chua dat kiem tra" và không cho phép xóa.
## Câu 5 
Xây dựng stored Procedure để xuất ra [temp_table] tất cả các thiết bị có liên quan đến phòng có mã phòng mp02 và có tình trạng "Not Pass" và nhân viên cụ thể kiểm tra thiết bị.
## Câu 6:
Chạy stored Procedure.
Đưa ra tất cả dữ liệu trong temp_table
   
# Sinh viên được gọi lên trình bày câu trả lời (Tiết 3)

Giáo viên nhận xét, góp ý, và trợ giúp (nếu cần).

