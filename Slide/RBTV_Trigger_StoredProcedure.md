# Bài tập View - Trigger - Procedure

# 1. Bài tập View
## Bài tập một: tạo VIEW từ hai bảng dưới đây hiển thị tất cả thông tin của hai bảng

![View 2 Table ](https://nglthu.github.io/Database/img/view2T.png)

Hình 1: Bảng 1: Lược đồ quan hệ giữa hai quan hệ (hai Bảng)

## Bài tập hai: tạo VIEW từ bốn bảng dưới đây hiển thị thông tin order number, product description, quantity order, and image :


![View 2 Table ](https://nglthu.github.io/Database/img/view4T.png)

Hình 2: Bảng 2: Lược đồ quan hệ giữa bốn quan hệ ( bốn bảng)

# 2. Bài tập Trigger
## Bài tập Trigger 1
![Trigger 1 ](https://nglthu.github.io/Database/img/trigger1.png)

## Bài tập Trigger 2
![Trigger 2 ](https://nglthu.github.io/Database/img/trigger2.png)

# 3. Bài tập Procedure
## Bài tập Stored Procedure 1
```
Tạo một SP, Có tên:	sp_customers(IN credit int)

Hiển thị customerNumber, creditLimit lớn hơn credit đầu vào

Hiển thị Stored Procedure sp_customer(200000)

```
## Bài tập Stored Procedure 2
```
Tạo một SP, Có tên:	quantity_in_stock(IN orderNumber int OUT stock_quality int)

Cập nhật số quantityInStock khi có order hay quantityOrder như Bảng 2. 

Hiển thị Stored Procedure quantity_in_stock(10, @stock_quantity)

```

# Phụ lục (Appendix)
## Trigger trong bảng Table trên MySQL workbench
![Chạy trigger trên bảng (Table) ](https://nglthu.github.io/Database/img/triggerEdit.png)

## Stored Procedure window trên MySQL workbench
![Cửa sổ chạy thủ tục ](https://nglthu.github.io/Database/img/storeProcedure.png)



## ON UPDATE RESTRICT ON DELETE CASCADE

## Cascade
![Cascade](https://nglthu.github.io/Database/img/cascade.png)

## Restrict

![Restrict](https://nglthu.github.io/Database/img/restrict.png)

## No Action


![No Action](https://nglthu.github.io/Database/img/noAction.png)

## Signal

```
SIGNAL is the way to “return” an error.
SIGNAL provides error information to a handler, to an outer portion of the application, or to the client.
It provides control over the error's characteristics (error number, SQLSTATE value, message).

Without SIGNAL, it is necessary to resort to workarounds such as deliberately referring to a nonexistent table to cause a routine to return an error.

```
[Hướng dẫn sử dụng SIGNAL](https://dev.mysql.com/doc/refman/8.0/en/signal.html)

## delimiter // delimiter ;

+ mysql client program to define a stored program containing semicolon characters, a problem arises. By default, mysql itself recognizes the semicolon as a statement delimiter, so you must redefine the delimiter temporarily to cause mysql to pass the entire stored program definition to the server.

+ To redefine the mysql delimiter, use the delimiter command.
  
```
delimiter //
[code]

delimiter ;

  ```

to enable the entire definition to be passed to the server as a single statement, and then restored to ; before invoking the procedure.
This enables the ; delimiter used in the procedure body to be passed through to the server rather than being interpreted by mysql itself.

Example :

![Delimiter](https://nglthu.github.io/Database/img/delimiter.png)
