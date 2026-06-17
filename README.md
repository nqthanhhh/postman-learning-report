# BÁO CÁO TÌM HIỂU CÔNG CỤ POSTMAN

## 1. Thông tin sinh viên

* Họ và tên: Nguyễn Quốc Thành
* MSSV: 23010038

---

## 2. Giới thiệu Postman

Postman là một công cụ hỗ trợ kiểm thử API phổ biến, cho phép lập trình viên gửi các HTTP Request và kiểm tra phản hồi từ server.

Các tính năng chính:

* Gửi HTTP Request (GET, POST, PUT, DELETE...)
* Kiểm thử API
* Quản lý Collection
* Tự động hóa kiểm thử bằng Test Script
* Hỗ trợ làm việc nhóm

---

## 3. Tài liệu tham khảo

### Video hướng dẫn

https://www.youtube.com/watch?v=MFxk5BZulVU

### Tài liệu khác

* https://learning.postman.com
* https://www.postman.com/api-platform/api-testing/
* https://www.geeksforgeeks.org/postman-tutorial/

---

## 4. Cài đặt Postman

### Bước 1: Tải Postman

Truy cập trang chủ Postman và tải phần mềm.

### Bước 2: Cài đặt

Tiến hành cài đặt theo hướng dẫn.

### Kết quả

![Cài đặt Postman](images/postman-install.png)

---

## 5. Thực hành gửi GET Request

### API sử dụng

https://jsonplaceholder.typicode.com/posts/1

### Thực hiện

* Chọn phương thức GET
* Nhập URL API
* Nhấn Send

### Kết quả

![GET Request](images/get-request.png)

Nhận được dữ liệu JSON trả về từ server.

---

## 6. Thực hành gửi POST Request

### API sử dụng

https://jsonplaceholder.typicode.com/posts

### Body

```json
{
  "title": "Postman Test",
  "body": "Hello API",
  "userId": 1
}
```

### Kết quả

![POST Request](images/post-request.png)

Server trả về dữ liệu đã được tạo mới.

---

## 7. Tạo Collection

Tạo Collection để quản lý các API đã kiểm thử.

### Kết quả

![Collection](images/collection.png)

---

## 8. Viết Test Script

Ví dụ:

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

### Kết quả

![Test Result](images/test-result.png)

Kiểm thử thành công.

---

## 9. Nhận xét

### Ưu điểm

* Giao diện dễ sử dụng.
* Hỗ trợ nhiều loại API.
* Dễ dàng quản lý Collection.
* Hỗ trợ viết Test Script.

### Nhược điểm

* Một số tính năng nâng cao yêu cầu tài khoản.
* Có thể tiêu tốn tài nguyên máy khi chạy nhiều Collection.

---

## 10. Kết luận

Sau khi tìm hiểu và thực hành, em đã nắm được các thao tác cơ bản trên Postman như gửi Request, kiểm tra Response, tạo Collection và viết Test Script để kiểm thử API.
