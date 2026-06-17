# BÁO CÁO TÌM HIỂU CÔNG CỤ POSTMAN

## 1. Thông tin sinh viên

* **Họ và tên:** Nguyễn Quốc Thành
* **MSSV:** 23010038

---

## 2. Giới thiệu Postman

Postman là công cụ hỗ trợ phát triển và kiểm thử API phổ biến, cho phép người dùng gửi các HTTP Request và kiểm tra phản hồi từ máy chủ một cách trực quan.

### Các tính năng chính

* Gửi HTTP Request (GET, POST, PUT, DELETE, PATCH...)
* Kiểm thử API
* Quản lý Collection
* Tự động hóa kiểm thử bằng Test Script
* Hỗ trợ làm việc nhóm
* Xuất và chia sẻ tài liệu API

---

## 3. Tài liệu tham khảo

### Video hướng dẫn

* https://www.youtube.com/watch?v=MFxk5BZulVU

### Tài liệu khác

* https://learning.postman.com
* https://www.postman.com/api-platform/api-testing/
* https://www.geeksforgeeks.org/postman-tutorial/

---

## 4. Cài đặt Postman

### Bước 1: Tải Postman

Truy cập trang chủ Postman và tải phần mềm theo hệ điều hành đang sử dụng.

### Bước 2: Cài đặt

Tiến hành cài đặt theo hướng dẫn của trình cài đặt.

### Kết quả

<img width="1920" height="953" alt="postman" src="https://github.com/user-attachments/assets/b0335dfe-018c-493c-8930-f52f4ca7f330" />)

---

## 5. Tạo Collection

Tạo Collection có tên **Postman Learning** để quản lý các API đã kiểm thử.

### Kết quả

![Collection](images/collection.png)

---

## 6. Thực hành gửi GET Request

### API sử dụng

```text
https://jsonplaceholder.typicode.com/posts/1
```

### Thực hiện

* Chọn phương thức GET.
* Nhập URL API.
* Nhấn **Send**.

### Kết quả

Server trả về dữ liệu JSON của bài viết có ID = 1.

![GET Request](images/get-post-1.png)

---

## 7. Thực hành gửi POST Request

### API sử dụng

```text
https://jsonplaceholder.typicode.com/posts
```

### Body

```json
{
  "title": "Postman Test",
  "body": "Hello API",
  "userId": 1
}
```

### Kết quả

Server trả về dữ liệu đã được tạo mới.

![POST Request](images/post-create.png)

---

## 8. Thực hành gửi PUT Request

### API sử dụng

```text
https://jsonplaceholder.typicode.com/posts/1
```

### Body

```json
{
  "id": 1,
  "title": "Updated Post",
  "body": "Updated content",
  "userId": 1
}
```

### Kết quả

Server trả về dữ liệu đã được cập nhật.

![PUT Request](images/put-update.png)

---

## 9. Thực hành gửi DELETE Request

### API sử dụng

```text
https://jsonplaceholder.typicode.com/posts/1
```

### Thực hiện

* Chọn phương thức DELETE.
* Nhập URL API.
* Nhấn **Send**.

### Kết quả

Server trả về mã trạng thái thành công.

![DELETE Request](images/delete-post.png)

---

## 10. Viết Test Script

Ví dụ kiểm tra mã trạng thái phản hồi:

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

### Kết quả

Kiểm thử thành công.

![Test Result](images/test-script.png)

---

## 11. Xuất Collection

Sau khi hoàn thành các API, Collection được xuất dưới định dạng **Collection v2.1** để chia sẻ và tái sử dụng.

### Kết quả

File xuất:

```text
postman_collection.json
```

---

## 12. Nhận xét

### Ưu điểm

* Giao diện dễ sử dụng.
* Hỗ trợ nhiều loại API.
* Dễ dàng quản lý Collection.
* Hỗ trợ viết Test Script.
* Tích hợp tốt với nhiều công cụ khác.

### Nhược điểm

* Một số tính năng nâng cao yêu cầu tài khoản trả phí.
* Có thể tiêu tốn tài nguyên máy khi chạy nhiều Collection.
* Cần thời gian làm quen với các tính năng nâng cao.

---

## 13. Kết luận

Sau khi tìm hiểu và thực hành, em đã nắm được các thao tác cơ bản trên Postman như:

* Gửi các phương thức HTTP: GET, POST, PUT và DELETE.
* Kiểm tra Response và Status Code.
* Tạo và quản lý Collection.
* Viết Test Script để kiểm thử API.
* Xuất Collection để chia sẻ và tái sử dụng.

Qua bài thực hành, em nhận thấy Postman là một công cụ mạnh mẽ, hỗ trợ hiệu quả trong quá trình phát triển và kiểm thử API.

---

## 14. Link GitHub Repository

Điền liên kết repository GitHub của bạn tại đây:

```text
https://github.com/ten-tai-khoan/ten-repository
```
